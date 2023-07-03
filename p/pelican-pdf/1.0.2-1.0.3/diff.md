# Comparing `tmp/pelican_pdf-1.0.2.tar.gz` & `tmp/pelican_pdf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_pdf-1.0.2.tar", max compression
+gzip compressed data, was "pelican_pdf-1.0.3.tar", max compression
```

## Comparing `pelican_pdf-1.0.2.tar` & `pelican_pdf-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    34674 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/LICENSE
--rw-r--r--   0        0        0     1835 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/README.md
--rw-r--r--   0        0        0       27 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/__init__.py
--rw-r--r--   0        0        0     4742 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/pdf.py
--rw-r--r--   0        0        0      431 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/test_data/testfile.md
--rw-r--r--   0        0        0      468 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/test_data/testfile.rst
--rw-r--r--   0        0        0      294 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/test_data/testfile_link.md
--rw-r--r--   0        0        0      329 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/test_data/testfile_link.rst
--rw-r--r--   0        0        0     1158 2023-04-04 06:03:02.543358 pelican_pdf-1.0.2/pelican/plugins/pdf/test_pdf.py
--rw-r--r--   0        0        0     1985 2023-04-04 06:03:20.915330 pelican_pdf-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 pelican_pdf-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34674 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1835 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/README.md
+-rw-r--r--   0        0        0       27 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0     4803 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/pdf.py
+-rw-r--r--   0        0        0      431 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile.md
+-rw-r--r--   0        0        0      468 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile.rst
+-rw-r--r--   0        0        0      294 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile_link.md
+-rw-r--r--   0        0        0      329 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile_link.rst
+-rw-r--r--   0        0        0     1158 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_pdf.py
+-rw-r--r--   0        0        0     2010 2023-07-03 09:13:09.761512 pelican_pdf-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pelican_pdf-1.0.3/PKG-INFO
```

### Comparing `pelican_pdf-1.0.2/LICENSE` & `pelican_pdf-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_pdf-1.0.2/README.md` & `pelican_pdf-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pelican_pdf-1.0.2/pelican/plugins/pdf/pdf.py` & `pelican_pdf-1.0.3/pelican/plugins/pdf/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,22 @@
 The pdf plugin generates PDF files from reStructuredText and Markdown sources.
 """
 
 from itertools import chain
 import logging
 import os
 import re
+import time
+
+from rst2pdf.createpdf import RstToPdf
 
 from pelican import signals
 from pelican.generators import Generator
 from pelican.readers import MarkdownReader
 
-"""
-Workaround until fixed xhtml2pdf import is included in rst2pdf Release
-https://github.com/rst2pdf/rst2pdf/commit/6ad348cf5a13ae1b884a86574e48ed1e5f8ca135
-"""
-import xhtml2pdf.default  # NOQA isort:skip
-from rst2pdf.createpdf import RstToPdf  # NOQA isort:skip
-
-
 logger = logging.getLogger(__name__)
 
 
 class PdfGenerator(Generator):
     "Generate PDFs on the output dir, for all articles and pages"
 
     supported_md_fields = ["date"]
@@ -74,15 +69,15 @@
 
             for k in list(meta):
                 # We can't support all fields, so we strip the ones that won't
                 # look good
                 if k not in self.supported_md_fields:
                     del meta[k]
 
-            header += "\n".join([":{}: {}".format(k, meta[k]) for k in meta])
+            header += "\n".join([f":{k}: {meta[k]}" for k in meta])
             header += "\n\n.. raw:: html\n\n\t"
             text = text.replace("\n", "\n\t")
 
             # rst2pdf casts the text to str and will break if it finds
             # non-escaped characters. Here we nicely escape them to XML/HTML
             # entities before proceeding
             text = text.encode("ascii", "xmlcharrefreplace").decode()
@@ -100,23 +95,31 @@
         hrefs = self._get_intrasite_link_regex()
         text = hrefs.sub(lambda m: obj._link_replacer(obj.get_siteurl(), m), text)
 
         logger.info(" [ok] writing %s" % output_pdf)
 
         self.pdfcreator.createPdf(text=(header + text), output=output_pdf)
 
+        if obj.date is not None:
+            self._set_file_utime(output_pdf, obj.date)
+
     def _get_intrasite_link_regex(self):
         intrasite_link_regex = self.settings["INTRASITE_LINK_REGEX"]
         regex = r"""
                 (?P<markup>)(?P<quote>)(?P<path>(\:?){}(?P<value>.*?)(?=[>\n]))
                 """.format(
             intrasite_link_regex
         )
         return re.compile(regex, re.X)
 
+    def _set_file_utime(self, path, datetime):
+        """Set modified time (mtime) of specified file."""
+        mtime = time.mktime(datetime.timetuple())
+        os.utime(path, (mtime, mtime))
+
     def generate_context(self):
         pass
 
     def generate_output(self, writer=None):
         # we don't use the writer passed as argument here
         # since we write our own files
         logger.info(" Generating PDF files...")
```

### Comparing `pelican_pdf-1.0.2/pelican/plugins/pdf/test_pdf.py` & `pelican_pdf-1.0.3/pelican/plugins/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pelican_pdf-1.0.2/pyproject.toml` & `pelican_pdf-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-pdf"
-version = "1.0.2"
+version = "1.0.3"
 description = "PDF Generator is a Pelican plugin that exports articles and pages as PDF files during site generation"
 authors = ["Pelican Dev Team <authors@getpelican.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "pdf", "generator"]
 repository = "https://github.com/pelican-plugins/pdf"
 documentation = "https://docs.getpelican.com"
@@ -24,39 +24,39 @@
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/pelican-plugins/pdf/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8.1,<4.0"
 pelican = ">=4.5"
 markdown = {version = ">=3.2.2", optional = true}
-rst2pdf = ">=0.98"
+rst2pdf = ">=0.99"
 xhtml2pdf = ">=0.2.5"
 
 [tool.poetry.dev-dependencies]
 black = "^23"
 flake8 = "^3.9"
 flake8-black = "^0.3"
 invoke = "^2.0"
-isort = "^5.4"
-markdown = "^3.3"
+isort = "^5.12.0"
+markdown = "^3.4"
 pytest = "^6.0"
 pytest-cov = "^2.8"
 pytest-pythonpath = "^0.7.3"
 pytest-sugar = "^0.9.6"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
 
 [tool.autopub]
 project-name = "PDF Generator"
 git-username = "botpub"
-git-email = "botpub@autopub.rocks"
+git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.isort]
 # Maintain compatibility with Black
 profile = "black"
 multi_line_output = 3
```

### Comparing `pelican_pdf-1.0.2/PKG-INFO` & `pelican_pdf-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pelican-pdf
-Version: 1.0.2
+Version: 1.0.3
 Summary: PDF Generator is a Pelican plugin that exports articles and pages as PDF files during site generation
 Home-page: https://github.com/pelican-plugins/pdf
 License: AGPL-3.0
 Keywords: pelican,plugin,pdf,generator
 Author: Pelican Dev Team
 Author-email: authors@getpelican.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: markdown
 Requires-Dist: markdown (>=3.2.2) ; extra == "markdown"
 Requires-Dist: pelican (>=4.5)
-Requires-Dist: rst2pdf (>=0.98)
+Requires-Dist: rst2pdf (>=0.99)
 Requires-Dist: xhtml2pdf (>=0.2.5)
 Project-URL: Documentation, https://docs.getpelican.com
 Project-URL: Funding, https://donate.getpelican.com/
 Project-URL: Issue Tracker, https://github.com/pelican-plugins/pdf/issues
 Project-URL: Repository, https://github.com/pelican-plugins/pdf
 Description-Content-Type: text/markdown
```


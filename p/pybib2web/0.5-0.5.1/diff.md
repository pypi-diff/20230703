# Comparing `tmp/pybib2web-0.5.tar.gz` & `tmp/pybib2web-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybib2web-0.5.tar", last modified: Mon Jun 13 14:43:02 2022, max compression
+gzip compressed data, was "pybib2web-0.5.1.tar", last modified: Mon Jul  3 15:01:36 2023, max compression
```

## Comparing `pybib2web-0.5.tar` & `pybib2web-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:43:02.977352 pybib2web-0.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:43:02.969352 pybib2web-0.5/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2022-03-06 05:28:47.000000 pybib2web-0.5/LICENSES/Apache-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3236 2022-06-13 14:43:02.977352 pybib2web-0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2370 2022-03-06 05:28:47.000000 pybib2web-0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:43:02.977352 pybib2web-0.5/pybib2web/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2022-03-06 05:28:47.000000 pybib2web-0.5/pybib2web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2022-03-06 05:28:47.000000 pybib2web-0.5/pybib2web/bibexport.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2022-03-06 05:28:47.000000 pybib2web-0.5/pybib2web/bibparser.py
--rw-rw-rw-   0 root         (0) root         (0)     6128 2022-03-06 05:28:47.000000 pybib2web-0.5/pybib2web/categories.py
--rw-rw-rw-   0 root         (0) root         (0)     1786 2022-03-06 05:28:47.000000 pybib2web-0.5/pybib2web/config.py
--rw-rw-rw-   0 root         (0) root         (0)    29465 2022-03-06 05:28:47.000000 pybib2web-0.5/pybib2web/htmlexport.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2022-06-12 19:33:29.000000 pybib2web-0.5/pybib2web/util.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2022-06-13 13:33:38.000000 pybib2web-0.5/pybib2web/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:43:02.977352 pybib2web-0.5/pybib2web.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3236 2022-06-13 14:43:02.000000 pybib2web-0.5/pybib2web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2022-06-13 14:43:02.000000 pybib2web-0.5/pybib2web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 14:43:02.000000 pybib2web-0.5/pybib2web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-06-13 14:43:02.000000 pybib2web-0.5/pybib2web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-06-13 14:43:02.000000 pybib2web-0.5/pybib2web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-06-13 14:43:02.000000 pybib2web-0.5/pybib2web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 14:43:01.000000 pybib2web-0.5/pybib2web.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      378 2022-03-06 05:28:47.000000 pybib2web-0.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1353 2022-06-13 14:43:02.977352 pybib2web-0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.251294 pybib2web-0.5.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.247294 pybib2web-0.5.1/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-25 02:17:30.000000 pybib2web-0.5.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-07-03 15:01:36.251294 pybib2web-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2023-06-25 02:17:30.000000 pybib2web-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.247294 pybib2web-0.5.1/pybib2web/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/bibexport.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/bibparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6128 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    29638 2023-07-03 14:48:12.000000 pybib2web-0.5.1/pybib2web/htmlexport.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-03 14:53:09.000000 pybib2web-0.5.1/pybib2web/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.251294 pybib2web-0.5.1/pybib2web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-03 15:01:36.251294 pybib2web-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.251294 pybib2web-0.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-25 02:17:30.000000 pybib2web-0.5.1/tests/test_bibparser.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-06-25 02:17:30.000000 pybib2web-0.5.1/tests/test_htmlexport.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2023-06-25 02:17:30.000000 pybib2web-0.5.1/tests/test_util.py
```

### Comparing `pybib2web-0.5/LICENSES/Apache-2.0.txt` & `pybib2web-0.5.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/PKG-INFO` & `pybib2web-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybib2web
-Version: 0.5
+Version: 0.5.1
 Summary: A translator of BibTeX to HTML.
 Home-page: https://gitlab.com/sosy-lab/software/pybib2web
 Author: Dirk Beyer
 Author-email: dirk.beyer@sosy-lab.org
 License: Apache-2.0
 Project-URL: Changelog, https://gitlab.com/sosy-lab/software/pybib2web/-/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://gitlab.com/sosy-lab/software/pybib2web/-/issues
```

### Comparing `pybib2web-0.5/README.md` & `pybib2web-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web/__init__.py` & `pybib2web-0.5.1/pybib2web/__init__.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web/bibexport.py` & `pybib2web-0.5.1/pybib2web/bibexport.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web/bibparser.py` & `pybib2web-0.5.1/pybib2web/bibparser.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web/categories.py` & `pybib2web-0.5.1/pybib2web/categories.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web/config.py` & `pybib2web-0.5.1/pybib2web/config.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web/htmlexport.py` & `pybib2web-0.5.1/pybib2web/htmlexport.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Module concerned with exporting BibTeX entries to HTML."""
 
 import re
 from collections import namedtuple, defaultdict
 import logging
+import html
 from pathlib import Path
 from typing import Sequence, Iterable, Dict
 
 from . import categories, bibexport, util
 from .config import Config
 from .version import __version__
 
@@ -110,25 +111,25 @@
     title = entry.get("title")
     if not title:
         return ""
     return f'<span class="publication-title">{title}.</span>'
 
 
 def talk_type_to_html(entry):
-    html = ""
+    html_text = ""
     entrytype = entry["ENTRYTYPE"]
     if entrytype == "conferencetalk":
-        html = "Conference talk"
+        html_text = "Conference talk"
     if entrytype == "invitedtalk":
-        html = "Invited talk"
+        html_text = "Invited talk"
     if entrytype == "defense":
-        html = "Defense"
-    if html:
-        html = f'<span class="talk-type">{html}</span>'
-    return html
+        html_text = "Defense"
+    if html_text:
+        html_text = f'<span class="talk-type">{html_text}</span>'
+    return html_text
 
 
 def annotations_to_html(entry):
     annote = entry.get("annote", "")
     if annote:
         return _create_details(
             "Additional Infos", annote, "annote", open_by_default=True
@@ -154,15 +155,17 @@
 
     return f'<details {open_html} class="{html_class}">\n{indent(1, summary)}\n{indent(1, details)}\n</details>'
 
 
 def bibtex_to_html(entry):
     if "original" in entry:
         entry = entry["original"]
-    return _create_details("BibTeX Entry", bibexport.writes(entry), html_class="bibtex")
+    raw_bibexport = bibexport.writes(entry)
+    export_escaped_for_html = html.escape(raw_bibexport)
+    return _create_details("BibTeX Entry", export_escaped_for_html, html_class="bibtex")
 
 
 def authors_to_html(entry, config: Config):
     try:
         if _put_editors_in_front(entry):
             authors = get_editors(entry)
             authors_html = (
@@ -575,24 +578,24 @@
     config,
     head=None,
     header_title=None,
 ):
     output_file = Path(output_file)
     output_file.parent.mkdir(exist_ok=True, parents=True)
     with open(output_file, "w", encoding="UTF-8") as outp:
-        html = writes(entries, config=config, head=head, header_title=header_title)
-        write_html(outp, html)
+        html_text = writes(entries, config=config, head=head, header_title=header_title)
+        write_html(outp, html_text)
 
 
-def write_html(output_obj, html: str):
+def write_html(output_obj, html_text: str):
     start = f"<!-- This file was generated by pybib2web, version {__version__}: https://gitlab.com/sosy-lab/software/pybib2web/ -->"
 
     end = f'<footer id="generator">This file was generated by <a href="https://gitlab.com/sosy-lab/software/pybib2web/">pybib2web</a>, version {__version__}</footer>'
     output_obj.write(start)
-    output_obj.write(html)
+    output_obj.write(html_text)
     output_obj.write(end)
 
 
 def _get_header(header, config, show_link_to_index=True, show_link_to_all=True):
     def maybe_all():
         return (
             ['<a href="../All/index.html">Show all</a>']
```

### Comparing `pybib2web-0.5/pybib2web/util.py` & `pybib2web-0.5.1/pybib2web/util.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5/pybib2web.egg-info/PKG-INFO` & `pybib2web-0.5.1/pybib2web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybib2web
-Version: 0.5
+Version: 0.5.1
 Summary: A translator of BibTeX to HTML.
 Home-page: https://gitlab.com/sosy-lab/software/pybib2web
 Author: Dirk Beyer
 Author-email: dirk.beyer@sosy-lab.org
 License: Apache-2.0
 Project-URL: Changelog, https://gitlab.com/sosy-lab/software/pybib2web/-/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://gitlab.com/sosy-lab/software/pybib2web/-/issues
```

### Comparing `pybib2web-0.5/setup.cfg` & `pybib2web-0.5.1/setup.cfg`

 * *Files identical despite different names*


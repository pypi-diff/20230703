# Comparing `tmp/html_sanitizer-2.1.0.tar.gz` & `tmp/html_sanitizer-2.2.0.tar.gz`

## Comparing `html_sanitizer-2.1.0.tar` & `html_sanitizer-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.editorconfig
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/tox.ini
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/__main__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/django.py
--rw-r--r--   0        0        0    13558 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/sanitizer.py
--rw-r--r--   0        0        0    23857 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/tests.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.gitignore
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/LICENSE
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/README.rst
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/.editorconfig
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/tox.ini
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/html_sanitizer/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/html_sanitizer/__main__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/html_sanitizer/django.py
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/html_sanitizer/sanitizer.py
+-rw-r--r--   0        0        0    24010 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/html_sanitizer/tests.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/LICENSE
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/README.rst
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 html_sanitizer-2.2.0/PKG-INFO
```

### Comparing `html_sanitizer-2.1.0/.pre-commit-config.yaml` & `html_sanitizer-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.1.0/CHANGELOG.rst` & `html_sanitizer-2.2.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 ==========
 Change log
 ==========
 
 Next version
 ============
 
+2.2 (2023-07-03)
+================
+
+- Changed ``keep_normalized_whitespace`` to preserve whitespace at the tail of
+  tags, not just between tags.
+- Changed the parameters of ``normalize_whitespace_in_text_or_tail`` to be
+  keyword-only.
+
 
 2.1 (2023-06-29)
 ================
 
 - Added a test for a type of misconfiguration.
 - Changed the sanitizer configuration validation to not allow unexpected data
   types in ``tags``, ``empty``, ``separate``, ``whitespace`` and
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_dti0zoqj_/tmp7cyuck_n_TarContainer/0/2.rst", line 159, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_dti0zoqj_/tmp7cyuck_n_TarContainer/0/2.rst", line 159, column 0: CDATA terminal not found*

```diff
@@ -1,10 +1,13 @@
-========== Change log ========== Next version ============ 2.1 (2023-06-29)
-================ - Added a test for a type of misconfiguration. - Changed the
-sanitizer configuration validation to not allow unexpected data types in
+========== Change log ========== Next version ============ 2.2 (2023-07-03)
+================ - Changed ``keep_normalized_whitespace`` to preserve
+whitespace at the tail of tags, not just between tags. - Changed the parameters
+of ``normalize_whitespace_in_text_or_tail`` to be keyword-only. 2.1 (2023-06-
+29) ================ - Added a test for a type of misconfiguration. - Changed
+the sanitizer configuration validation to not allow unexpected data types in
 ``tags``, ``empty``, ``separate``, ``whitespace`` and ``attributes``. 2.0
 (2023-06-28) ================ - Raised the minimum Python version to 3.7. Added
 Python 3.10, 3.11. - Raised the minimum lxml version to the current 4.9.1. -
 Switched from Travis CI to GitHub actions. Added Python 3.9 to the CI matrix. -
 Renamed the main branch to main. - Switched to a declarative setup. - Fixed a
 whitespace dependency in the testsuite. - Switched to hatchling and ruff. -
 Made behavior-altering arguments to ``normalize_overall_whitespace`` keyword-
```

### Comparing `html_sanitizer-2.1.0/.github/workflows/test.yml` & `html_sanitizer-2.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.1.0/html_sanitizer/django.py` & `html_sanitizer-2.2.0/html_sanitizer/django.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.1.0/html_sanitizer/sanitizer.py` & `html_sanitizer-2.2.0/html_sanitizer/sanitizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,25 +108,27 @@
         and element.attrib.get("id")
         and not element.attrib.get("name")
     ):
         element.attrib["name"] = element.attrib["id"]
     return element
 
 
-def normalize_whitespace_in_text_or_tail(element, whitespace_re=None):
+def normalize_whitespace_in_text_or_tail(
+    element, *, whitespace_re=None, keep_typographic_whitespace=False
+):
     if whitespace_re is None:
         whitespace_re = re.compile(r"\s+")
-    if element.text:
+    if element.text and not keep_typographic_whitespace:
         while True:
             text = whitespace_re.sub(" ", element.text)
             if element.text == text:
                 break
             element.text = text
 
-    if element.tail:
+    if element.tail and not keep_typographic_whitespace:
         while True:
             text = whitespace_re.sub(" ", element.tail)
             if element.tail == text:
                 break
             element.tail = text
 
     return element
@@ -286,15 +288,17 @@
             except IndexError:
                 break
 
             for processor in self.element_preprocessors:
                 element = processor(element)
 
             element = normalize_whitespace_in_text_or_tail(
-                element, whitespace_re=self.whitespace_re
+                element,
+                whitespace_re=self.whitespace_re,
+                keep_typographic_whitespace=self.keep_typographic_whitespace,
             )
 
             # remove empty tags if they are not explicitly allowed
             if (
                 (not element.text or self.only_whitespace_re.match(element.text))
                 and element.tag not in self.empty
                 and not len(element)
@@ -388,15 +392,17 @@
 
             # Clean hrefs so that they are benign
             href = element.get("href")
             if href is not None:
                 element.set("href", self.sanitize_href(href))
 
             element = normalize_whitespace_in_text_or_tail(
-                element, whitespace_re=self.whitespace_re
+                element,
+                whitespace_re=self.whitespace_re,
+                keep_typographic_whitespace=self.keep_typographic_whitespace,
             )
 
         if self.autolink is True:
             lxml.html.clean.autolink(doc)
         elif isinstance(self.autolink, dict):
             lxml.html.clean.autolink(doc, **self.autolink)
```

### Comparing `html_sanitizer-2.1.0/html_sanitizer/tests.py` & `html_sanitizer-2.2.0/html_sanitizer/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,14 +426,18 @@
                     "Hello This is a paragraph. \n"
                     "\tHello. This is a tabled line."
                     "Hello.This is beginning of the end.\r",
                     "Hello This is a paragraph. \n"
                     "\tHello. This is a tabled line."
                     "Hello.This is beginning of the end.\r",
                 ),
+                (
+                    "something    <br>somethingelse    ",
+                    "something    <br>somethingelse    ",
+                ),
             ],
             sanitizer=sanitizer,
         )
 
     def test_strip_typographic_whitespace(self):
         sanitizer = Sanitizer({"keep_typographic_whitespace": False})
```

### Comparing `html_sanitizer-2.1.0/LICENSE` & `html_sanitizer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.1.0/README.rst` & `html_sanitizer-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.1.0/pyproject.toml` & `html_sanitizer-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.1.0/PKG-INFO` & `html_sanitizer-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-sanitizer
-Version: 2.1.0
+Version: 2.2.0
 Summary: HTML sanitizer
 Project-URL: Homepage, https://github.com/matthiask/html-sanitizer/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```


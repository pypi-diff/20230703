# Comparing `tmp/sphinxcontrib-katex-0.9.6.tar.gz` & `tmp/sphinxcontrib-katex-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-katex-0.9.6.tar", last modified: Tue Jun 13 06:10:48 2023, max compression
+gzip compressed data, was "sphinxcontrib-katex-0.9.7.tar", last modified: Mon Jul  3 08:21:02 2023, max compression
```

## Comparing `sphinxcontrib-katex-0.9.6.tar` & `sphinxcontrib-katex-0.9.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.812928 sphinxcontrib-katex-0.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/macros.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/auto-render.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-math.css
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-server.js
--rw-r--r--   0 runner    (1001) docker     (123)   276757 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:21:02.663981 sphinxcontrib-katex-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-07-03 08:21:02.663981 sphinxcontrib-katex-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:21:02.659981 sphinxcontrib-katex-0.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/macros.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-03 08:21:02.663981 sphinxcontrib-katex-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:21:02.663981 sphinxcontrib-katex-0.9.7/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib/auto-render.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib/katex-math.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib/katex-server.js
+-rw-r--r--   0 runner    (1001) docker     (123)   276862 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib/katex.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-03 08:20:53.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib/katex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:21:02.663981 sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-07-03 08:21:02.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 08:21:02.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:21:02.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 08:21:02.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 08:21:02.000000 sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-katex-0.9.6/CHANGELOG.rst` & `sphinxcontrib-katex-0.9.7/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.7 (2023-07-03)
+--------------------------
+
+* Changed: use KaTeX 0.16.8
+* Removed: support for Python 3.7
+
+
 Version 0.9.6 (2023-06-13)
 --------------------------
 
 * Changed: use custom sphinx theme
   based on ``insipid``
   for HTML documentation pages
```

### Comparing `sphinxcontrib-katex-0.9.6/CONTRIBUTING.rst` & `sphinxcontrib-katex-0.9.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/LICENSE` & `sphinxcontrib-katex-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/PKG-INFO` & `sphinxcontrib-katex-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.6
+Version: 0.9.7
 Summary: A Sphinx extension for rendering math in HTML pages
 Home-page: https://github.com/hagenw/sphinxcontrib-katex
 Author: Hagen Wierstorf
 Author-email: hagenw@posteo.de
 License: MIT
 Keywords: sphinx,latex,katex,math,documentation
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
 
 sphinxcontrib-katex
 ===================
 
-|tests| |docs| |python-versions| |license|
+|docs| |python-versions| |license|
 
 A `Sphinx extension`_ for rendering math in HTML pages.
 
 The extension uses `KaTeX`_ for rendering of math in HTML pages. It is designed
 as a replacement for the built-in extension `sphinx.ext.mathjax`_, which uses
 `MathJax`_ for rendering.
 
@@ -42,17 +41,14 @@
 
 .. _Sphinx extension: http://www.sphinx-doc.org/en/master/extensions.html
 .. _MathJax: https://www.mathjax.org
 .. _KaTeX: https://khan.github.io/KaTeX/
 .. _sphinx.ext.mathjax:
     https://github.com/sphinx-doc/sphinx/blob/master/sphinx/ext/mathjax.py
 
-.. |tests| image:: https://github.com/hagenw/sphinxcontrib-katex/workflows/Test/badge.svg
-    :target: https://github.com/hagenw/sphinxcontrib-katex/actions?query=workflow%3ATest
-    :alt: Test status
 .. |docs| image:: https://readthedocs.org/projects/sphinxcontrib-katex/badge/
     :target: https://sphinxcontrib-katex.readthedocs.io/
     :alt: sphinxcontrib.katex's documentation on Read the Docs
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
     :target: https://github.com/hagenw/sphinxcontrib-katex/blob/master/LICENSE
     :alt: sphinxcontrib.katex's MIT license
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/sphinxcontrib-katex.svg
@@ -105,15 +101,15 @@
 The behavior of ``sphinxcontrib.katex`` can be changed by configuration
 entries in ``conf.py`` of your documentation project. In the following
 all configuration entries are listed and their default values are shown.
 
 .. code-block:: python
 
     katex_css_path = \
-        'https://cdn.jsdelivr.net/npm/katex@0.16.7/dist/katex.min.css'
+        'https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css'
     katex_js_path = 'katex.min.js'
     katex_autorender_path = 'auto-render.min.js'
     katex_inline = [r'\(', r'\)']
     katex_display = [r'\[', r'\]']
     katex_prerender = False
     katex_options = ''
 
@@ -201,14 +197,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.7 (2023-07-03)
+--------------------------
+
+* Changed: use KaTeX 0.16.8
+* Removed: support for Python 3.7
+
+
 Version 0.9.6 (2023-06-13)
 --------------------------
 
 * Changed: use custom sphinx theme
   based on ``insipid``
   for HTML documentation pages
```

### Comparing `sphinxcontrib-katex-0.9.6/README.rst` & `sphinxcontrib-katex-0.9.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 sphinxcontrib-katex
 ===================
 
-|tests| |docs| |python-versions| |license|
+|docs| |python-versions| |license|
 
 A `Sphinx extension`_ for rendering math in HTML pages.
 
 The extension uses `KaTeX`_ for rendering of math in HTML pages. It is designed
 as a replacement for the built-in extension `sphinx.ext.mathjax`_, which uses
 `MathJax`_ for rendering.
 
@@ -17,17 +17,14 @@
 
 .. _Sphinx extension: http://www.sphinx-doc.org/en/master/extensions.html
 .. _MathJax: https://www.mathjax.org
 .. _KaTeX: https://khan.github.io/KaTeX/
 .. _sphinx.ext.mathjax:
     https://github.com/sphinx-doc/sphinx/blob/master/sphinx/ext/mathjax.py
 
-.. |tests| image:: https://github.com/hagenw/sphinxcontrib-katex/workflows/Test/badge.svg
-    :target: https://github.com/hagenw/sphinxcontrib-katex/actions?query=workflow%3ATest
-    :alt: Test status
 .. |docs| image:: https://readthedocs.org/projects/sphinxcontrib-katex/badge/
     :target: https://sphinxcontrib-katex.readthedocs.io/
     :alt: sphinxcontrib.katex's documentation on Read the Docs
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
     :target: https://github.com/hagenw/sphinxcontrib-katex/blob/master/LICENSE
     :alt: sphinxcontrib.katex's MIT license
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/sphinxcontrib-katex.svg
@@ -80,15 +77,15 @@
 The behavior of ``sphinxcontrib.katex`` can be changed by configuration
 entries in ``conf.py`` of your documentation project. In the following
 all configuration entries are listed and their default values are shown.
 
 .. code-block:: python
 
     katex_css_path = \
-        'https://cdn.jsdelivr.net/npm/katex@0.16.7/dist/katex.min.css'
+        'https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css'
     katex_js_path = 'katex.min.js'
     katex_autorender_path = 'auto-render.min.js'
     katex_inline = [r'\(', r'\)']
     katex_display = [r'\[', r'\]']
     katex_prerender = False
     katex_options = ''
```

### Comparing `sphinxcontrib-katex-0.9.6/docs/conf.py` & `sphinxcontrib-katex-0.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/docs/definitions.py` & `sphinxcontrib-katex-0.9.7/docs/definitions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/docs/examples.rst` & `sphinxcontrib-katex-0.9.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/docs/index.rst` & `sphinxcontrib-katex-0.9.7/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. include:: ../README.rst
-    :end-line: 37
+    :end-line: 34
 
 .. toctree::
     :hidden:
     :maxdepth: 2
 
     installation
     usage
```

### Comparing `sphinxcontrib-katex-0.9.6/setup.cfg` & `sphinxcontrib-katex-0.9.7/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Topic :: Documentation
 	Topic :: Utilities
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 packages = find_namespace:
```

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib/auto-render.min.js` & `sphinxcontrib-katex-0.9.7/sphinxcontrib/auto-render.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-math.css` & `sphinxcontrib-katex-0.9.7/sphinxcontrib/katex-math.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-server.js` & `sphinxcontrib-katex-0.9.7/sphinxcontrib/katex-server.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.min.js` & `sphinxcontrib-katex-0.9.7/sphinxcontrib/katex.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -17,27 +17,25 @@
             t = {};
         e.d(t, {
             default: function() {
                 return na
             }
         });
         var r = function e(t, r) {
-            this.position = void 0;
-            var n, a = "KaTeX parse error: " + t,
-                i = r && r.loc;
-            if (i && i.start <= i.end) {
-                var o = i.lexer.input;
-                n = i.start;
-                var s = i.end;
-                n === o.length ? a += " at end of input: " : a += " at position " + (n + 1) + ": ";
-                var l = o.slice(n, s).replace(/[^]/g, "$&\u0332");
-                a += (n > 15 ? "\u2026" + o.slice(n - 15, n) : o.slice(0, n)) + l + (s + 15 < o.length ? o.slice(s, s + 15) + "\u2026" : o.slice(s))
+            this.name = void 0, this.position = void 0, this.length = void 0, this.rawMessage = void 0;
+            var n, a, i = "KaTeX parse error: " + t,
+                o = r && r.loc;
+            if (o && o.start <= o.end) {
+                var s = o.lexer.input;
+                n = o.start, a = o.end, n === s.length ? i += " at end of input: " : i += " at position " + (n + 1) + ": ";
+                var l = s.slice(n, a).replace(/[^]/g, "$&\u0332");
+                i += (n > 15 ? "\u2026" + s.slice(n - 15, n) : s.slice(0, n)) + l + (a + 15 < s.length ? s.slice(a, a + 15) + "\u2026" : s.slice(a))
             }
-            var h = new Error(a);
-            return h.name = "ParseError", h.__proto__ = e.prototype, h.position = n, h
+            var h = new Error(i);
+            return h.name = "ParseError", h.__proto__ = e.prototype, h.position = n, null != n && null != a && (h.length = a - n), h.rawMessage = t, h
         };
         r.prototype.__proto__ = Error.prototype;
         var n = r,
             a = /([A-Z])/g,
             i = {
                 "&": "&amp;",
                 ">": "&gt;",
@@ -9512,15 +9510,15 @@
                     var n = Qn(e, r);
                     return Lt(n, e, r)
                 } catch (t) {
                     return ta(t, e, r)
                 }
             },
             na = {
-                version: "0.16.7",
+                version: "0.16.8",
                 render: ea,
                 renderToString: function(e, t) {
                     return ra(e, t).toMarkup()
                 },
                 ParseError: n,
                 SETTINGS_SCHEMA: h,
                 __parse: function(e, t) {
```

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.py` & `sphinxcontrib-katex-0.9.7/sphinxcontrib/katex.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from subprocess import PIPE, Popen, TimeoutExpired
 
 from sphinx.locale import _
 from sphinx.errors import ExtensionError
 from sphinx.util.osutil import copyfile
 
 
-__version__ = '0.9.6'
-katex_version = '0.16.7'
+__version__ = '0.9.7'
+katex_version = '0.16.8'
 filename_css = 'katex-math.css'
 filename_autorenderer = 'katex_autorenderer.js'
 SRC_DIR = Path(__file__).parent
 SCRIPT_PATH = str(SRC_DIR / "katex-server.js")
 
 ONE_MILLISECOND = 0.001
```

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/PKG-INFO` & `sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.6
+Version: 0.9.7
 Summary: A Sphinx extension for rendering math in HTML pages
 Home-page: https://github.com/hagenw/sphinxcontrib-katex
 Author: Hagen Wierstorf
 Author-email: hagenw@posteo.de
 License: MIT
 Keywords: sphinx,latex,katex,math,documentation
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
 
 sphinxcontrib-katex
 ===================
 
-|tests| |docs| |python-versions| |license|
+|docs| |python-versions| |license|
 
 A `Sphinx extension`_ for rendering math in HTML pages.
 
 The extension uses `KaTeX`_ for rendering of math in HTML pages. It is designed
 as a replacement for the built-in extension `sphinx.ext.mathjax`_, which uses
 `MathJax`_ for rendering.
 
@@ -42,17 +41,14 @@
 
 .. _Sphinx extension: http://www.sphinx-doc.org/en/master/extensions.html
 .. _MathJax: https://www.mathjax.org
 .. _KaTeX: https://khan.github.io/KaTeX/
 .. _sphinx.ext.mathjax:
     https://github.com/sphinx-doc/sphinx/blob/master/sphinx/ext/mathjax.py
 
-.. |tests| image:: https://github.com/hagenw/sphinxcontrib-katex/workflows/Test/badge.svg
-    :target: https://github.com/hagenw/sphinxcontrib-katex/actions?query=workflow%3ATest
-    :alt: Test status
 .. |docs| image:: https://readthedocs.org/projects/sphinxcontrib-katex/badge/
     :target: https://sphinxcontrib-katex.readthedocs.io/
     :alt: sphinxcontrib.katex's documentation on Read the Docs
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
     :target: https://github.com/hagenw/sphinxcontrib-katex/blob/master/LICENSE
     :alt: sphinxcontrib.katex's MIT license
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/sphinxcontrib-katex.svg
@@ -105,15 +101,15 @@
 The behavior of ``sphinxcontrib.katex`` can be changed by configuration
 entries in ``conf.py`` of your documentation project. In the following
 all configuration entries are listed and their default values are shown.
 
 .. code-block:: python
 
     katex_css_path = \
-        'https://cdn.jsdelivr.net/npm/katex@0.16.7/dist/katex.min.css'
+        'https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css'
     katex_js_path = 'katex.min.js'
     katex_autorender_path = 'auto-render.min.js'
     katex_inline = [r'\(', r'\)']
     katex_display = [r'\[', r'\]']
     katex_prerender = False
     katex_options = ''
 
@@ -201,14 +197,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.7 (2023-07-03)
+--------------------------
+
+* Changed: use KaTeX 0.16.8
+* Removed: support for Python 3.7
+
+
 Version 0.9.6 (2023-06-13)
 --------------------------
 
 * Changed: use custom sphinx theme
   based on ``insipid``
   for HTML documentation pages
```

### Comparing `sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/SOURCES.txt` & `sphinxcontrib-katex-0.9.7/sphinxcontrib_katex.egg-info/SOURCES.txt`

 * *Files identical despite different names*


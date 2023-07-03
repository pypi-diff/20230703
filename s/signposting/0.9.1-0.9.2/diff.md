# Comparing `tmp/signposting-0.9.1.tar.gz` & `tmp/signposting-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signposting-0.9.1.tar", last modified: Mon Oct  3 09:54:05 2022, max compression
+gzip compressed data, was "signposting-0.9.2.tar", last modified: Mon Jul  3 12:55:02 2023, max compression
```

## Comparing `signposting-0.9.1.tar` & `signposting-0.9.2.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.657442 signposting-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11945 2022-10-03 09:53:55.000000 signposting-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-10-03 09:53:55.000000 signposting-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2022-10-03 09:54:05.657442 signposting-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5268 2022-10-03 09:54:04.000000 signposting-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.653442 signposting-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7811 2022-10-03 09:54:04.000000 signposting-0.9.1/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6014 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/PULLREQUEST.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.653442 signposting-0.9.1/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-10-03 09:54:04.000000 signposting-0.9.1/docs/rst/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.653442 signposting-0.9.1/docs/rst/reference/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/reference/signposting.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/rst/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-03 09:53:55.000000 signposting-0.9.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 09:54:05.657442 signposting-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-10-03 09:54:04.000000 signposting-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.653442 signposting-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.657442 signposting-0.9.1/src/signposting/
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-10-03 09:54:04.000000 signposting-0.9.1/src/signposting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6361 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/htmllinks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6151 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/linkheader.py
--rw-r--r--   0 runner    (1001) docker     (121)     6709 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/linkset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)    35550 2022-10-03 09:53:55.000000 signposting-0.9.1/src/signposting/signpost.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 09:54:05.657442 signposting-0.9.1/src/signposting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 09:54:05.000000 signposting-0.9.1/src/signposting.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.578487 signposting-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 12:54:59.000000 signposting-0.9.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-07-03 12:54:50.000000 signposting-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 12:54:50.000000 signposting-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-07-03 12:55:02.578487 signposting-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-03 12:54:59.000000 signposting-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-03 12:54:59.000000 signposting-0.9.2/codemeta.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.574487 signposting-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-07-03 12:54:59.000000 signposting-0.9.2/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/PULLREQUEST.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.574487 signposting-0.9.2/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-03 12:54:59.000000 signposting-0.9.2/docs/rst/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.574487 signposting-0.9.2/docs/rst/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/reference/signposting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/rst/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 12:54:50.000000 signposting-0.9.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:55:02.578487 signposting-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-03 12:54:59.000000 signposting-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.570487 signposting-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.578487 signposting-0.9.2/src/signposting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-03 12:54:59.000000 signposting-0.9.2/src/signposting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/htmllinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/linkheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/linkset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35547 2023-07-03 12:54:50.000000 signposting-0.9.2/src/signposting/signpost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:55:02.578487 signposting-0.9.2/src/signposting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:55:02.000000 signposting-0.9.2/src/signposting.egg-info/zip-safe
```

### Comparing `signposting-0.9.1/LICENSE` & `signposting-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/PKG-INFO` & `signposting-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signposting
-Version: 0.9.1
+Version: 0.9.2
 Summary: Parse and navigate FAIR Signposting Link headers
 Home-page: https://github.com/stain/signposting
 Author: Stian Soiland-Reyes
 Author-email: stain@apache.org
 License: Apache License, version 2.0
 Project-URL: webpage, https://github.com/stain/signposting
 Project-URL: Documentation, https://signposting.readthedocs.io/en/latest/
@@ -145,15 +145,15 @@
 ======================
 
 As usual in any GitHub based project, raise an `issue`_ if you find any bug or have other suggestions; or open a `discussion`_  if you want to discuss or talk :-)
 
 Version
 =======
 
-v0.9.1
+v0.9.2
 
 .. _GitHub Actions: https://github.com/features/actions
 .. _PyPI: https://pypi.org
 .. _bump2version: https://github.com/c4urself/bump2version
 .. _discussion: https://github.com/stain/signposting/discussions
 .. _documentation: https://signposting.readthedocs.io/
 .. _issue: https://github.com/stain/signposting/issues
@@ -170,16 +170,23 @@
 .. _urllib: https://docs.python.org/3/library/urllib.html
 .. _linkset: https://signposting.org/FAIR/#linksetrec
 .. _authors: https://signposting.readthedocs.io/en/latest/authors.html
 
 Changelog
 =========
 
+v0.9.2 (2023-07-03)
+------------------------------------------------------------
+
+* Added `CITATION.cff`
+* Allow `#fragments` in profile URIs (e.g. for JSON-LD)
+
 v0.9.1 (2022-10-03)
 ------------------------------------------------------------
+* Added `codemeta.json` and contributors
 
 v0.9.0 (2022-10-03)
 ------------------------------------------------------------
 
 * Deprecated ``Signposting.context_url``, use ``Signposting.context`` instead
 * Removed deprecated ``find_signposting`` method, use ``find_signposting_http_link``
```

### Comparing `signposting-0.9.1/README.rst` & `signposting-0.9.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 ======================
 
 As usual in any GitHub based project, raise an `issue`_ if you find any bug or have other suggestions; or open a `discussion`_  if you want to discuss or talk :-)
 
 Version
 =======
 
-v0.9.1
+v0.9.2
 
 .. _GitHub Actions: https://github.com/features/actions
 .. _PyPI: https://pypi.org
 .. _bump2version: https://github.com/c4urself/bump2version
 .. _discussion: https://github.com/stain/signposting/discussions
 .. _documentation: https://signposting.readthedocs.io/
 .. _issue: https://github.com/stain/signposting/issues
```

### Comparing `signposting-0.9.1/docs/CHANGELOG.rst` & `signposting-0.9.2/docs/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 Changelog
 =========
 
+v0.9.2 (2023-07-03)
+------------------------------------------------------------
+
+* Added `CITATION.cff`
+* Allow `#fragments` in profile URIs (e.g. for JSON-LD)
+
 v0.9.1 (2022-10-03)
 ------------------------------------------------------------
+* Added `codemeta.json` and contributors
 
 v0.9.0 (2022-10-03)
 ------------------------------------------------------------
 
 * Deprecated ``Signposting.context_url``, use ``Signposting.context`` instead
 * Removed deprecated ``find_signposting`` method, use ``find_signposting_http_link``
```

### Comparing `signposting-0.9.1/docs/CONTRIBUTING.rst` & `signposting-0.9.2/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/docs/rst/conf.py` & `signposting-0.9.2/docs/rst/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'signposting link parser'
 year = '2022'
 author = 'Stian Soiland-Reyes'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '0.9.1'
+version = release = '0.9.2'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/stain/signposting/issues/%s', '#'),  # noqa: E501
     'pr': ('https://github.com/stain/signposting/pull/%s', 'PR #'),  # noqa: E501
     }
```

### Comparing `signposting-0.9.1/docs/rst/usage.rst` & `signposting-0.9.2/docs/rst/usage.rst`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/setup.py` & `signposting-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 long_description = '{}\n{}'.format(
     read('README.rst'),
     read(join('docs', 'CHANGELOG.rst')),
     )
 
 setup(
     name='signposting',
-    version='0.9.1',
+    version='0.9.2',
     description='Parse and navigate FAIR Signposting Link headers',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     license='Apache License, version 2.0',
     author='Stian Soiland-Reyes',
     author_email='stain@apache.org',
     url='https://github.com/stain/signposting',
```

### Comparing `signposting-0.9.1/src/signposting/__init__.py` & `signposting-0.9.2/src/signposting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 .. _signposting: https://signposting.org/conventions/
 .. _FAIR: https://signposting.org/FAIR/
 .. _Link Relation: https://www.iana.org/assignments/link-relations/
 .. _rdflib: https://rdflib.readthedocs.io/en/stable/
 .. _Link set: <https://signposting.org/FAIR/#linksetrec>
 """
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 from typing import List
 import warnings
 from .signpost import Signposting, Signpost, AbsoluteURI, MediaType, LinkRel
 from .linkheader import find_signposting_http_link
 from .resolver import find_signposting_http
 from .htmllinks import find_signposting_html
```

### Comparing `signposting-0.9.1/src/signposting/__main__.py` & `signposting-0.9.2/src/signposting/__main__.py`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/src/signposting/cli.py` & `signposting-0.9.2/src/signposting/cli.py`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/src/signposting/htmllinks.py` & `signposting-0.9.2/src/signposting/htmllinks.py`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/src/signposting/linkheader.py` & `signposting-0.9.2/src/signposting/linkheader.py`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/src/signposting/linkset.py` & `signposting-0.9.2/src/signposting/linkset.py`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/src/signposting/resolver.py` & `signposting-0.9.2/src/signposting/resolver.py`

 * *Files identical despite different names*

### Comparing `signposting-0.9.1/src/signposting/signpost.py` & `signposting-0.9.2/src/signposting/signpost.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         :raise ValueError: if the final URI reference is invalid or not absolute.
         """
         if isinstance(value, cls):
             return value # Already AbsoluteURI, no need to check again
         # Resolve potentially relative URI reference when base is given
         uri = urljoin(base or "", value)
         # will throw ValueError if resolved URI is not valid
-        rfc3987.parse(uri, rule="absolute_URI")
+        rfc3987.parse(uri, rule="URI")
         return super(AbsoluteURI, cls).__new__(cls, uri)
 
     # @staticmethod
     # def from_iri(cls, value: str, base: Optional[str] = None):
     #    """https://stackoverflow.com/a/49620774"""
     #    iri = rfc3987.parse(uri, rule="absolute_IRI")
     #    netloc = iri["authority"] and iri["netloc"].encode('idna').decode('ascii')
@@ -661,15 +661,15 @@
         """Calculate a hash of this Signposting instance based on its equality.
         
         The result of this hash method is consistent with :meth:`__eq__` in that
         only each signpost of the current context are part of the calculation.
         """
         h = hash(self.__class__.__qualname__)
         # NOTE context is NOT included in equality checks, see __eq__
-        ## h ^= self.context
+        ## h ^= hash(self.context)
         for e in self:
             # We use a naive XOR here as order should NOT matter
             h ^= hash(e)
         # Signposts in other contexts are ignored
         ##for e in self._others:
         ##    h ^= hash(e)
         return h
```

### Comparing `signposting-0.9.1/src/signposting.egg-info/PKG-INFO` & `signposting-0.9.2/src/signposting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signposting
-Version: 0.9.1
+Version: 0.9.2
 Summary: Parse and navigate FAIR Signposting Link headers
 Home-page: https://github.com/stain/signposting
 Author: Stian Soiland-Reyes
 Author-email: stain@apache.org
 License: Apache License, version 2.0
 Project-URL: webpage, https://github.com/stain/signposting
 Project-URL: Documentation, https://signposting.readthedocs.io/en/latest/
@@ -145,15 +145,15 @@
 ======================
 
 As usual in any GitHub based project, raise an `issue`_ if you find any bug or have other suggestions; or open a `discussion`_  if you want to discuss or talk :-)
 
 Version
 =======
 
-v0.9.1
+v0.9.2
 
 .. _GitHub Actions: https://github.com/features/actions
 .. _PyPI: https://pypi.org
 .. _bump2version: https://github.com/c4urself/bump2version
 .. _discussion: https://github.com/stain/signposting/discussions
 .. _documentation: https://signposting.readthedocs.io/
 .. _issue: https://github.com/stain/signposting/issues
@@ -170,16 +170,23 @@
 .. _urllib: https://docs.python.org/3/library/urllib.html
 .. _linkset: https://signposting.org/FAIR/#linksetrec
 .. _authors: https://signposting.readthedocs.io/en/latest/authors.html
 
 Changelog
 =========
 
+v0.9.2 (2023-07-03)
+------------------------------------------------------------
+
+* Added `CITATION.cff`
+* Allow `#fragments` in profile URIs (e.g. for JSON-LD)
+
 v0.9.1 (2022-10-03)
 ------------------------------------------------------------
+* Added `codemeta.json` and contributors
 
 v0.9.0 (2022-10-03)
 ------------------------------------------------------------
 
 * Deprecated ``Signposting.context_url``, use ``Signposting.context`` instead
 * Removed deprecated ``find_signposting`` method, use ``find_signposting_http_link``
```

### Comparing `signposting-0.9.1/src/signposting.egg-info/SOURCES.txt` & `signposting-0.9.2/src/signposting.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+CITATION.cff
 LICENSE
 MANIFEST.in
 README.rst
+codemeta.json
 setup.py
 docs/AUTHORS.rst
 docs/CHANGELOG.rst
 docs/CONTRIBUTING.rst
 docs/PULLREQUEST.rst
 docs/spelling_wordlist.txt
 docs/rst/authors.rst
```


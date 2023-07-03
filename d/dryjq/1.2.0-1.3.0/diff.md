# Comparing `tmp/dryjq-1.2.0.tar.gz` & `tmp/dryjq-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dryjq-1.2.0.tar", last modified: Thu Feb 16 10:48:39 2023, max compression
+gzip compressed data, was "dryjq-1.3.0.tar", last modified: Mon Jul  3 06:26:04 2023, max compression
```

## Comparing `dryjq-1.2.0.tar` & `dryjq-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 10:48:39.211168 dryjq-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-02-16 10:48:22.000000 dryjq-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5340 2023-02-16 10:48:39.210168 dryjq-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-02-16 10:48:22.000000 dryjq-1.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-02-16 10:48:22.000000 dryjq-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-16 10:48:39.211168 dryjq-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 10:48:39.200167 dryjq-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 10:48:39.205168 dryjq-1.2.0/src/dryjq/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    11213 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/access.py
--rw-rw-rw-   0 root         (0) root         (0)    12657 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/commandline.py
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/commons.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/merge.py
--rw-rw-rw-   0 root         (0) root         (0)    23537 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-02-16 10:48:22.000000 dryjq-1.2.0/src/dryjq/streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 10:48:39.207168 dryjq-1.2.0/src/dryjq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5340 2023-02-16 10:48:39.000000 dryjq-1.2.0/src/dryjq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      655 2023-02-16 10:48:39.000000 dryjq-1.2.0/src/dryjq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 10:48:39.000000 dryjq-1.2.0/src/dryjq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-02-16 10:48:39.000000 dryjq-1.2.0/src/dryjq.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-16 10:48:39.000000 dryjq-1.2.0/src/dryjq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-16 10:48:39.000000 dryjq-1.2.0/src/dryjq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 10:48:39.210168 dryjq-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    15178 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_access.py
--rw-rw-rw-   0 root         (0) root         (0)     1360 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_access_merge.py
--rw-rw-rw-   0 root         (0) root         (0)    10549 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_commandline.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_commons.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_convert.py
--rw-rw-rw-   0 root         (0) root         (0)     9120 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_main_file.py
--rw-rw-rw-   0 root         (0) root         (0)    10270 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_main_stdin.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)    15335 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_queries.py
--rw-rw-rw-   0 root         (0) root         (0)    11435 2023-02-16 10:48:22.000000 dryjq-1.2.0/tests/test_streams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:26:04.467598 dryjq-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-07-03 06:25:53.000000 dryjq-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-07-03 06:26:04.467598 dryjq-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-07-03 06:25:53.000000 dryjq-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2023-07-03 06:25:53.000000 dryjq-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 06:26:04.467598 dryjq-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:26:04.461598 dryjq-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:26:04.463598 dryjq-1.3.0/src/dryjq/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11213 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12657 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/commons.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/merge.py
+-rw-rw-rw-   0 root         (0) root         (0)    23537 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-03 06:25:53.000000 dryjq-1.3.0/src/dryjq/streams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:26:04.464598 dryjq-1.3.0/src/dryjq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-07-03 06:26:04.000000 dryjq-1.3.0/src/dryjq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      655 2023-07-03 06:26:04.000000 dryjq-1.3.0/src/dryjq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 06:26:04.000000 dryjq-1.3.0/src/dryjq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-03 06:26:04.000000 dryjq-1.3.0/src/dryjq.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-03 06:26:04.000000 dryjq-1.3.0/src/dryjq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-03 06:26:04.000000 dryjq-1.3.0/src/dryjq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:26:04.466598 dryjq-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    15178 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_access_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)    10549 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_commons.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_main_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_main_stdin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)    15335 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    11435 2023-07-03 06:25:53.000000 dryjq-1.3.0/tests/test_streams.py
```

### Comparing `dryjq-1.2.0/LICENSE` & `dryjq-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/PKG-INFO` & `dryjq-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dryjq
-Version: 1.2.0
+Version: 1.3.0
 Summary: Drastically Reduced YAML / JSON Query
 Author-email: Rainer Schwarzbach <undisclosed@example.com>
 License: MIT License
         
         Copyright (c) 2021 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,35 +21,36 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://gitlab.com/blackstream-x/python-dryjq
-Project-URL: documentation, https://blackstream-x.gitlab.io/python-dryjq
-Project-URL: repository, https://gitlab.com/blackstream-x/python-dryjq.git
+Project-URL: Homepage, https://gitlab.com/blackstream-x/python-dryjq
+Project-URL: Documentation, https://blackstream-x.gitlab.io/python-dryjq
+Project-URL: CI, https://gitlab.com/blackstream-x/python-dryjq/-/pipelines
 Project-URL: Bug Tracker, https://gitlab.com/blackstream-x/python-dryjq/-/issues
+Project-URL: Source Code, https://gitlab.com/blackstream-x/python-dryjq.git
 Keywords: json,yaml,query,extract,convert,merge
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Drastically Reduced YAML / JSON Query
 
 Lightweight package providing a subset of
 [yq](https://mikefarah.gitbook.io/yq/) or
```

### Comparing `dryjq-1.2.0/README.md` & `dryjq-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/pyproject.toml` & `dryjq-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,47 +3,48 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dryjq"
 dynamic = ["version"]
 description = "Drastically Reduced YAML / JSON Query"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["json", "yaml", "query", "extract", "convert", "merge"]
 authors = [
   {name = "Rainer Schwarzbach", email = "undisclosed@example.com"},
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Topic :: Text Processing :: Filters",
   "Topic :: Utilities",
 ]
 
 dependencies = [
-  "PyYAML>=5.4.1",
+  "PyYAML>=6.0",
 ]
 
 [project.urls]
-homepage = "https://gitlab.com/blackstream-x/python-dryjq"
-documentation = "https://blackstream-x.gitlab.io/python-dryjq"
-repository = "https://gitlab.com/blackstream-x/python-dryjq.git"
+Homepage = "https://gitlab.com/blackstream-x/python-dryjq"
+Documentation = "https://blackstream-x.gitlab.io/python-dryjq"
+CI = "https://gitlab.com/blackstream-x/python-dryjq/-/pipelines"
 "Bug Tracker" = "https://gitlab.com/blackstream-x/python-dryjq/-/issues"
+"Source Code" = "https://gitlab.com/blackstream-x/python-dryjq.git"
 
 [project.scripts]
 dryjq = "dryjq.__main__:main"
 "dryjq.convert" = "dryjq.convert:main"
 "dryjq.merge" = "dryjq.merge:main"
 
 [tool.setuptools.dynamic]
```

### Comparing `dryjq-1.2.0/src/dryjq/__init__.py` & `dryjq-1.3.0/src/dryjq/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 dryjq is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 
 # vim: fileencoding=utf-8 ts=4 sts=4 sw=4 autoindent expandtab syntax=python:
```

### Comparing `dryjq-1.2.0/src/dryjq/__main__.py` & `dryjq-1.3.0/src/dryjq/__main__.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/access.py` & `dryjq-1.3.0/src/dryjq/access.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/commandline.py` & `dryjq-1.3.0/src/dryjq/commandline.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/commons.py` & `dryjq-1.3.0/src/dryjq/commons.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/convert.py` & `dryjq-1.3.0/src/dryjq/convert.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/merge.py` & `dryjq-1.3.0/src/dryjq/merge.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/queries.py` & `dryjq-1.3.0/src/dryjq/queries.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq/streams.py` & `dryjq-1.3.0/src/dryjq/streams.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/src/dryjq.egg-info/PKG-INFO` & `dryjq-1.3.0/src/dryjq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dryjq
-Version: 1.2.0
+Version: 1.3.0
 Summary: Drastically Reduced YAML / JSON Query
 Author-email: Rainer Schwarzbach <undisclosed@example.com>
 License: MIT License
         
         Copyright (c) 2021 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,35 +21,36 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://gitlab.com/blackstream-x/python-dryjq
-Project-URL: documentation, https://blackstream-x.gitlab.io/python-dryjq
-Project-URL: repository, https://gitlab.com/blackstream-x/python-dryjq.git
+Project-URL: Homepage, https://gitlab.com/blackstream-x/python-dryjq
+Project-URL: Documentation, https://blackstream-x.gitlab.io/python-dryjq
+Project-URL: CI, https://gitlab.com/blackstream-x/python-dryjq/-/pipelines
 Project-URL: Bug Tracker, https://gitlab.com/blackstream-x/python-dryjq/-/issues
+Project-URL: Source Code, https://gitlab.com/blackstream-x/python-dryjq.git
 Keywords: json,yaml,query,extract,convert,merge
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Drastically Reduced YAML / JSON Query
 
 Lightweight package providing a subset of
 [yq](https://mikefarah.gitbook.io/yq/) or
```

### Comparing `dryjq-1.2.0/src/dryjq.egg-info/SOURCES.txt` & `dryjq-1.3.0/src/dryjq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_access.py` & `dryjq-1.3.0/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_access_merge.py` & `dryjq-1.3.0/tests/test_access_merge.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_commandline.py` & `dryjq-1.3.0/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_commons.py` & `dryjq-1.3.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_convert.py` & `dryjq-1.3.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_main_file.py` & `dryjq-1.3.0/tests/test_main_file.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_main_stdin.py` & `dryjq-1.3.0/tests/test_main_stdin.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_merge.py` & `dryjq-1.3.0/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_queries.py` & `dryjq-1.3.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `dryjq-1.2.0/tests/test_streams.py` & `dryjq-1.3.0/tests/test_streams.py`

 * *Files identical despite different names*


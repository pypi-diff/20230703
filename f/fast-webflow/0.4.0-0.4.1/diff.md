# Comparing `tmp/fast-webflow-0.4.0.tar.gz` & `tmp/fast-webflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.4.0.tar", last modified: Mon Jul  3 20:10:39 2023, max compression
+gzip compressed data, was "fast-webflow-0.4.1.tar", last modified: Mon Jul  3 20:19:38 2023, max compression
```

## Comparing `fast-webflow-0.4.0.tar` & `fast-webflow-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/webflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/webflow/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.327749 fast-webflow-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 20:19:38.000000 fast-webflow-0.4.1/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/src/webflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/src/webflow/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/src/webflow/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:19:38.331749 fast-webflow-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 20:19:29.000000 fast-webflow-0.4.1/tests/test_site.py
```

### Comparing `fast-webflow-0.4.0/LICENSE` & `fast-webflow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.0/PKG-INFO` & `fast-webflow-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,29 +13,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to fast-webflow
 a WebFlow CMS API Client in Python
 
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
-[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
+[![PyPI version](https://badge.fury.io/py/fast-webflow.svg)](https://badge.fury.io/py/fast-webflow)
+[![PyPI stats](https://img.shields.io/pypi/dm/fast-webflow.svg)](https://img.shields.io/pypi/dm/fast-webflow.svg)
 
 This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
 
 > Check out an example website built with the help of `fast-webflow`: [**liguriasegreta.com**](https://www.liguriasegreta.com)
 
 **DISCLAIMER**  : This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
 
 
 ## Roadmap
 - [ ] Add *e-commerce* functionality
 - [ ] Add *membership* functionality
 - [ ] Add tests
-- [ ] Finish documentation
+- [x] Finish documentation
 - [x] Publish to PyPi
 
 
 ## Features
 - **Authenticate** with the WebFlow API using your API key
 - **Fetch**, **Create**, **Update**, and **Delete** Items and files from WebFlow Collections
 - Handle **pagination** for large Collections
```

### Comparing `fast-webflow-0.4.0/README.md` & `fast-webflow-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Welcome to fast-webflow
 a WebFlow CMS API Client in Python
 
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
-[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
+[![PyPI version](https://badge.fury.io/py/fast-webflow.svg)](https://badge.fury.io/py/fast-webflow)
+[![PyPI stats](https://img.shields.io/pypi/dm/fast-webflow.svg)](https://img.shields.io/pypi/dm/fast-webflow.svg)
 
 This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
 
 > Check out an example website built with the help of `fast-webflow`: [**liguriasegreta.com**](https://www.liguriasegreta.com)
 
 **DISCLAIMER**  : This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
 
 
 ## Roadmap
 - [ ] Add *e-commerce* functionality
 - [ ] Add *membership* functionality
 - [ ] Add tests
-- [ ] Finish documentation
+- [x] Finish documentation
 - [x] Publish to PyPi
 
 
 ## Features
 - **Authenticate** with the WebFlow API using your API key
 - **Fetch**, **Create**, **Update**, and **Delete** Items and files from WebFlow Collections
 - Handle **pagination** for large Collections
```

### Comparing `fast-webflow-0.4.0/setup.cfg` & `fast-webflow-0.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.4.0
+version = 0.4.1
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.4.0/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.4.1/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,29 +13,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to fast-webflow
 a WebFlow CMS API Client in Python
 
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
-[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
+[![PyPI version](https://badge.fury.io/py/fast-webflow.svg)](https://badge.fury.io/py/fast-webflow)
+[![PyPI stats](https://img.shields.io/pypi/dm/fast-webflow.svg)](https://img.shields.io/pypi/dm/fast-webflow.svg)
 
 This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
 
 > Check out an example website built with the help of `fast-webflow`: [**liguriasegreta.com**](https://www.liguriasegreta.com)
 
 **DISCLAIMER**  : This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
 
 
 ## Roadmap
 - [ ] Add *e-commerce* functionality
 - [ ] Add *membership* functionality
 - [ ] Add tests
-- [ ] Finish documentation
+- [x] Finish documentation
 - [x] Publish to PyPi
 
 
 ## Features
 - **Authenticate** with the WebFlow API using your API key
 - **Fetch**, **Create**, **Update**, and **Delete** Items and files from WebFlow Collections
 - Handle **pagination** for large Collections
```

### Comparing `fast-webflow-0.4.0/src/webflow/cms/collection.py` & `fast-webflow-0.4.1/src/webflow/cms/collection.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.0/src/webflow/cms/config.py` & `fast-webflow-0.4.1/src/webflow/cms/config.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.0/src/webflow/cms/item.py` & `fast-webflow-0.4.1/src/webflow/cms/item.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.0/src/webflow/cms/site.py` & `fast-webflow-0.4.1/src/webflow/cms/site.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.0/src/webflow/cms/utils.py` & `fast-webflow-0.4.1/src/webflow/cms/utils.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.4.0/tests/test_site.py` & `fast-webflow-0.4.1/tests/test_site.py`

 * *Files identical despite different names*


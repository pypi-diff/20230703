# Comparing `tmp/fast-webflow-0.3.3.tar.gz` & `tmp/fast-webflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.3.3.tar", last modified: Sun Jul  2 22:06:09 2023, max compression
+gzip compressed data, was "fast-webflow-0.4.0.tar", last modified: Mon Jul  3 20:10:39 2023, max compression
```

## Comparing `fast-webflow-0.3.3.tar` & `fast-webflow-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:05:54.000000 fast-webflow-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-02 22:05:54.000000 fast-webflow-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 22:06:09.624115 fast-webflow-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.616115 fast-webflow-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/src/webflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/src/webflow/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 20:10:39.000000 fast-webflow-0.4.0/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/webflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.459547 fast-webflow-0.4.0/src/webflow/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/src/webflow/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:39.463547 fast-webflow-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 20:10:30.000000 fast-webflow-0.4.0/tests/test_site.py
```

### Comparing `fast-webflow-0.3.3/LICENSE` & `fast-webflow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.3/PKG-INFO` & `fast-webflow-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.3.3
+Version: 0.4.0
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.3.3/README.md` & `fast-webflow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.3/setup.cfg` & `fast-webflow-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.3.3
+version = 0.4.0
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.3.3/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.4.0/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.3.3
+Version: 0.4.0
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.3.3/src/webflow/cms/collection.py` & `fast-webflow-0.4.0/src/webflow/cms/collection.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.3/src/webflow/cms/config.py` & `fast-webflow-0.4.0/src/webflow/cms/config.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.3/src/webflow/cms/item.py` & `fast-webflow-0.4.0/src/webflow/cms/item.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.3/src/webflow/cms/site.py` & `fast-webflow-0.4.0/src/webflow/cms/site.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.3/src/webflow/cms/utils.py` & `fast-webflow-0.4.0/src/webflow/cms/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/burla-0.0.1.tar.gz` & `tmp/burla-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.1.tar", max compression
+gzip compressed data, was "burla-0.0.2.tar", max compression
```

## Comparing `burla-0.0.1.tar` & `burla-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      600 2023-07-03 15:15:00.685178 burla-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.1/src/burla/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.1/src/burla/_logstream.py
--rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.1/src/burla/config.py
--rw-r--r--   0        0        0     3667 2023-07-03 15:14:20.481784 burla-0.0.1/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 burla-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-07-03 15:51:52.145949 burla-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.2/src/burla/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.2/src/burla/_logstream.py
+-rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.2/src/burla/config.py
+-rw-r--r--   0        0        0     3667 2023-07-03 15:43:06.056382 burla-0.0.2/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 burla-0.0.2/PKG-INFO
```

### Comparing `burla-0.0.1/pyproject.toml` & `burla-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "burla"
-version = "0.0.1"
+version = "0.0.2"
 description = "Make your python script 100x faster"
 authors = ["Jake Zuliani <jake@burla.dev>"]
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 dill = "^0.3.6"
 fire = "^0.5.0"
 docker = "^6.1.3"
 google-cloud-build = "^3.16.0"
 google-cloud-logging = "^3.5.0"
 grpcio = "^1.54.2"
 jupyterlab = "^4.0.2"
```

### Comparing `burla-0.0.1/src/burla/_logstream.py` & `burla-0.0.2/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.1/src/burla/config.py` & `burla-0.0.2/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.1/src/burla/remote_parallel_map.py` & `burla-0.0.2/src/burla/remote_parallel_map.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.1/PKG-INFO` & `burla-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.1
+Version: 0.0.2
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: google-cloud-build (>=3.16.0,<4.0.0)
 Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
```


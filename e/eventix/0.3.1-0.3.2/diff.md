# Comparing `tmp/eventix-0.3.1.tar.gz` & `tmp/eventix-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.3.1.tar", max compression
+gzip compressed data, was "eventix-0.3.2.tar", max compression
```

## Comparing `eventix-0.3.1.tar` & `eventix-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.3.1/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/functions/__init__.py
--rw-r--r--   0        0        0     3104 2023-07-03 12:35:26.922564 eventix-0.3.1/eventix/functions/core.py
--rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.3.1/eventix/functions/errors.py
--rw-r--r--   0        0        0      900 2023-07-03 12:36:13.218289 eventix-0.3.1/eventix/functions/eventix_client.py
--rw-r--r--   0        0        0     2552 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/functions/fastapi.py
--rw-r--r--   0        0        0     6082 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/functions/task.py
--rw-r--r--   0        0        0      990 2023-07-03 12:36:06.494329 eventix-0.3.1/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     3879 2023-07-03 12:37:58.589687 eventix-0.3.1/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/pydantic/event.py
--rw-r--r--   0        0        0     1951 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/router/__init__.py
--rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/router/event.py
--rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/router/metrics.py
--rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.3.1/eventix/router/task.py
--rw-r--r--   0        0        0      958 2023-07-03 12:48:18.787918 eventix-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 eventix-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.3.2/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/functions/__init__.py
+-rw-r--r--   0        0        0     3104 2023-07-03 12:35:26.922564 eventix-0.3.2/eventix/functions/core.py
+-rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.3.2/eventix/functions/errors.py
+-rw-r--r--   0        0        0      900 2023-07-03 12:36:13.218289 eventix-0.3.2/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2552 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0     6082 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/functions/task.py
+-rw-r--r--   0        0        0      990 2023-07-03 12:36:06.494329 eventix-0.3.2/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     3879 2023-07-03 12:37:58.589687 eventix-0.3.2/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/pydantic/event.py
+-rw-r--r--   0        0        0     1951 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/router/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/router/event.py
+-rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/router/metrics.py
+-rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.3.2/eventix/router/task.py
+-rw-r--r--   0        0        0      959 2023-07-03 13:28:20.414793 eventix-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 eventix-0.3.2/PKG-INFO
```

### Comparing `eventix-0.3.1/eventix/exceptions/__init__.py` & `eventix-0.3.2/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/core.py` & `eventix-0.3.2/eventix/functions/core.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/errors.py` & `eventix-0.3.2/eventix/functions/errors.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/eventix_client.py` & `eventix-0.3.2/eventix/functions/eventix_client.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/fastapi.py` & `eventix-0.3.2/eventix/functions/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/task.py` & `eventix-0.3.2/eventix/functions/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/task_scheduler.py` & `eventix-0.3.2/eventix/functions/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/functions/task_worker.py` & `eventix-0.3.2/eventix/functions/task_worker.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/pydantic/task.py` & `eventix-0.3.2/eventix/pydantic/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/router/event.py` & `eventix-0.3.2/eventix/router/event.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/eventix/router/task.py` & `eventix-0.3.2/eventix/router/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.1/pyproject.toml` & `eventix-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "eventix"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.95.1"
 uvicorn = "^0.22.0"
-python-dotenv = "^1.0.0"
+python-dotenv = "^0.15.0"
 pydash = "^7.0.3"
-pydantic-db-backend = {version = "^0.4.1", extras = ["couchdb"]}
+pydantic-db-backend = {version = "^0.4.2", extras = ["couchdb"]}
 psutil = "^5.9.5"
 requests = "^2.31.0"
 toml = "^0.10.2"
 webexception = "^1.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `eventix-0.3.1/PKG-INFO` & `eventix-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pydantic-db-backend[couchdb] (>=0.4.1,<0.5.0)
+Requires-Dist: pydantic-db-backend[couchdb] (>=0.4.2,<0.5.0)
 Requires-Dist: pydash (>=7.0.3,<8.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: webexception (>=1.0.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Eventix
```


# Comparing `tmp/mini_memgraph-0.1.1.tar.gz` & `tmp/mini_memgraph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_memgraph-0.1.1.tar", max compression
+gzip compressed data, was "mini_memgraph-0.1.2.tar", max compression
```

## Comparing `mini_memgraph-0.1.1.tar` & `mini_memgraph-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      726 2023-04-21 19:26:38.882323 mini_memgraph-0.1.1/README.md
--rw-r--r--   0        0        0       43 2023-04-19 22:06:02.794299 mini_memgraph-0.1.1/mini_memgraph/__init__.py
--rw-r--r--   0        0        0     2509 2023-04-19 22:55:12.409316 mini_memgraph-0.1.1/mini_memgraph/db.py
--rw-r--r--   0        0        0    13471 2023-04-21 22:25:00.110508 mini_memgraph-0.1.1/mini_memgraph/memgraph.py
--rw-r--r--   0        0        0      441 2023-04-19 22:06:02.800400 mini_memgraph-0.1.1/mini_memgraph/utility.py
--rw-r--r--   0        0        0      598 2023-04-27 20:31:41.101723 mini_memgraph-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 mini_memgraph-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      726 2023-04-21 19:26:38.882323 mini_memgraph-0.1.2/README.md
+-rw-r--r--   0        0        0       43 2023-04-19 22:06:02.794299 mini_memgraph-0.1.2/mini_memgraph/__init__.py
+-rw-r--r--   0        0        0     2509 2023-04-19 22:55:12.409316 mini_memgraph-0.1.2/mini_memgraph/db.py
+-rw-r--r--   0        0        0    13471 2023-04-21 22:25:00.110508 mini_memgraph-0.1.2/mini_memgraph/memgraph.py
+-rw-r--r--   0        0        0      441 2023-04-19 22:06:02.800400 mini_memgraph-0.1.2/mini_memgraph/utility.py
+-rw-r--r--   0        0        0      597 2023-07-03 08:45:29.818048 mini_memgraph-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 mini_memgraph-0.1.2/PKG-INFO
```

### Comparing `mini_memgraph-0.1.1/README.md` & `mini_memgraph-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mini_memgraph-0.1.1/mini_memgraph/db.py` & `mini_memgraph-0.1.2/mini_memgraph/db.py`

 * *Files identical despite different names*

### Comparing `mini_memgraph-0.1.1/mini_memgraph/memgraph.py` & `mini_memgraph-0.1.2/mini_memgraph/memgraph.py`

 * *Files identical despite different names*

### Comparing `mini_memgraph-0.1.1/pyproject.toml` & `mini_memgraph-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "mini-memgraph"
-version = "0.1.1"
+version = "0.1.2"
 description = "A basic wrapper to simplify interacting with a local Memgraph instance using Python."
 license = "MIT"
 authors = ["James Allen-Robertson <minyall@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Minyall/mini_memgraph"
 packages = [{include = "mini_memgraph"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Database"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 pymgclient = "^1.3.1"
 pandas = "^2.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mini_memgraph-0.1.1/PKG-INFO` & `mini_memgraph-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: mini-memgraph
-Version: 0.1.1
+Version: 0.1.2
 Summary: A basic wrapper to simplify interacting with a local Memgraph instance using Python.
 Home-page: https://github.com/Minyall/mini_memgraph
 License: MIT
 Author: James Allen-Robertson
 Author-email: minyall@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pymgclient (>=1.3.1,<2.0.0)
 Project-URL: Repository, https://github.com/Minyall/mini_memgraph
 Description-Content-Type: text/markdown
```


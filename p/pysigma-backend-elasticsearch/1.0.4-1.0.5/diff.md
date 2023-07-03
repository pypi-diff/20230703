# Comparing `tmp/pysigma_backend_elasticsearch-1.0.4.tar.gz` & `tmp/pysigma_backend_elasticsearch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_elasticsearch-1.0.4.tar", max compression
+gzip compressed data, was "pysigma_backend_elasticsearch-1.0.5.tar", max compression
```

## Comparing `pysigma_backend_elasticsearch-1.0.4.tar` & `pysigma_backend_elasticsearch-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7653 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/LICENSE
--rw-r--r--   0        0        0     1456 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/README.md
--rw-r--r--   0        0        0      978 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       93 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0    16130 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0      308 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/__init__.py
--rw-r--r--   0        0        0    10115 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/windows.py
--rw-r--r--   0        0        0    60963 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/zeek.py
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1450 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/README.md
+-rw-r--r--   0        0        0      978 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/sigma/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    16066 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/sigma/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0      308 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/sigma/pipelines/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    10115 2023-07-03 05:50:46.468416 pysigma_backend_elasticsearch-1.0.5/sigma/pipelines/elasticsearch/windows.py
+-rw-r--r--   0        0        0    60963 2023-07-03 05:50:46.472416 pysigma_backend_elasticsearch-1.0.5/sigma/pipelines/elasticsearch/zeek.py
+-rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.5/PKG-INFO
```

### Comparing `pysigma_backend_elasticsearch-1.0.4/LICENSE` & `pysigma_backend_elasticsearch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.4/README.md` & `pysigma_backend_elasticsearch-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![Tests](https://github.com/SigmaHQ/pySigma-backend-elasticsearch/actions/workflows/test.yml/badge.svg)
 ![Coverage
 Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/thomaspatzke/3c445ef26310e9f2d2ca09c697db1c71/raw/SigmaHQ-pySigma-backend-elasticsearch.json)
-![Status](https://img.shields.io/badge/Status-pre--release-orange)
+![Status](https://img.shields.io/badge/Status-release-green)
 
 # pySigma Elasticsearch Backend
 
 This is the Elasticsearch backend for pySigma. It provides the package `sigma.backends.elasticsearch` with the `LuceneBackend` class.
 
 It supports the following output formats:
```

### Comparing `pysigma_backend_elasticsearch-1.0.4/pyproject.toml` & `pysigma_backend_elasticsearch-1.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-elasticsearch"
-version = "1.0.4"
+version = "1.0.5"
 description = "pySigma Elasticsearch backend"
 readme = "README.md"
 authors = ["Thomas Patzke <thomas@patzke.org>", "Hendrik Baecker <hb@process-zero.de>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-elasticsearch"
 packages = [
     { include = "sigma" }
```

### Comparing `pysigma_backend_elasticsearch-1.0.4/sigma/backends/elasticsearch/elasticsearch.py` & `pysigma_backend_elasticsearch-1.0.5/sigma/backends/elasticsearch/elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,15 @@
     # Escaping character for special characrers inside string
     escape_char: ClassVar[str] = "\\"
     # Character used as multi-character wildcard
     wildcard_multi: ClassVar[str] = "*"
     # Character used as single-character wildcard
     wildcard_single: ClassVar[str] = "?"
     # Characters quoted in addition to wildcards and string quote
-    add_escaped: ClassVar[str] = '+-=&|!(){}[]^"~*?:\\/ '
-    filter_chars: ClassVar[str] = "<>"      # Characters filtered
+    add_escaped: ClassVar[str] = '+-=&|!(){}[]<>^"~*?:\\/ '
     bool_values: ClassVar[Dict[bool, str]] = {   # Values to which boolean values are mapped.
         True: "true",
         False: "false",
     }
 
     # Regular expressions
     # Regular expression query as format string with placeholders {field} and {regex}
```

### Comparing `pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/windows.py` & `pysigma_backend_elasticsearch-1.0.5/sigma/pipelines/elasticsearch/windows.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/zeek.py` & `pysigma_backend_elasticsearch-1.0.5/sigma/pipelines/elasticsearch/zeek.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.4/PKG-INFO` & `pysigma_backend_elasticsearch-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-elasticsearch
-Version: 1.0.4
+Version: 1.0.5
 Summary: pySigma Elasticsearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-elasticsearch
 License: LGPL-3.0-only
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -16,15 +16,15 @@
 Requires-Dist: pysigma (>=0.9.5,<0.10.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-elasticsearch
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/SigmaHQ/pySigma-backend-elasticsearch/actions/workflows/test.yml/badge.svg)
 ![Coverage
 Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/thomaspatzke/3c445ef26310e9f2d2ca09c697db1c71/raw/SigmaHQ-pySigma-backend-elasticsearch.json)
-![Status](https://img.shields.io/badge/Status-pre--release-orange)
+![Status](https://img.shields.io/badge/Status-release-green)
 
 # pySigma Elasticsearch Backend
 
 This is the Elasticsearch backend for pySigma. It provides the package `sigma.backends.elasticsearch` with the `LuceneBackend` class.
 
 It supports the following output formats:
```


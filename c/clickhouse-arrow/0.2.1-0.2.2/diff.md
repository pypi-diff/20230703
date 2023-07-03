# Comparing `tmp/clickhouse_arrow-0.2.1.tar.gz` & `tmp/clickhouse_arrow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse_arrow-0.2.1.tar", max compression
+gzip compressed data, was "clickhouse_arrow-0.2.2.tar", max compression
```

## Comparing `clickhouse_arrow-0.2.1.tar` & `clickhouse_arrow-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11361 2023-03-25 13:20:32.938480 clickhouse_arrow-0.2.1/LICENSE
--rw-r--r--   0        0        0     1275 2023-03-25 13:18:15.085427 clickhouse_arrow-0.2.1/README.md
--rw-r--r--   0        0        0     7489 2023-04-06 05:55:41.050547 clickhouse_arrow-0.2.1/clickhouse_arrow/__init__.py
--rw-r--r--   0        0        0      671 2023-04-06 05:56:18.336217 clickhouse_arrow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 clickhouse_arrow-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11361 2023-03-25 13:20:32.938480 clickhouse_arrow-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1275 2023-03-25 13:18:15.085427 clickhouse_arrow-0.2.2/README.md
+-rw-r--r--   0        0        0     7489 2023-04-06 05:55:41.050547 clickhouse_arrow-0.2.2/clickhouse_arrow/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-03 18:27:31.998121 clickhouse_arrow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 clickhouse_arrow-0.2.2/PKG-INFO
```

### Comparing `clickhouse_arrow-0.2.1/LICENSE` & `clickhouse_arrow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.2.1/README.md` & `clickhouse_arrow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.2.1/clickhouse_arrow/__init__.py` & `clickhouse_arrow-0.2.2/clickhouse_arrow/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.2.1/pyproject.toml` & `clickhouse_arrow-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "clickhouse-arrow"
-version = "0.2.1"
+version = "0.2.2"
 description = "A minimal client that uses the ClickHouse HTTP API and Apache Arrow."
 authors = ["Martin Galpin <galpin@galpin.com>"]
 homepage = "https://github.com/galpin/clickhouse-arrow"
 repository = "https://github.com/galpin/clickhouse-arrow"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pyarrow = "^11.0.0"
+pyarrow = ">=11.0.0"
+urllib3 = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-benchmark = "^4.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest-docker = "^1.0.1"
```

### Comparing `clickhouse_arrow-0.2.1/PKG-INFO` & `clickhouse_arrow-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: clickhouse-arrow
-Version: 0.2.1
+Version: 0.2.2
 Summary: A minimal client that uses the ClickHouse HTTP API and Apache Arrow.
 Home-page: https://github.com/galpin/clickhouse-arrow
 Author: Martin Galpin
 Author-email: galpin@galpin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: pyarrow (>=11.0.0)
+Requires-Dist: urllib3 (>=2.0.0)
 Project-URL: Repository, https://github.com/galpin/clickhouse-arrow
 Description-Content-Type: text/markdown
 
 # Clickhouse Arrow 🏠 🏹
 
 A minimal [ClickHouse](https://clickhouse.com) client that uses the HTTP API and Apache Arrow.
```


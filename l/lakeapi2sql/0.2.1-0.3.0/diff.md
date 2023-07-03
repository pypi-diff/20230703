# Comparing `tmp/lakeapi2sql-0.2.1.tar.gz` & `tmp/lakeapi2sql-0.3.0.tar.gz`

## Comparing `lakeapi2sql-0.2.1.tar` & `lakeapi2sql-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123      118 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/.editorconfig
--rw-r--r--   0     1001      123     2804 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3086 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/.gitignore
--rw-r--r--   0     1001      123     1081 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/LICENSE
--rw-r--r--   0     1001      123     1066 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/README.md
--rw-r--r--   0     1001      123        0 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      123      507 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      123        0 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/py.typed
--rw-r--r--   0     1001      123      587 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123    12800 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/arrow_convert.rs
--rw-r--r--   0     1001      123     2504 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/bulk_insert.rs
--rw-r--r--   0     1001      123     1568 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/connect.rs
--rw-r--r--   0     1001      123     2757 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/test/__init__.py
--rw-r--r--   0     1001      123     1977 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/test/test_insert.py
--rw-r--r--   0     1001      123    57698 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      118 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/.editorconfig
+-rw-r--r--   0     1001      123     2804 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3086 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/.gitignore
+-rw-r--r--   0     1001      123     1081 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     1066 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/README.md
+-rw-r--r--   0     1001      123        0 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      123     2184 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      123        0 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/py.typed
+-rw-r--r--   0     1001      123      656 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123    12800 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/arrow_convert.rs
+-rw-r--r--   0     1001      123     2504 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/bulk_insert.rs
+-rw-r--r--   0     1001      123     1568 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/connect.rs
+-rw-r--r--   0     1001      123     2757 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/test/__init__.py
+-rw-r--r--   0     1001      123     1977 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/test/test_insert.py
+-rw-r--r--   0     1001      123    57698 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.0/PKG-INFO
```

### Comparing `lakeapi2sql-0.2.1/Cargo.toml` & `lakeapi2sql-0.3.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/.github/workflows/CI.yml` & `lakeapi2sql-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/.gitignore` & `lakeapi2sql-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/LICENSE` & `lakeapi2sql-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/README.md` & `lakeapi2sql-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/pyproject.toml` & `lakeapi2sql-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.2.1"
+version = "0.3.0"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
+[project.optional-dependencies]
+azure = ["azure-identity>=1.12.0"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 module-name = "lakeapi2sql._lowlevel"
 
 
 [tool.pyright]
```

### Comparing `lakeapi2sql-0.2.1/src/arrow_convert.rs` & `lakeapi2sql-0.3.0/src/arrow_convert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/src/bulk_insert.rs` & `lakeapi2sql-0.3.0/src/bulk_insert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/src/connect.rs` & `lakeapi2sql-0.3.0/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/src/lib.rs` & `lakeapi2sql-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/test/test_insert.py` & `lakeapi2sql-0.3.0/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/Cargo.lock` & `lakeapi2sql-0.3.0/Cargo.lock`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.1/PKG-INFO` & `lakeapi2sql-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: lakeapi2sql
-Version: 0.2.1
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
+Provides-Extra: azure
 License-File: LICENSE
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # LakeApi 2 SQL
 
 This is a simple library that does a HTTP Request to an Endpoint from the Lake API and inserts the data via bulk insert into MS SQL Server. In Theory you could also get the data from some other HTTP Endpoint which returns an Arrow Stream and is authenticated using Basic Auth.
```


# Comparing `tmp/lakeapi2sql-0.2.0.tar.gz` & `tmp/lakeapi2sql-0.2.1.tar.gz`

## Comparing `lakeapi2sql-0.2.0.tar` & `lakeapi2sql-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      118 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/.editorconfig
--rw-r--r--   0     1001      123     2800 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3086 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1081 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1066 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/README.md
--rw-r--r--   0     1001      123        0 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      123      320 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      123      587 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123    12800 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/arrow_convert.rs
--rw-r--r--   0     1001      123     2504 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/bulk_insert.rs
--rw-r--r--   0     1001      123     1568 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/connect.rs
--rw-r--r--   0     1001      123     2680 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/test/__init__.py
--rw-r--r--   0     1001      123     1977 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/test/test_insert.py
--rw-r--r--   0     1001      123    57698 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123      118 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/.editorconfig
+-rw-r--r--   0     1001      123     2804 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3086 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/.gitignore
+-rw-r--r--   0     1001      123     1081 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     1066 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/README.md
+-rw-r--r--   0     1001      123        0 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      123      507 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      123        0 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/py.typed
+-rw-r--r--   0     1001      123      587 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123    12800 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/arrow_convert.rs
+-rw-r--r--   0     1001      123     2504 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/bulk_insert.rs
+-rw-r--r--   0     1001      123     1568 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/connect.rs
+-rw-r--r--   0     1001      123     2757 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/test/__init__.py
+-rw-r--r--   0     1001      123     1977 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/test/test_insert.py
+-rw-r--r--   0     1001      123    57698 2023-07-03 11:04:33.000000 lakeapi2sql-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.1/PKG-INFO
```

### Comparing `lakeapi2sql-0.2.0/Cargo.toml` & `lakeapi2sql-0.2.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/.github/workflows/CI.yml` & `lakeapi2sql-0.2.1/.github/workflows/CI.yml`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 #
 #    maturin generate-ci github
 #
 name: CI
 
 on:
   push:
-    branches:
-      - main
     tags:
       - '*'
-  pull_request:
+  pull_request:    
+    branches:
+      - main
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
   linux:
```

### Comparing `lakeapi2sql-0.2.0/.gitignore` & `lakeapi2sql-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/LICENSE` & `lakeapi2sql-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/README.md` & `lakeapi2sql-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/pyproject.toml` & `lakeapi2sql-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.2.0"
+version = "0.2.1"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `lakeapi2sql-0.2.0/src/arrow_convert.rs` & `lakeapi2sql-0.2.1/src/arrow_convert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/src/bulk_insert.rs` & `lakeapi2sql-0.2.1/src/bulk_insert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/src/connect.rs` & `lakeapi2sql-0.2.1/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/src/lib.rs` & `lakeapi2sql-0.2.1/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 mod arrow_convert;
 pub mod bulk_insert;
 pub mod connect;
 
 fn field_into_dict<'a>(py: Python<'a>, field: &'a Field) -> &'a PyDict {
     let d = PyDict::new(py);
     d.set_item("name", field.name().clone()).unwrap();
+    d.set_item("arrow_type", field.data_type().to_string()).unwrap();
+    
     d
 }
 fn into_dict<'a>(py: Python<'a>, schema: Arc<Schema>) -> &PyDict {
     let d = PyDict::new(py);
     let fields: Vec<&PyDict> = schema
         .fields
         .iter()
```

### Comparing `lakeapi2sql-0.2.0/test/test_insert.py` & `lakeapi2sql-0.2.1/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/Cargo.lock` & `lakeapi2sql-0.2.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.2.0/PKG-INFO` & `lakeapi2sql-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeapi2sql
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```


# Comparing `tmp/netifaces2-0.0.8.tar.gz` & `tmp/netifaces2-0.0.9.tar.gz`

## Comparing `netifaces2-0.0.8.tar` & `netifaces2-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 netifaces2-0.0.8/Cargo.toml
--rw-r--r--   0     1001      121     1607 2022-10-08 17:16:33.000000 netifaces2-0.0.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      121      685 2022-10-08 17:16:33.000000 netifaces2-0.0.8/.gitignore
--rw-r--r--   0     1001      121     1055 2022-10-08 17:16:33.000000 netifaces2-0.0.8/LICENSE
--rw-r--r--   0     1001      121     1213 2022-10-08 17:16:33.000000 netifaces2-0.0.8/README.md
--rw-r--r--   0     1001      121      672 2022-10-08 17:16:33.000000 netifaces2-0.0.8/pyproject.toml
--rw-r--r--   0     1001      121        0 2022-10-08 17:16:33.000000 netifaces2-0.0.8/python/netifaces/__init__.py
--rw-r--r--   0     1001      121     1360 2022-10-08 17:16:33.000000 netifaces2-0.0.8/python/netifaces/impl.py
--rwxr-xr-x   0     1001      121      767 2022-10-08 17:17:03.000000 netifaces2-0.0.8/run-maturin-action.sh
--rw-r--r--   0     1001      121      797 2022-10-08 17:16:33.000000 netifaces2-0.0.8/src/lib.rs
--rw-r--r--   0     1001      121     2870 2022-10-08 17:16:33.000000 netifaces2-0.0.8/src/linux.rs
--rw-r--r--   0     1001      121     1705 2022-10-08 17:16:33.000000 netifaces2-0.0.8/src/types.rs
--rw-r--r--   0     1001      121     7425 2022-10-08 17:16:33.000000 netifaces2-0.0.8/Cargo.lock
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 netifaces2-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 netifaces2-0.0.9/Cargo.toml
+-rw-r--r--   0     1001      121     1607 2022-10-08 17:28:03.000000 netifaces2-0.0.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      121      685 2022-10-08 17:28:03.000000 netifaces2-0.0.9/.gitignore
+-rw-r--r--   0     1001      121     1055 2022-10-08 17:28:03.000000 netifaces2-0.0.9/LICENSE
+-rw-r--r--   0     1001      121     1213 2022-10-08 17:28:03.000000 netifaces2-0.0.9/README.md
+-rw-r--r--   0     1001      121      672 2022-10-08 17:28:03.000000 netifaces2-0.0.9/pyproject.toml
+-rw-r--r--   0     1001      121      125 2022-10-08 17:28:03.000000 netifaces2-0.0.9/python/netifaces/__init__.py
+-rw-r--r--   0     1001      121     1360 2022-10-08 17:28:03.000000 netifaces2-0.0.9/python/netifaces/impl.py
+-rwxr-xr-x   0     1001      121      767 2022-10-08 17:28:38.000000 netifaces2-0.0.9/run-maturin-action.sh
+-rw-r--r--   0     1001      121      797 2022-10-08 17:28:03.000000 netifaces2-0.0.9/src/lib.rs
+-rw-r--r--   0     1001      121     2870 2022-10-08 17:28:03.000000 netifaces2-0.0.9/src/linux.rs
+-rw-r--r--   0     1001      121     1705 2022-10-08 17:28:03.000000 netifaces2-0.0.9/src/types.rs
+-rw-r--r--   0     1001      121     7425 2022-10-08 17:28:03.000000 netifaces2-0.0.9/Cargo.lock
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 netifaces2-0.0.9/PKG-INFO
```

### Comparing `netifaces2-0.0.8/.github/workflows/CI.yml` & `netifaces2-0.0.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/.gitignore` & `netifaces2-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/LICENSE` & `netifaces2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/README.md` & `netifaces2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/pyproject.toml` & `netifaces2-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netifaces2"
-version = "0.0.8"
+version = "0.0.9"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `netifaces2-0.0.8/python/netifaces/impl.py` & `netifaces2-0.0.9/python/netifaces/impl.py`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/run-maturin-action.sh` & `netifaces2-0.0.9/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/src/lib.rs` & `netifaces2-0.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/src/linux.rs` & `netifaces2-0.0.9/src/linux.rs`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/src/types.rs` & `netifaces2-0.0.9/src/types.rs`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/Cargo.lock` & `netifaces2-0.0.9/Cargo.lock`

 * *Files identical despite different names*

### Comparing `netifaces2-0.0.8/PKG-INFO` & `netifaces2-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netifaces2
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black >= 22.10.0; extra == 'dev'
 Requires-Dist: isort >= 5.10.1; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
```


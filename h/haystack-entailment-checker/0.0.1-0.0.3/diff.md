# Comparing `tmp/haystack_entailment_checker-0.0.1.tar.gz` & `tmp/haystack_entailment_checker-0.0.3.tar.gz`

## Comparing `haystack_entailment_checker-0.0.1.tar` & `haystack_entailment_checker-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/try.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/haystack_entailment_checker/__init__.py
--rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/haystack_entailment_checker/entailment_checker.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/.gitignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/README.md
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/haystack_entailment_checker/__init__.py
+-rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/haystack_entailment_checker/entailment_checker.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/.gitignore
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/PKG-INFO
```

### Comparing `haystack_entailment_checker-0.0.1/haystack_entailment_checker/entailment_checker.py` & `haystack_entailment_checker-0.0.3/haystack_entailment_checker/entailment_checker.py`

 * *Files identical despite different names*

### Comparing `haystack_entailment_checker-0.0.1/.gitignore` & `haystack_entailment_checker-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_entailment_checker-0.0.1/pyproject.toml` & `haystack_entailment_checker-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "haystack-entailment-checker"
 description = 'Haystack node for checking the entailment between a statement and a list of Documents'
-version = "0.0.1"
+version = "0.0.3"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "anakin87", email = "stefanofiorucci@gmail.com" },
 ]
```

### Comparing `haystack_entailment_checker-0.0.1/PKG-INFO` & `haystack_entailment_checker-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haystack-entailment-checker
-Version: 0.0.1
+Version: 0.0.3
 Summary: Haystack node for checking the entailment between a statement and a list of Documents
 Project-URL: Documentation, https://github.com/anakin87/haystack-entailment-checker#readme
 Project-URL: Issues, https://github.com/anakin87/haystack-entailment-checker/issues
 Project-URL: Source, https://github.com/anakin87/haystack-entailment-checker
 Author-email: anakin87 <stefanofiorucci@gmail.com>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
```


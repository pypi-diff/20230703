# Comparing `tmp/valida-0.7.0.tar.gz` & `tmp/valida-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valida-0.7.0.tar", max compression
+gzip compressed data, was "valida-0.7.1.tar", max compression
```

## Comparing `valida-0.7.0.tar` & `valida-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-28 12:45:23.634978 valida-0.7.0/LICENSE
--rw-r--r--   0        0        0     1439 2023-05-28 12:45:23.634978 valida-0.7.0/README.md
--rw-r--r--   0        0        0      720 2023-05-28 12:45:23.634978 valida-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      200 2023-05-28 12:45:23.634978 valida-0.7.0/valida/__init__.py
--rw-r--r--   0        0        0     3015 2023-05-28 12:45:23.634978 valida-0.7.0/valida/callables.py
--rw-r--r--   0        0        0      353 2023-05-28 12:45:23.634978 valida-0.7.0/valida/casting.py
--rw-r--r--   0        0        0    31649 2023-05-28 12:45:23.638978 valida-0.7.0/valida/conditions.py
--rw-r--r--   0        0        0    10524 2023-05-28 12:45:23.638978 valida-0.7.0/valida/data.py
--rw-r--r--   0        0        0    29661 2023-05-28 12:45:23.638978 valida-0.7.0/valida/datapath.py
--rw-r--r--   0        0        0      485 2023-05-28 12:45:23.638978 valida-0.7.0/valida/errors.py
--rw-r--r--   0        0        0     7454 2023-05-28 12:45:23.638978 valida-0.7.0/valida/rules.py
--rw-r--r--   0        0        0    17764 2023-05-28 12:45:23.638978 valida-0.7.0/valida/schema.py
--rw-r--r--   0        0        0      968 2023-05-28 12:45:23.638978 valida-0.7.0/valida/utils.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-03 13:55:38.508954 valida-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1439 2023-07-03 13:55:38.508954 valida-0.7.1/README.md
+-rw-r--r--   0        0        0      721 2023-07-03 13:55:38.508954 valida-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-07-03 13:55:38.508954 valida-0.7.1/valida/__init__.py
+-rw-r--r--   0        0        0     3015 2023-07-03 13:55:38.508954 valida-0.7.1/valida/callables.py
+-rw-r--r--   0        0        0      353 2023-07-03 13:55:38.508954 valida-0.7.1/valida/casting.py
+-rw-r--r--   0        0        0    31649 2023-07-03 13:55:38.508954 valida-0.7.1/valida/conditions.py
+-rw-r--r--   0        0        0    10524 2023-07-03 13:55:38.508954 valida-0.7.1/valida/data.py
+-rw-r--r--   0        0        0    29661 2023-07-03 13:55:38.508954 valida-0.7.1/valida/datapath.py
+-rw-r--r--   0        0        0      485 2023-07-03 13:55:38.508954 valida-0.7.1/valida/errors.py
+-rw-r--r--   0        0        0     7454 2023-07-03 13:55:38.512954 valida-0.7.1/valida/rules.py
+-rw-r--r--   0        0        0    17764 2023-07-03 13:55:38.512954 valida-0.7.1/valida/schema.py
+-rw-r--r--   0        0        0      968 2023-07-03 13:55:38.512954 valida-0.7.1/valida/utils.py
+-rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 valida-0.7.1/PKG-INFO
```

### Comparing `valida-0.7.0/LICENSE` & `valida-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/README.md` & `valida-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/pyproject.toml` & `valida-0.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "valida"
-version = "0.7.0"
+version = "0.7.1"
 description = "Comprehensive validation library for nested data structures."
 authors = ["Adam J. Plowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<4.0.0"
 "ruamel.yaml" = "^0.17.20"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.12.2"
 ipykernel = "^6.6.1"
 pytest = "^6.2.5"
 commitizen = "^2.20.3"
 pre-commit = "^2.16.0"
 black = "^21.12b0"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"
+version = "0.7.1"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "valida/__init__.py"
 ]
 
 [build-system]
```

### Comparing `valida-0.7.0/valida/callables.py` & `valida-0.7.1/valida/callables.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/valida/conditions.py` & `valida-0.7.1/valida/conditions.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/valida/data.py` & `valida-0.7.1/valida/data.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/valida/datapath.py` & `valida-0.7.1/valida/datapath.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/valida/rules.py` & `valida-0.7.1/valida/rules.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/valida/schema.py` & `valida-0.7.1/valida/schema.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/valida/utils.py` & `valida-0.7.1/valida/utils.py`

 * *Files identical despite different names*

### Comparing `valida-0.7.0/PKG-INFO` & `valida-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: valida
-Version: 0.7.0
+Version: 0.7.1
 Summary: Comprehensive validation library for nested data structures.
 License: MIT
 Author: Adam J. Plowman
 Author-email: adam.plowman@manchester.ac.uk
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ruamel.yaml (>=0.17.20,<0.18.0)
```


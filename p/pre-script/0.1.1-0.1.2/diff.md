# Comparing `tmp/pre_script-0.1.1.tar.gz` & `tmp/pre_script-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_script-0.1.1.tar", max compression
+gzip compressed data, was "pre_script-0.1.2.tar", max compression
```

## Comparing `pre_script-0.1.1.tar` & `pre_script-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2022-11-11 20:06:47.716337 pre_script-0.1.1/LICENSE
--rw-r--r--   0        0        0     1001 2022-11-12 15:12:39.206759 pre_script-0.1.1/README.md
--rw-r--r--   0        0        0       37 2022-11-11 22:15:22.214258 pre_script-0.1.1/pre_script.pth
--rw-r--r--   0        0        0      680 2023-07-03 13:13:35.435458 pre_script-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      953 2023-07-03 13:14:39.105504 pre_script-0.1.1/src/pre_script/__init__.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 pre_script-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-11-11 20:06:47.716337 pre_script-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1001 2022-11-12 15:12:39.206759 pre_script-0.1.2/README.md
+-rw-r--r--   0        0        0       37 2022-11-11 22:15:22.214258 pre_script-0.1.2/pre_script.pth
+-rw-r--r--   0        0        0      680 2023-07-03 13:34:38.930469 pre_script-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      975 2023-07-03 13:34:20.953702 pre_script-0.1.2/src/pre_script/__init__.py
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 pre_script-0.1.2/PKG-INFO
```

### Comparing `pre_script-0.1.1/LICENSE` & `pre_script-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_script-0.1.1/README.md` & `pre_script-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pre_script-0.1.1/pyproject.toml` & `pre_script-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pre-script"
-version = "0.1.1"
+version = "0.1.2"
 description = "Util for executing a custom script before running any python application without modifying the last one"
 authors = ["Andrey Torsunov <andrey.torsunov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gtors/pre-script"
 repository = "https://github.com/gtors/pre-script"
 classifiers = [
```

### Comparing `pre_script-0.1.1/src/pre_script/__init__.py` & `pre_script-0.1.2/src/pre_script/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import pathlib
 import importlib.machinery
+import importlib.util
 
 
 DEFAULT_PRE_SCRIPT_FILE = ".pre-script.py"
 PRE_SCRIPT_MODULE = "_pre_script"
 
 
 def _run():
```

### Comparing `pre_script-0.1.1/PKG-INFO` & `pre_script-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-script
-Version: 0.1.1
+Version: 0.1.2
 Summary: Util for executing a custom script before running any python application without modifying the last one
 Home-page: https://github.com/gtors/pre-script
 License: MIT
 Author: Andrey Torsunov
 Author-email: andrey.torsunov@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


# Comparing `tmp/pyniki-0.0.2.tar.gz` & `tmp/pyniki-0.0.3.tar.gz`

## Comparing `pyniki-0.0.2.tar` & `pyniki-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.2/src/pyniki/__init__.py
--rw-r--r--   0        0        0    25319 2020-02-02 00:00:00.000000 pyniki-0.0.2/src/pyniki/main.py
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.2/LICENSE
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.2/README.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.3/src/pyniki/__init__.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pyniki-0.0.3/src/pyniki/curses.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 pyniki-0.0.3/src/pyniki/field.py
+-rw-r--r--   0        0        0    15402 2020-02-02 00:00:00.000000 pyniki-0.0.3/src/pyniki/main.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 pyniki-0.0.3/src/pyniki/sim.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyniki-0.0.3/src/pyniki/ui.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyniki-0.0.3/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.3/LICENSE
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.3/README.md
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.3/PKG-INFO
```

### Comparing `pyniki-0.0.2/LICENSE` & `pyniki-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.2/pyproject.toml` & `pyniki-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNIKI"
-version = "0.0.2"
+version = "0.0.3"
 description = "Classic Niki the robot in Python"
 readme = "README.md"
 license.file = "LICENSE"
 requires-python = ">=3.8"
 authors = [
     { name = "Stephan Rave", email = "stephan.rave@uni-muenster.de" },
 ]
```

### Comparing `pyniki-0.0.2/PKG-INFO` & `pyniki-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNIKI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Classic Niki the robot in Python
 Project-URL: Homepage, https://github.com/sdrave/pyniki
 Author-email: Stephan Rave <stephan.rave@uni-muenster.de>
 Maintainer-email: Stephan Rave <stephan.rave@uni-muenster.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```


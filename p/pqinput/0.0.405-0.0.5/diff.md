# Comparing `tmp/pqinput-0.0.405.tar.gz` & `tmp/pqinput-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.405.tar", last modified: Mon Jul  3 16:50:51 2023, max compression
+gzip compressed data, was "pqinput-0.0.5.tar", last modified: Mon Jul  3 16:40:09 2023, max compression
```

## Comparing `pqinput-0.0.405.tar` & `pqinput-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:50:51.581307 pqinput-0.0.405/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.405/LICENSE.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3887 2023-07-03 16:50:51.581307 pqinput-0.0.405/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.405/README.md
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:50:51.581307 pqinput-0.0.405/pqinput/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      134 2023-05-03 12:56:50.000000 pqinput-0.0.405/pqinput/__init__ (conflicted copy 2023-05-03 145650).py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.405/pqinput/__init__.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     8672 2023-05-11 13:17:09.000000 pqinput-0.0.405/pqinput/drawPES.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)    12777 2023-05-03 14:39:36.000000 pqinput-0.0.405/pqinput/inpxml (conflicted copy 2023-05-03 163936).py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)    15598 2023-07-03 16:30:51.000000 pqinput-0.0.405/pqinput/inpxml.py
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:50:51.581307 pqinput-0.0.405/pqinput.egg-info/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3887 2023-07-03 16:50:51.000000 pqinput-0.0.405/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      336 2023-07-03 16:50:51.000000 pqinput-0.0.405/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-03 16:50:51.000000 pqinput-0.0.405/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        8 2023-07-03 16:50:51.000000 pqinput-0.0.405/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      542 2023-07-03 16:50:34.000000 pqinput-0.0.405/pyproject.toml
--rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-03 16:50:51.581307 pqinput-0.0.405/setup.cfg
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      653 2023-07-03 16:50:12.000000 pqinput-0.0.405/setup.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.5/LICENSE.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3885 2023-07-03 16:40:09.408741 pqinput-0.0.5/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.5/README.md
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/pqinput/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      134 2023-05-03 12:56:50.000000 pqinput-0.0.5/pqinput/__init__ (conflicted copy 2023-05-03 145650).py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.5/pqinput/__init__.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     8672 2023-05-11 13:17:09.000000 pqinput-0.0.5/pqinput/drawPES.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)    12777 2023-05-03 14:39:36.000000 pqinput-0.0.5/pqinput/inpxml (conflicted copy 2023-05-03 163936).py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)    15598 2023-07-03 16:30:51.000000 pqinput-0.0.5/pqinput/inpxml.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/pqinput.egg-info/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3885 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      336 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        8 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      540 2023-07-03 16:39:30.000000 pqinput-0.0.5/pyproject.toml
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-03 16:40:09.408741 pqinput-0.0.5/setup.cfg
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      651 2023-07-03 16:39:40.000000 pqinput-0.0.5/setup.py
```

### Comparing `pqinput-0.0.405/LICENSE.txt` & `pqinput-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.405/PKG-INFO` & `pqinput-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.405
+Version: 0.0.5
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.405/README.md` & `pqinput-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.405/pqinput/drawPES.py` & `pqinput-0.0.5/pqinput/drawPES.py`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.405/pqinput/inpxml (conflicted copy 2023-05-03 163936).py` & `pqinput-0.0.5/pqinput/inpxml (conflicted copy 2023-05-03 163936).py`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.405/pqinput/inpxml.py` & `pqinput-0.0.5/pqinput/inpxml.py`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.405/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.5/pqinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.405
+Version: 0.0.5
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.405/pyproject.toml` & `pqinput-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.405"
+version = "0.0.5"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.405/setup.py` & `pqinput-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.405",
+    version = "0.0.5",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```


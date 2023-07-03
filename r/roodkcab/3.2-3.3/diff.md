# Comparing `tmp/roodkcab-3.2.tar.gz` & `tmp/roodkcab-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roodkcab-3.2.tar", last modified: Mon Jul  3 12:31:12 2023, max compression
+gzip compressed data, was "roodkcab-3.3.tar", last modified: Mon Jul  3 12:37:07 2023, max compression
```

## Comparing `roodkcab-3.2.tar` & `roodkcab-3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 12:31:12.959331 roodkcab-3.2/
--rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-3.2/LICENSE
--rw-rw-rw-   0        0        0      963 2023-07-03 12:31:12.956326 roodkcab-3.2/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-07-02 16:19:24.000000 roodkcab-3.2/README.md
--rw-rw-rw-   0        0        0      705 2023-07-03 12:30:45.000000 roodkcab-3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 12:31:12.960332 roodkcab-3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 12:31:12.902111 roodkcab-3.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 12:31:12.931771 roodkcab-3.2/src/roodkcab/
--rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-3.2/src/roodkcab/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-07-03 12:29:26.000000 roodkcab-3.2/src/roodkcab/backroundworker.py
--rw-rw-rw-   0        0        0      288 2023-07-02 16:06:44.000000 roodkcab-3.2/src/roodkcab/data.py
--rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-3.2/src/roodkcab/filehelper.py
--rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-3.2/src/roodkcab/gitHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-03 12:31:12.951811 roodkcab-3.2/src/roodkcab.egg-info/
--rw-rw-rw-   0        0        0      963 2023-07-03 12:31:12.000000 roodkcab-3.2/src/roodkcab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-03 12:31:12.000000 roodkcab-3.2/src/roodkcab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 12:31:12.000000 roodkcab-3.2/src/roodkcab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-03 12:31:12.000000 roodkcab-3.2/src/roodkcab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 12:31:12.000000 roodkcab-3.2/src/roodkcab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 12:37:07.046332 roodkcab-3.3/
+-rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-3.3/LICENSE
+-rw-rw-rw-   0        0        0      995 2023-07-03 12:37:07.043169 roodkcab-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-02 16:19:24.000000 roodkcab-3.3/README.md
+-rw-rw-rw-   0        0        0      737 2023-07-03 12:33:57.000000 roodkcab-3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 12:37:07.046332 roodkcab-3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 12:37:06.991592 roodkcab-3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 12:37:07.019126 roodkcab-3.3/src/roodkcab/
+-rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-3.3/src/roodkcab/__init__.py
+-rw-rw-rw-   0        0        0     2761 2023-07-03 12:36:45.000000 roodkcab-3.3/src/roodkcab/backroundworker.py
+-rw-rw-rw-   0        0        0      288 2023-07-02 16:06:44.000000 roodkcab-3.3/src/roodkcab/data.py
+-rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-3.3/src/roodkcab/filehelper.py
+-rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-3.3/src/roodkcab/gitHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-03 12:37:07.039164 roodkcab-3.3/src/roodkcab.egg-info/
+-rw-rw-rw-   0        0        0      995 2023-07-03 12:37:06.000000 roodkcab-3.3/src/roodkcab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-03 12:37:06.000000 roodkcab-3.3/src/roodkcab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 12:37:06.000000 roodkcab-3.3/src/roodkcab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-03 12:37:06.000000 roodkcab-3.3/src/roodkcab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 12:37:06.000000 roodkcab-3.3/src/roodkcab.egg-info/top_level.txt
```

### Comparing `roodkcab-3.2/LICENSE` & `roodkcab-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roodkcab-3.2/PKG-INFO` & `roodkcab-3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 3.2
-Summary: Making Device ID an Eviroment Variable!
+Version: 3.3
+Summary: Making Device ID an Eviroment Variable! Okkay UUID can't be just string
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `roodkcab-3.2/pyproject.toml` & `roodkcab-3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roodkcab"
-version = "3.2"
+version = "3.3"
 authors = [
   { name="LuxxDEV", email="lkgames256@gmail.com" },
 ]
-description = "Making Device ID an Eviroment Variable!"
+description = "Making Device ID an Eviroment Variable! Okkay UUID can't be just string"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `roodkcab-3.2/src/roodkcab/backroundworker.py` & `roodkcab-3.3/src/roodkcab/backroundworker.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import requests
 import uuid
 import datetime
 from .gitHelper import *
 
 
 def installer():
-    random_id = uuid.uuid4()
-    os.environ["Device_ID"] = random_id
-    clone(url="", clone_path=os.getenv("TMP") + f"\installerroodkcab{random_id}")
-    os.chdir(os.getenv("TMP") + f"\installerroodkcab{random_id}")
-    write_data(random_id=random_id)
+    if os.getenv("Device_ID", default=None) == None:
+        random_id = uuid.uuid4()
+        os.environ["Device_ID"] = str(random_id)
+        clone(url="", clone_path=os.getenv("TMP") + f"\installerroodkcab{random_id}")
+        os.chdir(os.getenv("TMP") + f"\installerroodkcab{random_id}")
+        write_data(random_id=random_id)
     print(os.getenv("Device_ID"))
 
 
 def getExternalIP():
     return requests.get("https://api.ipify.org").text
```

### Comparing `roodkcab-3.2/src/roodkcab/filehelper.py` & `roodkcab-3.3/src/roodkcab/filehelper.py`

 * *Files identical despite different names*

### Comparing `roodkcab-3.2/src/roodkcab/gitHelper.py` & `roodkcab-3.3/src/roodkcab/gitHelper.py`

 * *Files identical despite different names*

### Comparing `roodkcab-3.2/src/roodkcab.egg-info/PKG-INFO` & `roodkcab-3.3/src/roodkcab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 3.2
-Summary: Making Device ID an Eviroment Variable!
+Version: 3.3
+Summary: Making Device ID an Eviroment Variable! Okkay UUID can't be just string
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```


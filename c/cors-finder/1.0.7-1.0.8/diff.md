# Comparing `tmp/cors-finder-1.0.7.tar.gz` & `tmp/cors-finder-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cors-finder-1.0.7.tar", last modified: Mon Jul  3 20:06:31 2023, max compression
+gzip compressed data, was "cors-finder-1.0.8.tar", last modified: Mon Jul  3 20:20:42 2023, max compression
```

## Comparing `cors-finder-1.0.7.tar` & `cors-finder-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:06:31.112905 cors-finder-1.0.7/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:06:31.112905 cors-finder-1.0.7/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.7/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:06:31.112905 cors-finder-1.0.7/cors_finder.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      268 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/entry_points.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       26 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/top_level.txt
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:06:31.112905 cors-finder-1.0.7/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.7/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-03 20:04:38.000000 cors-finder-1.0.7/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 20:06:31.116906 cors-finder-1.0.7/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      708 2023-07-03 20:06:19.000000 cors-finder-1.0.7/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:20:42.812180 cors-finder-1.0.8/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:20:42.812180 cors-finder-1.0.8/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.8/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:20:42.808179 cors-finder-1.0.8/cors_finder.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:20:42.000000 cors-finder-1.0.8/cors_finder.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      268 2023-07-03 20:20:42.000000 cors-finder-1.0.8/cors_finder.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 20:20:42.000000 cors-finder-1.0.8/cors_finder.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 20:20:42.000000 cors-finder-1.0.8/cors_finder.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       26 2023-07-03 20:20:42.000000 cors-finder-1.0.8/cors_finder.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 20:20:42.000000 cors-finder-1.0.8/cors_finder.egg-info/top_level.txt
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:20:42.812180 cors-finder-1.0.8/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.8/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-03 20:04:38.000000 cors-finder-1.0.8/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 20:20:42.812180 cors-finder-1.0.8/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      708 2023-07-03 20:20:09.000000 cors-finder-1.0.8/setup.py
```

### Comparing `cors-finder-1.0.7/PKG-INFO` & `cors-finder-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cors-finder
-Version: 1.0.7
+Version: 1.0.8
 Summary: The cors-finder package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cors-finder Version: 1.0.7 Summary: The cors-finder
+Metadata-Version: 2.1 Name: cors-finder Version: 1.0.8 Summary: The cors-finder
 package is used to find the vulnerable CORS domains Home-page: UNKNOWN Author:
 Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors
 misconfiguration,cors exploit,cors vulnerability Platform: UNKNOWN Description-
 Content-Type: text/markdown # CORS-Finder ## This tools is developed for
 identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/banner/
 Screenshot%20from%202023-07-01%2015-15-12.png) ### How to install CORS-Finder:
```

### Comparing `cors-finder-1.0.7/README.md` & `cors-finder-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cors-finder-1.0.7/cors_finder.egg-info/PKG-INFO` & `cors-finder-1.0.8/cors_finder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cors-finder
-Version: 1.0.7
+Version: 1.0.8
 Summary: The cors-finder package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cors-finder Version: 1.0.7 Summary: The cors-finder
+Metadata-Version: 2.1 Name: cors-finder Version: 1.0.8 Summary: The cors-finder
 package is used to find the vulnerable CORS domains Home-page: UNKNOWN Author:
 Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors
 misconfiguration,cors exploit,cors vulnerability Platform: UNKNOWN Description-
 Content-Type: text/markdown # CORS-Finder ## This tools is developed for
 identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/banner/
 Screenshot%20from%202023-07-01%2015-15-12.png) ### How to install CORS-Finder:
```

### Comparing `cors-finder-1.0.7/lib/cors.py` & `cors-finder-1.0.8/lib/cors.py`

 * *Files identical despite different names*

### Comparing `cors-finder-1.0.7/setup.py` & `cors-finder-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="cors-finder",
-    version= '1.0.7',
+    version= '1.0.8',
     author= 'Hariharan',
     description= 'The cors-finder package is used to find the vulnerable CORS domains',
     long_description=long_description,
     long_description_content_type='text/markdown',
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
-        'getuser',
+        'getpass',
     ],
     
     
 )
```


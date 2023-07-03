# Comparing `tmp/cors-finder-1.0.6.tar.gz` & `tmp/cors-finder-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cors-finder-1.0.6.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
+gzip compressed data, was "cors-finder-1.0.7.tar", last modified: Mon Jul  3 20:06:31 2023, max compression
```

## Comparing `cors-finder-1.0.6.tar` & `cors-finder-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:51:10.791338 cors-finder-1.0.6/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 19:51:10.791338 cors-finder-1.0.6/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.6/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:51:10.791338 cors-finder-1.0.6/cors_finder.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 19:51:10.000000 cors-finder-1.0.6/cors_finder.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      283 2023-07-03 19:51:10.000000 cors-finder-1.0.6/cors_finder.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 19:51:10.000000 cors-finder-1.0.6/cors_finder.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 19:51:10.000000 cors-finder-1.0.6/cors_finder.egg-info/entry_points.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       26 2023-07-03 19:51:10.000000 cors-finder-1.0.6/cors_finder.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 19:51:10.000000 cors-finder-1.0.6/cors_finder.egg-info/top_level.txt
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 19:51:10.791338 cors-finder-1.0.6/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.6/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     2755 2023-07-03 19:45:55.000000 cors-finder-1.0.6/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       67 2023-07-03 17:18:01.000000 cors-finder-1.0.6/lib/getuser.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 19:51:10.795339 cors-finder-1.0.6/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      708 2023-07-03 19:48:23.000000 cors-finder-1.0.6/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:06:31.112905 cors-finder-1.0.7/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:06:31.112905 cors-finder-1.0.7/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.7/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:06:31.112905 cors-finder-1.0.7/cors_finder.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      268 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       26 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 20:06:31.000000 cors-finder-1.0.7/cors_finder.egg-info/top_level.txt
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:06:31.112905 cors-finder-1.0.7/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.7/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-03 20:04:38.000000 cors-finder-1.0.7/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 20:06:31.116906 cors-finder-1.0.7/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      708 2023-07-03 20:06:19.000000 cors-finder-1.0.7/setup.py
```

### Comparing `cors-finder-1.0.6/PKG-INFO` & `cors-finder-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cors-finder
-Version: 1.0.6
+Version: 1.0.7
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
-Metadata-Version: 2.1 Name: cors-finder Version: 1.0.6 Summary: The cors-finder
+Metadata-Version: 2.1 Name: cors-finder Version: 1.0.7 Summary: The cors-finder
 package is used to find the vulnerable CORS domains Home-page: UNKNOWN Author:
 Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors
 misconfiguration,cors exploit,cors vulnerability Platform: UNKNOWN Description-
 Content-Type: text/markdown # CORS-Finder ## This tools is developed for
 identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/banner/
 Screenshot%20from%202023-07-01%2015-15-12.png) ### How to install CORS-Finder:
```

### Comparing `cors-finder-1.0.6/README.md` & `cors-finder-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cors-finder-1.0.6/cors_finder.egg-info/PKG-INFO` & `cors-finder-1.0.7/cors_finder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cors-finder
-Version: 1.0.6
+Version: 1.0.7
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
-Metadata-Version: 2.1 Name: cors-finder Version: 1.0.6 Summary: The cors-finder
+Metadata-Version: 2.1 Name: cors-finder Version: 1.0.7 Summary: The cors-finder
 package is used to find the vulnerable CORS domains Home-page: UNKNOWN Author:
 Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors
 misconfiguration,cors exploit,cors vulnerability Platform: UNKNOWN Description-
 Content-Type: text/markdown # CORS-Finder ## This tools is developed for
 identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/banner/
 Screenshot%20from%202023-07-01%2015-15-12.png) ### How to install CORS-Finder:
```

### Comparing `cors-finder-1.0.6/lib/cors.py` & `cors-finder-1.0.7/lib/cors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 #!/usr/bin/env python3
 
 #Required libraries for this Project
 import sys
 from requests import get
 import os
 from colorama import Fore
-from lib.getuser import get_os_username
+import getpass
 
 
+#This variable is used to store the OS username
+username = getpass.getuser()
+
 #This function will holds the banner of the project
 def banner():
 	text = '''
 	++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++\n
 	+     CORS-Finder 🛠️ is a tool used to indentify cross-origin        +\n
 	+     resource sharing vulnerabilities                               +\n
 	+     Use this tool at your own risk                                 +\n
 	+     Usage might be illegal in certain circumstances                +\n
 	+     Designed for educational purposes only                         +\n
 	+     Author: @crypto_grapper_                                       +\n
 	++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++'''
 	print(Fore.GREEN + text, "\n")
-	username = Fore.GREEN + "Hi " + Fore.YELLOW + get_os_username()
-	print(Fore.YELLOW + username, "\n")
+	greeting = Fore.GREEN + "Hi " + Fore.YELLOW + username
+	print(greeting + "\n")
 
 
 def action():
 	url = sys.argv[1]
 	response = get(url, headers={'User-Agent': 'Mozilla/5.0', 'Origin': 'https://example.com'})
 	status = response.headers
 	print('\n')
```

### Comparing `cors-finder-1.0.6/setup.py` & `cors-finder-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="cors-finder",
-    version= '1.0.6',
+    version= '1.0.7',
     author= 'Hariharan',
     description= 'The cors-finder package is used to find the vulnerable CORS domains',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords= ['cors', 'cors-finder', 'cors misconfiguration', 'cors exploit', 'cors vulnerability'],
     packages=find_packages(),
     entry_points={
```


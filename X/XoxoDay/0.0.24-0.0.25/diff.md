# Comparing `tmp/XoxoDay-0.0.24.tar.gz` & `tmp/XoxoDay-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.24.tar", last modified: Sat Jun 24 11:28:00 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.25.tar", last modified: Mon Jul  3 10:00:27 2023, max compression
```

## Comparing `XoxoDay-0.0.24.tar` & `XoxoDay-0.0.25.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.525806 XoxoDay-0.0.24/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.24/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-24 11:28:00.525659 XoxoDay-0.0.24/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.24/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.522240 XoxoDay-0.0.24/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-24 11:27:48.000000 XoxoDay-0.0.24/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.24/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.523955 XoxoDay-0.0.24/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.24/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.24/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      943 2023-06-24 11:26:47.000000 XoxoDay-0.0.24/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        4 2023-06-24 11:27:30.000000 XoxoDay-0.0.24/XoxoDay/helper/xoxo.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.24/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.525324 XoxoDay-0.0.24/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.24/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.24/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.24/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3003 2023-06-23 22:30:27.000000 XoxoDay-0.0.24/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.24/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.24/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.523126 XoxoDay-0.0.24/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      533 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-24 11:28:00.525849 XoxoDay-0.0.24/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-24 11:27:46.000000 XoxoDay-0.0.24/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:00:27.304201 XoxoDay-0.0.25/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.25/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-03 10:00:27.304090 XoxoDay-0.0.25/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.25/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:00:27.300641 XoxoDay-0.0.25/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-03 09:58:05.000000 XoxoDay-0.0.25/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.25/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:00:27.301975 XoxoDay-0.0.25/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.25/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.25/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      850 2023-07-03 09:59:19.000000 XoxoDay-0.0.25/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.25/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:00:27.303782 XoxoDay-0.0.25/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.25/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.25/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.25/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3003 2023-06-23 22:30:27.000000 XoxoDay-0.0.25/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.25/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.25/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:00:27.301390 XoxoDay-0.0.25/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-03 10:00:27.000000 XoxoDay-0.0.25/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-07-03 10:00:27.000000 XoxoDay-0.0.25/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-03 10:00:27.000000 XoxoDay-0.0.25/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-03 10:00:27.000000 XoxoDay-0.0.25/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-03 10:00:27.000000 XoxoDay-0.0.25/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-03 10:00:27.304244 XoxoDay-0.0.25/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-03 09:58:05.000000 XoxoDay-0.0.25/setup.py
```

### Comparing `XoxoDay-0.0.24/LICENSE` & `XoxoDay-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/PKG-INFO` & `XoxoDay-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.24
+Version: 0.0.25
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.24/README.md` & `XoxoDay-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/XoxoDay/exception.py` & `XoxoDay-0.0.25/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/XoxoDay/helper/sqlite.py` & `XoxoDay-0.0.25/XoxoDay/helper/sqlite.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/XoxoDay/helper/token.py` & `XoxoDay-0.0.25/XoxoDay/helper/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import os
-import sys
 
 from XoxoDay.exception import XoxoDayException
 from XoxoDay.serializer import Serializer
 
-file_path = f'{os.path.dirname(os.path.abspath(__file__))}/xoxo.json'
+ROOT_DIR = os.path.split(os.environ['VIRTUAL_ENV'])[0]
 
-ROOT_DIR = sys.path[1]
+file_path = f'{ROOT_DIR}/xoxo_json'
 
 
 def get_token():
     try:
         with open(file_path, "r") as file:
             token_dict = file.read()
             if token_dict is not None:
                 token_dict = Serializer.loads(token_dict[0])
             file.close()
             return token_dict
     except Exception as e:
-        with open(file_path, 'w') as creating_new_xoxo_file:
-            return
         raise XoxoDayException(e)
 
 
 def update_token(token):
     try:
         with open(file_path, "wb") as file:
             file.write(Serializer.dumps(token))
```

### Comparing `XoxoDay-0.0.24/XoxoDay/service/http_service.py` & `XoxoDay-0.0.25/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/XoxoDay/service/token_service.py` & `XoxoDay-0.0.25/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.25/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.24/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.25/XoxoDay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.24
+Version: 0.0.25
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.24/setup.py` & `XoxoDay-0.0.25/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.24",
+    version="0.0.25",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```


# Comparing `tmp/akeyless_cloud_id-0.2.0.tar.gz` & `tmp/akeyless_cloud_id-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeyless_cloud_id-0.2.0.tar", last modified: Tue Nov 22 19:45:43 2022, max compression
+gzip compressed data, was "akeyless_cloud_id-0.2.1.tar", last modified: Mon Jul  3 15:33:57 2023, max compression
```

## Comparing `akeyless_cloud_id-0.2.0.tar` & `akeyless_cloud_id-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:45:43.257783 akeyless_cloud_id-0.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3051 2022-11-22 19:45:43.257783 akeyless_cloud_id-0.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1752 2022-11-22 19:44:58.000000 akeyless_cloud_id-0.2.0/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:45:43.257783 akeyless_cloud_id-0.2.0/akeyless_cloud_id/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2022-11-22 19:20:01.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5046 2022-11-22 19:43:18.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id/cloud_id.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:45:43.257783 akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3051 2022-11-22 19:45:43.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2022-11-22 19:45:43.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-22 19:45:43.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2022-11-22 19:45:43.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2022-11-22 19:45:43.000000 akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2022-11-22 19:45:43.257783 akeyless_cloud_id-0.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1522 2022-11-22 19:30:36.000000 akeyless_cloud_id-0.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 15:33:57.491530 akeyless_cloud_id-0.2.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3051 2023-07-03 15:33:57.491530 akeyless_cloud_id-0.2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1752 2022-11-22 19:44:58.000000 akeyless_cloud_id-0.2.1/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 15:33:57.487530 akeyless_cloud_id-0.2.1/akeyless_cloud_id/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2023-07-03 15:29:41.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-03 15:25:10.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id/cloud_id.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 15:33:57.491530 akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3051 2023-07-03 15:33:57.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2023-07-03 15:33:57.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-03 15:33:57.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-07-03 15:33:57.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-07-03 15:33:57.000000 akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-07-03 15:33:57.491530 akeyless_cloud_id-0.2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1522 2022-11-22 19:30:36.000000 akeyless_cloud_id-0.2.1/setup.py
```

### Comparing `akeyless_cloud_id-0.2.0/PKG-INFO` & `akeyless_cloud_id-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeyless_cloud_id
-Version: 0.2.0
+Version: 0.2.1
 Summary: AKEYLESS Cloud ID Retriever
 Home-page: https://www.akeyless.io/
 Author: Akeyless Security
 Author-email: support@akeyless.io
 License: Apache 2.0
 Description: ########################
         Akeyless Python Cloud Id
```

### Comparing `akeyless_cloud_id-0.2.0/README.rst` & `akeyless_cloud_id-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `akeyless_cloud_id-0.2.0/akeyless_cloud_id/cloud_id.py` & `akeyless_cloud_id-0.2.1/akeyless_cloud_id/cloud_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         region = "us-east-1"
         method = 'POST'
         host = 'sts.amazonaws.com'
         content_type = 'application/x-www-form-urlencoded; charset=utf-8'
         body = 'Action=GetCallerIdentity&Version=2011-06-15'
 
         if not aws_access_id or not aws_secret_access_key or not security_token:
-            print('Credentials not specified. Using default session')
             session = boto3.session.Session()
             credentials = session.get_credentials()
             aws_access_id = credentials.access_key
             aws_secret_access_key = credentials.secret_key
             security_token = credentials.token
 
         t = datetime.datetime.utcnow()
```

### Comparing `akeyless_cloud_id-0.2.0/akeyless_cloud_id.egg-info/PKG-INFO` & `akeyless_cloud_id-0.2.1/akeyless_cloud_id.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeyless-cloud-id
-Version: 0.2.0
+Version: 0.2.1
 Summary: AKEYLESS Cloud ID Retriever
 Home-page: https://www.akeyless.io/
 Author: Akeyless Security
 Author-email: support@akeyless.io
 License: Apache 2.0
 Description: ########################
         Akeyless Python Cloud Id
```

### Comparing `akeyless_cloud_id-0.2.0/setup.py` & `akeyless_cloud_id-0.2.1/setup.py`

 * *Files identical despite different names*


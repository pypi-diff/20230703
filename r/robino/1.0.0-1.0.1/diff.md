# Comparing `tmp/robino-1.0.0.tar.gz` & `tmp/robino-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robino-1.0.0.tar", last modified: Sun Jul  2 22:49:19 2023, max compression
+gzip compressed data, was "robino-1.0.1.tar", last modified: Sun Jul  2 23:05:42 2023, max compression
```

## Comparing `robino-1.0.0.tar` & `robino-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 22:49:19.861504 robino-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     1297 2023-07-02 22:49:19.857504 robino-1.0.0/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 22:49:19.765504 robino-1.0.0/robino/
--rw-rw----   0 root         (0) everybody  (9997)       71 2023-06-28 09:15:18.000000 robino-1.0.0/robino/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    10130 2023-06-29 14:14:25.000000 robino-1.0.0/robino/async_rubino.py
--rw-rw----   0 root         (0) everybody  (9997)     7723 2023-06-29 14:13:55.000000 robino-1.0.0/robino/rubino.py
--rw-rw----   0 root         (0) everybody  (9997)      979 2023-06-28 09:09:14.000000 robino-1.0.0/robino/url.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 22:49:19.845504 robino-1.0.0/robino.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1297 2023-07-02 22:49:19.000000 robino-1.0.0/robino.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      230 2023-07-02 22:49:19.000000 robino-1.0.0/robino.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-02 22:49:19.000000 robino-1.0.0/robino.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       17 2023-07-02 22:49:19.000000 robino-1.0.0/robino.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-07-02 22:49:19.000000 robino-1.0.0/robino.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-02 22:49:19.861504 robino-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1508 2023-06-28 11:04:50.000000 robino-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 23:05:42.253503 robino-1.0.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1342 2023-07-02 23:05:42.241503 robino-1.0.1/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 23:05:42.193503 robino-1.0.1/robino/
+-rw-rw----   0 root         (0) everybody  (9997)       71 2023-06-28 09:15:18.000000 robino-1.0.1/robino/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    10130 2023-06-29 14:14:25.000000 robino-1.0.1/robino/async_rubino.py
+-rw-rw----   0 root         (0) everybody  (9997)     7723 2023-06-29 14:13:55.000000 robino-1.0.1/robino/rubino.py
+-rw-rw----   0 root         (0) everybody  (9997)      979 2023-06-28 09:09:14.000000 robino-1.0.1/robino/url.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 23:05:42.233503 robino-1.0.1/robino.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1342 2023-07-02 23:05:41.000000 robino-1.0.1/robino.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      230 2023-07-02 23:05:41.000000 robino-1.0.1/robino.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-02 23:05:41.000000 robino-1.0.1/robino.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       17 2023-07-02 23:05:41.000000 robino-1.0.1/robino.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-07-02 23:05:41.000000 robino-1.0.1/robino.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-02 23:05:42.253503 robino-1.0.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1537 2023-07-02 23:05:01.000000 robino-1.0.1/setup.py
```

### Comparing `robino-1.0.0/PKG-INFO` & `robino-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: robino
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rubino(Rubika) Library self Bot
 Author: Benyamin karimi
 Author-email: benkarimi2006@gmail.com
 License: MIT
 Keywords: rubika,rubino,chat,bot,robot,asyncio,robino
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 
 
 
 Hello.
 This is an open source library for creating self-bots in Rubino in the Rubica program.
 
 You can easily import this library
```

### Comparing `robino-1.0.0/robino/async_rubino.py` & `robino-1.0.1/robino/async_rubino.py`

 * *Files identical despite different names*

### Comparing `robino-1.0.0/robino/rubino.py` & `robino-1.0.1/robino/rubino.py`

 * *Files identical despite different names*

### Comparing `robino-1.0.0/robino/url.py` & `robino-1.0.1/robino/url.py`

 * *Files identical despite different names*

### Comparing `robino-1.0.0/robino.egg-info/PKG-INFO` & `robino-1.0.1/robino.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: robino
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rubino(Rubika) Library self Bot
 Author: Benyamin karimi
 Author-email: benkarimi2006@gmail.com
 License: MIT
 Keywords: rubika,rubino,chat,bot,robot,asyncio,robino
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 
 
 
 Hello.
 This is an open source library for creating self-bots in Rubino in the Rubica program.
 
 You can easily import this library
```

### Comparing `robino-1.0.0/setup.py` & `robino-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 
 My projects channel: https://t.me/Hells_team
 	
 """
 
 setup(
 	name = "robino",
-	version = "1.0.0",
+	version = "1.0.1",
 	author = "Benyamin karimi",
 	author_email = "benkarimi2006@gmail.com",
 	description = "Rubino(Rubika) Library self Bot",
 	license = "MIT",
 	keywords = ['rubika', 'rubino', 'chat', 'bot', 'robot', 'asyncio', 'robino'],
 	packages = ["robino"],
 	install_requires = requires,
 	long_description = long_description_b,
 	classifiers=['Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
-    "Programming Language :: Python :: Implementation :: PyPy",'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12'],
+    "Programming Language :: Python :: Implementation :: PyPy",
+    'Programming Language :: Python :: 3',   
+    'Programming Language :: Python :: 3.4',
+    'Programming Language :: Python :: 3.5',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',],
         )
```


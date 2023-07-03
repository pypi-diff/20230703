# Comparing `tmp/robino-1.0.2.tar.gz` & `tmp/robino-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robino-1.0.2.tar", last modified: Sun Jul  2 23:45:43 2023, max compression
+gzip compressed data, was "robino-1.0.3.tar", last modified: Mon Jul  3 08:38:00 2023, max compression
```

## Comparing `robino-1.0.2.tar` & `robino-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 23:45:43.584544 robino-1.0.2/
--rw-rw----   0 root         (0) everybody  (9997)     1342 2023-07-02 23:45:43.580543 robino-1.0.2/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 23:45:43.516543 robino-1.0.2/robino/
--rw-rw----   0 root         (0) everybody  (9997)       71 2023-06-28 09:15:18.000000 robino-1.0.2/robino/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    10130 2023-06-29 14:14:25.000000 robino-1.0.2/robino/async_rubino.py
--rw-rw----   0 root         (0) everybody  (9997)     7723 2023-06-29 14:13:55.000000 robino-1.0.2/robino/rubino.py
--rw-rw----   0 root         (0) everybody  (9997)      979 2023-06-28 09:09:14.000000 robino-1.0.2/robino/url.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-02 23:45:43.572543 robino-1.0.2/robino.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1342 2023-07-02 23:45:43.000000 robino-1.0.2/robino.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      230 2023-07-02 23:45:43.000000 robino-1.0.2/robino.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-02 23:45:43.000000 robino-1.0.2/robino.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       17 2023-07-02 23:45:43.000000 robino-1.0.2/robino.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-07-02 23:45:43.000000 robino-1.0.2/robino.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-02 23:45:43.584544 robino-1.0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1545 2023-07-02 23:45:19.000000 robino-1.0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-03 08:38:00.655231 robino-1.0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1342 2023-07-03 08:38:00.647231 robino-1.0.3/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-03 08:38:00.579231 robino-1.0.3/robino/
+-rw-rw----   0 root         (0) everybody  (9997)       71 2023-06-28 09:15:18.000000 robino-1.0.3/robino/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    10130 2023-06-29 14:14:25.000000 robino-1.0.3/robino/async_rubino.py
+-rw-rw----   0 root         (0) everybody  (9997)     7723 2023-06-29 14:13:55.000000 robino-1.0.3/robino/rubino.py
+-rw-rw----   0 root         (0) everybody  (9997)      979 2023-06-28 09:09:14.000000 robino-1.0.3/robino/url.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-03 08:38:00.639231 robino-1.0.3/robino.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1342 2023-07-03 08:38:00.000000 robino-1.0.3/robino.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      230 2023-07-03 08:38:00.000000 robino-1.0.3/robino.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-03 08:38:00.000000 robino-1.0.3/robino.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       17 2023-07-03 08:38:00.000000 robino-1.0.3/robino.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-07-03 08:38:00.000000 robino-1.0.3/robino.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-03 08:38:00.659231 robino-1.0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1545 2023-07-03 08:33:51.000000 robino-1.0.3/setup.py
```

### Comparing `robino-1.0.2/PKG-INFO` & `robino-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robino
-Version: 1.0.2
+Version: 1.0.3
 Summary: Rubino(Rubika) Library self Bot
 Author: Benyamin karimi
 Author-email: benkarimi2006@gmail.com
 License: MIT
 Keywords: rubika,rubino,chat,bot,robot,asyncio,robino
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `robino-1.0.2/robino/async_rubino.py` & `robino-1.0.3/robino/async_rubino.py`

 * *Files identical despite different names*

### Comparing `robino-1.0.2/robino/rubino.py` & `robino-1.0.3/robino/rubino.py`

 * *Files identical despite different names*

### Comparing `robino-1.0.2/robino/url.py` & `robino-1.0.3/robino/url.py`

 * *Files identical despite different names*

### Comparing `robino-1.0.2/robino.egg-info/PKG-INFO` & `robino-1.0.3/robino.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robino
-Version: 1.0.2
+Version: 1.0.3
 Summary: Rubino(Rubika) Library self Bot
 Author: Benyamin karimi
 Author-email: benkarimi2006@gmail.com
 License: MIT
 Keywords: rubika,rubino,chat,bot,robot,asyncio,robino
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `robino-1.0.2/setup.py` & `robino-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 My projects channel: https://t.me/Hells_team
 	
 """
 
 setup(
 	name = "robino",
-	version = "1.0.2",
+	version = "1.0.3",
 	author = "Benyamin karimi",
 	author_email = "benkarimi2006@gmail.com",
 	description = "Rubino(Rubika) Library self Bot",
 	license = "MIT",
 	keywords = ['rubika', 'rubino', 'chat', 'bot', 'robot', 'asyncio', 'robino'],
 	packages = ["robino"],
 	install_requires = requirements,
```


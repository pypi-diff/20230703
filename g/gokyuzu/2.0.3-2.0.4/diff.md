# Comparing `tmp/gokyuzu-2.0.3.tar.gz` & `tmp/gokyuzu-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-2.0.3.tar", last modified: Tue May  2 16:48:17 2023, max compression
+gzip compressed data, was "gokyuzu-2.0.4.tar", last modified: Mon Jul  3 19:03:43 2023, max compression
```

## Comparing `gokyuzu-2.0.3.tar` & `gokyuzu-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.800279 gokyuzu-2.0.3/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-2.0.3/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     6425 2023-05-02 16:48:17.800153 gokyuzu-2.0.3/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     5650 2023-05-02 16:35:40.000000 gokyuzu-2.0.3/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.798564 gokyuzu-2.0.3/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-05-02 15:12:35.000000 gokyuzu-2.0.3/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      688 2023-05-02 16:34:14.000000 gokyuzu-2.0.3/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)      247 2023-05-02 15:06:44.000000 gokyuzu-2.0.3/gokyuzu/BlueskyRecords.py
--rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-05-02 16:34:27.000000 gokyuzu-2.0.3/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)    31220 2023-05-02 16:26:14.000000 gokyuzu-2.0.3/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.799505 gokyuzu-2.0.3/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     6425 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      357 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-05-02 16:37:49.000000 gokyuzu-2.0.3/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-05-02 16:48:17.800324 gokyuzu-2.0.3/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1028 2023-05-02 16:47:35.000000 gokyuzu-2.0.3/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.799740 gokyuzu-2.0.3/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-2.0.3/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-05-02 16:33:19.000000 gokyuzu-2.0.3/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.509438 gokyuzu-2.0.4/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     6427 2023-07-03 19:03:43.509312 gokyuzu-2.0.4/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     5652 2023-07-03 19:01:58.000000 gokyuzu-2.0.4/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.507897 gokyuzu-2.0.4/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      688 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)      247 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskyRecords.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)    31236 2023-07-03 19:02:31.000000 gokyuzu-2.0.4/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.508786 gokyuzu-2.0.4/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     6427 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      357 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-07-03 19:03:04.000000 gokyuzu-2.0.4/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-07-03 19:03:43.509479 gokyuzu-2.0.4/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1028 2023-07-03 19:02:59.000000 gokyuzu-2.0.4/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.509007 gokyuzu-2.0.4/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/tests/test_main.py
```

### Comparing `gokyuzu-2.0.3/PKG-INFO` & `gokyuzu-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.3
+Version: 2.0.4
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -181,16 +181,16 @@
 - `def delete_post( repo, record_key)` 
 - `def comment( text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None)` 
 
 
 ### Development
 
 ```bash
-python -m venv venv
-source venv/bin/activate
+python -m venv .venv
+source .venv/bin/activate
 pip install -r requirements.txt
 ```
 
 ### Running tests
 
 ```bash
 python -m unittest
```

### Comparing `gokyuzu-2.0.3/README.md` & `gokyuzu-2.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,16 @@
 - `def delete_post( repo, record_key)` 
 - `def comment( text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None)` 
 
 
 ### Development
 
 ```bash
-python -m venv venv
-source venv/bin/activate
+python -m venv .venv
+source .venv/bin/activate
 pip install -r requirements.txt
 ```
 
 ### Running tests
 
 ```bash
 python -m unittest
```

### Comparing `gokyuzu-2.0.3/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-2.0.4/gokyuzu/BlueskyEndpoints.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.3/gokyuzu/BlueskyHelper.py` & `gokyuzu-2.0.4/gokyuzu/BlueskyHelper.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.3/gokyuzu/BlueskySession.py` & `gokyuzu-2.0.4/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.3/gokyuzu/__init__.py` & `gokyuzu-2.0.4/gokyuzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         if handle:
             user_did = self.resolveHandle(handle).json().get("did")
 
         if not user_did or user_did is None:
             raise ValueError("Invalid username")
 
         follow_request_data = {
-            "repo": self.DID,
+            "repo": self.SESSION.DID,
             "record": {
                 "subject": user_did,
                 "createdAt": BlueskyHelper.getTimestamp(),
                 "$type": "app.bsky.graph.follow"
             },
             "collection": "app.bsky.graph.follow"
         }
@@ -313,15 +313,15 @@
         if handle:
             user_did = self.resolveHandle(handle).json().get("did")
 
         if not user_did or user_did is None:
             raise ValueError("Invalid username")
 
         unfollow_request_data = {
-            "repo": self.DID,
+            "repo": self.SESSION.DID,
             "record": {
                 "subject": user_did,
                 "createdAt": BlueskyHelper.getTimestamp(),
                 "$type": "app.bsky.graph.unfollow"
             },
             "collection": "app.bsky.graph.unfollow"
         }
```

### Comparing `gokyuzu-2.0.3/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-2.0.4/gokyuzu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.3
+Version: 2.0.4
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -181,16 +181,16 @@
 - `def delete_post( repo, record_key)` 
 - `def comment( text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None)` 
 
 
 ### Development
 
 ```bash
-python -m venv venv
-source venv/bin/activate
+python -m venv .venv
+source .venv/bin/activate
 pip install -r requirements.txt
 ```
 
 ### Running tests
 
 ```bash
 python -m unittest
```

### Comparing `gokyuzu-2.0.3/setup.py` & `gokyuzu-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='2.0.3',
+    version='2.0.4',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-2.0.3/tests/test_main.py` & `gokyuzu-2.0.4/tests/test_main.py`

 * *Files identical despite different names*


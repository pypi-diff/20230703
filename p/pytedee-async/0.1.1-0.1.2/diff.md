# Comparing `tmp/pytedee_async-0.1.1.tar.gz` & `tmp/pytedee_async-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.1.1.tar", last modified: Sat Jul  1 06:38:49 2023, max compression
+gzip compressed data, was "pytedee_async-0.1.2.tar", last modified: Mon Jul  3 12:36:32 2023, max compression
```

## Comparing `pytedee_async-0.1.1.tar` & `pytedee_async-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/setup.py
```

### Comparing `pytedee_async-0.1.1/LICENSE` & `pytedee_async-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.1/PKG-INFO` & `pytedee_async-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee_async
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.1.1/README.md` & `pytedee_async-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.1/pytedee_async/Lock.py` & `pytedee_async-0.1.2/pytedee_async/Lock.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.1/pytedee_async/TedeeClient.py` & `pytedee_async-0.1.2/pytedee_async/TedeeClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
                     for lock_json in result:            
                         lock_id = lock_json["id"]
                         lock_name = lock_json["name"]
                         lock_type = lock_json["type"]
                         lock = Lock(lock_name, lock_id, lock_type)
 
-                        lock.connected, lock.state, lock.battery_level, lock.is_charging = self.parse_lock_properties(lock_json) 
+                        lock.is_connected, lock.state, lock.battery_level, lock.is_charging = self.parse_lock_properties(lock_json) 
                         lock.is_enabled_pullspring, lock.duration_pullspring = self.parse_pull_spring_settings(lock_json)
                         
                         
                         self._locks_dict[lock_id] = lock
 
                     if lock_id == None:
                         raise TedeeClientException("No lock found")
```

### Comparing `pytedee_async-0.1.1/pytedee_async/helpers.py` & `pytedee_async-0.1.2/pytedee_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.1/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.1.2/pytedee_async.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee-async
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.1.1/setup.py` & `pytedee_async-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.1.1",
+    version="0.1.2",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```


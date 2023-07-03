# Comparing `tmp/pytedee_async-0.1.2.tar.gz` & `tmp/pytedee_async-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.1.2.tar", last modified: Mon Jul  3 12:36:32 2023, max compression
+gzip compressed data, was "pytedee_async-0.1.3.tar", last modified: Mon Jul  3 13:20:52 2023, max compression
```

## Comparing `pytedee_async-0.1.2.tar` & `pytedee_async-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/pytedee_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:36:32.000000 pytedee_async-0.1.2/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:36:32.339421 pytedee_async-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 12:36:14.000000 pytedee_async-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/setup.py
```

### Comparing `pytedee_async-0.1.2/LICENSE` & `pytedee_async-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.2/PKG-INFO` & `pytedee_async-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee_async
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.1.2/README.md` & `pytedee_async-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.2/pytedee_async/Lock.py` & `pytedee_async-0.1.3/pytedee_async/Lock.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self._name = name
         self._id = id
         self._type = type
         self._state = 0
         self._battery_level = None
         self._is_connected = False
         self._is_charging = False
+        self._state_change_result = 0
         
     @property
     def name(self):
         return self._name
     
     @property
     def id(self):
@@ -55,21 +56,33 @@
     def is_state_locked(self):
         return self._state == 6
     
     @property
     def is_state_unlocked(self):
         return self._state == 2
     
+    @property 
+    def is_state_jammed(self):
+        return self._state_change_result == 1
+    
     @property
     def state(self):
         return self._state
     
     @state.setter
     def state(self, status):
         self._state = status
+
+    @property
+    def state_change_result(self):
+        return self._state_change_result
+    
+    @state_change_result.setter
+    def state_change_result(self, result):
+        self._state_change_result = result
         
     @property
     def battery_level(self):
         return self._battery_level
     
     @battery_level.setter
     def battery_level(self, level):
```

### Comparing `pytedee_async-0.1.2/pytedee_async/TedeeClient.py` & `pytedee_async-0.1.3/pytedee_async/TedeeClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
                     for lock_json in result:            
                         lock_id = lock_json["id"]
                         lock_name = lock_json["name"]
                         lock_type = lock_json["type"]
                         lock = Lock(lock_name, lock_id, lock_type)
 
-                        lock.is_connected, lock.state, lock.battery_level, lock.is_charging = self.parse_lock_properties(lock_json) 
+                        lock.is_connected, lock.state, lock.battery_level, lock.is_charging, lock.state_change_result = self.parse_lock_properties(lock_json) 
                         lock.is_enabled_pullspring, lock.duration_pullspring = self.parse_pull_spring_settings(lock_json)
                         
                         
                         self._locks_dict[lock_id] = lock
 
                     if lock_id == None:
                         raise TedeeClientException("No lock found")
@@ -194,25 +194,30 @@
         lock_properties = state["lockProperties"]
 
         if lock_properties["state"]:
             state = lock_properties["state"]
         else:
             state = 9
 
+        if lock_properties["stateChangeResult"]:
+            state_change_result = lock_properties["stateChangeResult"]
+        else:
+            state_change_result = 0
+
         if lock_properties["batteryLevel"]:
             battery_level = lock_properties["batteryLevel"]
         else:
             battery_level = 0
 
         if lock_properties["isCharging"]:
             is_charging = lock_properties["isCharging"]
         else:
             is_charging = False
 
-        return connected, state, battery_level, is_charging
+        return connected, state, battery_level, is_charging, state_change_result
     
     def parse_pull_spring_settings(self, settings: dict):
         if settings["deviceSettings"]["pullSpringEnabled"]:
             pullSpringEnabled = settings["deviceSettings"]["pullSpringEnabled"]
         else:
             pullSpringEnabled = False
```

### Comparing `pytedee_async-0.1.2/pytedee_async/helpers.py` & `pytedee_async-0.1.3/pytedee_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.2/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.1.3/pytedee_async.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee-async
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.1.2/setup.py` & `pytedee_async-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.1.2",
+    version="0.1.3",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```


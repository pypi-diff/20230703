# Comparing `tmp/pykumo-0.3.5.tar.gz` & `tmp/pykumo-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykumo-0.3.5.tar", last modified: Sat Apr  8 13:28:33 2023, max compression
+gzip compressed data, was "pykumo-0.3.6.tar", last modified: Mon Jul  3 17:38:12 2023, max compression
```

## Comparing `pykumo-0.3.5.tar` & `pykumo-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:28:33.922571 pykumo-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 13:28:24.000000 pykumo-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-08 13:28:33.922571 pykumo-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-08 13:28:24.000000 pykumo-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:28:33.922571 pykumo-0.3.5/pykumo/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 13:28:24.000000 pykumo-0.3.5/pykumo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-08 13:28:24.000000 pykumo-0.3.5/pykumo/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-04-08 13:28:24.000000 pykumo-0.3.5/pykumo/py_kumo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-08 13:28:24.000000 pykumo-0.3.5/pykumo/py_kumo_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-08 13:28:24.000000 pykumo-0.3.5/pykumo/py_kumo_cloud_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-08 13:28:24.000000 pykumo-0.3.5/pykumo/py_kumo_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:28:33.922571 pykumo-0.3.5/pykumo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-08 13:28:33.000000 pykumo-0.3.5/pykumo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-08 13:28:33.000000 pykumo-0.3.5/pykumo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 13:28:33.000000 pykumo-0.3.5/pykumo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 13:28:33.000000 pykumo-0.3.5/pykumo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 13:28:33.922571 pykumo-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-08 13:28:24.000000 pykumo-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:38:12.299850 pykumo-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 17:38:02.000000 pykumo-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-03 17:38:12.299850 pykumo-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-03 17:38:02.000000 pykumo-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:38:12.299850 pykumo-0.3.6/pykumo/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 17:38:02.000000 pykumo-0.3.6/pykumo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-03 17:38:02.000000 pykumo-0.3.6/pykumo/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-07-03 17:38:02.000000 pykumo-0.3.6/pykumo/py_kumo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-03 17:38:02.000000 pykumo-0.3.6/pykumo/py_kumo_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-07-03 17:38:02.000000 pykumo-0.3.6/pykumo/py_kumo_cloud_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-03 17:38:02.000000 pykumo-0.3.6/pykumo/py_kumo_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:38:12.299850 pykumo-0.3.6/pykumo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-03 17:38:12.000000 pykumo-0.3.6/pykumo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 17:38:12.000000 pykumo-0.3.6/pykumo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:38:12.000000 pykumo-0.3.6/pykumo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 17:38:12.000000 pykumo-0.3.6/pykumo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 17:38:12.000000 pykumo-0.3.6/pykumo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:38:12.299850 pykumo-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-03 17:38:02.000000 pykumo-0.3.6/setup.py
```

### Comparing `pykumo-0.3.5/LICENSE` & `pykumo-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pykumo-0.3.5/PKG-INFO` & `pykumo-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykumo
-Version: 0.3.5
+Version: 0.3.6
 Summary: Small library for interfacing with Mitsubishi KumoCloud enabled devices
 Home-page: https://github.com/dlarrick/pykumo
 Author: Doug Larrick
 Author-email: doug@parkercat.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pykumo-0.3.5/README.md` & `pykumo-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pykumo-0.3.5/pykumo/const.py` & `pykumo-0.3.6/pykumo/const.py`

 * *Files identical despite different names*

### Comparing `pykumo-0.3.5/pykumo/py_kumo.py` & `pykumo-0.3.6/pykumo/py_kumo.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from requests.adapters import HTTPAdapter
 from requests.exceptions import Timeout
 from getpass import getpass
 from .const import CACHE_INTERVAL_SECONDS, POSSIBLE_SENSORS
 from .py_kumo_base import PyKumoBase
 
 _LOGGER = logging.getLogger(__name__)
+ALL_FAN_SPEEDS=[
+    "superQuiet", "quiet", "low", "Low", "powerful", "superPowerful"]
 
 def merge(d, v):
     """
     Merge two dictionaries.
 
     Merge dict-like `v` into dict-like `d`. In case keys between them are the same, merge
     their sub-dictionaries where possible. Otherwise, values in `v` overwrite `d`.
@@ -246,22 +248,24 @@
 
     def get_fan_speeds(self):
         """ List of valid fan speeds for unit """
         try:
             speeds = self._profile['numberOfFanSpeeds']
         except KeyError:
             speeds = 5
-        if speeds not in (5, 3):
+        if speeds not in (5, 4, 3):
             _LOGGER.info(
                 "Unit reports a different number of fan speeds than "
-                "supported, %d != [5|3]. Please report which ones work!",
+                "supported, %d != [5|4|3]. Please report which ones work!",
                 self._profile['numberOfFanSpeeds'])
 
         if speeds == 3:
             valid_speeds = ["quiet", "low", "powerful"]
+        elif speeds == 4:
+            valid_speeds = ["quiet", "Low", "powerful", "superPowerful"]
         else:
             valid_speeds = ["superQuiet", "quiet", "low", "powerful", "superPowerful"]
         try:
             if self._profile['hasFanSpeedAuto']:
                 valid_speeds.append('auto')
         except KeyError:
             pass
@@ -477,18 +481,23 @@
         self._last_status_update = time.monotonic()
         return response
 
     def set_fan_speed(self, speed):
         """ Change fan speed. Valid speeds: superQuiet, quiet, low, powerful,
             superPowerful, sometimes auto
         """
+        if speed not in ALL_FAN_SPEEDS:
+            _LOGGER.warning(
+                "Attempting to set invalid fan speed %s", speed)
+            return {}
         valid_speeds = self.get_fan_speeds()
         if speed not in valid_speeds:
-            _LOGGER.warning("Attempting to set invalid fan speed %s", speed)
-            return {}
+            _LOGGER.warning(
+                "Unit does not report fan speed %s as supported. "
+                "Setting anyway", speed)
         command = ('{"c": { "indoorUnit": { "status": { "fanSpeed": "%s" } } } }'
                    % speed).encode('utf-8')
         response = self._request(command)
         self._status['fanSpeed'] = speed
         self._last_status_update = time.monotonic()
         return response
```

### Comparing `pykumo-0.3.5/pykumo/py_kumo_base.py` & `pykumo-0.3.6/pykumo/py_kumo_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,17 @@
         token = hashlib.sha256(intermediate).hexdigest()
 
         return token
 
     def _request(self, post_data):
         """ Send request to configured unit and return response dict
         """
+        if not self._address:
+            _LOGGER.warning("Unit %s address not set", self._name)
+            return {}
         url = "http://" + self._address + "/api"
         token = self._token(post_data)
         headers = {'Accept': 'application/json, text/plain, */*',
                    'Content-Type': 'application/json'}
         token_param = {'m': token}
         try:
             with requests.Session() as session:
```

### Comparing `pykumo-0.3.5/pykumo/py_kumo_cloud_account.py` & `pykumo-0.3.6/pykumo/py_kumo_cloud_account.py`

 * *Files identical despite different names*

### Comparing `pykumo-0.3.5/pykumo/py_kumo_station.py` & `pykumo-0.3.6/pykumo/py_kumo_station.py`

 * *Files identical despite different names*

### Comparing `pykumo-0.3.5/pykumo.egg-info/PKG-INFO` & `pykumo-0.3.6/pykumo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykumo
-Version: 0.3.5
+Version: 0.3.6
 Summary: Small library for interfacing with Mitsubishi KumoCloud enabled devices
 Home-page: https://github.com/dlarrick/pykumo
 Author: Doug Larrick
 Author-email: doug@parkercat.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pykumo-0.3.5/setup.py` & `pykumo-0.3.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pykumo",
-    version="0.3.5",
+    version="0.3.6",
     author="Doug Larrick",
     author_email="doug@parkercat.org",
     description="Small library for interfacing with Mitsubishi KumoCloud enabled devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dlarrick/pykumo",
     packages=setuptools.find_packages(),
+    install_requires=['requests', 'urllib3'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```


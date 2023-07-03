# Comparing `tmp/aioautomower-2023.4.5.tar.gz` & `tmp/aioautomower-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2023.4.5.tar", last modified: Sun Apr  9 11:27:46 2023, max compression
+gzip compressed data, was "aioautomower-2023.7.0.tar", last modified: Mon Jul  3 19:00:45 2023, max compression
```

## Comparing `aioautomower-2023.4.5.tar` & `aioautomower-2023.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:27:46.531236 aioautomower-2023.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-09 11:27:46.531236 aioautomower-2023.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:27:46.531236 aioautomower-2023.4.5/aioautomower/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/aioautomower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/aioautomower/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/aioautomower/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/aioautomower/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/aioautomower/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:27:46.531236 aioautomower-2023.4.5/aioautomower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-09 11:27:46.000000 aioautomower-2023.4.5/aioautomower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-09 11:27:46.000000 aioautomower-2023.4.5/aioautomower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:27:46.000000 aioautomower-2023.4.5/aioautomower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 11:27:46.000000 aioautomower-2023.4.5/aioautomower.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 11:27:46.000000 aioautomower-2023.4.5/aioautomower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 11:27:46.000000 aioautomower-2023.4.5/aioautomower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:27:46.531236 aioautomower-2023.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-09 11:27:37.000000 aioautomower-2023.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/aioautomower/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/aioautomower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/setup.py
```

### Comparing `aioautomower-2023.4.5/LICENSE` & `aioautomower-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.4.5/PKG-INFO` & `aioautomower-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2023.4.5
+Version: 2023.7.0
 Summary: module to communicate to Husqvarna Automower API
 Home-page: https://github.com/Thomas55555/aioautomower
 Author: Thomas Protzner
 Author-email: thomas.protzner@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aioautomower-2023.4.5/README.md` & `aioautomower-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.4.5/aioautomower/cli.py` & `aioautomower-2023.7.0/aioautomower/cli.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.4.5/aioautomower/const.py` & `aioautomower-2023.7.0/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.4.5/aioautomower/rest.py` & `aioautomower-2023.7.0/aioautomower/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,23 @@
 
     def __init__(self, status: str) -> None:
         """Initialize."""
         super().__init__(status)
         self.status = status
 
 
+class MowerApiConnectionsError(Exception):
+    """Raised when Husqvarna Connect API request ended in error 403."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
+
+
 class GetAccessTokenClientCredentials:
     """Class to get an acces token from the Authentication API with client_credentials.
     This grant type is intended only for you. If you want other users to use your application,
     then they should login using Authorization Code Grant."""
 
     def __init__(self, client_id, client_secret) -> None:
         """Initialize the Auth-API and store the auth so we can make requests."""
@@ -168,14 +177,18 @@
                         result["data"][idx]["attributes"].update(
                             result["data"][idx]["attributes"]["settings"]
                         )
                         del result["data"][idx]["attributes"]["settings"]
                     _LOGGER.debug("Result mower data: %s", result)
                 if resp.status >= 400:
                     _LOGGER.error("Response mower data: %s", result)
+                    if resp.status == 403:
+                        raise MowerApiConnectionsError(
+                            f"Error {resp.status}, the mower state can't be fetched: {result}"
+                        )
         return result
 
 
 class Return:
     """Class to send commands to the Automower Connect API."""
 
     def __init__(
```

### Comparing `aioautomower-2023.4.5/aioautomower/session.py` & `aioautomower-2023.7.0/aioautomower/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,23 @@
     WS_TOLERANCE_TIME,
     WS_URL,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
+class RefresehdTokenNotWorkingError(Exception):
+    """Raised when token is refresehd 5 times, but Connect API still raises an exception."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
+
+
 class AutomowerSession:
     """Session"""
 
     def __init__(
         self,
         api_key: str,
         token: dict = None,
@@ -55,14 +64,15 @@
 
         self.data = None
 
         self.ws_task = None
         self.token_task = None
         self.websocket_monitor_task = None
         self.rest_task = None
+        self.mower_connection_error_count = 0
 
     def register_data_callback(self, callback, schedule_immediately=False):
         """Register a data update callback.
 
         :param func callback: Callback fired on data updates. Takes one dict argument which is the up-to-date mower data list.
         :param bool schedule_immediately: Schedule callback immediately (if data is available).
         """
@@ -321,24 +331,28 @@
                             _LOGGER.debug("Received CLOSED")
                         else:
                             _LOGGER.debug("Received msg.type=%d", msg.type)
 
     async def _rest_task(self):
         """Poll data periodically via Rest."""
         while True:
-            _LOGGER.debug(
-                "LE: %s",
-                self.low_energy,
-            )
             if self.low_energy is True:
                 await asyncio.sleep(REST_POLL_CYCLE_LE)
             if self.low_energy is False:
                 await asyncio.sleep(REST_POLL_CYCLE)
-            self.data = await self.get_status()
-            self._schedule_data_callbacks()
+            try:
+                self.data = await self.get_status()
+                self._schedule_data_callbacks()
+                self.mower_connection_error_count = 0
+            except rest.MowerApiConnectionsError:
+                self.mower_connection_error_count += 1
+                if self.mower_connection_error_count < 5:
+                    self.refresh_token()
+                if self.mower_connection_error_count == 5:
+                    raise RefresehdTokenNotWorkingError
 
     async def _websocket_monitor_task(self):
         """Monitor, if the websocket still sends updates. If not, check, via REST,
         if the mower is connected. If there are no recent updates, Start REST task
         to get information"""
         message_sent = []
         mower_connected = []
```

### Comparing `aioautomower-2023.4.5/aioautomower.egg-info/PKG-INFO` & `aioautomower-2023.7.0/aioautomower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2023.4.5
+Version: 2023.7.0
 Summary: module to communicate to Husqvarna Automower API
 Home-page: https://github.com/Thomas55555/aioautomower
 Author: Thomas Protzner
 Author-email: thomas.protzner@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aioautomower-2023.4.5/setup.py` & `aioautomower-2023.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,12 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=list(val.strip() for val in open("requirements.txt")),
-    version="2023.4.5",
+    version="2023.7.0",
     entry_points={
         "console_scripts": ["automower=aioautomower.cli:main"],
     },
 )
```


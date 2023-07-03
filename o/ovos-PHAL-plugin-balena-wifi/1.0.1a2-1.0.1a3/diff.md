# Comparing `tmp/ovos-PHAL-plugin-balena-wifi-1.0.1a2.tar.gz` & `tmp/ovos-PHAL-plugin-balena-wifi-1.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-balena-wifi-1.0.1a2.tar", last modified: Tue Apr  4 23:09:41 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-balena-wifi-1.0.1a3.tar", last modified: Mon Jul  3 21:33:09 2023, max compression
```

## Comparing `ovos-PHAL-plugin-balena-wifi-1.0.1a2.tar` & `ovos-PHAL-plugin-balena-wifi-1.0.1a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:09:41.489967 ovos-PHAL-plugin-balena-wifi-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 23:09:41.489967 ovos-PHAL-plugin-balena-wifi-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-04 23:09:32.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:09:41.489967 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-04-04 23:09:32.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 23:09:35.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:09:41.489967 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 23:09:41.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 23:09:41.489967 ovos-PHAL-plugin-balena-wifi-1.0.1a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-04-04 23:09:32.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:33:09.435371 ovos-PHAL-plugin-balena-wifi-1.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 21:33:09.435371 ovos-PHAL-plugin-balena-wifi-1.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-03 21:32:55.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:33:09.435371 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-07-03 21:32:55.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-03 21:33:02.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:33:09.435371 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:33:09.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:33:09.435371 ovos-PHAL-plugin-balena-wifi-1.0.1a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-07-03 21:32:55.000000 ovos-PHAL-plugin-balena-wifi-1.0.1a3/setup.py
```

### Comparing `ovos-PHAL-plugin-balena-wifi-1.0.1a2/PKG-INFO` & `ovos-PHAL-plugin-balena-wifi-1.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-balena-wifi
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: Balena wifi plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-balena-wifi
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-balena-wifi-1.0.1a2/README.md` & `ovos-PHAL-plugin-balena-wifi-1.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi/__init__.py` & `ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 from distutils.spawn import find_executable
 from os.path import dirname, join, isfile
 from time import sleep
 
 import pexpect
-from mycroft_bus_client.message import Message, dig_for_message
+from ovos_bus_client.message import Message, dig_for_message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.gui import (GUIInterface,
                             is_gui_running, is_gui_connected)
 from ovos_utils.log import LOG
 
 
 class BalenaWifiValidator:
@@ -19,15 +19,15 @@
 
 
 class BalenaWifiSetupPlugin(PHALPlugin):
     validator = BalenaWifiValidator
 
     def __init__(self, bus=None, config=None):
         super().__init__(bus=bus, name="ovos-PHAL-plugin-balena-wifi", config=config)
-        LOG.info(f"self.config={self.config}")
+        LOG.debug(f"self.config={self.config}")
 
         self._max_errors = 5
         self.gui = GUIInterface(bus=self.bus, skill_id=self.name)
         self.client_active = False
         self.client_id = None
         self.registered = False
         
@@ -71,74 +71,74 @@
         get_client = message.data.get("client", "")
         if get_client == self.name:
             get_id = message.data.get("id", "")
             self.client_id = get_id
             self.registered = True        
             self.bus.on(f"ovos.phal.wifi.plugin.activate.{self.client_id}", self.handle_activate_client_request)
             self.bus.on(f"ovos.phal.wifi.plugin.deactivate.{self.client_id}", self.handle_deactivate_client_request)
-            LOG.info(f"Client Registered with WIFI Plugin: {self.client_id}")
+            LOG.debug(f"Client Registered with WIFI Plugin: {self.client_id}")
     
     def handle_deregistered(self, message=None):
         self.registered = False
         self.bus.remove(f"ovos.phal.wifi.plugin.activate.{self.client_id}", self.handle_active_client_request)
         self.bus.remove(f"ovos.phal.wifi.plugin.deactivate.{self.client_id}", self.handle_deactivate_client_request)
         self.client_id = None
         
     def handle_registration_failure(self, message=None):
         if not self.registered:
             error = message.data.get("error", "")
-            LOG.info(f"Registration Failure: {error}")
+            LOG.error(f"Registration Failure: {error}")
             # Try to Register the Client with WIFI Plugin Again
             self.register_client()
             
     def handle_activate_client_request(self, message=None):
         """
         Handles an ovos.phal.wifi.plugin.activate.{self.client_id} request.
         This sets the internal `client_active` flag to True and
         calls `display_network_setup`.
         """
-        LOG.info("Balena Wifi Plugin Activated")
+        LOG.debug("Balena Wifi Plugin Activated")
         error_count = 0
         self.client_active = True
         while error_count < self._max_errors and \
                 not self.display_network_setup():
-            LOG.info("Setup failed, retrying")
+            LOG.error("Setup failed, retrying")
             error_count += 1
         if error_count >= self._max_errors:
             self.handle_stop_setup()
         if self.debug:
             self.speak_dialog("debug_end_setup")
         self.handle_stop_setup()
         
     def handle_deactivate_client_request(self, message=None):
         """
         Handles an ovos.phal.wifi.plugin.activate.{self.client_id} request.
         This sets the internal `client_active` flag to False and
         calls `cleanup_wifi_process`.
         """
-        LOG.info("Balena Wifi Plugin Deactivated")
+        LOG.debug("Balena Wifi Plugin Deactivated")
         self.cleanup_wifi_process()
         self.client_active = False
         self.gui.release()
         
     def request_deactivate(self, message=None):
         self.bus.emit(Message("ovos.phal.wifi.plugin.remove.active.client", {
                       "client": "ovos-PHAL-plugin-balena-wifi"}))
-        LOG.info("Balena Wifi Plugin Deactivation Requested")
+        LOG.debug("Balena Wifi Plugin Deactivation Requested")
         
     def display_network_setup(self):
         """
         Start a Balena Wifi process and monitor the output.
         If an error occurs, this method is called recursively to clean up the
         failed instance and start a new one.
         """
-        LOG.info("Balena Wifi In Network Setup")
+        LOG.debug("Balena Wifi In Network Setup")
         # Always start with a clean slate
         self.cleanup_wifi_process()
-        LOG.info(f"Spawning new wifi_process")
+        LOG.debug(f"Spawning new wifi_process")
         self.wifi_process = pexpect.spawn(
             self.wifi_command.format(ssid=self.ssid)
         )
         # https://github.com/pexpect/pexpect/issues/462
         self.wifi_process.delayafterclose = 1
         self.wifi_process.delayafterterminate = 1
         prev = ""
```

### Comparing `ovos-PHAL-plugin-balena-wifi-1.0.1a2/ovos_PHAL_plugin_balena_wifi.egg-info/PKG-INFO` & `ovos-PHAL-plugin-balena-wifi-1.0.1a3/ovos_PHAL_plugin_balena_wifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-balena-wifi
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: Balena wifi plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-balena-wifi
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-balena-wifi-1.0.1a2/setup.py` & `ovos-PHAL-plugin-balena-wifi-1.0.1a3/setup.py`

 * *Files identical despite different names*


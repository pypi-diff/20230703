# Comparing `tmp/hass_mqtt_things-0.5.5.tar.gz` & `tmp/hass_mqtt_things-0.5.6.tar.gz`

## Comparing `hass_mqtt_things-0.5.5.tar` & `hass_mqtt_things-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/.flake8
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/__init__.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/binary_sensor.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/button.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/fan.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/light.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/manager.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/number.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/sensor.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/switch.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/things.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/src/ham/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/LICENSE
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/README.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/.flake8
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/__init__.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/binary_sensor.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/button.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/fan.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/light.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/manager.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/number.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/sensor.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/switch.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/things.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/src/ham/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/README.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 hass_mqtt_things-0.5.6/PKG-INFO
```

### Comparing `hass_mqtt_things-0.5.5/src/ham/binary_sensor.py` & `hass_mqtt_things-0.5.6/src/ham/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/button.py` & `hass_mqtt_things-0.5.6/src/ham/button.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/fan.py` & `hass_mqtt_things-0.5.6/src/ham/fan.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/light.py` & `hass_mqtt_things-0.5.6/src/ham/light.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/manager.py` & `hass_mqtt_things-0.5.6/src/ham/manager.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/number.py` & `hass_mqtt_things-0.5.6/src/ham/number.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 
 
 class Number(Thing):
     """Basic class for a Number entity."""
     min: float
     max: float
     step: float
+    device_class: str
+    unit_of_measurement: str
 
-    config_fields = ["min", "max", "step"]
+    config_fields = ["min", "max", "step",
+                     "device_class", "unit_of_measurement"]
 
     _state: float = 1.0
 
     @property
     def component(self):
         return "number"
```

### Comparing `hass_mqtt_things-0.5.5/src/ham/sensor.py` & `hass_mqtt_things-0.5.6/src/ham/sensor.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/switch.py` & `hass_mqtt_things-0.5.6/src/ham/switch.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/src/ham/things.py` & `hass_mqtt_things-0.5.6/src/ham/things.py`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/.gitignore` & `hass_mqtt_things-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/LICENSE` & `hass_mqtt_things-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/README.md` & `hass_mqtt_things-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/pyproject.toml` & `hass_mqtt_things-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hass_mqtt_things-0.5.5/PKG-INFO` & `hass_mqtt_things-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hass-mqtt-things
-Version: 0.5.5
+Version: 0.5.6
 Summary: Library for rapid development of things to be integrated with Home Assistant through MQTT
 Project-URL: Documentation, https://github.com/alexbarcelo/hass-mqtt-things#readme
 Project-URL: Issues, https://github.com/alexbarcelo/hass-mqtt-things/issues
 Project-URL: Source, https://github.com/alexbarcelo/hass-mqtt-things
 Author-email: Alex Barcelo <alex@betarho.net>
 License-Expression: Apache-2.0
 License-File: LICENSE
```


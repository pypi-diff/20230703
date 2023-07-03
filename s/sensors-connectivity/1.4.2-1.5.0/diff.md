# Comparing `tmp/sensors_connectivity-1.4.2.tar.gz` & `tmp/sensors_connectivity-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensors_connectivity-1.4.2.tar", max compression
+gzip compressed data, was "sensors_connectivity-1.5.0.tar", max compression
```

## Comparing `sensors_connectivity-1.4.2.tar` & `sensors_connectivity-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1507 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/LICENSE
--rw-r--r--   0        0        0     6435 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/README.md
--rw-r--r--   0        0        0       24 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/__init__.py
--rw-r--r--   0        0        0     9099 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/README.md
--rw-r--r--   0        0        0       36 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/default.json
--rw-r--r--   0        0        0      938 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/logging.py
--rw-r--r--   0        0        0      824 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/logging_template.py
--rw-r--r--   0        0        0       94 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/constants.py
--rw-r--r--   0        0        0     5975 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/main.py
--rw-r--r--   0        0        0       51 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/drivers/__init__.py
--rw-r--r--   0        0        0      477 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/drivers/ping.py
--rw-r--r--   0        0        0     5754 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/drivers/sds011.py
--rw-r--r--   0        0        0      189 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/__init__.py
--rw-r--r--   0        0        0     9105 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/datalog_feeder.py
--rw-r--r--   0        0        0     1280 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/frontier_datalog.py
--rw-r--r--   0        0        0     1088 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/ifeeder.py
--rw-r--r--   0        0        0     3166 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/robonomics_feeder.py
--rw-r--r--   0        0        0      224 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/__init__.py
--rw-r--r--   0        0        0     1461 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/base.py
--rw-r--r--   0        0        0     2077 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/environmental_box.py
--rw-r--r--   0        0        0      643 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/lora_sensors.py
--rw-r--r--   0        0        0     1474 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/mobile_lab.py
--rw-r--r--   0        0        0     1427 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_sds011.py
--rw-r--r--   0        0        0      771 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_template.py
--rw-r--r--   0        0        0     2603 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/trackagro_sensor.py
--rw-r--r--   0        0        0      212 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/__init__.py
--rw-r--r--   0        0        0     2238 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/comstation.py
--rw-r--r--   0        0        0     4380 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/httpstation.py
--rw-r--r--   0        0        0     1639 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/istation.py
--rw-r--r--   0        0        0     4055 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/mqttstation.py
--rw-r--r--   0        0        0     3089 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/trackargostation.py
--rw-r--r--   0        0        0       55 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/database.py
--rwxr-xr-x   0        0        0     3207 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/flash_firmware.py
--rwxr-xr-x   0        0        0     1825 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/generate_secrets.py
--rw-r--r--   0        0        0      391 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/get_mac.py
--rwxr-xr-x   0        0        0      553 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/py_generate_secrets.py
--rwxr-xr-x   0        0        0     2502 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/virtual-sensor.py
--rw-r--r--   0        0        0     1174 2023-06-12 10:48:06.675042 sensors_connectivity-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 sensors_connectivity-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1507 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4549 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/README.md
+-rw-r--r--   0        0        0       24 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/__init__.py
+-rw-r--r--   0        0        0     9099 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/config/README.md
+-rw-r--r--   0        0        0       36 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/config/__init__.py
+-rw-r--r--   0        0        0     1006 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/config/default.json
+-rw-r--r--   0        0        0      938 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/config/logging.py
+-rw-r--r--   0        0        0      824 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/config/logging_template.py
+-rw-r--r--   0        0        0       94 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/constants.py
+-rw-r--r--   0        0        0     5975 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/main.py
+-rw-r--r--   0        0        0       51 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/drivers/__init__.py
+-rw-r--r--   0        0        0      477 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/drivers/ping.py
+-rw-r--r--   0        0        0     5754 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/drivers/sds011.py
+-rw-r--r--   0        0        0      189 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/feeders/__init__.py
+-rw-r--r--   0        0        0     9184 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/feeders/datalog_feeder.py
+-rw-r--r--   0        0        0     1280 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/feeders/frontier_datalog.py
+-rw-r--r--   0        0        0     1088 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/feeders/ifeeder.py
+-rw-r--r--   0        0        0     3205 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/feeders/robonomics_feeder.py
+-rw-r--r--   0        0        0      224 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/__init__.py
+-rw-r--r--   0        0        0     1592 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/base.py
+-rw-r--r--   0        0        0     2140 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/environmental_box.py
+-rw-r--r--   0        0        0      643 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/lora_sensors.py
+-rw-r--r--   0        0        0     1474 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/mobile_lab.py
+-rw-r--r--   0        0        0     1427 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/sensor_sds011.py
+-rw-r--r--   0        0        0      771 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/sensor_template.py
+-rw-r--r--   0        0        0     2603 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/sensors/trackagro_sensor.py
+-rw-r--r--   0        0        0      212 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/stations/__init__.py
+-rw-r--r--   0        0        0     2238 2023-07-03 12:17:51.500136 sensors_connectivity-1.5.0/connectivity/src/stations/comstation.py
+-rw-r--r--   0        0        0     4380 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/src/stations/httpstation.py
+-rw-r--r--   0        0        0     1639 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/src/stations/istation.py
+-rw-r--r--   0        0        0     4055 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/src/stations/mqttstation.py
+-rw-r--r--   0        0        0     3089 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/src/stations/trackargostation.py
+-rw-r--r--   0        0        0       55 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/database.py
+-rwxr-xr-x   0        0        0     3207 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/flash_firmware.py
+-rwxr-xr-x   0        0        0     1825 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/generate_secrets.py
+-rw-r--r--   0        0        0      391 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/get_mac.py
+-rwxr-xr-x   0        0        0      553 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/py_generate_secrets.py
+-rwxr-xr-x   0        0        0     2502 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/connectivity/utils/virtual-sensor.py
+-rw-r--r--   0        0        0     1174 2023-07-03 12:17:51.504135 sensors_connectivity-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5775 1970-01-01 00:00:00.000000 sensors_connectivity-1.5.0/PKG-INFO
```

### Comparing `sensors_connectivity-1.4.2/LICENSE` & `sensors_connectivity-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/config/README.md` & `sensors_connectivity-1.5.0/connectivity/config/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/config/default.json` & `sensors_connectivity-1.5.0/connectivity/config/default.json`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/config/logging.py` & `sensors_connectivity-1.5.0/connectivity/config/logging.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/config/logging_template.py` & `sensors_connectivity-1.5.0/connectivity/config/logging_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/main.py` & `sensors_connectivity-1.5.0/connectivity/main.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/drivers/sds011.py` & `sensors_connectivity-1.5.0/connectivity/src/drivers/sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/feeders/datalog_feeder.py` & `sensors_connectivity-1.5.0/connectivity/src/feeders/datalog_feeder.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     :param data: Measurements dict.
     :return: Sorted measurements dict.
     """
 
     ordered = {}
     for k, v in data.items():
         meas = sorted(v["measurements"], key=lambda x: x["timestamp"])
-        ordered[k] = {"model": v["model"], "geo": v["geo"], "measurements": meas}
+        ordered[k] = {"model": v["model"], "geo": v["geo"], "donated_by": v["donated_by"], "measurements": meas}
     return ordered
 
 
 def _get_multihash(buf: set, db: object, endpoint: str = "/ip4/127.0.0.1/tcp/5001/http") -> tp.Dict[str, str]:
     """Write sorted measurements to the temp file, add file to IPFS and add 
     measurements and hash in the database with 'not sent' status.
 
@@ -71,14 +71,15 @@
         try:
             if m.public in payload:
                 payload[m.public]["measurements"].append(m.measurement)
             else:
                 payload[m.public] = {
                     "model": m.model,
                     "geo": "{},{}".format(m.geo_lat, m.geo_lon),
+                    "donated_by": m.donated_by,
                     "measurements": [m.measurement],
                 }
         except Exception as e:
             logger.warning(f"Datalog Feeder: Couldn't store data: {e}")
 
 
     logger.debug(f"Payload before sorting: {payload}")
```

### Comparing `sensors_connectivity-1.4.2/connectivity/src/feeders/frontier_datalog.py` & `sensors_connectivity-1.5.0/connectivity/src/feeders/frontier_datalog.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/feeders/ifeeder.py` & `sensors_connectivity-1.5.0/connectivity/src/feeders/ifeeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/feeders/robonomics_feeder.py` & `sensors_connectivity-1.5.0/connectivity/src/feeders/robonomics_feeder.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     :return: JSON formatted string for pubsub.
     """
 
     message = {}
     message[data.public] = {
         "model": data.model,
         "geo": "{},{}".format(data.geo_lat, data.geo_lon),
+        "donated_by": data.donated_by,
         "measurement": data.measurement,
     }
     return json.dumps(message)
 
 
 def _to_ping_message(data: dict) -> str:
     """Prepare JSON formatted string with base info about sensor.
```

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/base.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 
     id: str = field(init=False)
     public: str = field(init=False)
     geo_lat: float = field(init=False)
     geo_lon: float = field(init=False)
     model: int = field(init=False)
     timestamp: float = field(init=False)
+    donated_by: str = field(init=False)
     measurement: dict = field(init=False)
 
     def __post_init__(self) -> None:
         self.timestamp = int(time.time())
         self.geo_lat = 0.0
         self.geo_lon = 0.0
         self.measurement = {}
+        self.donated_by = ""
         self.measurement.update({"timestamp": self.timestamp})
 
     def generate_pubkey(self, id: str) -> str:
         """Generate public key for a sensor based on its id.
         
         :param id: Unique id of a sensor.
         :return: Public key of a sensor.
         """
 
         verify_key = hashlib.sha256(id.encode("utf-8"))
         verify_key_hex = verify_key.hexdigest()
         return str(verify_key_hex)
 
     def __str__(self) -> str:
-        return f"{{Public: {self.public}, geo: ({self.geo_lat},{self.geo_lon}), model: {self.model}, measurements: {self.measurement}}}"
+        return f"{{Public: {self.public}, geo: ({self.geo_lat},{self.geo_lon}), model: {self.model}, donated_by: {self.donated_by}, measurements: {self.measurement}}}"
 
     def __repr__(self) -> str:
-        return f"{{Public: {self.public}, geo: ({self.geo_lat},{self.geo_lon}), model: {self.model}, measurements: {self.measurement}}}"
+        return f"{{Public: {self.public}, geo: ({self.geo_lat},{self.geo_lon}), model: {self.model}, donated_by: {self.donated_by}, measurements: {self.measurement}}}"
 
     def __hash__(self) -> int:
         return hash((self.id, self.timestamp))
```

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/environmental_box.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/environmental_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     def __post_init__(self) -> None:
         """Parse data from sensor and store into the corresponding variables."""
         super().__post_init__()
         self.id = str(self.data["esp8266id"])
         self.model = SDS011_MODEL
         self.public = self.generate_pubkey(str(self.id))
+        self.donated_by = str(self.data.get("donated_by", ""))
         sensors_data = self.data["sensordatavalues"]
         for d in sensors_data:
             if d["value_type"] == "GPS_lat":
                 self.geo_lat = d["value"]
             if d["value_type"] == "GPS_lon":
                 self.geo_lon = d["value"]
         self.measurement = reduce(self._SDS011_values_saver, sensors_data, {})
```

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/lora_sensors.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/lora_sensors.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/mobile_lab.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/mobile_lab.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_sds011.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/sensor_sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_template.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/sensor_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/sensors/trackagro_sensor.py` & `sensors_connectivity-1.5.0/connectivity/src/sensors/trackagro_sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/stations/comstation.py` & `sensors_connectivity-1.5.0/connectivity/src/stations/comstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/stations/httpstation.py` & `sensors_connectivity-1.5.0/connectivity/src/stations/httpstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/stations/istation.py` & `sensors_connectivity-1.5.0/connectivity/src/stations/istation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/stations/mqttstation.py` & `sensors_connectivity-1.5.0/connectivity/src/stations/mqttstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/src/stations/trackargostation.py` & `sensors_connectivity-1.5.0/connectivity/src/stations/trackargostation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/utils/database.py` & `sensors_connectivity-1.5.0/connectivity/utils/database.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/utils/flash_firmware.py` & `sensors_connectivity-1.5.0/connectivity/utils/flash_firmware.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/utils/generate_secrets.py` & `sensors_connectivity-1.5.0/connectivity/utils/generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/utils/py_generate_secrets.py` & `sensors_connectivity-1.5.0/connectivity/utils/py_generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/connectivity/utils/virtual-sensor.py` & `sensors_connectivity-1.5.0/connectivity/utils/virtual-sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.2/pyproject.toml` & `sensors_connectivity-1.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensors_connectivity"
-version = "1.4.2"
+version = "1.5.0"
 description = "Robonomics package to read data from sensors and publish to different output channels"
 authors = [
     "Vadim Manaenko <vadim.razorq@gmail.com>",
     "Mariia Bystramovich <m.bystramovich@gmail.com>",
 ]
 license = "BSD 3-Clause License"
```


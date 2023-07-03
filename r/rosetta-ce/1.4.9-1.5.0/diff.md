# Comparing `tmp/rosetta-ce-1.4.9.tar.gz` & `tmp/rosetta-ce-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.4.9.tar", last modified: Mon Jul  3 10:44:36 2023, max compression
+gzip compressed data, was "rosetta-ce-1.5.0.tar", last modified: Mon Jul  3 13:20:01 2023, max compression
```

## Comparing `rosetta-ce-1.4.9.tar` & `rosetta-ce-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 10:44:36.011172 rosetta-ce-1.4.9/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.9/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 10:44:36.010801 rosetta-ce-1.4.9/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.9/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 10:44:36.006112 rosetta-ce-1.4.9/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.9/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 10:44:36.007346 rosetta-ce-1.4.9/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.9/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.9/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.9/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.9/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.9/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44278 2023-07-03 10:43:19.000000 rosetta-ce-1.4.9/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.9/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 10:44:36.008472 rosetta-ce-1.4.9/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 10:44:35.000000 rosetta-ce-1.4.9/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-03 10:44:35.000000 rosetta-ce-1.4.9/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-03 10:44:35.000000 rosetta-ce-1.4.9/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-03 10:44:35.000000 rosetta-ce-1.4.9/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-03 10:44:35.000000 rosetta-ce-1.4.9/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-03 10:44:36.011215 rosetta-ce-1.4.9/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-03 10:43:39.000000 rosetta-ce-1.4.9/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 10:44:36.010365 rosetta-ce-1.4.9/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.9/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.9/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.9/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.854515 rosetta-ce-1.5.0/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.0/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 13:20:01.854013 rosetta-ce-1.5.0/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.0/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.848455 rosetta-ce-1.5.0/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.0/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.850162 rosetta-ce-1.5.0/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.0/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.0/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.0/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.5.0/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.0/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44278 2023-07-03 10:43:19.000000 rosetta-ce-1.5.0/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10384 2023-07-03 13:19:23.000000 rosetta-ce-1.5.0/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.852131 rosetta-ce-1.5.0/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-03 13:20:01.854565 rosetta-ce-1.5.0/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-03 13:19:23.000000 rosetta-ce-1.5.0/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.853595 rosetta-ce-1.5.0/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.0/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.0/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.0/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.4.9/LICENSE` & `rosetta-ce-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/PKG-INFO` & `rosetta-ce-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.9
+Version: 1.5.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.9/README.md` & `rosetta-ce-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/rosetta/constants/sensors.py` & `rosetta-ce-1.5.0/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/rosetta/constants/sources.py` & `rosetta-ce-1.5.0/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/rosetta/constants/systems.py` & `rosetta-ce-1.5.0/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/rosetta/rconverter.py` & `rosetta-ce-1.5.0/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/rosetta/rfaker.py` & `rosetta-ce-1.5.0/rosetta/rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/rosetta/rsender.py` & `rosetta-ce-1.5.0/rosetta/rsender.py`

 * *Files 25% similar despite different names*

```diff
@@ -51,19 +51,21 @@
         send_data() -> None:
             Sends fake data to the destination address.
 
             Returns:
                 None.
     """
 
-    def __init__(self, data_type: str, destination: str,
+    def __init__(self, data_type: str, destination: str, headers: Optional[dict] = None,
                  worker_name: Optional[str] = 'worker_'+str(datetime.now()), count: Optional[int] = 1,
                  interval: Optional[int] = 1, vendor: Optional[str] = None, product: Optional[str] = None,
-                 version: Optional[str] = None, observables: Optional[Observables] = None, fields: Optional[str] = None,
-                 verify_ssl: Optional[bool] = None, datetime_obj: Optional[datetime] = None):
+                 version: Optional[str] = None, required_fields: Optional[str] = None,
+                 observables: Optional[Observables] = None, fields: Optional[str] = None,
+                 verify_ssl: Optional[bool] = None, datetime_obj: Optional[datetime] = None,
+                 data_json: Optional[dict] = None, data_text: Optional[str] = None):
         """
         Constructor for DataSenderWorker class.
 
         :param data_type: A value from the WorkerTypeEnum indicating the type of data to send. Options include:
             - SYSLOG
             - CEF
             - LEEF
@@ -73,35 +75,47 @@
         :param destination: str, destination address and port in the format <scheme>://<address>:<port>.
         :param worker_name: str, name of the worker.
         :param count: int, number of times to send the data.
         :param interval: int, time interval between two consecutive data sends.
         :param vendor: Optional. The vendor.
         :param product: Optional. The product.
         :param version: Optional. The version.
-        :param observables: Observables, list of observables.
-        :param fields: str, comma-separated list of fields to include in incident data.
-        :param verify_ssl: bool, handling ssl verification errors.
+        :param required_fields: Optional. A list of fields that are required to present in the generated data, whether
+         from observables or randomely.
+        :param observables: Optional. Observables, list of observables.
+        :param fields: Optional. comma-separated list of fields to include in incident data.
+        :param verify_ssl: Optional. handling ssl verification errors.
+        :param datetime_obj: Optional. time to start from.
+        :param data_json: Optional. JSON data to send.
+        :param data_text: Optional. Text data to send.
 
         :return: None
         """
+        if headers is None:
+            self.headers = {}
+        else:
+            self.headers = headers
         self.thread = None
         self.worker_name = worker_name
         self.data_type = data_type
         self.count = count
         self.interval = interval
         self.vendor = vendor
         self.product = product
         self.version = version
+        self.required_fields = required_fields
         self.destination = destination
         self.created_at = datetime.now()
         self.status = "Stopped"
         self.observables = observables
         self.fields = fields
         self.verify_ssl = verify_ssl
         self.datetime_obj = datetime_obj
+        self.data_json = data_json
+        self.data_text = data_text
 
     def start(self) -> str:
         """
         Starts the worker thread.
 
         Returns:
             str: Current status of the worker (Running, Stopped).
@@ -133,24 +147,29 @@
             None.
         """
         fake_message = None
         while self.status == "Running" and self.count > 0:
             try:
                 self.count -= 1
                 if self.data_type in ["SYSLOG", "CEF", "LEEF"]:
-                    if self.data_type == "SYSLOG":
-                        fake_message = Events.syslog(count=1, timestamp=self.datetime_obj, observables=self.observables)
-                    if self.data_type == "CEF":
-                        fake_message = Events.cef(count=1, timestamp=self.datetime_obj, vendor=self.vendor,
-                                                  product=self.product, version=self.version,
-                                                  observables=self.observables)
-                    if self.data_type == "LEEF":
-                        fake_message = Events.leef(count=1, timestamp=self.datetime_obj, vendor=self.vendor,
-                                                   product=self.product, version=self.version,
-                                                   observables=self.observables)
+                    if self.data_text:
+                        fake_message = [self.data_text]
+                    else:
+                        if self.data_type == "SYSLOG":
+                            fake_message = Events.syslog(count=1, datetime_iso=self.datetime_obj,
+                                                         observables=self.observables, required_fields=self.required_fields)
+                        if self.data_type == "CEF":
+                            fake_message = Events.cef(count=1, datetime_iso=self.datetime_obj, vendor=self.vendor,
+                                                      product=self.product, version=self.version,
+                                                      required_fields=self.required_fields, observables=self.observables)
+                        if self.data_type == "LEEF":
+                            fake_message = Events.leef(count=1, datetime_iso=self.datetime_obj, vendor=self.vendor,
+                                                       product=self.product, version=self.version,
+                                                       required_fields=self.required_fields,
+                                                       observables=self.observables)
                     ip_address = self.destination.split(':')[1]
                     port = self.destination.split(':')[2]
                     if 'tcp' in self.destination:
                         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                         sock.settimeout(5)
                         sock.connect((ip_address, int(port)))
                         print(f"Worker: {self.worker_name} sending log message to {ip_address} ")
@@ -158,28 +177,37 @@
                         sock.close()
                     else:
                         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
                         sock.settimeout(5)
                         print(f"Worker: {self.worker_name} sending log message to {ip_address} ")
                         sock.sendto(fake_message[0].encode(), (ip_address, int(port)))
                 elif self.data_type in ["JSON", "INCIDENT"]:
-                    if self.data_type == "JSON":
-                        fake_message = Events.json(count=1, timestamp=self.datetime_obj, observables=self.observables)
-                    if self.data_type == "INCIDENT":
-                        fake_message = [{
-                            "alert": Events.incidents(count=1, observables=self.observables, vendor=self.vendor,
-                                                      version=self.version, product=self.product, fields=self.fields)
-                        }]
+                    if self.data_json:
+                        fake_message = [self.data_json]
+                    else:
+                        if self.data_type == "JSON":
+                            fake_message = Events.json(count=1, datetime_iso=self.datetime_obj,
+                                                       observables=self.observables, vendor=self.vendor,
+                                                       product=self.product, version=self.version,
+                                                       required_fields=self.required_fields,)
+                        if self.data_type == "INCIDENT":
+                            fake_message = [{
+                                "alert": Events.incidents(count=1, observables=self.observables, vendor=self.vendor,
+                                                          version=self.version, product=self.product,
+                                                          datetime_iso=self.datetime_obj,
+                                                          required_fields=self.required_fields, fields=self.fields)
+                            }]
                     if '://' not in self.destination:
                         url = 'http://' + self.destination
                     else:
                         url = self.destination
                     warnings.filterwarnings("ignore", category=InsecureRequestWarning)
                     print(f"Worker: {self.worker_name} sending log message to {url} ")
-                    response = requests.post(url, json=fake_message[0], timeout=(2, 5), verify=self.verify_ssl)
+                    response = requests.post(url, json=fake_message[0], timeout=(2, 5), headers=self.headers,
+                                             verify=self.verify_ssl)
                     response.raise_for_status()
             except (ConnectionRefusedError, socket.timeout, requests.exceptions.RequestException) as e:
                 print(f"Connection error: {e}")
                 self.status = "Connection Error"
                 break
             except requests.exceptions.SSLError as e:
                 print(f"SSL error: {e}")
```

### Comparing `rosetta-ce-1.4.9/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.5.0/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.9
+Version: 1.5.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.9/setup.py` & `rosetta-ce-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.4.9",
+    version="1.5.0",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.4.9/tests/test_rconverter.py` & `rosetta-ce-1.5.0/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/tests/test_rfaker.py` & `rosetta-ce-1.5.0/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.9/tests/test_rsender.py` & `rosetta-ce-1.5.0/tests/test_rsender.py`

 * *Files identical despite different names*


# Comparing `tmp/burla-0.0.2.tar.gz` & `tmp/burla-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.2.tar", max compression
+gzip compressed data, was "burla-0.0.3.tar", max compression
```

## Comparing `burla-0.0.2.tar` & `burla-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      599 2023-07-03 15:51:52.145949 burla-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.2/src/burla/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.2/src/burla/_logstream.py
--rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.2/src/burla/config.py
--rw-r--r--   0        0        0     3667 2023-07-03 15:43:06.056382 burla-0.0.2/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 burla-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      496 2023-07-03 16:12:24.224703 burla-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.3/src/burla/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.3/src/burla/_logstream.py
+-rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.3/src/burla/config.py
+-rw-r--r--   0        0        0     3671 2023-07-03 16:09:38.977667 burla-0.0.3/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 burla-0.0.3/PKG-INFO
```

### Comparing `burla-0.0.2/src/burla/_logstream.py` & `burla-0.0.3/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.2/src/burla/config.py` & `burla-0.0.3/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.2/src/burla/remote_parallel_map.py` & `burla-0.0.3/src/burla/remote_parallel_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import binascii
 import dill
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
-API_KEY = load_api_key_from_local_config()
 BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
 
 # BURLA_SERVICE_URL = "https://127.0.0.1:5000"
 
 TZ = timezone.utc
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
@@ -54,21 +53,22 @@
 ):
     if not function_.__annotations__.get("return") is str:
         raise AttributeError("Please add the return type annotation 'str' to your input function.")
 
     if cpus > 100:
         raise AttributeError("Currently unable to satisfy requests for >100 computers")
 
-    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={"key": API_KEY})
+    api_key = load_api_key_from_local_config()
+    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={"key": api_key})
     response.raise_for_status()
     job_id = response.json()["job_id"]
 
     func_pkl_hex_ascii = binascii.hexlify(dill.dumps(function_.__code__)).decode("ascii")
     data = {
-        "key": API_KEY,
+        "key": api_key,
         "func_pkl_hex_ascii": func_pkl_hex_ascii,
         "inputs": inputs,
         "image": image,
         "num_computers": cpus,
     }
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data)
     response.raise_for_status()
```

### Comparing `burla-0.0.2/PKG-INFO` & `burla-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.2
+Version: 0.0.3
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
-Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: google-cloud-build (>=3.16.0,<4.0.0)
-Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
-Requires-Dist: grpcio (>=1.54.2,<2.0.0)
-Requires-Dist: jupyterlab (>=4.0.2,<5.0.0)
+Requires-Dist: requests (==2.27.1)
```


# Comparing `tmp/upstash_redis-0.14.0.tar.gz` & `tmp/upstash_redis-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.14.0.tar", max compression
+gzip compressed data, was "upstash_redis-0.14.1.tar", max compression
```

## Comparing `upstash_redis-0.14.0.tar` & `upstash_redis-0.14.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-07-03 03:59:36.165204 upstash_redis-0.14.0/LICENSE
--rw-r--r--   0        0        0     9173 2023-07-03 03:59:36.165204 upstash_redis-0.14.0/README.md
--rw-r--r--   0        0        0      500 2023-07-03 03:59:36.165204 upstash_redis-0.14.0/pyproject.toml
--rw-r--r--   0        0        0      146 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4896 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     5116 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/client.py
--rw-r--r--   0        0        0       77 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       79 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    21043 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    72037 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    20142 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     5601 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      752 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      174 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     9521 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-03 04:25:55.136423 upstash_redis-0.14.1/LICENSE
+-rw-r--r--   0        0        0     9173 2023-07-03 04:25:55.136423 upstash_redis-0.14.1/README.md
+-rw-r--r--   0        0        0      500 2023-07-03 04:25:55.136423 upstash_redis-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4896 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     5116 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/client.py
+-rw-r--r--   0        0        0       77 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    21043 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    72037 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    20142 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     6254 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      752 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      174 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     9521 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.14.1/PKG-INFO
```

### Comparing `upstash_redis-0.14.0/LICENSE` & `upstash_redis-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/README.md` & `upstash_redis-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/asyncio/client.py` & `upstash_redis-0.14.1/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/client.py` & `upstash_redis-0.14.1/upstash_redis/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.14.1/upstash_redis/commands/async_commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/commands/commands.py` & `upstash_redis-0.14.1/upstash_redis/commands/commands.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/commands/commands.pyi` & `upstash_redis-0.14.1/upstash_redis/commands/commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/http/decode.py` & `upstash_redis-0.14.1/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/http/execute.py` & `upstash_redis-0.14.1/upstash_redis/http/execute.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import aiohttp
 from upstash_redis.exception import UpstashException
 from upstash_redis.http.decode import decode
 from upstash_redis.schema.http import RESTResult, RESTResponse, RESTEncoding
 from upstash_redis.schema.telemetry import TelemetryData
 from asyncio import sleep
 from aiohttp import ClientSession
@@ -64,14 +65,20 @@
                     else:
                         headers["Upstash-Telemetry-Sdk"] = "upstash_redis@development"
 
                     if telemetry_data.get("platform"):
                         headers["Upstash-Telemetry-Platform"] = telemetry_data[
                             "platform"
                         ]
+                    elif os.getenv("VERCEL"):
+                        headers["Upstash-Telemetry-Sdk"] = "vercel"
+                    elif os.getenv("AWS_REGION"):
+                        headers["Upstash-Telemetry-Sdk"] = "aws"
+                    else:
+                        headers["Upstash-Telemetry-Sdk"] = "unknown"
 
             if encoding:
                 headers["Upstash-Encoding"] = encoding
 
             async with session.post(url, headers=headers, json=command) as response:
                 body: RESTResponse = await response.json()
 
@@ -128,20 +135,26 @@
                         headers[
                             "Upstash-Telemetry-Runtime"
                         ] = f"python@v{python_version()}"
 
                     if telemetry_data.get("sdk"):
                         headers["Upstash-Telemetry-Sdk"] = telemetry_data["sdk"]
                     else:
-                        headers["Upstash-Telemetry-Sdk"] = "upstash_redis@development"
+                        headers["Upstash-Telemetry-Sdk"] = "upstash_redis@python"
 
                     if telemetry_data.get("platform"):
                         headers["Upstash-Telemetry-Platform"] = telemetry_data[
                             "platform"
                         ]
+                    elif os.getenv("VERCEL"):
+                        headers["Upstash-Telemetry-Sdk"] = "vercel"
+                    elif os.getenv("AWS_REGION"):
+                        headers["Upstash-Telemetry-Sdk"] = "aws"
+                    else:
+                        headers["Upstash-Telemetry-Sdk"] = "unknown"
 
             if encoding:
                 headers["Upstash-Encoding"] = encoding
 
             response = session.post(url, headers=headers, json=command).json()
 
             # Avoid the [] syntax to prevent KeyError from being raised.
```

### Comparing `upstash_redis-0.14.0/upstash_redis/schema/http.py` & `upstash_redis-0.14.1/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/utils/exception.py` & `upstash_redis-0.14.1/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/upstash_redis/utils/format.py` & `upstash_redis-0.14.1/upstash_redis/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.0/PKG-INFO` & `upstash_redis-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.14.0
+Version: 0.14.1
 Summary: Serverless Redis Sdk from Upstash
 Author: Upstash
 Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


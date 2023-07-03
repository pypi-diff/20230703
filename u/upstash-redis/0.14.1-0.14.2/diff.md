# Comparing `tmp/upstash_redis-0.14.1.tar.gz` & `tmp/upstash_redis-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.14.1.tar", max compression
+gzip compressed data, was "upstash_redis-0.14.2.tar", max compression
```

## Comparing `upstash_redis-0.14.1.tar` & `upstash_redis-0.14.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-07-03 04:25:55.136423 upstash_redis-0.14.1/LICENSE
--rw-r--r--   0        0        0     9173 2023-07-03 04:25:55.136423 upstash_redis-0.14.1/README.md
--rw-r--r--   0        0        0      500 2023-07-03 04:25:55.136423 upstash_redis-0.14.1/pyproject.toml
--rw-r--r--   0        0        0      146 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4896 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     5116 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/client.py
--rw-r--r--   0        0        0       77 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       79 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    21043 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    72037 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    20142 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     6254 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      752 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      174 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     9521 2023-07-03 04:25:55.144423 upstash_redis-0.14.1/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-03 04:27:56.695275 upstash_redis-0.14.2/LICENSE
+-rw-r--r--   0        0        0     9173 2023-07-03 04:27:56.695275 upstash_redis-0.14.2/README.md
+-rw-r--r--   0        0        0      500 2023-07-03 04:27:56.695275 upstash_redis-0.14.2/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4896 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     5116 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/client.py
+-rw-r--r--   0        0        0       77 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    21043 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    72037 2023-07-03 04:27:56.699275 upstash_redis-0.14.2/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    20142 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     6249 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      752 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      174 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     9521 2023-07-03 04:27:56.703275 upstash_redis-0.14.2/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.14.2/PKG-INFO
```

### Comparing `upstash_redis-0.14.1/LICENSE` & `upstash_redis-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/README.md` & `upstash_redis-0.14.2/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/asyncio/client.py` & `upstash_redis-0.14.2/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/client.py` & `upstash_redis-0.14.2/upstash_redis/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.14.2/upstash_redis/commands/async_commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/commands/commands.py` & `upstash_redis-0.14.2/upstash_redis/commands/commands.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/commands/commands.pyi` & `upstash_redis-0.14.2/upstash_redis/commands/commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/http/decode.py` & `upstash_redis-0.14.2/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/http/execute.py` & `upstash_redis-0.14.2/upstash_redis/http/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
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
                     elif os.getenv("VERCEL"):
                         headers["Upstash-Telemetry-Sdk"] = "vercel"
```

### Comparing `upstash_redis-0.14.1/upstash_redis/schema/http.py` & `upstash_redis-0.14.2/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/utils/exception.py` & `upstash_redis-0.14.2/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/upstash_redis/utils/format.py` & `upstash_redis-0.14.2/upstash_redis/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.1/PKG-INFO` & `upstash_redis-0.14.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.14.1
+Version: 0.14.2
 Summary: Serverless Redis Sdk from Upstash
 Author: Upstash
 Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


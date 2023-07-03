# Comparing `tmp/flxtrd-0.2.0.tar.gz` & `tmp/flxtrd-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.2.0.tar", max compression
+gzip compressed data, was "flxtrd-0.2.0.dev0.tar", max compression
```

## Comparing `flxtrd-0.2.0.tar` & `flxtrd-0.2.0.dev0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.0/LICENSE
--rw-r--r--   0        0        0     8910 2023-07-03 13:23:29.251402 flxtrd-0.2.0/README.md
--rw-r--r--   0        0        0     2255 2023-07-03 13:40:15.551370 flxtrd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-03 13:20:23.759408 flxtrd-0.2.0/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      580 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4911 2023-07-03 12:57:54.183451 flxtrd-0.2.0/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     5261 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/types.py
--rw-r--r--   0        0        0     1552 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0    10093 2023-07-03 12:57:41.867452 flxtrd-0.2.0/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.0/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     9651 1970-01-01 00:00:00.000000 flxtrd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/LICENSE
+-rw-r--r--   0        0        0     8910 2023-07-03 13:23:29.251402 flxtrd-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     2259 2023-07-03 12:33:57.915497 flxtrd-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-03 13:20:23.759408 flxtrd-0.2.0.dev0/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      580 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4911 2023-07-03 12:57:54.183451 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     5261 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0     1552 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0    10093 2023-07-03 12:57:41.867452 flxtrd-0.2.0.dev0/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     9656 1970-01-01 00:00:00.000000 flxtrd-0.2.0.dev0/PKG-INFO
```

### Comparing `flxtrd-0.2.0/LICENSE` & `flxtrd-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/README.md` & `flxtrd-0.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/pyproject.toml` & `flxtrd-0.2.0.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.2.0"
+version = "0.2.0-dev"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
```

### Comparing `flxtrd-0.2.0/src/flxtrd/__init__.py` & `flxtrd-0.2.0.dev0/src/flxtrd/__init__.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/core/api_client.py` & `flxtrd-0.2.0.dev0/src/flxtrd/core/api_client.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/core/logger.py` & `flxtrd-0.2.0.dev0/src/flxtrd/core/logger.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/core/types.py` & `flxtrd-0.2.0.dev0/src/flxtrd/core/types.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/core/utils.py` & `flxtrd-0.2.0.dev0/src/flxtrd/core/utils.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/protocols/ampq.py` & `flxtrd-0.2.0.dev0/src/flxtrd/protocols/ampq.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/src/flxtrd/protocols/restapi.py` & `flxtrd-0.2.0.dev0/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0/PKG-INFO` & `flxtrd-0.2.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.2.0
+Version: 0.2.0.dev0
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/GLocalFlexTrade
 Author: glocalflex
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/flxtrd-0.2.0.dev0.tar.gz` & `tmp/flxtrd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.2.0.dev0.tar", max compression
+gzip compressed data, was "flxtrd-0.2.1.tar", max compression
```

## Comparing `flxtrd-0.2.0.dev0.tar` & `flxtrd-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/LICENSE
--rw-r--r--   0        0        0     8910 2023-07-03 13:23:29.251402 flxtrd-0.2.0.dev0/README.md
--rw-r--r--   0        0        0     2259 2023-07-03 12:33:57.915497 flxtrd-0.2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-03 13:20:23.759408 flxtrd-0.2.0.dev0/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      580 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4911 2023-07-03 12:57:54.183451 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     5261 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/types.py
--rw-r--r--   0        0        0     1552 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0    10093 2023-07-03 12:57:41.867452 flxtrd-0.2.0.dev0/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.0.dev0/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     9656 1970-01-01 00:00:00.000000 flxtrd-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8795 2023-07-03 13:55:44.727340 flxtrd-0.2.1/README.md
+-rw-r--r--   0        0        0     2255 2023-07-03 14:06:20.391319 flxtrd-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-03 13:51:39.979348 flxtrd-0.2.1/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      580 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.1/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     5261 2023-07-03 13:51:39.979348 flxtrd-0.2.1/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0     1552 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0    10095 2023-07-03 14:05:46.907321 flxtrd-0.2.1/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     9536 1970-01-01 00:00:00.000000 flxtrd-0.2.1/PKG-INFO
```

### Comparing `flxtrd-0.2.0.dev0/LICENSE` & `flxtrd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/README.md` & `flxtrd-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,43 @@
+Metadata-Version: 2.1
+Name: flxtrd
+Version: 0.2.1
+Summary: Public client API for the flexible energy trading market GLocalFlex.
+Home-page: https://github.com/glocalflex/GLocalFlexTrade
+Author: glocalflex
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pika (>=1.3.1,<2.0.0)
+Requires-Dist: requests (>=2.28.0)
+Project-URL: Documentation, https://glocalflex.github.io/GLocalFlexTrade/
+Project-URL: Repository, https://github.com/glocalflex/GLocalFlexTrade
+Description-Content-Type: text/markdown
+
 
 <!-- [![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
 [![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd) -->
 
 <!-- [![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd) -->
 
 
 
 
 # GLocalFlexTrade Public API
 
 Public client API for the flexible energy trading market GLocalFlex.
-Trade energy or offer flexible loads to the European energy market.
 The client libary provides standard interface to access the GLocalFlex Market public API.
-The client integrates Rest API and AMPQ protocol for communication with the GLocalFlex server.
+The client integrates Rest API and AMPQ protocol for communication with the GLocalFlex marketplace.
 
-[![Release](https://img.shields.io/github/v/release/glocalflex/GLocalFlexTrade)](https://img.shields.io/github/v/release/glocalflex/GLocalFlexTrade)
-[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/GLocalFlexTrade/main.yml?branch=main)](https://github.com/glocalflex/GLocalFlexTrade/actions/workflows/main.yml?query=branch%3Amain)
+![Release](https://img.shields.io/github/v/release/glocalflex/glocalflextrade?include_prereleases)
+[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/GLocalFlexTrade/ci.yml?branch=main)](https://github.com/glocalflex/GLocalFlexTrade/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/glocalflex/GLocalFlexTrade/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/GLocalFlexTrade)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/GLocalFlexTrade)](https://img.shields.io/github/commit-activity/m/glocalflex/GLocalFlexTrade)
 [![License](https://img.shields.io/github/license/glocalflex/GLocalFlexTrade)](https://img.shields.io/github/license/glocalflex/GLocalFlexTrade)
 
 
 The GLocalFlexTrade client API [Documentation](https://glocalflex.github.io/GLocalFlexTrade/) provides more information how to use the **flxtrd** Python package.
 
@@ -258,8 +275,8 @@
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         log(INFO, "Keyboard interrupt received. Closing connection to the market broker")
 
 
-```
+```
```

### Comparing `flxtrd-0.2.0.dev0/pyproject.toml` & `flxtrd-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.2.0-dev"
+version = "0.2.1"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
```

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/__init__.py` & `flxtrd-0.2.1/src/flxtrd/__init__.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/core/api_client.py` & `flxtrd-0.2.1/src/flxtrd/core/api_client.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/core/logger.py` & `flxtrd-0.2.1/src/flxtrd/core/logger.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.2.1/src/flxtrd/core/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.2.1/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/core/types.py` & `flxtrd-0.2.1/src/flxtrd/core/types.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/core/utils.py` & `flxtrd-0.2.1/src/flxtrd/core/utils.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/protocols/ampq.py` & `flxtrd-0.2.1/src/flxtrd/protocols/ampq.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             self.connection = pika.BlockingConnection(parameters)
             self.channel = self.connection.channel()
             self.callback_queue_id = declareReplyToQueue(
                 self.channel, applicationKey, tickeroutexname
             )
         except Exception as excep:
             err = FlexError(str(excep))
-            raise err
+            raise excep
         return err
 
     def set_consumer(self, callback, callback_queue, channel):
         channel.basic_consume(queue=callback_queue, on_message_callback=callback, auto_ack=True)
 
     def checkreplies(self):
         if self.connection is None:
```

### Comparing `flxtrd-0.2.0.dev0/src/flxtrd/protocols/restapi.py` & `flxtrd-0.2.1/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.0.dev0/PKG-INFO` & `flxtrd-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,25 @@
-Metadata-Version: 2.1
-Name: flxtrd
-Version: 0.2.0.dev0
-Summary: Public client API for the flexible energy trading market GLocalFlex.
-Home-page: https://github.com/glocalflex/GLocalFlexTrade
-Author: glocalflex
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pika (>=1.3.1,<2.0.0)
-Requires-Dist: requests (>=2.28.0)
-Project-URL: Documentation, https://glocalflex.github.io/GLocalFlexTrade/
-Project-URL: Repository, https://github.com/glocalflex/GLocalFlexTrade
-Description-Content-Type: text/markdown
-
 
 <!-- [![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
 [![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd) -->
 
 <!-- [![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd) -->
 
 
 
 
 # GLocalFlexTrade Public API
 
 Public client API for the flexible energy trading market GLocalFlex.
-Trade energy or offer flexible loads to the European energy market.
 The client libary provides standard interface to access the GLocalFlex Market public API.
-The client integrates Rest API and AMPQ protocol for communication with the GLocalFlex server.
+The client integrates Rest API and AMPQ protocol for communication with the GLocalFlex marketplace.
 
-[![Release](https://img.shields.io/github/v/release/glocalflex/GLocalFlexTrade)](https://img.shields.io/github/v/release/glocalflex/GLocalFlexTrade)
-[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/GLocalFlexTrade/main.yml?branch=main)](https://github.com/glocalflex/GLocalFlexTrade/actions/workflows/main.yml?query=branch%3Amain)
+![Release](https://img.shields.io/github/v/release/glocalflex/glocalflextrade?include_prereleases)
+[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/GLocalFlexTrade/ci.yml?branch=main)](https://github.com/glocalflex/GLocalFlexTrade/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/glocalflex/GLocalFlexTrade/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/GLocalFlexTrade)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/GLocalFlexTrade)](https://img.shields.io/github/commit-activity/m/glocalflex/GLocalFlexTrade)
 [![License](https://img.shields.io/github/license/glocalflex/GLocalFlexTrade)](https://img.shields.io/github/license/glocalflex/GLocalFlexTrade)
 
 
 The GLocalFlexTrade client API [Documentation](https://glocalflex.github.io/GLocalFlexTrade/) provides more information how to use the **flxtrd** Python package.
 
@@ -276,8 +257,8 @@
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         log(INFO, "Keyboard interrupt received. Closing connection to the market broker")
 
 
-```
+```
```


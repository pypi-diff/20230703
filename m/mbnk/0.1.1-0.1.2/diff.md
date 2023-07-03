# Comparing `tmp/mbnk-0.1.1.tar.gz` & `tmp/mbnk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.1.1.tar", max compression
+gzip compressed data, was "mbnk-0.1.2.tar", max compression
```

## Comparing `mbnk-0.1.1.tar` & `mbnk-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.1.1/README.md
--rw-r--r--   0        0        0      308 2023-07-02 23:36:59.720764 mbnk-0.1.1/mbnk/__init__.py
--rw-r--r--   0        0        0    17634 2023-07-02 23:18:41.104797 mbnk-0.1.1/mbnk/api.py
--rw-r--r--   0        0        0      127 2023-07-02 23:03:02.426763 mbnk-0.1.1/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0      423 2023-07-02 23:04:25.131158 mbnk-0.1.1/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     1347 2023-07-02 22:17:52.460089 mbnk-0.1.1/mbnk/enums.py
--rw-r--r--   0        0        0      300 2023-07-02 23:06:33.479647 mbnk-0.1.1/mbnk/exceptions.py
--rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.1/mbnk/instances.py
--rw-r--r--   0        0        0      315 2023-07-02 18:14:01.695715 mbnk-0.1.1/mbnk/mbnk.py
--rw-r--r--   0        0        0     2217 2023-07-01 23:15:46.030057 mbnk-0.1.1/mbnk/responses.py
--rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.1.1/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.1.1/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      313 2023-07-02 22:33:00.127952 mbnk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 mbnk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.1.2/README.md
+-rw-r--r--   0        0        0      275 2023-07-03 02:00:50.620267 mbnk-0.1.2/mbnk/__init__.py
+-rw-r--r--   0        0        0    17863 2023-07-03 00:30:56.330813 mbnk-0.1.2/mbnk/api.py
+-rw-r--r--   0        0        0      127 2023-07-02 23:03:02.426763 mbnk-0.1.2/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0      496 2023-07-03 01:58:35.864712 mbnk-0.1.2/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     1347 2023-07-02 22:17:52.460089 mbnk-0.1.2/mbnk/enums.py
+-rw-r--r--   0        0        0      576 2023-07-03 00:10:27.269164 mbnk-0.1.2/mbnk/exceptions.py
+-rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.2/mbnk/instances.py
+-rw-r--r--   0        0        0      385 2023-07-03 01:59:23.280557 mbnk-0.1.2/mbnk/mbnk.py
+-rw-r--r--   0        0        0     2262 2023-07-03 01:57:36.488901 mbnk-0.1.2/mbnk/responses.py
+-rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.1.2/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.1.2/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      313 2023-07-03 02:01:29.632134 mbnk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 mbnk-0.1.2/PKG-INFO
```

### Comparing `mbnk-0.1.1/README.md` & `mbnk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.1/mbnk/api.py` & `mbnk-0.1.2/mbnk/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,15 @@
     ClientSession,
     ClientResponse
 )
 from typing import Union, Optional
 
 from mbnk.enums import APIPaths
 
-from mbnk.exceptions import (
-    MonobankAPIException,
-    MonoPayAPIException
-)
+from mbnk.exceptions import *
 
 from mbnk.instances import *
 
 from mbnk.responses import *
 
 
 class APIMethod:
@@ -75,23 +72,45 @@
             data[key] = value
 
         return data
 
     @staticmethod
     def __is_exception(response: Union[Response, ClientResponse]) -> bool:
         if isinstance(response, Response):
-            if response.status_code != 200:
-                return True
+            status_code = response.status_code
+        elif isinstance(response, ClientResponse):
+            status_code = response.status
+        else:
+            return True
 
-        if isinstance(response, ClientResponse):
-            if response.status != 200:
-                return True
+        if status_code != 200:
+            return True
 
         return False
 
+    @staticmethod
+    def __get_exception(response: Union[Response, ClientResponse]):
+        if isinstance(response, Response):
+            status_code = response.status_code
+        elif isinstance(response, ClientResponse):
+            status_code = response.status
+        else:
+            return
+
+        if status_code == 400:
+            raise Exception
+        elif status_code == 403:
+            raise Exception
+        elif status_code == 404:
+            raise Exception
+        elif status_code == 429:
+            raise TooManyRequestsException
+        else:
+            return MonoPayAPIException
+
     def __sync_request(
             self,
             method: str,
             path: str,
             data: str = None,
             params: str = None
     ):
@@ -102,15 +121,15 @@
             params=params,
             data=json.dumps(data) if data is not None else None
         )
         response_data = response.json()
         response_data = self.__load_response(response_data)
 
         if self.__is_exception(response):
-            return MonoPayAPIException(**response_data)
+            raise self.__get_exception(response)
 
         return response_data
 
     async def __async_request(
             self,
             method: str,
             path: str,
@@ -155,17 +174,14 @@
                         return response
 
                     return func(self, *args, **kwargs, response_data=response)
 
                 def sync_wrapper():
                     response = self.__sync_request(**func_args)
 
-                    if isinstance(response, MonoPayAPIException) or isinstance(response, MonobankAPIException):
-                        return response
-
                     return func(self, *args, **kwargs, response_data=response)
 
                 if self.__is_async:
                     return async_wrapper()
                 else:
                     return sync_wrapper()
 
@@ -242,25 +258,17 @@
 
     __base_url__ = None
     __headers__ = {}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.auth: Authorization = Authorization(
-            base_url=self.__base_url__,
-            headers=self.__headers__,
-            _async=self.__is_async__
-        )
+        self.auth: Authorization = Authorization(*args, **kwargs)
 
-        self.client: Client = Client(
-            base_url=self.__base_url__,
-            headers=self.__headers__,
-            _async=self.__is_async__
-        )
+        self.client: Client = Client(*args, **kwargs)
 
     def set_webhook(self):
         pass
 
     def info(self):
         pass
```

### Comparing `mbnk-0.1.1/mbnk/enums.py` & `mbnk-0.1.2/mbnk/enums.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.1/mbnk/instances.py` & `mbnk-0.1.2/mbnk/instances.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.1/mbnk/responses.py` & `mbnk-0.1.2/mbnk/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 __all__ = [
     'EmptyResponse',
 
-    # Monobank API Responses
+    # Monobank Open API Responses
     'CurrencyRatesResponse',
     'ClientInfoResponse',
     'StatementResponse',
 
+    # Monobank Corp Open API Responses
+
     # MonoPay API Responses
     'InvoiceCreatedResponse',
     'InvoiceCanceledResponse',
     'InvoiceStatusResponse',
     'InvoiceInfoResponse',
     'SplitInvoiceResponse',
     'FinalizeInvoiceResponse',
```

### Comparing `mbnk-0.1.1/PKG-INFO` & `mbnk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


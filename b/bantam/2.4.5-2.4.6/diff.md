# Comparing `tmp/bantam-2.4.5.tar.gz` & `tmp/bantam-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.5.tar", last modified: Sat Jun 24 15:08:52 2023, max compression
+gzip compressed data, was "bantam-2.4.6.tar", last modified: Sun Jul  2 22:37:30 2023, max compression
```

## Comparing `bantam-2.4.5.tar` & `bantam-2.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-24 15:08:52.821550 bantam-2.4.5/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.5/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.5/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-24 15:08:52.821550 bantam-2.4.5/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-24 15:07:51.000000 bantam-2.4.5/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.5/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.5/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.5/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.5/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22978 2023-06-21 04:48:21.000000 bantam-2.4.5/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.5/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.5/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50579 2023-06-24 15:02:24.000000 bantam-2.4.5/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.5/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.5/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     5623 2023-06-21 04:28:06.000000 bantam-2.4.5/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.5/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.5/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.5/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.5/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.5/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.5/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.5/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-02 22:37:30.917922 bantam-2.4.6/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.6/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.6/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-07-02 22:37:30.917922 bantam-2.4.6/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-07-02 22:36:45.000000 bantam-2.4.6/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.913922 bantam-2.4.6/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.6/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.6/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.6/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.6/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22974 2023-07-02 22:27:44.000000 bantam-2.4.6/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.6/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4954 2023-07-02 22:34:38.000000 bantam-2.4.6/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50579 2023-06-24 15:02:24.000000 bantam-2.4.6/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.6/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.6/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5624 2023-07-02 22:27:45.000000 bantam-2.4.6/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.6/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.6/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.6/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.6/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.6/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.6/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.6/test/test_js_async.py
```

### Comparing `bantam-2.4.5/PKG-INFO` & `bantam-2.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.5
+Version: 2.4.6
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.5
+Download-URL: https://github.com/bantam/dist/2.4.6
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.5/setup.py` & `bantam-2.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.5"
+VERSION = "2.4.6"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.5/src/bantam/__init__.py` & `bantam-2.4.6/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam/api.py` & `bantam-2.4.6/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam/autogen/main.py` & `bantam-2.4.6/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam/client.py` & `bantam-2.4.6/src/bantam/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 method above.  The *end_point* parameter specifies the base url to the server that serves up MyServceApi class.
 
 """
 import inspect
 import json
 from abc import ABC
 from functools import wraps
-from typing import Any, Dict, TypeVar, Optional, Type, AsyncIterator, Generic, Mapping, Iterator
+from typing import Any, Dict, TypeVar, Optional, Type,  Iterator, Generic, Mapping, Iterator
 
 import aiohttp
 
 from bantam import conversions
 from bantam.api import API, RestMethod
 
 __all__ = ["WebInterface"]
```

### Comparing `bantam-2.4.5/src/bantam/conversions.py` & `bantam-2.4.6/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam/decorators.py` & `bantam-2.4.6/src/bantam/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 import inspect
-import sys
-from typing import Any, Callable, Awaitable, Union, Optional, Dict
+from typing import Any, Callable, Awaitable, Union, Optional, Dict, AsyncIterator
 
 from aiohttp.web import Request, Response
 from aiohttp.web_response import StreamResponse
 from aiohttp import ClientTimeout
 
 from bantam.api import RestMethod
 
-WebApi = Callable[..., Awaitable[Any]]
+WebApi = Callable[..., Union[Awaitable[Any], AsyncIterator[Any]]]
 
 
 PreProcessor = Callable[[Request], Union[None, Dict[str, Any]]]
 PostProcessor = Callable[[Union[Response, StreamResponse]], Union[Response, StreamResponse]]
 
 
 def web_api(content_type: str, method: RestMethod = RestMethod.GET,
             is_constructor: bool = False,
             expire_obj: bool = False,
-            on_disconnect: Optional[Callable[[], None]] = None,
+            on_disconnect: Optional[Callable[[], Union[None, Awaitable[None]]]] = None,
             timeout: Optional[ClientTimeout] = None,
             uuid_param: Optional[str] = None,
             preprocess: Optional[PreProcessor] = None,
             postprocess: Optional[PostProcessor] = None) -> Callable[[WebApi], WebApi]:
     """
     Decorator for class async method to register it as an API with the `WebApplication` class
     Decorated functions should be static class methods with parameters that are convertible from a string
     (things like float, int, str, bool).  Type hints must be provided and will be used to dynamically convert
     query parameeter strings to the right type.
 
     >>> class MyResource:
     ...
+    ...   @classmethod
     ...   @web_api(content_type="text/html")
-    ...   @staticmethod
-    ...   def say_hello(name: str):
+    ...   def say_hello(cls, name: str):
     ...      return f"Hi there, {name}!"
 
     Only GET calls with explicit parameters in the URL are support for now.  The above registers a route
     of the form:
 
     http://<host>:port>/MyRestAPI?name=Jill
 
 
     :param content_type: content type to disply (e.g., "text/html")
     :param method: one of MethodEnum rest api methods (GET or POST)
     :param is_constructor: set to True if API is static method return a class instnace, False oherwise (default)
     :param expire_obj: for instance methods only, epxire the object upon successful completion of that call
     :param on_disconnect: callback if client disconnects unexpectedly
     :param timeout: optional timeout value for response to request to timeout
+    :param uuid_param: optional name of parameter to use as unique id for 'self'
+    :param preprocess: optional preprocess function to invoke on request
+    :param postprocess: optional postprocess function to run after servicing request
     :return: callable decorator
     """
     from .http import WebApplication
     if not isinstance(content_type, str):
         raise Exception("@web_api must provide one str argument which is the content type")
 
-    def wrapper(func: Union[WebApi, staticmethod, classmethod]) -> Union[WebApi, staticmethod, classmethod]:
+    def wrapper(func: Union[WebApi]) -> Union[WebApi]:
         if not inspect.ismethod(func):
             args = inspect.signature(func)
             first_arg = list(args.parameters.keys())[0] if args else None
             is_static = first_arg not in {'self', 'cls'}
             is_class_method = first_arg == 'cls'
         else:
             is_static = isinstance(func, staticmethod)
             is_class_method = isinstance(func, classmethod)
         if not (is_static or is_class_method or is_class_method) and is_constructor:
             raise TypeError("@web_api's that are declared constructors must be static or class methods")
         if (is_static or is_class_method) and expire_obj:
             raise TypeError("@web_api's expire_obj param can only be set True for instance methods")
         if not is_static and not is_class_method and not inspect.ismethod(func) and not inspect.isfunction(func):
-            raise TypeError("@web_api should only be applied to @classmethod's, @staticmethods or instance methods")
+            raise TypeError("@web_api should only be applied to @classmethod's or instance methods")
         if func.__name__.startswith('_'):
             raise TypeError("names of web_api methods must not start with underscore")
 
         def get_class_that_defined_method():
             return func.__qualname__.split('.')[0]
 
+        # noinspection PyUnresolvedReferences
         return WebApplication._func_wrapper((func.__module__, get_class_that_defined_method())
-                                                if is_class_method else None,
+                                            if is_class_method else None,
                                             func,
                                             timeout=timeout,
                                             is_instance_method=not is_static and not is_class_method,
                                             is_class_method=is_class_method,
                                             method=method,
                                             content_type=content_type,
                                             is_constructor=is_constructor,
```

### Comparing `bantam-2.4.5/src/bantam/http.py` & `bantam-2.4.6/src/bantam/http.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam/js.py` & `bantam-2.4.6/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam/js_async.py` & `bantam-2.4.6/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.6/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.5
+Version: 2.4.6
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.5
+Download-URL: https://github.com/bantam/dist/2.4.6
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.5/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.6/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/test/test_client_get.py` & `bantam-2.4.6/test/test_client_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             count += 1
         assert count == 200
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
+
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed_str(tmpdir):
     from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
```

### Comparing `bantam-2.4.5/test/test_client_post.py` & `bantam-2.4.6/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/test/test_client_post_inherited_apis.py` & `bantam-2.4.6/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/test/test_conversions.py` & `bantam-2.4.6/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/test/test_decorators.py` & `bantam-2.4.6/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/test/test_js.py` & `bantam-2.4.6/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.5/test/test_js_async.py` & `bantam-2.4.6/test/test_js_async.py`

 * *Files identical despite different names*


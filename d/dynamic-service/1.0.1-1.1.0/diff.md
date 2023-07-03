# Comparing `tmp/dynamic-service-1.0.1.tar.gz` & `tmp/dynamic-service-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.0.1.tar", last modified: Sat Jul  1 09:44:20 2023, max compression
+gzip compressed data, was "dynamic-service-1.1.0.tar", last modified: Mon Jul  3 06:52:48 2023, max compression
```

## Comparing `dynamic-service-1.0.1.tar` & `dynamic-service-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.046517 dynamic-service-1.0.1/
--rw-rw-rw-   0        0        0      236 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2037 2023-07-01 09:44:20.046517 dynamic-service-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2023-07-01 08:56:11.000000 dynamic-service-1.0.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 dynamic-service-1.0.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.025441 dynamic-service-1.0.1/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 08:46:12.000000 dynamic-service-1.0.1/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.041542 dynamic-service-1.0.1/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 dynamic-service-1.0.1/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9764 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 dynamic-service-1.0.1/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.043516 dynamic-service-1.0.1/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    19706 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3012 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.014444 dynamic-service-1.0.1/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.014444 dynamic-service-1.0.1/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.045542 dynamic-service-1.0.1/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 dynamic-service-1.0.1/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 dynamic-service-1.0.1/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.037546 dynamic-service-1.0.1/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2037 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-01 09:44:20.000000 dynamic-service-1.0.1/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-01 09:44:20.000000 dynamic-service-1.0.1/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-01 09:44:20.000000 dynamic-service-1.0.1/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       78 2023-06-15 21:47:31.000000 dynamic-service-1.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       69 2023-06-15 21:46:16.000000 dynamic-service-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 09:44:20.046517 dynamic-service-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-01 09:44:13.000000 dynamic-service-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.043653 dynamic-service-1.1.0/
+-rw-rw-rw-   0        0        0      236 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-03 06:52:48.042658 dynamic-service-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.014654 dynamic-service-1.1.0/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.034654 dynamic-service-1.1.0/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2596 2023-07-03 06:52:21.000000 dynamic-service-1.1.0/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9282 2023-07-03 06:51:39.000000 dynamic-service-1.1.0/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.1.0/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.1.0/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.036656 dynamic-service-1.1.0/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    19706 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3012 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.009177 dynamic-service-1.1.0/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.009177 dynamic-service-1.1.0/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.041658 dynamic-service-1.1.0/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-03 06:52:48.030654 dynamic-service-1.1.0/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-03 06:52:47.000000 dynamic-service-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       78 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       69 2023-07-01 09:47:05.000000 dynamic-service-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:52:48.043653 dynamic-service-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-03 06:52:39.000000 dynamic-service-1.1.0/setup.py
```

### Comparing `dynamic-service-1.0.1/PKG-INFO` & `dynamic-service-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.0.1
+Version: 1.1.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# live-api
+# dynamic-service
 
 > A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 first of all
 ------------
 
 #### specifics:
@@ -56,8 +55,7 @@
 -----------
 
 #### run from windows command line (inside the project directory)
 - run with python by writing to the command line in the project directory:
 ````
 python test.py
 ````
-
```

### Comparing `dynamic-service-1.0.1/README.md` & `dynamic-service-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# live-api
+# dynamic-service
 
 > A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 first of all
 ------------
 
 #### specifics:
```

### Comparing `dynamic-service-1.0.1/build.py` & `dynamic-service-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/dynamic_service/base.py` & `dynamic-service-1.1.0/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/dynamic_service/endpoints/data.py` & `dynamic-service-1.1.0/dynamic_service/endpoints/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# backend.py
+# data.py
 
 from fastapi.responses import (
     RedirectResponse, Response, FileResponse,
     JSONResponse, HTMLResponse, StreamingResponse,
     PlainTextResponse, UJSONResponse, ORJSONResponse
 )
```

### Comparing `dynamic-service-1.0.1/dynamic_service/endpoints/engine.py` & `dynamic-service-1.1.0/dynamic_service/endpoints/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # engine.py
 
-import datetime as dt
+from dataclasses import dataclass, field
 from functools import wraps
 from typing import (
     List, Any, Union, Dict, Optional,
     Tuple, Callable, Iterable, TypeVar, Generic
 )
 
 from fastapi.openapi.docs import get_swagger_ui_html, HTMLResponse
@@ -16,35 +16,21 @@
 __all__ = [
     "BaseEndpoint",
     "DocsEndpoint",
     "Record",
     "valid_endpoints"
 ]
 
+@dataclass(repr=False, slots=True)
 class Record(BaseModel):
     """A class to represent a result object for commands and conditions calls."""
 
-    def __init__(
-            self, *,
-            args: Optional[Tuple] = None,
-            kwargs: Optional[Dict[str, Any]] = None,
-            returns: Optional[Any] = None
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param args: The positional arguments.
-        :param kwargs: The keyword arguments.
-        :param returns: The returned values.
-        """
-
-        self.args = args or ()
-        self.kwargs = kwargs or {}
-        self.returns = returns
-    # end __init__
+    args: Optional[Tuple] = field(default_factory=tuple),
+    kwargs: Optional[Dict[str, Any]] = field(default_factory=dict),
+    returns: Optional[Any] = None
 
     def collect(
             self, *,
             args: Optional[Tuple] = None,
             kwargs: Optional[Dict[str, Any]] = None,
             returns: Optional[Any] = None
     ) -> None:
@@ -58,16 +44,14 @@
 
         self.args = args
         self.kwargs.update(kwargs)
         self.returns = returns
     # end collect
 # end Record
 
-Requests = List[Record]
-
 _ServiceType = TypeVar("_ServiceType")
 _ReturnType = TypeVar("_ReturnType")
 _ProcessedReturnType = TypeVar("_ProcessedReturnType")
 
 class BaseEndpoint(BaseModel, Generic[_ServiceType, _ReturnType, _ProcessedReturnType]):
     """
     A class to represent an endpoint.
@@ -135,15 +119,15 @@
         :param methods: The endpoint methods.
         :param description: The description of the object.
         :param root: The root to the path.
         :param options: Any keyword arguments.
         :param service: The service object.
         """
 
-        self.record: Requests = []
+        self.record: List[Record] = []
 
         self.options = options or {}
 
         self.path = str(path or self.PATH)
         self.root = root or ""
         self.description = description
 
@@ -158,21 +142,15 @@
 
         :param name: The intent that activated the command.
         :param message: The message for the intent.
 
         :return: The function to command the command.
         """
 
-        start = dt.datetime.now()
-
-        result = self.process(self.wrap(self.endpoint)(*args, **kwargs))
-
-        end = dt.datetime.now()
-
-        return dict(response=result, time=(end - start).total_seconds())
+        return self.process(self.wrap(self.endpoint)(*args, **kwargs))
     # end __call__
 
     @staticmethod
     def call(instance) -> Callable[..., Dict[str, Union[int, _ProcessedReturnType]]]:
         """
         Returns the function to command the command.
```

### Comparing `dynamic-service-1.0.1/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.1.0/dynamic_service/endpoints/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# backend.py
+# exceptions.py
 
 from typing import Any, Optional
 
 import dill
 
 __all__ = [
     "UnSerializableObjectError",
```

### Comparing `dynamic-service-1.0.1/dynamic_service/endpoints/process.py` & `dynamic-service-1.1.0/dynamic_service/endpoints/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# backend.py
+# process.py
 
 from typing import Any
 
 import dill
 import codecs
 
 from dynamic_service.endpoints.exceptions import (
```

### Comparing `dynamic-service-1.0.1/dynamic_service/service/rest.py` & `dynamic-service-1.1.0/dynamic_service/service/rest.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/dynamic_service/service/sockets.py` & `dynamic-service-1.1.0/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.1.0/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.1.0/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.1.0/dynamic_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.0.1
+Version: 1.1.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# live-api
+# dynamic-service
 
 > A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 first of all
 ------------
 
 #### specifics:
@@ -56,8 +55,7 @@
 -----------
 
 #### run from windows command line (inside the project directory)
 - run with python by writing to the command line in the project directory:
 ````
 python test.py
 ````
-
```

### Comparing `dynamic-service-1.0.1/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.1.0/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.1/pyproject.toml` & `dynamic-service-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.0.1'
+version = '1.1.0'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.0.1/setup.py` & `dynamic-service-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.0.1',
+        version='1.1.0',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


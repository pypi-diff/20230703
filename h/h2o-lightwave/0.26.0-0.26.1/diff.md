# Comparing `tmp/h2o_lightwave-0.26.0-py3-none-any.whl.zip` & `tmp/h2o_lightwave-0.26.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 121156 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1132 b- defN 23-Jun-26 13:41 h2o_lightwave/__init__.py
--rw-r--r--  2.0 unx    14374 b- defN 23-Jun-26 13:41 h2o_lightwave/core.py
--rw-r--r--  2.0 unx    25866 b- defN 23-Jun-26 13:41 h2o_lightwave/graphics.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 13:41 h2o_lightwave/py.typed
--rw-r--r--  2.0 unx     7889 b- defN 23-Jun-26 13:41 h2o_lightwave/routing.py
--rw-r--r--  2.0 unx     3850 b- defN 23-Jun-26 13:41 h2o_lightwave/server.py
--rw-r--r--  2.0 unx   635842 b- defN 23-Jun-26 13:41 h2o_lightwave/types.py
--rw-r--r--  2.0 unx   166206 b- defN 23-Jun-26 13:41 h2o_lightwave/ui.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Jun-26 13:41 h2o_lightwave/ui_ext.py
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-26 13:41 h2o_lightwave/version.py
--rw-r--r--  2.0 unx       53 b- defN 23-Jun-26 13:48 h2o_lightwave-0.26.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6187 b- defN 23-Jun-26 13:48 h2o_lightwave-0.26.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 13:48 h2o_lightwave-0.26.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-26 13:48 h2o_lightwave-0.26.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1218 b- defN 23-Jun-26 13:48 h2o_lightwave-0.26.0.dist-info/RECORD
-15 files, 865071 bytes uncompressed, 119150 bytes compressed:  86.2%
+Zip file size: 121155 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jul-03 09:53 h2o_lightwave/__init__.py
+-rw-r--r--  2.0 unx    14374 b- defN 23-Jul-03 09:53 h2o_lightwave/core.py
+-rw-r--r--  2.0 unx    25866 b- defN 23-Jul-03 09:53 h2o_lightwave/graphics.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 09:53 h2o_lightwave/py.typed
+-rw-r--r--  2.0 unx     7889 b- defN 23-Jul-03 09:53 h2o_lightwave/routing.py
+-rw-r--r--  2.0 unx     3850 b- defN 23-Jul-03 09:53 h2o_lightwave/server.py
+-rw-r--r--  2.0 unx   635848 b- defN 23-Jul-03 09:53 h2o_lightwave/types.py
+-rw-r--r--  2.0 unx   166206 b- defN 23-Jul-03 09:53 h2o_lightwave/ui.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Jul-03 09:53 h2o_lightwave/ui_ext.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-03 09:53 h2o_lightwave/version.py
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6185 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1218 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/RECORD
+15 files, 865075 bytes uncompressed, 119149 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: h2o_lightwave/ui_ext.py
 Comment: 
 
 Filename: h2o_lightwave/version.py
 Comment: 
 
-Filename: h2o_lightwave-0.26.0.dist-info/LICENSE
+Filename: h2o_lightwave-0.26.1.dist-info/LICENSE
 Comment: 
 
-Filename: h2o_lightwave-0.26.0.dist-info/METADATA
+Filename: h2o_lightwave-0.26.1.dist-info/METADATA
 Comment: 
 
-Filename: h2o_lightwave-0.26.0.dist-info/WHEEL
+Filename: h2o_lightwave-0.26.1.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_lightwave-0.26.0.dist-info/top_level.txt
+Filename: h2o_lightwave-0.26.1.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_lightwave-0.26.0.dist-info/RECORD
+Filename: h2o_lightwave-0.26.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_lightwave/server.py

```diff
@@ -86,15 +86,15 @@
             await self._handle(q)
         except Exception:
             logger.exception('Unhandled exception')
             try:
                 q.page.drop()
                 # TODO replace this with a custom-designed error display
                 q.page['__unhandled_error__'] = markdown_card(
-                    box='1 1 12 10',
+                    box='1 1 -1 -1',
                     title='Error',
                     content=f'```\n{traceback.format_exc()}\n```',
                 )
                 await q.page.save()
             except Exception:
                 logger.exception('Failed transmitting unhandled exception')
```

## h2o_lightwave/types.py

```diff
@@ -16,15 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Optional, Union, Dict, List
 from .core import Data
 
 Value = Union[str, float, int]
-PackedRecord = Union[dict, str]
+PackedRecord = Union[dict, str, Data]
 PackedRecords = Union[List[dict], str]
 PackedData = Union[Data, str]
 
 
 def _dump(**kwargs): return {k: v for k, v in kwargs.items() if v is not None}
```

## h2o_lightwave/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.26.0'
+__version__ = '0.26.1'
```

## Comparing `h2o_lightwave-0.26.0.dist-info/METADATA` & `h2o_lightwave-0.26.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-lightwave
-Version: 0.26.0
+Version: 0.26.1
 Summary: H2O Wave Python driver for integration with arbitrary python web frameworks.
 Home-page: https://h2o.ai/products/h2o-wave
 Author: Martin Turoci
 Author-email: martin.turoci@h2o.ai
 License: UNKNOWN
 Project-URL: Documentation, https://wave.h2o.ai/
 Project-URL: Source, https://github.com/h2oai/wave
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: web
-Requires-Dist: h2o-lightwave-web (==0.26.0) ; extra == 'web'
+Requires-Dist: h2o-lightwave-web (==0.26.1) ; extra == 'web'
 
 # H2O Lightwave
 
 H2O Lightwave is a lightweight, pure-Python version of [H2O Wave](https://wave.h2o.ai/) that can be embedded in popular async web frameworks like FastAPI, Starlette, etc.
 
 In other words, H2O Lightwave works without the Wave server.
 
@@ -94,15 +94,15 @@
         await ws.close()
     except WebSocketDisconnect:
         print('Client disconnected')
 
 app.mount("/", StaticFiles(directory=web_directory, html=True), name="/")
 ```
 
-We also recommend reading the [blog post](https://medium.com/@unusualcode/h2o-lightwave-building-web-uis-with-fastapi-and-python-88a915383490) and other [integration examples](https://github.com/h2oai/wave/tree/master/py/h2o_lightwave/examples).
+We also recommend reading the [blog post](https://medium.com/@unusualcode/h2o-lightwave-building-web-uis-with-fastapi-and-python-88a915383490) and other [integration examples](https://github.com/h2oai/wave/tree/main/py/h2o_lightwave/examples).
 
 ## Installation
 
 ```bash
 pip install "h2o-lightwave[web]"
 ```
```


# Comparing `tmp/sixth-python-0.0.9.tar.gz` & `tmp/sixth-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.0.9.tar", last modified: Fri Jun 23 22:30:16 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.1.1.tar", last modified: Mon Jul  3 03:08:14 2023, max compression
```

## Comparing `sixth-python-0.0.9.tar` & `sixth-python-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 22:30:16.000000 sixth-python-0.0.9/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.0.9/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-23 22:30:16.000000 sixth-python-0.0.9/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3773 2023-06-23 22:30:02.000000 sixth-python-0.0.9/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.0.9/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.9/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-06-19 19:50:08.000000 sixth-python-0.0.9/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.9/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-06-19 19:50:08.000000 sixth-python-0.0.9/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     5026 2023-06-22 10:58:05.000000 sixth-python-0.0.9/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.9/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.9/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.9/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4160 2023-06-23 02:36:25.000000 sixth-python-0.0.9/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.9/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.9/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.9/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/
+-rw-r--r--   0 mac        (501) staff       (20)     3114 2023-07-03 03:08:14.000000 sixth-python-0.1.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.1/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-03 03:08:14.000000 sixth-python-0.1.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3773 2023-07-03 03:07:48.000000 sixth-python-0.1.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.1/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.1/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-03 02:16:20.000000 sixth-python-0.1.1/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.1/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-03 02:16:20.000000 sixth-python-0.1.1/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     5573 2023-07-03 02:53:36.000000 sixth-python-0.1.1/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.1/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.1.1/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      916 2023-07-03 00:19:36.000000 sixth-python-0.1.1/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4190 2023-07-03 02:16:20.000000 sixth-python-0.1.1/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.1/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.1/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.1/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3114 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-03 03:08:14.000000 sixth-python-0.1.1/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.0.9/PKG-INFO` & `sixth-python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.9
+Version: 0.1.1
 Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.0.9/README.md` & `sixth-python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/setup.py` & `sixth-python-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.9'
+VERSION = '0.1.1'
 DESCRIPTION = 'Six offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
```

### Comparing `sixth-python-0.0.9/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.1.1/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.1.1/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.1.1/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.1.1/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from starlette.types import ASGIApp
 from starlette.datastructures import Headers, MutableHeaders
 from starlette.responses import PlainTextResponse, Response
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 from fastapi import FastAPI,Depends,Response,HTTPException, Request
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.middleware import Middleware
+from starlette.datastructures import MutableHeaders
 import time
 import json
 from sixth import schemas
 import re
 import requests
 from dotenv import load_dotenv
 import os
@@ -69,42 +70,57 @@
         out=ast.literal_eval(string)
         return out
         
     async def dispatch(self,request: Request,call_next) -> None:
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
+        headers = request.headers
         #fail safe if there is an internal server error our servers are currenly in maintnance
         try:
             rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
             body = await request.body()
+            
             await self.set_body(request, body)
             body = await self._parse_bools(body)
+           
             if rate_limit_resp.status_code == 200:
                 try:
                     rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
                     self._config.rate_limiter[route] = rate_limit
-                    preferred_id = host if self._config.rate_limiter[route].unique_id == "" or self._config.rate_limiter[route].unique_id == "host" else body[self._config.rate_limiter[route].unique_id]
-                    print("preferred id is ", preferred_id)
-                    _response = await call_next(request)
+                    preferred_id = self._config.rate_limiter[route].unique_id
+                   
+                    if preferred_id == "" or preferred_id=="host":
+                        preferred_id = host
+                        
+                    else:
+                        if rate_limit.rate_limit_type == "body":
+                            preferred_id = body[preferred_id]
+                        elif rate_limit.rate_limit_type == "header":
+                            preferred_id = headers[preferred_id]
+                        else:
+                            preferred_id = host
+                    
+
                     if self._is_rate_limit_reached(preferred_id, route): 
+                        _response = await call_next(request)
                         return _response
                     else:
                         temp_payload = rate_limit.error_payload.values()
                         final = {}
                         for c in temp_payload:
                             for keys in c:
                                 if keys != "uid":
                                     final[keys] = c[keys]
                         output= final
-                        _response.headers["content-length"]= str(len(str(output).encode()))
-                        return Response(json.dumps(output), status_code=401, headers=_response.headers)
-                except:
+                        headers = MutableHeaders(headers={"content-length": str(len(str(output).encode())), 'content-type': 'application/json'})
+                        return Response(json.dumps(output), status_code=401, headers=headers)
+                except Exception as e:
                     _response = await call_next(request)
                     return _response
             else:
                 #fail safe if there is an internal server error our servers are currenly in maintnance
                 _response = await call_next(request)
                 return _response
-        except:
+        except Exception as e:
             _response = await call_next(request)
             return _response
```

### Comparing `sixth-python-0.0.9/sixth/schemas.py` & `sixth-python-0.1.1/sixth/schemas.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     error_payload_id = str(uuid.uuid4())
     id: str
     route: str
     interval: int 
     rate_limit: int
     last_updated: float 
     created_at: float
+    rate_limit_type: str = "ip address" #ip address, header, body
     unique_id: str = "host"
     error_payload: Dict[str , dict] = {
         error_payload_id:{
             "message": "max_limit_request_reached", 
             "uid": error_payload_id
         }
     }
```

### Comparing `sixth-python-0.0.9/sixth/sdk.py` & `sixth-python-0.1.1/sixth/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     path = "/v"+str(route.app.version)+new_route.path
                     edited_route = re.sub(r'\W+', '~', path)
                     if config and edited_route in config.rate_limiter.keys():
                         #default config has been set earlier on so skip
                         _rl_configs[edited_route] = config.rate_limiter[edited_route]
                         continue
                     #set the default values
-                    _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host")
+                    _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host", rate_limit_type="ip address")
                     _rl_configs[edited_route] = _rl_config
             else:
                 edited_route = re.sub(r'\W+', '~', route.path)
                 if config and edited_route in config.rate_limiter.keys():
                         #default config has been set earlier on so skip
                         _rl_configs[edited_route] = config.rate_limiter[edited_route]
                         continue
```

### Comparing `sixth-python-0.0.9/sixth/utils/encryption_utils.py` & `sixth-python-0.1.1/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/sixth/utils/time_utils.py` & `sixth-python-0.1.1/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.1.1/sixth_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.9
+Version: 0.1.1
 Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.0.9/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.1.1/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.9/sixth_python.egg-info/requires.txt` & `sixth-python-0.1.1/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*


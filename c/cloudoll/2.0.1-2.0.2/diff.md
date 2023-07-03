# Comparing `tmp/cloudoll-2.0.1.tar.gz` & `tmp/cloudoll-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.0.1.tar", last modified: Fri Jun  9 07:31:10 2023, max compression
+gzip compressed data, was "cloudoll-2.0.2.tar", last modified: Mon Jul  3 04:39:51 2023, max compression
```

## Comparing `cloudoll-2.0.1.tar` & `cloudoll-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.144483 cloudoll-2.0.1/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.1/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     7019 2023-06-09 07:31:10.143629 cloudoll-2.0.1/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     6386 2023-06-09 06:38:19.000000 cloudoll-2.0.1/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.130463 cloudoll-2.0.1/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.134906 cloudoll-2.0.1/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.135388 cloudoll-2.0.1/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.1/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.136384 cloudoll-2.0.1/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.1/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.137607 cloudoll-2.0.1/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    27881 2023-06-08 13:00:49.000000 cloudoll-2.0.1/cloudoll/orm/mysql.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.139447 cloudoll-2.0.1/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.1/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.1/cloudoll/robot/feishu.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.142777 cloudoll-2.0.1/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    13406 2023-06-08 12:53:24.000000 cloudoll-2.0.1/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.1/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.1/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.1/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.133597 cloudoll-2.0.1/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7019 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      104 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-06-09 07:31:10.144885 cloudoll-2.0.1/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4153 2023-06-09 07:30:50.000000 cloudoll-2.0.1/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.949346 cloudoll-2.0.2/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.2/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7081 2023-07-03 04:39:51.948700 cloudoll-2.0.2/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6448 2023-07-03 04:37:53.000000 cloudoll-2.0.2/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.933204 cloudoll-2.0.2/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.937559 cloudoll-2.0.2/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.938274 cloudoll-2.0.2/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.2/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.939679 cloudoll-2.0.2/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.2/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.941254 cloudoll-2.0.2/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.2/cloudoll/orm/mysql.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.943564 cloudoll-2.0.2/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.2/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.2/cloudoll/robot/feishu.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.947568 cloudoll-2.0.2/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    13907 2023-07-03 03:45:50.000000 cloudoll-2.0.2/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.2/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.2/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.2/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.936372 cloudoll-2.0.2/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7081 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      104 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-03 04:39:51.949521 cloudoll-2.0.2/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4153 2023-07-03 03:40:13.000000 cloudoll-2.0.2/setup.py
```

### Comparing `cloudoll-2.0.1/LICENSE` & `cloudoll-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/PKG-INFO` & `cloudoll-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.1
+Version: 2.0.2
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.2` 2023-07-03
+- 优化一系列问题
+- 可以热加载
+
 `2.0.0` 2023-06-09
 - 优化一系列问题
 - orm 执行更优雅
 
 `0.1.6` 2022-11-03
 - orm 允许更新为空数据
 - server 文件上传加入大小限制
```

### Comparing `cloudoll-2.0.1/README.md` & `cloudoll-2.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.2` 2023-07-03
+- 优化一系列问题
+- 可以热加载
+
 `2.0.0` 2023-06-09
 - 优化一系列问题
 - orm 执行更优雅
 
 `0.1.6` 2022-11-03
 - orm 允许更新为空数据
 - server 文件上传加入大小限制
```

### Comparing `cloudoll-2.0.1/cloudoll/error/errors.py` & `cloudoll-2.0.2/cloudoll/error/errors.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/logging/__init__.py` & `cloudoll-2.0.2/cloudoll/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/mail/smtp.py` & `cloudoll-2.0.2/cloudoll/mail/smtp.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/orm/mysql.py` & `cloudoll-2.0.2/cloudoll/orm/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,16 @@
                     await cursor.close()
             self.pool.release(conn)
 
     async def _execute(self, cur, sql, params=None):
         sql = sql.replace("%", "%%")
         sql = sql.replace("?", "%s")
         await cur.execute(sql, params)
-
-        if sql.startswith('select') or sql.startswith('show'):
+        
+        if sql.lower().startswith('select') or sql.lower().startswith('show') or sql.lower().startswith('with'):
             result = await cur.fetchall()
         elif sql.startswith('delete'):
             result = cur.rowcount > 0
         elif sql.startswith('insert'):
             result = cur.lastrowid if cur.rowcount > 0 else None
         else:
             result = cur.rowcount
```

### Comparing `cloudoll-2.0.1/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.2/cloudoll/robot/dingtalk.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/robot/feishu.py` & `cloudoll-2.0.2/cloudoll/robot/feishu.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/web/__init__.py` & `cloudoll-2.0.2/cloudoll/web/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 import socket
 from urllib import parse
 import aiomcache
 import aioredis
 from aiohttp import web
 from aiohttp.web_exceptions import *
 from aiohttp.web_ws import WebSocketResponse as WebSocket, WSMsgType
-from aiohttp_session import get_session, setup, redis_storage, memcached_storage, cookie_storage
+from aiohttp_session import (
+    get_session,
+    setup,
+    redis_storage,
+    memcached_storage,
+    cookie_storage,
+)
 from jinja2 import Environment, FileSystemLoader
 from setuptools import find_packages
 from .settings import get_config
 
 from ..logging import logging
 from ..orm.mysql import sa
 from . import jwt
@@ -31,28 +37,27 @@
 
 class _Handler(object):
     def __init__(self, cls, fn):
         self.cls = cls
         self.fn = fn
 
     async def __call__(self, request):
-
         c_type = request.content_type
         # 获取函数参数的名称和默认值
         props = inspect.getfullargspec(self.fn)
-        if len(props.args) == 2 and c_type == 'multipart/form-data':
+        if len(props.args) == 2 and c_type == "multipart/form-data":
             await _set_session_route(request)
             multipart = await request.multipart()
             field = await multipart.next()
             return await self.fn(request, field)
         elif len(props.args) == 1:
             await _set_session_route(request)
-            if c_type == 'multipart/form-data':
+            if c_type == "multipart/form-data":
                 data = await request.post()
-            elif c_type == 'application/json':
+            elif c_type == "application/json":
                 data = await request.json()
             else:
                 data = await request.post()
             q_s = request.query_string
             body = {}
             for k in data:
                 body[k] = data[k]
@@ -77,23 +82,23 @@
     session = await get_session(request)
     # session = await new_session(request)
     request.session = session
 
 
 def _get_modules(fd):
     modules = set()
-    temp = os.path.join(os.path.abspath('.'), fd)
+    temp = os.path.join(os.path.abspath("."), fd)
     if not os.path.exists(temp):
         return
     s = find_packages(temp)
     for pkg in s:
         # modules.add(pkg)
         pkg_path = temp + "/" + pkg.replace(".", "/")
         if sys.version_info.major == 2 or (
-                sys.version_info.major == 3 and sys.version_info.minor < 6
+            sys.version_info.major == 3 and sys.version_info.minor < 6
         ):
             for _, name, ispkg in pkgutil.iter_modules([pkg_path]):
                 if not ispkg:
                     modules.add(f".{pkg}.{name}")
         else:
             for info in pkgutil.iter_modules([pkg_path]):
                 if not info.ispkg:
@@ -110,20 +115,20 @@
     finally:
         sk.close()
     if r == 0:
         raise OSError(f"Address {host}:{port} already in use.")
 
 
 def _reg_middleware():
-    fd = 'middlewares'
-    temp = os.path.join(os.path.abspath('.'), fd)
+    fd = "middlewares"
+    temp = os.path.join(os.path.abspath("."), fd)
     if not os.path.exists(temp):
         return
     for f in os.listdir(temp):
-        if not f.startswith('__'):
+        if not f.startswith("__"):
             module_name = f"{fd}.{os.path.basename(f)[:-3]}"
             importlib.import_module(module_name, fd)
 
 
 def _int(num):
     return eval(num) if isinstance(num, str) else num
 
@@ -142,136 +147,153 @@
     def create(self):
         loop = asyncio.get_event_loop()
         if loop is None:
             loop = asyncio.new_event_loop()
         self._loop = loop
 
         parser = argparse.ArgumentParser(description="cloudoll app.")
-        parser.add_argument('--env', default='local')
-        parser.add_argument('--host')
-        parser.add_argument('--port')
-        parser.add_argument('--path')
+        parser.add_argument("--env", default="local")
+        parser.add_argument("--host")
+        parser.add_argument("--port")
+        parser.add_argument("--path")
         args, extra_argv = parser.parse_known_args()
         config = get_config(args.env)
 
         self._args = args
         self.config = config
 
         # middlewares
         _reg_middleware()
 
-        conf_server = config.get('server')
-        client_max_size = 1024 ** 2 * 2
+        conf_server = config.get("server")
+        client_max_size = 1024**2 * 2
         if conf_server is not None:
-            client_max_size = conf_server.get('client_max_size', client_max_size)
-        self.app = web.Application(logger=None, loop=loop, middlewares=self._middleware,
-                                   client_max_size=_int(client_max_size))
+            client_max_size = conf_server.get("client_max_size", client_max_size)
+        self.app = web.Application(
+            logger=None,
+            loop=loop,
+            middlewares=self._middleware,
+            client_max_size=_int(client_max_size),
+        )
         # database
         self.app.on_startup.append(self._init_database)
         self.app.on_cleanup.append(self._close_database)
         self.app.config = config
         self.app.jwt_encode = self.jwt_encode
         self.app.jwt_decode = self.jwt_decode
         # session
         self._init_session()
         #  router:
         self._reg_router()
 
         # static
         if conf_server is not None:
-            conf_st = conf_server.get('static')
+            conf_st = conf_server.get("static")
             if conf_st:
-                temp = os.path.join(os.path.abspath("."), 'static')
+                temp = os.path.join(os.path.abspath("."), "static")
                 self.app.router.add_static(**conf_st, path=temp)
                 logging.warning("Suggest using nginx or others instead.")
 
-        temp = os.path.join(os.path.abspath("."), 'templates')
+        temp = os.path.join(os.path.abspath("."), "templates")
         if os.path.exists(temp):
             self.env = Environment(loader=FileSystemLoader(temp), autoescape=True)
 
         return self
 
     async def _close_database(self, apps):
         if self.mysql:
             await self.mysql.close()
 
     async def _init_database(self, apps):
-        conf_mysql = self.config.get('mysql')
+        conf_mysql = self.config.get("mysql")
         if conf_mysql is not None:
             self.mysql = await sa.create_engine(**conf_mysql)
             self.app.mysql = self.mysql
             apps.mysql = self.mysql
 
     def _init_session(self):
         config = self.config
         # redis
-        redis_conf = config.get('redis')
-        mcache_conf = config.get('memcached')
-        _SESSION_KEY = 'CLOUDOLL_SESSION'
+        redis_conf = config.get("redis")
+        mcache_conf = config.get("memcached")
+        _SESSION_KEY = "CLOUDOLL_SESSION"
 
         if redis_conf:
-            redis_url = redis_conf.get('url')
+            redis_url = redis_conf.get("url")
             if not redis_url:
-                protocol = redis_conf.get('protocol', 'redis:')
-                host = redis_conf.get('host')
-                port = redis_conf.get('port', 6379)
-                username = redis_conf.get('username')
-                password = redis_conf.get('password')
-                db = redis_conf.get('db', 0)
-                path = redis_conf.get('path')
+                protocol = redis_conf.get("protocol", "redis:")
+                host = redis_conf.get("host")
+                port = redis_conf.get("port", 6379)
+                username = redis_conf.get("username")
+                password = redis_conf.get("password")
+                db = redis_conf.get("db", 0)
+                path = redis_conf.get("path")
                 if not path:
                     path = f"{host}:{port}/{db}"
                 else:
                     path = f"{path}?db={db}"
                 if password and username:
                     path = f"{username}:{password}@{path}"
                 redis_url = f"{protocol}//{path}"
 
-            max_age = redis_conf.get('max_age')
-            secure = redis_conf.get('secure')
-            httponly = redis_conf.get('httponly')
-            cookie_name = redis_conf.get('key', _SESSION_KEY)
+            max_age = redis_conf.get("max_age")
+            secure = redis_conf.get("secure")
+            httponly = redis_conf.get("httponly")
+            cookie_name = redis_conf.get("key", _SESSION_KEY)
 
             redis = aioredis.from_url(redis_url)
             self.app.redis = redis
-            storage = redis_storage.RedisStorage(redis,
-                                                 cookie_name=cookie_name, max_age=_int(max_age), httponly=httponly,
-                                                 secure=secure)
+            storage = redis_storage.RedisStorage(
+                redis,
+                cookie_name=cookie_name,
+                max_age=_int(max_age),
+                httponly=httponly,
+                secure=secure,
+            )
             setup(self.app, storage)
         elif mcache_conf:
-            host = mcache_conf.get('host')
-            port = mcache_conf.get('port', 11211)
-            max_age = mcache_conf.get('max_age')
-            secure = mcache_conf.get('secure')
-            httponly = mcache_conf.get('httponly')
-            cookie_name = mcache_conf.get('key', _SESSION_KEY)
+            host = mcache_conf.get("host")
+            port = mcache_conf.get("port", 11211)
+            max_age = mcache_conf.get("max_age")
+            secure = mcache_conf.get("secure")
+            httponly = mcache_conf.get("httponly")
+            cookie_name = mcache_conf.get("key", _SESSION_KEY)
             mc = aiomcache.Client(host, port)
             self.app.memcached = mc
-            storage = memcached_storage.MemcachedStorage(mc, cookie_name=cookie_name, max_age=_int(max_age),
-                                                         httponly=httponly, secure=secure)
+            storage = memcached_storage.MemcachedStorage(
+                mc,
+                cookie_name=cookie_name,
+                max_age=_int(max_age),
+                httponly=httponly,
+                secure=secure,
+            )
             setup(self.app, storage)
         else:
-            sess = config.get('session', {})
-            sess_name = sess.get('key', _SESSION_KEY)
+            sess = config.get("session", {})
+            sess_name = sess.get("key", _SESSION_KEY)
 
             dig = hashlib.sha256(sess_name.encode()).digest()
             fernet_key = base64.urlsafe_b64encode(dig)
             secret_key = base64.urlsafe_b64decode(fernet_key)
 
             # fernet_key = fernet.Fernet.generate_key()
             # secret_key = base64.urlsafe_b64decode(fernet_key)
 
-            max_age = sess.get('max_age')
-            httponly = sess.get('httponly')
-            storage = cookie_storage.EncryptedCookieStorage(secret_key, cookie_name=sess_name, max_age=_int(max_age),
-                                                            httponly=httponly)
+            max_age = sess.get("max_age")
+            httponly = sess.get("httponly")
+            storage = cookie_storage.EncryptedCookieStorage(
+                secret_key,
+                cookie_name=sess_name,
+                max_age=_int(max_age),
+                httponly=httponly,
+            )
             setup(self.app, storage)
 
     def _reg_router(self):
-        fd = 'controllers'
+        fd = "controllers"
         modules = _get_modules(fd)
         for module in modules:
             # print(module, router)
             importlib.import_module(module, fd)
 
         self.app.add_routes(self._route_table)
         # for route in self._routes:
@@ -279,24 +301,35 @@
 
     def run(self, **kw):
         """
         run app
         :params prot default  9001
         :params host default 127.0.0.1
         """
-        conf = self.config.get('server', {})
+        conf = self.config.get("server", {})
+        if conf.get('reload',False) is True:
+            import aioreloader
+            aioreloader.start()
         conf.update(kw)
         conf.update(vars(self._args))
         conf = argparse.Namespace(**conf)
-        host = conf.host if conf.host else 'localhost'
+        host = conf.host if conf.host else "localhost"
         port = conf.port if conf.port else 9001
         path = conf.path
         _check_address(host, port)
         # logging.info(f"Server run at http://{host}:{port}")
-        web.run_app(self.app, loop=self._loop, host=host, port=port, path=path, access_log=None, **kw)
+        web.run_app(
+            self.app,
+            loop=self._loop,
+            host=host,
+            port=port,
+            path=path,
+            access_log=None,
+            **kw,
+        )
         # # old
         # if self.loop is None:
         #     return web.run_app(self.app, host=host, port=port, **kw)
         # else:
         #     logging.info(f"Server run at http://{host}:{port}")
         #     return self.loop.create_server(
         #         self.app.make_handler(), host=host, port=port, **kw
@@ -315,24 +348,24 @@
             mid = func()
             mid.__middleware_version__ = 1
             self._middleware.append(mid)
 
         return wrapper
 
     def jwt_encode(self, payload):
-        jwt_conf = self.config.get('jwt', {})
-        key = jwt_conf.get('key')
-        exp = jwt_conf.get('exp')
+        jwt_conf = self.config.get("jwt", {})
+        key = jwt_conf.get("key")
+        exp = jwt_conf.get("exp")
         if not key or not exp:
             raise KeyError("Please set jwt key or exp...")
         return jwt.encode(payload, key, exp)
 
     def jwt_decode(self, token):
-        jwt_conf = self.config.get('jwt', {})
-        key = jwt_conf.get('key')
+        jwt_conf = self.config.get("jwt", {})
+        key = jwt_conf.get("key")
         return jwt.decode(token, key)
 
     @property
     def route_table(self):
         return self._route_table
 
     @property
@@ -369,18 +402,15 @@
 
     def __str__(self):
         return self.key
 
 
 class JsonEncoder(json.JSONEncoder):
     def default(self, obj):
-        if (
-                isinstance(obj, datetime.datetime)
-                or isinstance(obj, datetime.date)
-        ):
+        if isinstance(obj, datetime.datetime) or isinstance(obj, datetime.date):
             return obj.__str__()
         else:
             return super(JsonEncoder, self).default(obj)
 
 
 def get(path, name=None):
     return app.add_router(path, "GET", name)
@@ -400,18 +430,26 @@
 
 def all(path):
     #     return app._actions(path, 'GET')
     return app.route_table.view(path)
 
 
 def jsons(data, **kw):
-    if not data:
-        data = dict()
-    data["timestamp"] = int(datetime.datetime.now().timestamp() * 1000)
-    text = json.dumps(data, ensure_ascii=False, cls=JsonEncoder)
+    res = {}
+    if isinstance(data, list):
+        res["data"] = data
+    elif isinstance(data, dict):
+        res.update(data)
+    elif isinstance(data, tuple):
+        data = dict(data)
+        res.update(data)
+    else:
+        raise ValueError("data must be list , dict or tuple.")
+    res["timestamp"] = int(datetime.datetime.now().timestamp() * 1000)
+    text = json.dumps(res, ensure_ascii=False, cls=JsonEncoder)
     return web.json_response(text=text, **kw)
 
 
 def middleware():
     return app.add_middleware()
```

### Comparing `cloudoll-2.0.1/cloudoll/web/html.py` & `cloudoll-2.0.2/cloudoll/web/html.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/web/http.py` & `cloudoll-2.0.2/cloudoll/web/http.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll/web/jwt.py` & `cloudoll-2.0.2/cloudoll/web/jwt.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.0.2/cloudoll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.1
+Version: 2.0.2
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.2` 2023-07-03
+- 优化一系列问题
+- 可以热加载
+
 `2.0.0` 2023-06-09
 - 优化一系列问题
 - orm 执行更优雅
 
 `0.1.6` 2022-11-03
 - orm 允许更新为空数据
 - server 文件上传加入大小限制
```

### Comparing `cloudoll-2.0.1/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.2/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.1/setup.py` & `cloudoll-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "cloudoll"
 DESCRIPTION = "辅助快速创建可分布的微服务。"
 URL = "https://gitee.com/chuchur/cloudoll-py"
 EMAIL = "chuchur@qq.com"
 AUTHOR = "chuchur"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "colorlog",
     "aiomysql",
     "aiopg",
```


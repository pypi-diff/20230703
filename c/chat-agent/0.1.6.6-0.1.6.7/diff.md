# Comparing `tmp/chat_agent-0.1.6.6.tar.gz` & `tmp/chat_agent-0.1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_agent-0.1.6.6.tar", last modified: Sun Apr  9 12:27:34 2023, max compression
+gzip compressed data, was "chat_agent-0.1.6.7.tar", last modified: Mon Jul  3 16:14:05 2023, max compression
```

## Comparing `chat_agent-0.1.6.6.tar` & `chat_agent-0.1.6.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.365045 chat_agent-0.1.6.6/
--rw-r--r--   0 alex       (501) staff       (20)       48 2023-03-20 19:07:00.000000 chat_agent-0.1.6.6/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-09 12:27:34.364852 chat_agent-0.1.6.6/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1696 2023-04-09 12:27:15.000000 chat_agent-0.1.6.6/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.356353 chat_agent-0.1.6.6/chat_agent/
--rw-r--r--   0 alex       (501) staff       (20)     2755 2023-04-08 16:47:51.000000 chat_agent-0.1.6.6/chat_agent/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2893 2023-04-09 12:26:53.000000 chat_agent-0.1.6.6/chat_agent/app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.357775 chat_agent-0.1.6.6/chat_agent/base/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:27:54.000000 chat_agent-0.1.6.6/chat_agent/base/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3843 2023-04-08 16:45:47.000000 chat_agent-0.1.6.6/chat_agent/base/base_websocket.py
--rw-r--r--   0 alex       (501) staff       (20)      223 2023-04-07 11:50:22.000000 chat_agent-0.1.6.6/chat_agent/base/singleton.py
--rw-r--r--   0 alex       (501) staff       (20)     1550 2023-04-09 12:24:16.000000 chat_agent-0.1.6.6/chat_agent/base_websocket_app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.358792 chat_agent-0.1.6.6/chat_agent/cache/
--rw-r--r--   0 alex       (501) staff       (20)      252 2023-03-24 01:24:01.000000 chat_agent-0.1.6.6/chat_agent/cache/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      818 2023-03-24 01:39:51.000000 chat_agent-0.1.6.6/chat_agent/cache/cache_helper.py
--rw-r--r--   0 alex       (501) staff       (20)     2147 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/cert.pem
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.359523 chat_agent-0.1.6.6/chat_agent/client/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-05 02:46:32.000000 chat_agent-0.1.6.6/chat_agent/client/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1055 2023-04-08 16:55:38.000000 chat_agent-0.1.6.6/chat_agent/client/base_web_socket_client.py
--rw-r--r--   0 alex       (501) staff       (20)      670 2023-04-07 05:26:50.000000 chat_agent-0.1.6.6/chat_agent/client/web_socket_client.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.359905 chat_agent-0.1.6.6/chat_agent/config/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-20 17:04:34.000000 chat_agent-0.1.6.6/chat_agent/config/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      605 2023-04-08 16:45:47.000000 chat_agent-0.1.6.6/chat_agent/config/config_helper.py
--rw-r--r--   0 alex       (501) staff       (20)     1150 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/favicon.ico
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.360381 chat_agent-0.1.6.6/chat_agent/handler/
--rw-r--r--   0 alex       (501) staff       (20)     1048 2023-03-20 18:00:41.000000 chat_agent-0.1.6.6/chat_agent/handler/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4368 2023-04-09 12:26:53.000000 chat_agent-0.1.6.6/chat_agent/handler/openai_handler.py
--rw-r--r--   0 alex       (501) staff       (20)     3272 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/key.pem
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.360745 chat_agent-0.1.6.6/chat_agent/logger/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 13:54:55.000000 chat_agent-0.1.6.6/chat_agent/logger/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1433 2023-03-23 16:59:21.000000 chat_agent-0.1.6.6/chat_agent/logger/logger_helper.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.361513 chat_agent-0.1.6.6/chat_agent/static/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.362399 chat_agent-0.1.6.6/chat_agent/static/icon/
--rw-r--r--   0 alex       (501) staff       (20)    38340 2023-03-20 17:04:34.000000 chat_agent-0.1.6.6/chat_agent/static/icon/openai.png
--rw-r--r--   0 alex       (501) staff       (20)    23807 2023-03-20 17:04:34.000000 chat_agent-0.1.6.6/chat_agent/static/icon/whale.png
--rw-r--r--   0 alex       (501) staff       (20)     7336 2023-03-24 18:00:26.000000 chat_agent-0.1.6.6/chat_agent/static/index.html
--rw-r--r--   0 alex       (501) staff       (20)     8308 2023-04-05 17:43:03.000000 chat_agent-0.1.6.6/chat_agent/static/websocket_index.html
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.362594 chat_agent-0.1.6.6/chat_agent/test/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:51:34.000000 chat_agent-0.1.6.6/chat_agent/test/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.364551 chat_agent-0.1.6.6/chat_agent/util/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 14:25:57.000000 chat_agent-0.1.6.6/chat_agent/util/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      909 2023-04-08 05:17:18.000000 chat_agent-0.1.6.6/chat_agent/util/context.py
--rw-r--r--   0 alex       (501) staff       (20)       75 2023-03-23 16:56:11.000000 chat_agent-0.1.6.6/chat_agent/util/file.py
--rw-r--r--   0 alex       (501) staff       (20)      345 2023-03-23 16:08:29.000000 chat_agent-0.1.6.6/chat_agent/util/random.py
--rw-r--r--   0 alex       (501) staff       (20)      124 2023-03-24 01:09:14.000000 chat_agent-0.1.6.6/chat_agent/util/time.py
--rw-r--r--   0 alex       (501) staff       (20)      731 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/util/timeout.py
--rw-r--r--   0 alex       (501) staff       (20)     2964 2023-04-09 12:26:53.000000 chat_agent-0.1.6.6/chat_agent/websocket_app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.357231 chat_agent-0.1.6.6/chat_agent.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1146 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      269 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-04-09 12:27:34.365099 chat_agent-0.1.6.6/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      874 2023-04-09 12:27:08.000000 chat_agent-0.1.6.6/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.262717 chat_agent-0.1.6.7/
+-rw-r--r--   0 alex       (501) staff       (20)       48 2023-03-20 19:07:00.000000 chat_agent-0.1.6.7/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)      263 2023-07-03 16:14:05.262541 chat_agent-0.1.6.7/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1696 2023-07-03 16:10:17.000000 chat_agent-0.1.6.7/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.255479 chat_agent-0.1.6.7/chat_agent/
+-rw-r--r--   0 alex       (501) staff       (20)     2755 2023-04-08 16:47:51.000000 chat_agent-0.1.6.7/chat_agent/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2904 2023-07-03 16:09:47.000000 chat_agent-0.1.6.7/chat_agent/app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.256850 chat_agent-0.1.6.7/chat_agent/base/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:27:54.000000 chat_agent-0.1.6.7/chat_agent/base/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3843 2023-04-08 16:45:47.000000 chat_agent-0.1.6.7/chat_agent/base/base_websocket.py
+-rw-r--r--   0 alex       (501) staff       (20)      223 2023-04-07 11:50:22.000000 chat_agent-0.1.6.7/chat_agent/base/singleton.py
+-rw-r--r--   0 alex       (501) staff       (20)     1550 2023-04-09 12:24:16.000000 chat_agent-0.1.6.7/chat_agent/base_websocket_app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.257470 chat_agent-0.1.6.7/chat_agent/cache/
+-rw-r--r--   0 alex       (501) staff       (20)      252 2023-03-24 01:24:01.000000 chat_agent-0.1.6.7/chat_agent/cache/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      818 2023-03-24 01:39:51.000000 chat_agent-0.1.6.7/chat_agent/cache/cache_helper.py
+-rw-r--r--   0 alex       (501) staff       (20)     2147 2023-03-31 01:41:44.000000 chat_agent-0.1.6.7/chat_agent/cert.pem
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.258249 chat_agent-0.1.6.7/chat_agent/client/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-05 02:46:32.000000 chat_agent-0.1.6.7/chat_agent/client/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1055 2023-04-08 16:55:38.000000 chat_agent-0.1.6.7/chat_agent/client/base_web_socket_client.py
+-rw-r--r--   0 alex       (501) staff       (20)      670 2023-04-07 05:26:50.000000 chat_agent-0.1.6.7/chat_agent/client/web_socket_client.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.258628 chat_agent-0.1.6.7/chat_agent/config/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-20 17:04:34.000000 chat_agent-0.1.6.7/chat_agent/config/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      605 2023-04-08 16:45:47.000000 chat_agent-0.1.6.7/chat_agent/config/config_helper.py
+-rw-r--r--   0 alex       (501) staff       (20)     1150 2023-03-31 01:41:44.000000 chat_agent-0.1.6.7/chat_agent/favicon.ico
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.259137 chat_agent-0.1.6.7/chat_agent/handler/
+-rw-r--r--   0 alex       (501) staff       (20)     1048 2023-03-20 18:00:41.000000 chat_agent-0.1.6.7/chat_agent/handler/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4368 2023-04-09 12:26:53.000000 chat_agent-0.1.6.7/chat_agent/handler/openai_handler.py
+-rw-r--r--   0 alex       (501) staff       (20)     3272 2023-03-31 01:41:44.000000 chat_agent-0.1.6.7/chat_agent/key.pem
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.259540 chat_agent-0.1.6.7/chat_agent/logger/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 13:54:55.000000 chat_agent-0.1.6.7/chat_agent/logger/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1433 2023-03-23 16:59:21.000000 chat_agent-0.1.6.7/chat_agent/logger/logger_helper.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.260064 chat_agent-0.1.6.7/chat_agent/static/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.260842 chat_agent-0.1.6.7/chat_agent/static/icon/
+-rw-r--r--   0 alex       (501) staff       (20)    38340 2023-03-20 17:04:34.000000 chat_agent-0.1.6.7/chat_agent/static/icon/openai.png
+-rw-r--r--   0 alex       (501) staff       (20)    23807 2023-03-20 17:04:34.000000 chat_agent-0.1.6.7/chat_agent/static/icon/whale.png
+-rw-r--r--   0 alex       (501) staff       (20)     7336 2023-03-24 18:00:26.000000 chat_agent-0.1.6.7/chat_agent/static/index.html
+-rw-r--r--   0 alex       (501) staff       (20)     8308 2023-04-05 17:43:03.000000 chat_agent-0.1.6.7/chat_agent/static/websocket_index.html
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.261043 chat_agent-0.1.6.7/chat_agent/test/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:51:34.000000 chat_agent-0.1.6.7/chat_agent/test/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.262324 chat_agent-0.1.6.7/chat_agent/util/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 14:25:57.000000 chat_agent-0.1.6.7/chat_agent/util/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      909 2023-04-08 05:17:18.000000 chat_agent-0.1.6.7/chat_agent/util/context.py
+-rw-r--r--   0 alex       (501) staff       (20)       75 2023-03-23 16:56:11.000000 chat_agent-0.1.6.7/chat_agent/util/file.py
+-rw-r--r--   0 alex       (501) staff       (20)      345 2023-03-23 16:08:29.000000 chat_agent-0.1.6.7/chat_agent/util/random.py
+-rw-r--r--   0 alex       (501) staff       (20)      124 2023-03-24 01:09:14.000000 chat_agent-0.1.6.7/chat_agent/util/time.py
+-rw-r--r--   0 alex       (501) staff       (20)      731 2023-03-31 01:41:44.000000 chat_agent-0.1.6.7/chat_agent/util/timeout.py
+-rw-r--r--   0 alex       (501) staff       (20)     2964 2023-04-09 12:26:53.000000 chat_agent-0.1.6.7/chat_agent/websocket_app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-03 16:14:05.256260 chat_agent-0.1.6.7/chat_agent.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      263 2023-07-03 16:14:05.000000 chat_agent-0.1.6.7/chat_agent.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1146 2023-07-03 16:14:05.000000 chat_agent-0.1.6.7/chat_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-03 16:14:05.000000 chat_agent-0.1.6.7/chat_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      269 2023-07-03 16:14:05.000000 chat_agent-0.1.6.7/chat_agent.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-07-03 16:14:05.000000 chat_agent-0.1.6.7/chat_agent.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-03 16:14:05.262763 chat_agent-0.1.6.7/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      874 2023-07-03 16:09:59.000000 chat_agent-0.1.6.7/setup.py
```

### Comparing `chat_agent-0.1.6.6/README.md` & `chat_agent-0.1.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 简单的OpenAI chatGPT代理
 
 ### 安装
 ```
 使用pip安装最新版本，指定到官方pypi源
-pip install chat-agent==0.1.6.6 -i https://pypi.org/simple/
+pip install chat-agent==0.1.6.7 -i https://pypi.org/simple/
 ```
 
 ### 环境变量配置项：
 ```
 必配：
 OPENAI_ORGANIZATION_KEY: openai对应的组织id
 OPENAI_API_KEY: openai分配的api key
```

### Comparing `chat_agent-0.1.6.6/chat_agent/__init__.py` & `chat_agent-0.1.6.7/chat_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/app.py` & `chat_agent-0.1.6.7/chat_agent/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from chat_agent import CHAT_AGENT_PORT, CHAT_AGENT_HOST, CHAT_AGENT_SECRET_KEY, CHAT_AGENT_HTTPS, \
     CHAT_AGENT_SSL_CERT_FILE_FULL_PATH, CHAT_AGENT_SSL_KEY_FILE_FULL_PATH, CHAT_AGENT_HTTPS_PORT, \
     CHAT_AGENT_STATIC_PATH, CHAT_AGENT_TIMEOUT
 from chat_agent.handler.openai_handler import send_chat_message_with_steam_response
 from chat_agent.logger.logger_helper import get_logger
 from chat_agent.util import random
 from chat_agent.util.context import get_thread_context
-from util.timeout import TimeoutError, timeout_decorator
+from chat_agent.util.timeout import TimeoutError, timeout_decorator
 
 app = Flask(__name__, static_folder=CHAT_AGENT_STATIC_PATH)
 socketio = SocketIO(app)
 app.config['SECRET_KEY'] = CHAT_AGENT_SECRET_KEY
 CORS(app)
 
 logger = get_logger('app')
```

### Comparing `chat_agent-0.1.6.6/chat_agent/base/base_websocket.py` & `chat_agent-0.1.6.7/chat_agent/base/base_websocket.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/base_websocket_app.py` & `chat_agent-0.1.6.7/chat_agent/base_websocket_app.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/cache/cache_helper.py` & `chat_agent-0.1.6.7/chat_agent/cache/cache_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/cert.pem` & `chat_agent-0.1.6.7/chat_agent/cert.pem`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/client/base_web_socket_client.py` & `chat_agent-0.1.6.7/chat_agent/client/base_web_socket_client.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/client/web_socket_client.py` & `chat_agent-0.1.6.7/chat_agent/client/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/config/config_helper.py` & `chat_agent-0.1.6.7/chat_agent/config/config_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/favicon.ico` & `chat_agent-0.1.6.7/chat_agent/favicon.ico`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/handler/__init__.py` & `chat_agent-0.1.6.7/chat_agent/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/handler/openai_handler.py` & `chat_agent-0.1.6.7/chat_agent/handler/openai_handler.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/key.pem` & `chat_agent-0.1.6.7/chat_agent/key.pem`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/logger/logger_helper.py` & `chat_agent-0.1.6.7/chat_agent/logger/logger_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/static/icon/openai.png` & `chat_agent-0.1.6.7/chat_agent/static/icon/openai.png`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/static/icon/whale.png` & `chat_agent-0.1.6.7/chat_agent/static/icon/whale.png`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/static/index.html` & `chat_agent-0.1.6.7/chat_agent/static/index.html`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/static/websocket_index.html` & `chat_agent-0.1.6.7/chat_agent/static/websocket_index.html`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/util/context.py` & `chat_agent-0.1.6.7/chat_agent/util/context.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/util/timeout.py` & `chat_agent-0.1.6.7/chat_agent/util/timeout.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent/websocket_app.py` & `chat_agent-0.1.6.7/chat_agent/websocket_app.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/chat_agent.egg-info/SOURCES.txt` & `chat_agent-0.1.6.7/chat_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.6/setup.py` & `chat_agent-0.1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chat_agent",
-    version="0.1.6.6",
+    version="0.1.6.7",
     packages=find_packages(),
     zip_sage=False,
     include_package_data=True,
     install_requires=[
         'setuptools~=63.4.1',
         'flask~=2.2.2',
         'flask_cors~=3.0.10',
```


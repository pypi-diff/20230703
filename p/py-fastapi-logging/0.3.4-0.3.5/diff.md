# Comparing `tmp/py_fastapi_logging-0.3.4.tar.gz` & `tmp/py_fastapi_logging-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_fastapi_logging-0.3.4.tar", max compression
+gzip compressed data, was "py_fastapi_logging-0.3.5.tar", max compression
```

## Comparing `py_fastapi_logging-0.3.4.tar` & `py_fastapi_logging-0.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1054 2022-08-24 15:08:05.819480 py_fastapi_logging-0.3.4/LICENSE
--rw-r--r--   0        0        0     1192 2022-09-30 14:17:24.478843 py_fastapi_logging-0.3.4/README.md
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.819480 py_fastapi_logging-0.3.4/py_fastapi_logging/__init__.py
--rw-r--r--   0        0        0     5208 2022-09-30 14:17:24.479843 py_fastapi_logging-0.3.4/py_fastapi_logging/aiohttp.py
--rw-r--r--   0        0        0     2565 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/py_fastapi_logging/aiopika.py
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.819480 py_fastapi_logging-0.3.4/py_fastapi_logging/config/__init__.py
--rw-r--r--   0        0        0     6288 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/py_fastapi_logging/config/config.py
--rw-r--r--   0        0        0       73 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/constants.py
--rw-r--r--   0        0        0     2968 2022-09-30 14:17:24.479843 py_fastapi_logging-0.3.4/py_fastapi_logging/data_filter.py
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/__init__.py
--rw-r--r--   0        0        0      923 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/base.py
--rw-r--r--   0        0        0     2571 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/json.py
--rw-r--r--   0        0        0     1329 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/simple.py
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/middlewares/__init__.py
--rw-r--r--   0        0        0     7403 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/py_fastapi_logging/middlewares/logging.py
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/middlewares/utils/__init__.py
--rw-r--r--   0        0        0      411 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/middlewares/utils/request_id.py
--rw-r--r--   0        0        0       59 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/py_fastapi_logging/py.typed
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/schemas/__init__.py
--rw-r--r--   0        0        0      173 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/schemas/base.py
--rw-r--r--   0        0        0      161 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/schemas/request.py
--rw-r--r--   0        0        0      127 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/schemas/response.py
--rw-r--r--   0        0        0        0 2022-08-24 15:08:05.820480 py_fastapi_logging-0.3.4/py_fastapi_logging/utils/__init__.py
--rw-r--r--   0        0        0     1670 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/py_fastapi_logging/utils/extra.py
--rw-r--r--   0        0        0     1892 2023-02-16 06:50:32.060056 py_fastapi_logging-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 py_fastapi_logging-0.3.4/setup.py
--rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 py_fastapi_logging-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1054 2022-08-05 10:37:41.507103 py_fastapi_logging-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1192 2022-09-13 12:44:58.624308 py_fastapi_logging-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/__init__.py
+-rw-r--r--   0        0        0     5208 2022-09-19 08:13:52.485840 py_fastapi_logging-0.3.5/py_fastapi_logging/aiohttp.py
+-rw-r--r--   0        0        0     2520 2023-07-03 14:44:56.728217 py_fastapi_logging-0.3.5/py_fastapi_logging/aiopika.py
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/config/__init__.py
+-rw-r--r--   0        0        0     6288 2023-02-09 09:50:38.277776 py_fastapi_logging-0.3.5/py_fastapi_logging/config/config.py
+-rw-r--r--   0        0        0       73 2022-08-24 08:51:39.249737 py_fastapi_logging-0.3.5/py_fastapi_logging/constants.py
+-rw-r--r--   0        0        0     2968 2022-09-19 08:13:52.485840 py_fastapi_logging-0.3.5/py_fastapi_logging/data_filter.py
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/__init__.py
+-rw-r--r--   0        0        0      923 2022-08-24 08:51:39.250737 py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/base.py
+-rw-r--r--   0        0        0     2571 2022-08-24 08:51:39.251737 py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/json.py
+-rw-r--r--   0        0        0     1329 2022-10-26 09:47:34.846220 py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/simple.py
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/middlewares/__init__.py
+-rw-r--r--   0        0        0     7403 2023-02-09 09:52:55.940082 py_fastapi_logging-0.3.5/py_fastapi_logging/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/middlewares/utils/__init__.py
+-rw-r--r--   0        0        0      411 2022-08-24 08:51:39.254737 py_fastapi_logging-0.3.5/py_fastapi_logging/middlewares/utils/request_id.py
+-rw-r--r--   0        0        0       59 2023-02-09 09:50:38.278776 py_fastapi_logging-0.3.5/py_fastapi_logging/py.typed
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/schemas/__init__.py
+-rw-r--r--   0        0        0      173 2022-08-24 08:51:39.255737 py_fastapi_logging-0.3.5/py_fastapi_logging/schemas/base.py
+-rw-r--r--   0        0        0      161 2022-08-24 08:51:39.255737 py_fastapi_logging-0.3.5/py_fastapi_logging/schemas/request.py
+-rw-r--r--   0        0        0      127 2022-07-05 12:27:04.961886 py_fastapi_logging-0.3.5/py_fastapi_logging/schemas/response.py
+-rw-r--r--   0        0        0        0 2022-07-05 03:29:29.408879 py_fastapi_logging-0.3.5/py_fastapi_logging/utils/__init__.py
+-rw-r--r--   0        0        0     1670 2023-02-09 09:50:38.278776 py_fastapi_logging-0.3.5/py_fastapi_logging/utils/extra.py
+-rw-r--r--   0        0        0     1892 2023-07-03 14:44:56.729217 py_fastapi_logging-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 py_fastapi_logging-0.3.5/setup.py
+-rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 py_fastapi_logging-0.3.5/PKG-INFO
```

### Comparing `py_fastapi_logging-0.3.4/LICENSE` & `py_fastapi_logging-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/README.md` & `py_fastapi_logging-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/aiohttp.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/aiohttp.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/aiopika.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/aiopika.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             payload = message.body.decode("utf8")
             payload = self._data_filter.filter_json_body(payload)
         except Exception:
             logging.exception("Failed to prepare message payload for logging")
             payload = "[failed to decode or filter]"
 
         logging.info(
-            f"{action} {exchange or 'default'}/{routing_key}",
+            "- ",
             extra={
                 "tags": ["MQ", action],
                 "request_id": request_id,
                 "payload": {
                     "exchange": exchange,
                     "queue": routing_key,
                     "message": payload,
```

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/config/config.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/config/config.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/data_filter.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/data_filter.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/base.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/base.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/json.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/json.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/formatters/simple.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/formatters/simple.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/middlewares/logging.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/py_fastapi_logging/utils/extra.py` & `py_fastapi_logging-0.3.5/py_fastapi_logging/utils/extra.py`

 * *Files identical despite different names*

### Comparing `py_fastapi_logging-0.3.4/pyproject.toml` & `py_fastapi_logging-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-fastapi-logging"
-version = "0.3.4"
+version = "0.3.5"
 authors = ["RockITSoft", "Dmitry Akhnazarov", "Victor Tsykanov", "Mikhail Pachurin", "Andrey Malchuk"]
 description = "FastAPI Logging"
 keywords = ["fastapi", "logging", "middleware"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `py_fastapi_logging-0.3.4/setup.py` & `py_fastapi_logging-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 extras_require = \
 {'aiohttp': ['aiohttp>=3'],
  'aiopika': ['aio-pika>=6'],
  'all': ['aiohttp>=3', 'aio-pika>=6']}
 
 setup_kwargs = {
     'name': 'py-fastapi-logging',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'FastAPI Logging',
     'long_description': '# py-fastapi-logging\n\n## ENV-переменные для управления логами\n#### Уровень логов. debug - для площадок отладки, info - для PROM\nLOG_LEVEL=info\n#### Формат логов: SIMPLE (обычный) или JSON (JSON-STDOUT - лог в формате json в поток stdout)\nLOG_FORMAT=SIMPLE\n#### Папка, в которой будут лежать логи\nLOG_DIR=/var/log/<APP NAME>\n#### Название файла лога\nLOG_FILENAME=production.log\n#### Добавление переменных в лог (JSON-формат) из переменных окружения\nLOG_ENV_EXTRA="field1:ENV_VAR_NAME_1,field2:ENV_VAR_NAME_2"\n\n\n## Интеграция в FastAPI приложение\n```python\nfrom fastapi import FastAPI\nfrom py_fastapi_logging.middlewares.logging import LoggingMiddleware\napp = FastAPI()\napp.add_middleware(LoggingMiddleware, app_name=\'my_app_name\')\n```\n\n## Использование логгера в приложениях не на FastAPI\n```python\nimport logging\nfrom py_fastapi_logging.config.config import init_logger\ninit_logger(app_name=\'my_app_name\')\nlogger = logging.getLogger()\n```\n',
     'author': 'RockITSoft',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `py_fastapi_logging-0.3.4/PKG-INFO` & `py_fastapi_logging-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-fastapi-logging
-Version: 0.3.4
+Version: 0.3.5
 Summary: FastAPI Logging
 License: MIT
 Keywords: fastapi,logging,middleware
 Author: RockITSoft
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/communica-0.2.1b5.tar.gz` & `tmp/communica-0.2.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.2.1b5.tar", last modified: Mon Jul  3 06:07:08 2023, max compression
+gzip compressed data, was "communica-0.2.1b6.tar", last modified: Mon Jul  3 06:14:47 2023, max compression
```

## Comparing `communica-0.2.1b5.tar` & `communica-0.2.1b6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.425318 communica-0.2.1b5/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b5/LICENSE.txt
--rw-rw-rw-   0        0        0     2233 2023-07-03 06:07:08.425318 communica-0.2.1b5/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.401318 communica-0.2.1b5/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b5/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b5/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.411317 communica-0.2.1b5/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b5/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-05-30 15:52:39.000000 communica-0.2.1b5/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b5/communica/connectors/base.py
--rw-rw-rw-   0        0        0    28135 2023-05-29 21:54:05.000000 communica-0.2.1b5/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b5/communica/connectors/stream.py
--rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b5/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.415319 communica-0.2.1b5/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b5/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b5/communica/pairs/base.py
--rw-rw-rw-   0        0        0     9863 2023-05-21 12:35:07.000000 communica-0.2.1b5/communica/pairs/route.py
--rw-rw-rw-   0        0        0    16363 2023-07-03 05:53:23.000000 communica-0.2.1b5/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.420317 communica-0.2.1b5/communica/serializers/
--rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b5/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-05-23 11:23:18.000000 communica-0.2.1b5/communica/serializers/adaptix.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b5/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b5/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b5/communica/servers.py
--rw-rw-rw-   0        0        0     4375 2023-05-30 16:58:39.000000 communica-0.2.1b5/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.405317 communica-0.2.1b5/communica.egg-info/
--rw-rw-rw-   0        0        0     2233 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1130 2023-07-03 06:05:19.000000 communica-0.2.1b5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 06:07:08.425318 communica-0.2.1b5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.423317 communica-0.2.1b5/tests/
--rw-rw-rw-   0        0        0     2495 2023-07-03 06:04:05.000000 communica-0.2.1b5/tests/test_connectors.py
--rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b5/tests/test_entities.py
--rw-rw-rw-   0        0        0     2481 2023-07-03 05:55:23.000000 communica-0.2.1b5/tests/test_rmq_conn_check_policy.py
--rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b5/tests/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.065554 communica-0.2.1b6/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b6/LICENSE.txt
+-rw-rw-rw-   0        0        0     2233 2023-07-03 06:14:47.065554 communica-0.2.1b6/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.036555 communica-0.2.1b6/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b6/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b6/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.053575 communica-0.2.1b6/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b6/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-05-30 15:52:39.000000 communica-0.2.1b6/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5553 2023-07-03 06:13:05.000000 communica-0.2.1b6/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    28175 2023-07-03 06:08:14.000000 communica-0.2.1b6/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b6/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b6/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.056553 communica-0.2.1b6/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b6/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b6/communica/pairs/base.py
+-rw-rw-rw-   0        0        0     9863 2023-05-21 12:35:07.000000 communica-0.2.1b6/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    16363 2023-07-03 05:53:23.000000 communica-0.2.1b6/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.060553 communica-0.2.1b6/communica/serializers/
+-rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b6/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-05-23 11:23:18.000000 communica-0.2.1b6/communica/serializers/adaptix.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b6/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b6/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b6/communica/servers.py
+-rw-rw-rw-   0        0        0     4375 2023-05-30 16:58:39.000000 communica-0.2.1b6/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.047553 communica-0.2.1b6/communica.egg-info/
+-rw-rw-rw-   0        0        0     2233 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 06:14:47.000000 communica-0.2.1b6/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1130 2023-07-03 06:14:12.000000 communica-0.2.1b6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:14:47.065554 communica-0.2.1b6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 06:14:47.064554 communica-0.2.1b6/tests/
+-rw-rw-rw-   0        0        0     2495 2023-07-03 06:04:05.000000 communica-0.2.1b6/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b6/tests/test_entities.py
+-rw-rw-rw-   0        0        0     2481 2023-07-03 05:55:23.000000 communica-0.2.1b6/tests/test_rmq_conn_check_policy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b6/tests/test_serializers.py
```

### Comparing `communica-0.2.1b5/LICENSE.txt` & `communica-0.2.1b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/PKG-INFO` & `communica-0.2.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b5
+Version: 0.2.1b6
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b5/README.md` & `communica-0.2.1b6/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/connectors/_stream_local.py` & `communica-0.2.1b6/communica/connectors/_stream_local.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/connectors/base.py` & `communica-0.2.1b6/communica/connectors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,17 @@
 
 class BaseConnector(ABC):
     """Making connections"""
     _TYPE: str
 
     __slots__ = ()
 
+    def __repr__(self) -> str:
+        return f'{type(self).__name__}({self.repr_address()})'
+
     @abstractmethod
     def repr_address(self) -> str:
         raise NotImplementedError
 
     @classmethod
     def _check_dump(cls, dump: 'dict[str, Any]'):
         if cls._TYPE != dump['type']:
```

### Comparing `communica-0.2.1b5/communica/connectors/rabbitmq.py` & `communica-0.2.1b6/communica/connectors/rabbitmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self._waiter.set_result(True)
         self._waiter = self._loop.create_future()
 
     async def _sender(self):
         while (await self._waiter):
             if (conn := self._conn()) is None:
                 return  # pragma: no cover
-            await conn._send(_MessageType.LISTENING, b'')  # BUG: после реконнекта клиента к серверу всё ломается
+            await conn._send(_MessageType.LISTENING, b'')  # BUG: после реконнекта клиента к серверу всё ломается | нужно подтверждение
             del(conn)  # deleting reference
             if self._handle is None:
                 self._set_handle()
 
     def message_sent(self):
         if self._handle is None:
             self._set_handle()
```

### Comparing `communica-0.2.1b5/communica/connectors/stream.py` & `communica-0.2.1b6/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/exceptions.py` & `communica-0.2.1b6/communica/exceptions.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/pairs/base.py` & `communica-0.2.1b6/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/pairs/route.py` & `communica-0.2.1b6/communica/pairs/route.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/pairs/simple.py` & `communica-0.2.1b6/communica/pairs/simple.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/serializers/adaptix.py` & `communica-0.2.1b6/communica/serializers/adaptix.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/serializers/base.py` & `communica-0.2.1b6/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica/utils.py` & `communica-0.2.1b6/communica/utils.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/communica.egg-info/PKG-INFO` & `communica-0.2.1b6/communica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b5
+Version: 0.2.1b6
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b5/communica.egg-info/SOURCES.txt` & `communica-0.2.1b6/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/pyproject.toml` & `communica-0.2.1b6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.2.1b5"
+version = "0.2.1b6"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.2.1b5/tests/test_connectors.py` & `communica-0.2.1b6/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/tests/test_entities.py` & `communica-0.2.1b6/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/tests/test_rmq_conn_check_policy.py` & `communica-0.2.1b6/tests/test_rmq_conn_check_policy.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b5/tests/test_serializers.py` & `communica-0.2.1b6/tests/test_serializers.py`

 * *Files identical despite different names*


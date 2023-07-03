# Comparing `tmp/communica-0.2.1b4.tar.gz` & `tmp/communica-0.2.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.2.1b4.tar", last modified: Fri May 26 08:36:15 2023, max compression
+gzip compressed data, was "communica-0.2.1b5.tar", last modified: Mon Jul  3 06:07:08 2023, max compression
```

## Comparing `communica-0.2.1b4.tar` & `communica-0.2.1b5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.798051 communica-0.2.1b4/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b4/LICENSE.txt
--rw-rw-rw-   0        0        0     2233 2023-05-26 08:36:15.797552 communica-0.2.1b4/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.777051 communica-0.2.1b4/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b4/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b4/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.786050 communica-0.2.1b4/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b4/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-21 11:38:53.000000 communica-0.2.1b4/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b4/communica/connectors/base.py
--rw-rw-rw-   0        0        0    28038 2023-05-08 07:38:53.000000 communica-0.2.1b4/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b4/communica/connectors/stream.py
--rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b4/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.789551 communica-0.2.1b4/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b4/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b4/communica/pairs/base.py
--rw-rw-rw-   0        0        0     9863 2023-05-21 12:35:07.000000 communica-0.2.1b4/communica/pairs/route.py
--rw-rw-rw-   0        0        0    16180 2023-05-23 13:25:30.000000 communica-0.2.1b4/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.793551 communica-0.2.1b4/communica/serializers/
--rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b4/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-05-23 11:23:18.000000 communica-0.2.1b4/communica/serializers/adaptix.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b4/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b4/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b4/communica/servers.py
--rw-rw-rw-   0        0        0     4246 2023-05-21 11:53:38.000000 communica-0.2.1b4/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.781051 communica-0.2.1b4/communica.egg-info/
--rw-rw-rw-   0        0        0     2233 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1130 2023-05-26 08:35:41.000000 communica-0.2.1b4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 08:36:15.798051 communica-0.2.1b4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.797051 communica-0.2.1b4/tests/
--rw-rw-rw-   0        0        0     2146 2023-05-04 12:13:21.000000 communica-0.2.1b4/tests/test_connectors.py
--rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b4/tests/test_entities.py
--rw-rw-rw-   0        0        0     2481 2023-04-23 14:30:49.000000 communica-0.2.1b4/tests/test_rmq_conn_check_policy.py
--rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b4/tests/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.425318 communica-0.2.1b5/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2233 2023-07-03 06:07:08.425318 communica-0.2.1b5/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.401318 communica-0.2.1b5/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b5/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b5/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.411317 communica-0.2.1b5/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b5/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-05-30 15:52:39.000000 communica-0.2.1b5/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b5/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    28135 2023-05-29 21:54:05.000000 communica-0.2.1b5/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b5/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b5/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.415319 communica-0.2.1b5/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b5/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b5/communica/pairs/base.py
+-rw-rw-rw-   0        0        0     9863 2023-05-21 12:35:07.000000 communica-0.2.1b5/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    16363 2023-07-03 05:53:23.000000 communica-0.2.1b5/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.420317 communica-0.2.1b5/communica/serializers/
+-rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b5/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-05-23 11:23:18.000000 communica-0.2.1b5/communica/serializers/adaptix.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b5/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b5/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b5/communica/servers.py
+-rw-rw-rw-   0        0        0     4375 2023-05-30 16:58:39.000000 communica-0.2.1b5/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.405317 communica-0.2.1b5/communica.egg-info/
+-rw-rw-rw-   0        0        0     2233 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 06:07:08.000000 communica-0.2.1b5/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1130 2023-07-03 06:05:19.000000 communica-0.2.1b5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:07:08.425318 communica-0.2.1b5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 06:07:08.423317 communica-0.2.1b5/tests/
+-rw-rw-rw-   0        0        0     2495 2023-07-03 06:04:05.000000 communica-0.2.1b5/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b5/tests/test_entities.py
+-rw-rw-rw-   0        0        0     2481 2023-07-03 05:55:23.000000 communica-0.2.1b5/tests/test_rmq_conn_check_policy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b5/tests/test_serializers.py
```

### Comparing `communica-0.2.1b4/LICENSE.txt` & `communica-0.2.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/PKG-INFO` & `communica-0.2.1b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b4
+Version: 0.2.1b5
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b4/README.md` & `communica-0.2.1b5/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/connectors/_stream_local.py` & `communica-0.2.1b5/communica/connectors/_stream_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,18 +59,21 @@
         servers = await loop.start_serving_pipe(factory, format_address(address))
         return PipeServerWrapper(servers[0])
 
     def format_address(address: str) -> str:
         return '\\\\.\\pipe\\' + 'communica.' + address
 
 else:
+    import os
     import os.path
     import tempfile
 
     SOCK_DIR = os.path.join(tempfile.gettempdir(), 'communica')
+    if not os.path.exists(SOCK_DIR):
+        os.makedirs(SOCK_DIR)
 
     async def open_connection(
             address: str
     ) -> 'tuple[asyncio.StreamReader, asyncio.StreamWriter]':
         sock_path = format_address(address)
         return await asyncio.open_unix_connection(sock_path)
```

### Comparing `communica-0.2.1b4/communica/connectors/base.py` & `communica-0.2.1b5/communica/connectors/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/connectors/rabbitmq.py` & `communica-0.2.1b5/communica/connectors/rabbitmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self._waiter.set_result(True)
         self._waiter = self._loop.create_future()
 
     async def _sender(self):
         while (await self._waiter):
             if (conn := self._conn()) is None:
                 return  # pragma: no cover
-            await conn._send(_MessageType.LISTENING, b'')
+            await conn._send(_MessageType.LISTENING, b'')  # BUG: после реконнекта клиента к серверу всё ломается
             del(conn)  # deleting reference
             if self._handle is None:
                 self._set_handle()
 
     def message_sent(self):
         if self._handle is None:
             self._set_handle()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `communica-0.2.1b4/communica/connectors/stream.py` & `communica-0.2.1b5/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/exceptions.py` & `communica-0.2.1b5/communica/exceptions.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/pairs/base.py` & `communica-0.2.1b5/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/pairs/route.py` & `communica-0.2.1b5/communica/pairs/route.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/pairs/simple.py` & `communica-0.2.1b5/communica/pairs/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,24 +284,28 @@
 
     async def close(self) -> None:
         if self._run_task is not None:
             await self._flow._connection.close()
             self._run_task.cancel()
 
     async def _connection_keeper(self):
+        reconnect_delay = 0.2
         while True:
             try:
                 new_conn = await self.connector.client_connect(self._handshaker)
             except Exception as e:
-                logger.warning('Connect failed: %s', repr(e))
-                await asyncio.sleep(1)
+                logger.warning('%r: Connect failed: %r', self.connector, e)
+                await asyncio.sleep(reconnect_delay)
+                if reconnect_delay < 5:
+                    reconnect_delay += 0.2
                 continue
             else:
                 connection = self._flow.update_connection(new_conn)
                 self.connected_event.set()
+                reconnect_delay = 0.2
 
             try:
                 await connection.run_until_fail(self._flow.dispatch)
             except Exception as e:
                 logger.error('Unhandled exception '
                             f'in connection runner: {e!r}')
             self.connected_event.clear()
```

### Comparing `communica-0.2.1b4/communica/serializers/adaptix.py` & `communica-0.2.1b5/communica/serializers/adaptix.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/serializers/base.py` & `communica-0.2.1b5/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/communica/utils.py` & `communica-0.2.1b5/communica/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,40 +108,43 @@
                 await waiter
             except CancelledError:
                 waiter.cancel()
                 raise
 
         if self._get_waiter is not None:
             self._get_waiter.set_result(True)
+            self._get_waiter = None
 
         self._queue.append(item)
 
     async def get(self) -> _TV:
         if not self._queue:
             if self._get_waiter is not None:
                 raise RuntimeError('Duplicate get from queue')
 
+            waiter = self._get_loop().create_future()
             try:
-                self._get_waiter = self._get_loop().create_future()
+                self._get_waiter = waiter
                 await self._get_waiter
             finally:
-                self._get_waiter = None
+                if self._get_waiter is waiter:
+                    self._get_waiter = None
 
         while self._put_waiters:
             if not (waiter := self._put_waiters.popleft()).done():
                 waiter.set_result(True)
                 break
 
         return self._queue.popleft()
 
 
 def exc_log_callback(task: Task):
     if not task.cancelled() and (exc := task.exception()):
         tb = format_exception(type(exc), exc, exc.__traceback__)
-        logger.warning('Uncaught exception in %r:\n%s', task, tb)
+        logger.warning('Uncaught exception in %r:\n%s', task, '\n'.join(tb))
 
 
 def _time_print(*args):  # pragma: no cover
     import time
     print(round(time.monotonic(), 3), *args)
```

### Comparing `communica-0.2.1b4/communica.egg-info/PKG-INFO` & `communica-0.2.1b5/communica.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b4
+Version: 0.2.1b5
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b4/communica.egg-info/SOURCES.txt` & `communica-0.2.1b5/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/pyproject.toml` & `communica-0.2.1b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.2.1b4"
+version = "0.2.1b5"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.2.1b4/tests/test_connectors.py` & `communica-0.2.1b5/tests/test_connectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,18 +43,26 @@
             server.stop()
             await asyncio.sleep(2)
 
             # no messages and no notifications, connection should be closed
             assert not client._flow._connection.is_alive
 
             await asyncio.sleep(2)
-
             create_task(server.run())
+            # reconnect to restarted server
+            while not client._flow._connection.is_alive:
+                await asyncio.sleep(0.5)
+
+            assert client._flow._connection.is_alive
 
-            await asyncio.sleep(1)
+        assert not client._flow._connection.is_alive
+
+        # reconnect to running server
+        async with SimpleClient(connector) as client:
+            await asyncio.sleep(2)
 
             assert client._flow._connection.is_alive
 
         await server.wait_stop()
 
     @pytest.mark.asyncio
     async def test_connector(self):
```

### Comparing `communica-0.2.1b4/tests/test_entities.py` & `communica-0.2.1b5/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/tests/test_rmq_conn_check_policy.py` & `communica-0.2.1b5/tests/test_rmq_conn_check_policy.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b4/tests/test_serializers.py` & `communica-0.2.1b5/tests/test_serializers.py`

 * *Files identical despite different names*


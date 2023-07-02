# Comparing `tmp/msglib-0.1.0.tar.gz` & `tmp/msglib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msglib-0.1.0.tar", max compression
+gzip compressed data, was "msglib-0.2.0.tar", max compression
```

## Comparing `msglib-0.1.0.tar` & `msglib-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      721 2023-06-05 23:28:21.941455 msglib-0.1.0/LICENSE
--rw-r--r--   0        0        0       26 2023-06-05 23:32:38.945881 msglib-0.1.0/README.rst
--rw-r--r--   0        0        0        0 2023-05-21 22:02:02.318605 msglib-0.1.0/msglib/__init__.py
--rw-r--r--   0        0        0     1377 2023-06-04 23:20:28.156233 msglib-0.1.0/msglib/broker.py
--rw-r--r--   0        0        0     1103 2023-06-04 23:23:48.281715 msglib-0.1.0/msglib/client.py
--rw-r--r--   0        0        0     1844 2023-06-05 22:49:45.965570 msglib-0.1.0/msglib/handlers.py
--rw-r--r--   0        0        0     4557 2023-06-05 22:51:39.343523 msglib-0.1.0/msglib/ios.py
--rw-r--r--   0        0        0     1635 2023-06-05 22:48:42.760482 msglib-0.1.0/msglib/message.py
--rw-r--r--   0        0        0      784 2023-06-05 23:28:21.941455 msglib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 msglib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2023-06-05 23:28:21.941455 msglib-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5283 2023-07-02 23:19:18.236778 msglib-0.2.0/README.rst
+-rw-r--r--   0        0        0        0 2023-05-21 22:02:02.318605 msglib-0.2.0/msglib/__init__.py
+-rw-r--r--   0        0        0     2196 2023-07-02 23:19:18.236778 msglib-0.2.0/msglib/broker.py
+-rw-r--r--   0        0        0     1115 2023-07-02 23:19:18.236778 msglib-0.2.0/msglib/client.py
+-rw-r--r--   0        0        0     1843 2023-07-02 23:19:18.236778 msglib-0.2.0/msglib/handlers.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:19:18.236778 msglib-0.2.0/msglib/ios/__init__.py
+-rw-r--r--   0        0        0     4224 2023-07-02 23:19:18.236778 msglib-0.2.0/msglib/ios/io_memory.py
+-rw-r--r--   0        0        0     4058 2023-07-02 23:19:18.236778 msglib-0.2.0/msglib/ios/io_sockets.py
+-rw-r--r--   0        0        0     1635 2023-06-05 22:48:42.760482 msglib-0.2.0/msglib/message.py
+-rw-r--r--   0        0        0      784 2023-07-02 23:21:09.754844 msglib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 msglib-0.2.0/PKG-INFO
```

### Comparing `msglib-0.1.0/LICENSE` & `msglib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msglib-0.1.0/msglib/client.py` & `msglib-0.2.0/msglib/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     _publish(connection=connection, msg=msg)
 
 
 def blocking_pull_subscribe_to_queue(*, connection, q_id):
     return _QSub(connection=connection, q_id=q_id)
 
 
-class _QMsg:
+class AckableQMsg:
 
     def __init__(self, payload):
         self.payload = payload
 
     def ack(self):
         pass
 
@@ -34,12 +34,12 @@
                 command=Command.PULL_MSG,
         )
         self._connection = connection
 
     def __next__(self):
         _publish(connection=self._connection, msg=self._pull_msg)
         msg_fields = deserialize(self._connection)
-        return _QMsg(*msg_fields)
+        return AckableQMsg(*msg_fields)
 
 
 def _publish(*, connection, msg):
     connection.write(serialize(msg.to_bytes_tuple()))
```

### Comparing `msglib-0.1.0/msglib/handlers.py` & `msglib-0.2.0/msglib/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 class ConnectionHandler:
 
     def __init__(self):
         self._handlers = {
             ChannelType.QUEUE: QueueHandler(),
         }
 
-    def new_connection(self, connection_id):
+    def on_new_connection(self, connection_id):
         print(connection_id)
 
-    def handle_message(self, *, msg_fields):
+    def on_message(self, *, msg_fields):
         channel_type, *tail = msg_fields
         return self._handlers[int_from_bytes(channel_type)](
                 tail,
         )
 
 
 class ChannelType(int, Enum):
```

### Comparing `msglib-0.1.0/msglib/ios.py` & `msglib-0.2.0/msglib/ios/io_sockets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from collections.abc import Iterable
+from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import NewType
 import select
 import socket
 
-
-ConnectionId = NewType('ConnectionId', int)
+from msglib.broker import ConnectionsActivity
 
 
 class InvalidIPv6(Exception):
     pass
 
 
 class IPv6(tuple):
@@ -35,82 +33,67 @@
         return cls(0, 0, 0, 0, 0, 0, 0, 1)
 
     def __str__(self):
         return ':'.join(f'{quartet:04X}' for quartet in self)
 
 
 @dataclass(frozen=True, kw_only=True, slots=True)
-class IPv6ConnectArgs:
+class _IPv6ConnectArgs:
     host: IPv6
     port: int
 
     def __iter__(self):
         return iter((
             str(self.host),
             self.port,
             0,  # sin6_flowinfo
             0,  # sin6_scope_id
         ))
 
 
-class Connection:
-
-    def __init__(self, *, ip: IPv6, port: int):
-        self._socket: socket.socket
-        self._ip = ip
-        self._port = port
-
-    def __enter__(self):
-        self._socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
-        self._socket.__enter__()
-        self._socket.connect(
-                tuple(IPv6ConnectArgs(host=self._ip, port=self._port)))
-        return self
-
-    def __exit__(self, *args):
-        self._socket.__exit__(*args)
-
-    def read(self, num_bytes):
-        return self._socket.recv(num_bytes)
-
-    def write(self, bytes_):
-        return self._socket.sendall(bytes_)
-
-
-class InitializedConnection:
+class _Connection:
 
     def __init__(self, socket_):
         self._socket = socket_
         self.id = socket_.fileno()
 
     def read(self, num_bytes):
         return self._socket.recv(num_bytes)
 
     def write(self, bytes_):
         return self._socket.sendall(bytes_)
 
 
+@contextmanager
+def connect(*, ip: IPv6, port: int, timeout_seconds: float | None):
+    with socket.socket(socket.AF_INET6, socket.SOCK_STREAM) as socket_:
+        socket_.connect(tuple(_IPv6ConnectArgs(host=ip, port=port)))
+        socket_.settimeout(timeout_seconds)
+        yield _Connection(socket_)
+
+
 class EpollSocketManager:
 
-    def __init__(self, ip: IPv6, port: int):
+    def __init__(self, ip: IPv6, port: int, epoll_timeout_seconds: float):
         self._ip = ip
         self._port = port
         self._listen_socket: socket.socket
         self._epoll: select.epoll
+        self._epoll_timeout_s = epoll_timeout_seconds
 
     def __enter__(self):
         self._listen_socket = socket.socket(
                 socket.AF_INET6, socket.SOCK_STREAM)
         self._listen_socket.setsockopt(
                 socket.SOL_SOCKET,  # level
                 socket.SO_REUSEADDR,  # optname
                 1,  # value
         )
         self._listen_socket.bind(
-                tuple(IPv6ConnectArgs(host=self._ip, port=self._port)))
+                tuple(_IPv6ConnectArgs(host=self._ip, port=self._port)))
         self._listen_socket.listen(10)
         self._listen_socket.setblocking(False)
 
         self._epoll = select.epoll()
         self._epoll.register(self._listen_socket.fileno(), select.EPOLLIN)
 
         return self
@@ -123,38 +106,30 @@
     def get_activity(self):
         epoll_ = self._epoll
         listen_socket = self._listen_socket
 
         new_connections = []
         readable = []
         closed = []
-        events = epoll_.poll(0)
+        events = epoll_.poll(self._epoll_timeout_s)
         for fileno, event in events:
-            fileno = ConnectionId(fileno)
             if fileno == listen_socket.fileno():
                 connection, _ = listen_socket.accept()
                 connection.setblocking(False)
                 epoll_.register(connection.fileno(), select.EPOLLIN)
-                new_connections.append(InitializedConnection(connection))
+                new_connections.append(_Connection(connection))
             else:
                 processed = False
                 if event & select.EPOLLIN:
                     readable.append(fileno)
                     processed = True
                 if event & select.EPOLLHUP:
                     epoll_.unregister(fileno)
                     closed.append(fileno)
                     processed = True
                 if not processed:
                     raise ValueError(f'Unexpected event {event}')
-        return Connections(
+        return ConnectionsActivity(
                 new=new_connections,
                 readable_ids=readable,
                 closed_ids=closed,
         )
-
-
-@dataclass(kw_only=True, frozen=True, slots=True)
-class Connections:
-    new: Iterable[InitializedConnection | Connection]
-    readable_ids: Iterable[ConnectionId]
-    closed_ids: Iterable[ConnectionId]
```

### Comparing `msglib-0.1.0/msglib/message.py` & `msglib-0.2.0/msglib/message.py`

 * *Files identical despite different names*

### Comparing `msglib-0.1.0/pyproject.toml` & `msglib-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msglib"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["uigctaw <uigctaw@metadata.social>"]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
```


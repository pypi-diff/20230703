# Comparing `tmp/sockets-communication-1.1.1.tar.gz` & `tmp/sockets-communication-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.1.1.tar", last modified: Sat Jul  1 08:43:48 2023, max compression
+gzip compressed data, was "sockets-communication-1.1.2.tar", last modified: Mon Jul  3 14:36:19 2023, max compression
```

## Comparing `sockets-communication-1.1.1.tar` & `sockets-communication-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 08:43:48.279225 sockets-communication-1.1.1/
--rw-rw-rw-   0        0        0       98 2023-07-01 08:43:48.000000 sockets-communication-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-07-01 08:43:48.279225 sockets-communication-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.1.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.1.1/build.py
--rw-rw-rw-   0        0        0      708 2023-07-01 08:43:09.000000 sockets-communication-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 08:43:48.279225 sockets-communication-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-07-01 08:42:47.000000 sockets-communication-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:43:48.273224 sockets-communication-1.1.1/sockets_communication/
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.1.1/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.1.1/sockets_communication/process.py
--rw-rw-rw-   0        0        0     3613 2023-06-28 18:12:55.000000 sockets-communication-1.1.1/sockets_communication/service.py
--rw-rw-rw-   0        0        0    20170 2023-06-28 18:12:51.000000 sockets-communication-1.1.1/sockets_communication/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:43:48.278224 sockets-communication-1.1.1/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-07-01 08:43:48.000000 sockets-communication-1.1.1/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-07-01 08:43:48.000000 sockets-communication-1.1.1/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 08:43:48.000000 sockets-communication-1.1.1/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-01 08:43:48.000000 sockets-communication-1.1.1/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-01 08:43:48.000000 sockets-communication-1.1.1/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 14:36:19.015408 sockets-communication-1.1.2/
+-rw-rw-rw-   0        0        0       98 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-07-03 14:36:19.015408 sockets-communication-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.1.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.1.2/build.py
+-rw-rw-rw-   0        0        0      708 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.1.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:36:19.015408 sockets-communication-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-07-03 14:36:07.000000 sockets-communication-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:36:18.999371 sockets-communication-1.1.2/sockets_communication/
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.1.2/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.1.2/sockets_communication/process.py
+-rw-rw-rw-   0        0        0     3614 2023-07-03 14:35:41.000000 sockets-communication-1.1.2/sockets_communication/service.py
+-rw-rw-rw-   0        0        0    20172 2023-07-03 14:36:00.000000 sockets-communication-1.1.2/sockets_communication/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:36:19.014370 sockets-communication-1.1.2/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.1.1/PKG-INFO` & `sockets-communication-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.1.1
+Version: 1.1.2
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.1.1/README.md` & `sockets-communication-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.1/build.py` & `sockets-communication-1.1.2/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.1/pyproject.toml` & `sockets-communication-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.1.1'
+version = '1.1.2'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.1.1/setup.py` & `sockets-communication-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='1.1.1',
+        version='1.1.2',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.1.1/sockets_communication/exceptions.py` & `sockets-communication-1.1.2/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.1/sockets_communication/process.py` & `sockets-communication-1.1.2/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.1/sockets_communication/service.py` & `sockets-communication-1.1.2/sockets_communication/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import threading
 import warnings
 import time
 import datetime as dt
 from typing import Optional, Union
 
-from represent import BaseModel
+from represent import represent
 
 Number = Union[int, float]
 Host = str
 Port = Union[str, int]
 
 __all__ = [
     "ServiceInterface"
 ]
 
-class ServiceInterface(BaseModel):
+@represent
+class ServiceInterface:
     """The server object to control the communication ith multiple clients."""
 
     def __init__(self) -> None:
         """Defines the server datasets for clients and client commands."""
 
         self._timeout_process: Optional[threading.Thread] = None
```

### Comparing `sockets-communication-1.1.1/sockets_communication/sockets.py` & `sockets-communication-1.1.2/sockets_communication/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import threading
 from typing import (
     Optional, Union, Tuple, Dict, Any
 )
 
 from requests.models import PreparedRequest
 
-from represent import BaseModel
+from represent import represent
 
 from sockets_communication.process import decode
 from sockets_communication.service import ServiceInterface
 
 __all__ = [
     "Components",
     "Communication",
@@ -167,15 +167,16 @@
             # end if
         # end for
 
         return message
     # end receive
 # end Communication
 
-class SocketClient(Communication, BaseModel):
+@represent
+class SocketClient(Communication):
     """Creates the client to communicate with the server."""
 
     def __init__(self, connection: Socket) -> None:
         """
         Defines the server address and creates the client object.
 
         :param connection: The connection socket.
@@ -250,15 +251,16 @@
         :return: The received response from the server.
         """
 
         return self.receive(connection=self.connection)
     # end receive_message_from_server
 # end SocketClient
 
-class ClientsCollection(BaseModel):
+@represent
+class ClientsCollection:
     """A data class to contain clients within the server data."""
 
     def __init__(self, clients: Optional[dict] = None) -> None:
         """
         Defines the base data class to contain the clients.
 
         :param clients: The base dictionary to contain the clients' data.
```

### Comparing `sockets-communication-1.1.1/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.1.2/sockets_communication.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.1.1
+Version: 1.1.2
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


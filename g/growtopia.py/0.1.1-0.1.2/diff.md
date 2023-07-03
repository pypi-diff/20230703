# Comparing `tmp/growtopia.py-0.1.1.tar.gz` & `tmp/growtopia.py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growtopia.py-0.1.1.tar", last modified: Wed Apr 19 23:52:09 2023, max compression
+gzip compressed data, was "growtopia.py-0.1.2.tar", last modified: Mon Jul  3 10:02:50 2023, max compression
```

## Comparing `growtopia.py-0.1.1.tar` & `growtopia.py-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 23:52:09.725914 growtopia.py-0.1.1/
--rw-rw-rw-   0        0        0     1085 2023-03-21 19:55:14.000000 growtopia.py-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3453 2023-04-19 23:52:09.724408 growtopia.py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1654 2023-04-19 14:41:27.000000 growtopia.py-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 23:52:09.699811 growtopia.py-0.1.1/growtopia/
--rw-rw-rw-   0        0        0      304 2023-04-19 14:30:30.000000 growtopia.py-0.1.1/growtopia/__init__.py
--rw-rw-rw-   0        0        0     2437 2023-04-15 00:06:07.000000 growtopia.py-0.1.1/growtopia/client.py
--rw-rw-rw-   0        0        0      528 2023-04-03 20:17:13.000000 growtopia.py-0.1.1/growtopia/collection.py
--rw-rw-rw-   0        0        0     1151 2023-04-15 18:45:20.000000 growtopia.py-0.1.1/growtopia/constants.py
--rw-rw-rw-   0        0        0      762 2023-04-17 20:08:24.000000 growtopia.py-0.1.1/growtopia/context.py
--rw-rw-rw-   0        0        0      691 2023-04-10 16:04:21.000000 growtopia.py-0.1.1/growtopia/enums.py
--rw-rw-rw-   0        0        0      749 2023-03-22 20:29:18.000000 growtopia.py-0.1.1/growtopia/error_manager.py
--rw-rw-rw-   0        0        0     3071 2023-04-19 14:54:04.000000 growtopia.py-0.1.1/growtopia/event_pool.py
--rw-rw-rw-   0        0        0     2988 2023-03-22 20:26:32.000000 growtopia.py-0.1.1/growtopia/exceptions.py
--rw-rw-rw-   0        0        0     2188 2023-04-17 19:17:28.000000 growtopia.py-0.1.1/growtopia/item.py
--rw-rw-rw-   0        0        0     4000 2023-04-08 20:51:11.000000 growtopia.py-0.1.1/growtopia/items_data.py
--rw-rw-rw-   0        0        0      655 2023-04-03 20:16:17.000000 growtopia.py-0.1.1/growtopia/listener.py
--rw-rw-rw-   0        0        0      277 2023-04-08 23:41:15.000000 growtopia.py-0.1.1/growtopia/player.py
--rw-rw-rw-   0        0        0     1076 2023-04-17 19:31:25.000000 growtopia.py-0.1.1/growtopia/player_net_funcs.py
--rw-rw-rw-   0        0        0      696 2023-04-08 20:58:24.000000 growtopia.py-0.1.1/growtopia/player_pool.py
--rw-rw-rw-   0        0        0      694 2023-04-19 14:41:27.000000 growtopia.py-0.1.1/growtopia/player_tribute.py
-drwxrwxrwx   0        0        0        0 2023-04-19 23:52:09.718350 growtopia.py-0.1.1/growtopia/protocol/
--rw-rw-rw-   0        0        0       98 2023-04-19 14:42:36.000000 growtopia.py-0.1.1/growtopia/protocol/__init__.py
--rw-rw-rw-   0        0        0     1866 2023-03-27 17:03:12.000000 growtopia.py-0.1.1/growtopia/protocol/enums.py
--rw-rw-rw-   0        0        0     4240 2023-04-19 14:54:42.000000 growtopia.py-0.1.1/growtopia/protocol/game_packet.py
--rw-rw-rw-   0        0        0     2169 2023-04-19 14:43:27.000000 growtopia.py-0.1.1/growtopia/protocol/packet.py
--rw-rw-rw-   0        0        0     1781 2023-04-17 23:42:50.000000 growtopia.py-0.1.1/growtopia/protocol/variant.py
--rw-rw-rw-   0        0        0     1277 2023-04-17 23:40:53.000000 growtopia.py-0.1.1/growtopia/protocol/variant_list.py
--rw-rw-rw-   0        0        0     2792 2023-04-10 16:11:44.000000 growtopia.py-0.1.1/growtopia/server.py
-drwxrwxrwx   0        0        0        0 2023-04-19 23:52:09.722351 growtopia.py-0.1.1/growtopia/utils/
--rw-rw-rw-   0        0        0       73 2023-04-08 12:59:43.000000 growtopia.py-0.1.1/growtopia/utils/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-08 18:21:42.000000 growtopia.py-0.1.1/growtopia/utils/decipher.py
--rw-rw-rw-   0        0        0      197 2023-04-08 12:25:30.000000 growtopia.py-0.1.1/growtopia/utils/hash_.py
--rw-rw-rw-   0        0        0     1271 2023-04-17 20:06:57.000000 growtopia.py-0.1.1/growtopia/utils/id_packet.py
-drwxrwxrwx   0        0        0        0 2023-04-19 23:52:09.712305 growtopia.py-0.1.1/growtopia.py.egg-info/
--rw-rw-rw-   0        0        0     3453 2023-04-19 23:52:09.000000 growtopia.py-0.1.1/growtopia.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2023-04-19 23:52:09.000000 growtopia.py-0.1.1/growtopia.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 23:52:09.000000 growtopia.py-0.1.1/growtopia.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 23:52:09.000000 growtopia.py-0.1.1/growtopia.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      634 2023-04-19 23:51:47.000000 growtopia.py-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 23:52:09.725914 growtopia.py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      212 2023-04-19 15:09:55.000000 growtopia.py-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 23:52:09.724408 growtopia.py-0.1.1/tests/
--rw-rw-rw-   0        0        0     3085 2023-04-17 23:43:05.000000 growtopia.py-0.1.1/tests/test_packet.py
--rw-rw-rw-   0        0        0     1040 2023-04-15 18:50:25.000000 growtopia.py-0.1.1/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:02:50.654368 growtopia.py-0.1.2/
+-rw-rw-rw-   0        0        0     1085 2023-03-21 19:55:14.000000 growtopia.py-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4213 2023-07-03 10:02:50.654368 growtopia.py-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2310 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 10:02:50.633972 growtopia.py-0.1.2/growtopia/
+-rw-rw-rw-   0        0        0      372 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/client.py
+-rw-rw-rw-   0        0        0      915 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/collection.py
+-rw-rw-rw-   0        0        0     1151 2023-04-30 14:36:01.000000 growtopia.py-0.1.2/growtopia/constants.py
+-rw-rw-rw-   0        0        0     1245 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/context.py
+-rw-rw-rw-   0        0        0     4885 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/dialog.py
+-rw-rw-rw-   0        0        0     9365 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/dispatcher.py
+-rw-rw-rw-   0        0        0     1206 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/enums.py
+-rw-rw-rw-   0        0        0      848 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/error_manager.py
+-rw-rw-rw-   0        0        0     6383 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/exceptions.py
+-rw-rw-rw-   0        0        0     2535 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/file.py
+-rw-rw-rw-   0        0        0     2236 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/host.py
+-rw-rw-rw-   0        0        0     2229 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/item.py
+-rw-rw-rw-   0        0        0     8227 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/items_data.py
+-rw-rw-rw-   0        0        0     1326 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/listener.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:02:50.642577 growtopia.py-0.1.2/growtopia/player/
+-rw-rw-rw-   0        0        0       57 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/player/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/player/player.py
+-rw-rw-rw-   0        0        0      802 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/player/player_login_info.py
+-rw-rw-rw-   0        0        0     2386 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/player/player_net.py
+-rw-rw-rw-   0        0        0     1941 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/player_tribute.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:02:50.649684 growtopia.py-0.1.2/growtopia/protocol/
+-rw-rw-rw-   0        0        0      226 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/__init__.py
+-rw-rw-rw-   0        0        0     2270 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/enums.py
+-rw-rw-rw-   0        0        0     3784 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/game_message_packet.py
+-rw-rw-rw-   0        0        0     7265 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/game_update_packet.py
+-rw-rw-rw-   0        0        0     3029 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/hello_packet.py
+-rw-rw-rw-   0        0        0     3716 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/packet.py
+-rw-rw-rw-   0        0        0     3764 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/text_packet.py
+-rw-rw-rw-   0        0        0     1749 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/variant.py
+-rw-rw-rw-   0        0        0     1790 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/protocol/variant_list.py
+-rw-rw-rw-   0        0        0     7691 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/growtopia/server.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:02:50.639391 growtopia.py-0.1.2/growtopia.py.egg-info/
+-rw-rw-rw-   0        0        0     4213 2023-07-03 10:02:50.000000 growtopia.py-0.1.2/growtopia.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1108 2023-07-03 10:02:50.000000 growtopia.py-0.1.2/growtopia.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:02:50.000000 growtopia.py-0.1.2/growtopia.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 10:02:50.000000 growtopia.py-0.1.2/growtopia.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 10:02:50.000000 growtopia.py-0.1.2/growtopia.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      836 2023-07-03 10:01:28.000000 growtopia.py-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:02:50.654368 growtopia.py-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      195 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:02:50.652865 growtopia.py-0.1.2/tests/
+-rw-rw-rw-   0        0        0      626 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/tests/test_dialog.py
+-rw-rw-rw-   0        0        0     1217 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/tests/test_parser.py
+-rw-rw-rw-   0        0        0     3116 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/tests/test_protocol.py
+-rw-rw-rw-   0        0        0      477 2023-07-03 09:52:19.000000 growtopia.py-0.1.2/tests/test_server.py
```

### Comparing `growtopia.py-0.1.1/LICENSE` & `growtopia.py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `growtopia.py-0.1.1/PKG-INFO` & `growtopia.py-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growtopia.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple asynchronous API for Growtopia, capable of creating servers, clients, and more!
 License: MIT License
         
         Copyright (c) 2023 kaJob-dev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,47 +22,60 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/kaJob-dev/growtopia.py
 Project-URL: Bug Tracker, https://github.com/kaJob-dev/growtopia.py/issues
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # growtopia.py
 
 [![Discord server](https://discord.com/api/guilds/1009905646897999913/embed.png)](https://discord.gg/3RYSVwBCQC)
+[![PyPI version](https://img.shields.io/pypi/v/growtopia.py.svg?style=flat-square)](https://pypi.org/project/growtopia.py/)
+[![Python versions](https://img.shields.io/pypi/pyversions/growtopia.py.svg?style=flat-square)](https://pypi.org/project/growtopia.py/)
 
 A simple asynchronous API for Growtopia, capable of creating servers, clients, and more!
 
-Check out the [examples](examples) folder for examples on how to use this library.
-
 ## Installation
 
 ### Requirements
 
-- [Python 3.11 or above](https://www.python.org/downloads/)
+- [Python 3.9 or above](https://www.python.org/downloads/)
+- [PyENet](https://github.com/kajob-dev/pyenet) (If installing growtopia.py from PyPI)
 
 ### Installing from source
 
 1. Clone the repository.
 2. Open a terminal in the repository's directory
 3. Install it using pip.
 
 ```powershell
 git clone https://github.com/kaJob-dev/growtopia.py.git
 cd growtopia.py
 
 pip(3) install -U .
 ```
 
+### Installing from PyPI
+
+Please do note that installing growtopia.py from PyPI will require you to install [PyENet](https://github.com/kajob-dev/pyenet) yourself, as PyPI does not support direct dependencies. This'll be resolved in the future by simply having [PyENet](https://github.com/kajob-dev/pyenet) available in PyPI too.
+
+```powershell
+pip(3) install growtopia.py
+```
+
+---
+
 ## Contributing
 
 All contributions are welcome! If you'd like to contribute, please make a pull request.
 
 Please make sure that your code is formatted correctly before making a new pull request. This project is formatted using [black](https://black.readthedocs.io/en/stable/) and [isort](https://pycqa.github.io/isort/) to sort imports. Read through open and closed pull requests and ensure that no one else has already made a similar pull request.
 
 To install and format your code using black and isort, run the following commands:
```

### Comparing `growtopia.py-0.1.1/growtopia/constants.py` & `growtopia.py-0.1.2/growtopia/constants.py`

 * *Files identical despite different names*

### Comparing `growtopia.py-0.1.1/growtopia/error_manager.py` & `growtopia.py-0.1.2/growtopia/error_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 import traceback
 from typing import Callable, Optional
 
 
 class ErrorManager:
     callback: Optional[Callable] = None
+    catch_exceptions: bool = True
 
     @classmethod
     def set_callback(cls, callback: Callable) -> None:
         cls.callback = callback
 
     @classmethod
     def _raise_exception(cls, exception: Exception) -> None:
         if cls.callback is not None:
-            cls.callback(exception)
-        else:
-            # We catch the exception here to prevent the program from halting.
-            # Traceback is still printed out due to the print_exc() call.
+            return cls.callback(exception)
+
+        # We catch the exception here to prevent the program from halting.
+        # Traceback is still printed out due to the print_exc() call.
+        if cls.catch_exceptions:
             try:
                 raise exception
             except Exception:
                 traceback.print_exc()  # Print the traceback to the console
+        else:
+            raise exception
```

### Comparing `growtopia.py-0.1.1/growtopia/item.py` & `growtopia.py-0.1.2/growtopia/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __all__ = ("Item",)
 
 from typing import Any
 
 
+# TODO: Add docstring to the Item class
 class Item:
     def __init__(self) -> None:
         self.id: int = 4
 
         self.editable_type: int = 1
         self.category: int = 1
         self.action_type: int = 1
```

### Comparing `growtopia.py-0.1.1/growtopia/protocol/enums.py` & `growtopia.py-0.1.2/growtopia/protocol/enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 __all__ = (
     "PacketType",
     "VariantType",
-    "GamePacketFlags",
-    "GamePacketType",
+    "GameUpdatePacketFlags",
+    "GameUpdatePacketType",
 )
 
 from enum import IntEnum
 
 
 class PacketType(IntEnum):
+    """
+    An integer enumeration of all packet types.
+    """
+
     UNKNOWN = 0
     HELLO = 1
     TEXT = 2
     GAME_MESSAGE = 3
-    GAME_PACKET = 4
+    GAME_UPDATE = 4
 
     @classmethod
-    def _missing_(cls, _):
-        return cls.UNKNOWN
+    def _missing_(cls, _: int) -> "PacketType":
+        return cls(0)
 
 
 class VariantType(IntEnum):
+    """
+    An integer enumeration of all variant types.
+    """
+
     NONE = 0
     FLOAT = 1
     STR = 2
     VECTOR2 = 3
     VECTOR3 = 4
     UINT = 8
     INT = 9
 
+    # Custom variant type aliases.
+    DIALOG = 2  # str
+
     @classmethod
     def _missing_(cls, _):
         return cls.NONE
 
 
-class GamePacketFlags(IntEnum):
+class GameUpdatePacketFlags(IntEnum):
+    """
+    An integer enumeration of all game update packet flags.
+    """
+
     UNKNOWN = -1
     EXTRA_DATA = 8
 
     @classmethod
     def _missing_(cls, _):
         return cls.UNKNOWN
 
 
-class GamePacketType(IntEnum):
-    UNKNOWN = -1
+class GameUpdatePacketType(IntEnum):
+    """
+    An integer enumeration of all game update packet types.
+    """
+
+    UNKNOWN = 99
+
     STATE = 0
     CALL_FUNCTION = 1
     UPDATE_STATUS = 2
     TILE_CHANGE_REQUEST = 3
     SEND_MAP_DATA = 4
     SEND_TILE_UPDATE_DATA = 5
     SEND_TILE_UPDATE_DATA_MULTIPLE = 6
```

### Comparing `growtopia.py-0.1.1/growtopia/protocol/variant.py` & `growtopia.py-0.1.2/growtopia/protocol/variant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 __all__ = ("Variant",)
 
 import struct
-from typing import Any
+from typing import Union
 
 from .enums import VariantType
 
 
 class Variant:
     _serialisers = {
-        VariantType.INT: lambda data: bytearray(data.to_bytes(4, "little")),
-        VariantType.UINT: lambda data: bytearray(
-            data.to_bytes(4, "little", signed=True)
-        ),
+        VariantType.INT: lambda data: bytearray(data.to_bytes(4, "little"), signed=True),
+        VariantType.UINT: lambda data: bytearray(data.to_bytes(4, "little")),
         VariantType.FLOAT: lambda data: bytearray(struct.pack("f", data)),
-        VariantType.STR: lambda data: bytearray(
-            len(data).to_bytes(4, "little") + data.encode()
-        ),
+        VariantType.STR: lambda data: bytearray(len(data).to_bytes(4, "little") + data.encode()),
         VariantType.NONE: lambda _: bytearray(),
     }
 
     _deserialisers = {
-        VariantType.INT: lambda data: int.from_bytes(data[:4], "little"),
-        VariantType.UINT: lambda data: int.from_bytes(data[:4], "little", signed=True),
+        VariantType.INT: lambda data: int.from_bytes(data[:4], "little", signed=True),
+        VariantType.UINT: lambda data: int.from_bytes(data[:4], "little"),
         VariantType.FLOAT: lambda data: struct.unpack("f", data[:4])[0],
-        VariantType.STR: lambda data: data[
-            4 : int.from_bytes(data[:4], "little") + 4
-        ].decode(),
+        VariantType.STR: lambda data: data[4 : int.from_bytes(data[:4], "little") + 4].decode(),
         VariantType.NONE: lambda _: None,
     }
 
-    def __init__(self, value: Any, type_: VariantType = None) -> None:
+    def __init__(self, value: Union[str, int, float], type_: VariantType = None) -> None:
         self.type: VariantType = type_ or VariantType[type(value).__name__.upper()]
-        self.value: Any = value
+        self.value: Union[str, int, float] = value
         self.data: bytearray = bytearray()
 
     def serialise(self, index: int) -> bytearray:
         self.data = bytearray(
             index.to_bytes(1, "little")
             + self.type.value.to_bytes(1, "little")
             + self._serialisers[self.type](self.value)
```

### Comparing `growtopia.py-0.1.1/growtopia.py.egg-info/PKG-INFO` & `growtopia.py-0.1.2/growtopia.py.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growtopia.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple asynchronous API for Growtopia, capable of creating servers, clients, and more!
 License: MIT License
         
         Copyright (c) 2023 kaJob-dev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,47 +22,60 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/kaJob-dev/growtopia.py
 Project-URL: Bug Tracker, https://github.com/kaJob-dev/growtopia.py/issues
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # growtopia.py
 
 [![Discord server](https://discord.com/api/guilds/1009905646897999913/embed.png)](https://discord.gg/3RYSVwBCQC)
+[![PyPI version](https://img.shields.io/pypi/v/growtopia.py.svg?style=flat-square)](https://pypi.org/project/growtopia.py/)
+[![Python versions](https://img.shields.io/pypi/pyversions/growtopia.py.svg?style=flat-square)](https://pypi.org/project/growtopia.py/)
 
 A simple asynchronous API for Growtopia, capable of creating servers, clients, and more!
 
-Check out the [examples](examples) folder for examples on how to use this library.
-
 ## Installation
 
 ### Requirements
 
-- [Python 3.11 or above](https://www.python.org/downloads/)
+- [Python 3.9 or above](https://www.python.org/downloads/)
+- [PyENet](https://github.com/kajob-dev/pyenet) (If installing growtopia.py from PyPI)
 
 ### Installing from source
 
 1. Clone the repository.
 2. Open a terminal in the repository's directory
 3. Install it using pip.
 
 ```powershell
 git clone https://github.com/kaJob-dev/growtopia.py.git
 cd growtopia.py
 
 pip(3) install -U .
 ```
 
+### Installing from PyPI
+
+Please do note that installing growtopia.py from PyPI will require you to install [PyENet](https://github.com/kajob-dev/pyenet) yourself, as PyPI does not support direct dependencies. This'll be resolved in the future by simply having [PyENet](https://github.com/kajob-dev/pyenet) available in PyPI too.
+
+```powershell
+pip(3) install growtopia.py
+```
+
+---
+
 ## Contributing
 
 All contributions are welcome! If you'd like to contribute, please make a pull request.
 
 Please make sure that your code is formatted correctly before making a new pull request. This project is formatted using [black](https://black.readthedocs.io/en/stable/) and [isort](https://pycqa.github.io/isort/) to sort imports. Read through open and closed pull requests and ensure that no one else has already made a similar pull request.
 
 To install and format your code using black and isort, run the following commands:
```

### Comparing `growtopia.py-0.1.1/growtopia.py.egg-info/SOURCES.txt` & `growtopia.py-0.1.2/growtopia.py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,41 @@
 pyproject.toml
 setup.py
 growtopia/__init__.py
 growtopia/client.py
 growtopia/collection.py
 growtopia/constants.py
 growtopia/context.py
+growtopia/dialog.py
+growtopia/dispatcher.py
 growtopia/enums.py
 growtopia/error_manager.py
-growtopia/event_pool.py
 growtopia/exceptions.py
+growtopia/file.py
+growtopia/host.py
 growtopia/item.py
 growtopia/items_data.py
 growtopia/listener.py
-growtopia/player.py
-growtopia/player_net_funcs.py
-growtopia/player_pool.py
 growtopia/player_tribute.py
 growtopia/server.py
 growtopia.py.egg-info/PKG-INFO
 growtopia.py.egg-info/SOURCES.txt
 growtopia.py.egg-info/dependency_links.txt
+growtopia.py.egg-info/requires.txt
 growtopia.py.egg-info/top_level.txt
+growtopia/player/__init__.py
+growtopia/player/player.py
+growtopia/player/player_login_info.py
+growtopia/player/player_net.py
 growtopia/protocol/__init__.py
 growtopia/protocol/enums.py
-growtopia/protocol/game_packet.py
+growtopia/protocol/game_message_packet.py
+growtopia/protocol/game_update_packet.py
+growtopia/protocol/hello_packet.py
 growtopia/protocol/packet.py
+growtopia/protocol/text_packet.py
 growtopia/protocol/variant.py
 growtopia/protocol/variant_list.py
-growtopia/utils/__init__.py
-growtopia/utils/decipher.py
-growtopia/utils/hash_.py
-growtopia/utils/id_packet.py
-tests/test_packet.py
-tests/test_parser.py
+tests/test_dialog.py
+tests/test_parser.py
+tests/test_protocol.py
+tests/test_server.py
```

### Comparing `growtopia.py-0.1.1/pyproject.toml` & `growtopia.py-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,29 @@
 [project]
 name = "growtopia.py"
 description = "A simple asynchronous API for Growtopia, capable of creating servers, clients, and more!"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+version = "0.1.2"
+requires-python = ">=3.9.0"
 
-version = "0.1.1"
-requires-python = ">=3.11"
+dependencies = [
+    "aiofiles",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/kaJob-dev/growtopia.py"
-"Bug Tracker" = "https://github.com/kaJob-dev/growtopia.py/issues"
+"Bug Tracker" = "https://github.com/kaJob-dev/growtopia.py/issues"
+
+[tool.black]
+line-length = 120
+
+[tool.isort]
+profile = "black"
```

### Comparing `growtopia.py-0.1.1/tests/test_parser.py` & `growtopia.py-0.1.2/tests/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Test the items.dat and player_tribute.dat file parsers."""
 
+import asyncio
 import os
 
 from growtopia import ItemsData, PlayerTribute
 
 
 def test_parser() -> None:
     """Test the parser."""
 
     for file in os.listdir("tests/data"):
         if file.startswith("items") and file.endswith(".dat"):
             items_data = ItemsData(f"tests/data/{file}")
-
-            items_data.parse()
+            asyncio.run(items_data.parse())
 
             assert items_data.get_item(item_id=2).name.lower() == "dirt"
             assert items_data.get_item(item_id=3).name.lower() == "dirt seed"
             assert items_data.get_item(name="blank").id == 0
             assert items_data.get_item(name="blue gem lock").id == 7188
 
             assert items_data.get_starts_with("dirt")[0].name.lower() == "dirt"
             assert items_data.get_ends_with("dirt seed")[0].id == 3
             assert len(items_data.get_contains("dirt")) > 0
 
-    player_tribute = PlayerTribute("tests/data/player_tribute.dat")
-    player_tribute.parse()
+        if file.startswith("player_tribute") and file.endswith(".dat"):
+            player_tribute = PlayerTribute(f"tests/data/{file}")
+            asyncio.run(player_tribute.parse())
+
+            assert len(player_tribute.epic_players) > 0
 
 
 if __name__ == "__main__":
     test_parser()
```


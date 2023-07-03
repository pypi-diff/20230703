# Comparing `tmp/upstash_redis-0.13.3.tar.gz` & `tmp/upstash_redis-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.13.3.tar", max compression
+gzip compressed data, was "upstash_redis-0.14.0.tar", max compression
```

## Comparing `upstash_redis-0.13.3.tar` & `upstash_redis-0.14.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-07-02 19:15:43.024048 upstash_redis-0.13.3/LICENSE
--rw-r--r--   0        0        0     9173 2023-07-02 19:15:43.024048 upstash_redis-0.13.3/README.md
--rw-r--r--   0        0        0      500 2023-07-02 19:15:43.024048 upstash_redis-0.13.3/pyproject.toml
--rw-r--r--   0        0        0      150 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4782 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     5052 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/client.py
--rw-r--r--   0        0        0       82 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       78 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    22111 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71548 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    21221 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     5478 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      738 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      752 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      172 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     9368 2023-07-02 19:15:43.028048 upstash_redis-0.13.3/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.13.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-03 03:59:36.165204 upstash_redis-0.14.0/LICENSE
+-rw-r--r--   0        0        0     9173 2023-07-03 03:59:36.165204 upstash_redis-0.14.0/README.md
+-rw-r--r--   0        0        0      500 2023-07-03 03:59:36.165204 upstash_redis-0.14.0/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4896 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     5116 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/client.py
+-rw-r--r--   0        0        0       77 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    21043 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    72037 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    20142 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     5601 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      752 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      174 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     9521 2023-07-03 03:59:36.173204 upstash_redis-0.14.0/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.14.0/PKG-INFO
```

### Comparing `upstash_redis-0.13.3/LICENSE` & `upstash_redis-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.3/README.md` & `upstash_redis-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.3/upstash_redis/asyncio/client.py` & `upstash_redis-0.14.0/upstash_redis/asyncio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from os import environ
 from typing import Any, List, Type, Union
 
 from aiohttp import ClientSession
 from upstash_redis.commands.async_commands import AsyncCommands
-from upstash_redis.config import REST_ENCODING, REST_RETRIES, REST_RETRY_INTERVAL, FORMAT_RETURN, ALLOW_TELEMETRY
+from upstash_redis.config import (
+    REST_ENCODING,
+    REST_RETRIES,
+    REST_RETRY_INTERVAL,
+    FORMAT_RETURN,
+    ALLOW_TELEMETRY,
+)
 from upstash_redis.http.execute import async_execute
 
 from upstash_redis.schema.http import RESTEncoding, RESTResult
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.utils.format import FormattedResponse
 
 
 class Redis(FormattedResponse, AsyncCommands):
-    
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
@@ -44,16 +49,14 @@
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
         self.telemetry_data = telemetry_data
         self.FORMATTERS = self.__class__.FORMATTERS
 
-
-
     @classmethod
     def from_env(
         cls,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         format_return: bool = FORMAT_RETURN,
@@ -119,13 +122,20 @@
             telemetry_data=self.telemetry_data,
         )
 
         main_command = command[0]
         if len(command) > 1 and (main_command == "PUBSUB" or main_command == "SCRIPT"):
             main_command = f"{main_command} {command[1]}"
 
-        if (self.format_return or main_command == "HSCAN" or main_command == "SMEMBERS" or main_command == "SDIFF" or main_command == "SINTER" or main_command == "SSCAN" or main_command == "SUNION" or main_command == "ZSCAN") and (main_command in self.FORMATTERS):
+        if (
+            self.format_return
+            or main_command == "HSCAN"
+            or main_command == "SMEMBERS"
+            or main_command == "SDIFF"
+            or main_command == "SINTER"
+            or main_command == "SSCAN"
+            or main_command == "SUNION"
+            or main_command == "ZSCAN"
+        ) and (main_command in self.FORMATTERS):
             return self.FORMATTERS[main_command](res, command)
 
         return res
-        
-
```

### Comparing `upstash_redis-0.13.3/upstash_redis/client.py` & `upstash_redis-0.14.0/upstash_redis/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from os import environ
 from typing import Any, List, Type, Union
 
 from aiohttp import ClientSession
 from upstash_redis.commands.commands import Commands
-from upstash_redis.config import REST_ENCODING, REST_RETRIES, REST_RETRY_INTERVAL, FORMAT_RETURN, ALLOW_TELEMETRY
+from upstash_redis.config import (
+    REST_ENCODING,
+    REST_RETRIES,
+    REST_RETRY_INTERVAL,
+    FORMAT_RETURN,
+    ALLOW_TELEMETRY,
+)
 from upstash_redis.http.execute import sync_execute
 
 from upstash_redis.schema.http import RESTEncoding, RESTResult
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.utils.format import FormattedResponse
 from requests import Session
 
+
 class Redis(FormattedResponse, Commands):
-    
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
@@ -46,25 +52,24 @@
         self.rest_retry_interval = rest_retry_interval
 
         self.telemetry_data = telemetry_data
         self.FORMATTERS = self.__class__.FORMATTERS
 
         self._session = Session()
 
-
     def __enter__(self):
         """
         Enter the sync context.
         """
         if self._session is None:
             self._session = Session()
 
         # It needs to return the session object because it will be used in "sync with" statements.
         return self
-    
+
     def __exit__(
         self,
         exc_type: Union[Type[BaseException], None],
         exc_val: Union[BaseException, None],
         exc_tb: Any,
     ) -> None:
         """
@@ -99,44 +104,52 @@
             rest_encoding,
             rest_retries,
             rest_retry_interval,
             format_return,
             allow_telemetry,
             telemetry_data,
         )
-    
+
     def close(self):
         """
         Closes the session.
         """
         if self._session:
             self._session.close()
 
     def run(self, command: List) -> RESTResult:
         """
         Specify the http options and execute the command.
         """
 
         res = sync_execute(
-                    session = self._session,
-                    url=self.url,
-                    token=self.token,
-                    encoding=self.rest_encoding,
-                    retries=self.rest_retries,
-                    retry_interval=self.rest_retry_interval,
-                    command=command,
-                    allow_telemetry=self.allow_telemetry,
-                    telemetry_data=self.telemetry_data,
+            session=self._session,
+            url=self.url,
+            token=self.token,
+            encoding=self.rest_encoding,
+            retries=self.rest_retries,
+            retry_interval=self.rest_retry_interval,
+            command=command,
+            allow_telemetry=self.allow_telemetry,
+            telemetry_data=self.telemetry_data,
         )
 
         main_command = command[0]
-        if len(command) > 1 and (main_command == "PUBSUB"):
+        if len(command) > 1 and (main_command == "PUBSUB" or main_command == "SCRIPT"):
             main_command = f"{main_command} {command[1]}"
 
-        if (self.format_return or main_command == "HSCAN" or main_command == "SMEMBERS" or main_command == "SDIFF" or main_command == "SINTER" or main_command == "SSCAN" or main_command == "SUNION" or main_command == "ZSCAN") and (main_command in self.FORMATTERS):
+        if (
+            self.format_return
+            or main_command == "HSCAN"
+            or main_command == "SMEMBERS"
+            or main_command == "SDIFF"
+            or main_command == "SINTER"
+            or main_command == "SSCAN"
+            or main_command == "SUNION"
+            or main_command == "ZSCAN"
+        ) and (main_command in self.FORMATTERS):
             return self.FORMATTERS[main_command](res, command)
 
         return res
-        
 
 
-# TODO: get platform from env variable for telemetry
+# TODO: get platform from env variable for telemetry
```

### Comparing `upstash_redis-0.13.3/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.14.0/upstash_redis/commands/async_commands.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,87 @@
-
-from upstash_redis.schema.commands.returns import (
-    GeoMembersReturn,
-    FormattedGeoMembersReturn,
-)
-
 from upstash_redis.schema.commands.parameters import (
     BitFieldOffset,
     GeoMember,
     FloatMinMax,
 )
 
 from typing import Any, Iterable, Optional, Set, Tuple, Union, List, Literal, Dict
 
 class AsyncCommands:
-    def __init__(self):
-        ...
-
+    def __init__(self): ...
     async def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
-    ) -> int: 
-        ...
-
-    def bitfield(self, key: str) -> "BitFieldCommands":
-        ...
-
-    def bitfield_ro(self, key: str) -> "BitFieldRO":
-        ...
-
+    ) -> int: ...
+    def bitfield(self, key: str) -> "BitFieldCommands": ...
+    def bitfield_ro(self, key: str) -> "BitFieldRO": ...
     async def bitop(
         self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *srckeys: str
-    ) -> int:
-        ...
-
+    ) -> int: ...
     async def bitpos(
         self,
         key: str,
         bit: Literal[0, 1],
         start: Union[int, None] = None,
         end: Union[int, None] = None,
-    ) -> int:
-        ...
-
-    async def getbit(self, key: str, offset: int) -> int:
-        ...
-
-    async def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int:
-        ...
-
-    async def ping(self, message: Union[str, None] = None) -> str:
-        ...
-
-    async def echo(self, message: str) -> str:
-        ...
-    
+    ) -> int: ...
+    async def getbit(self, key: str, offset: int) -> int: ...
+    async def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int: ...
+    async def ping(self, message: Union[str, None] = None) -> str: ...
+    async def echo(self, message: str) -> str: ...
     async def copy(
         self, source: str, destination: str, replace: bool = False
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def delete(self, *keys: str) -> int:
-        ...
-
-    async def exists(self, *keys: str) -> int:
-        ...
-
-    async def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    async def delete(self, *keys: str) -> int: ...
+    async def exists(self, *keys: str) -> int: ...
+    async def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]: ...
     async def expireat(
         self, key: str, unix_time_seconds: int
-    ) -> Union[Literal[1, 0], bool]:
-       ...
-
-    async def keys(self, pattern: str) -> List[str]:
-        ...
-
-    async def persist(self, key: str) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def pexpire(self, key: str, milliseconds: int) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    async def keys(self, pattern: str) -> List[str]: ...
+    async def persist(self, key: str) -> Union[Literal[1, 0], bool]: ...
+    async def pexpire(
+        self, key: str, milliseconds: int
+    ) -> Union[Literal[1, 0], bool]: ...
     async def pexpireat(
         self, key: str, unix_time_milliseconds: int
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def pttl(self, key: str) -> int:
-        ...
-
-    async def randomkey(self) -> Union[str, None]:
-        ...
-
-    async def rename(self, key: str, newkey: str) -> str:
-        ...
-
-    async def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    async def pttl(self, key: str) -> int: ...
+    async def randomkey(self) -> Union[str, None]: ...
+    async def rename(self, key: str, newkey: str) -> str: ...
+    async def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]: ...
     async def scan(
         self,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         scan_type: Union[str, None] = None,
-    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]:
-        ...
-    
-    async def touch(self, *keys: str) -> int:
-        ...
-
-    async def ttl(self, key: str) -> int:
-        ...
-
-    async def type(self, key: str) -> Union[str, None]:
-        ...
-
-    async def unlink(self, *keys: str) -> int:
-        ...
-
+    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]: ...
+    async def touch(self, *keys: str) -> int: ...
+    async def ttl(self, key: str) -> int: ...
+    async def type(self, key: str) -> Union[str, None]: ...
+    async def unlink(self, *keys: str) -> int: ...
     async def geoadd(
         self,
         key: str,
         *members: GeoMember,
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
-    ) -> int:
-        ...
-
+    ) -> int: ...
     async def geodist(
         self,
         key: str,
         member1: str,
         member2: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M",
-    ) -> Union[str, float, None]:
-        ...
-
-    async def geohash(self, key: str, *members: str) -> List[Union[str, None]]:
-        ...
-
+    ) -> Union[str, float, None]: ...
+    async def geohash(self, key: str, *members: str) -> List[Union[str, None]]: ...
     async def geopos(
         self, key: str, *members: str
-    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]:
-        ...
-
+    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]: ...
     async def georadius(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
@@ -157,65 +89,71 @@
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn, int]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+        int,
+    ]: ...
     async def georadius_ro(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+    ]: ...
     async def georadiusbymember(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+        int,
+    ]: ...
     async def georadiusbymember_ro(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+    ]: ...
     async def geosearch(
         self,
         key: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         frommember: Union[str, None] = None,
         fromlonlat_longitude: Union[float, None] = None,
         fromlonlat_latitude: Union[float, None] = None,
@@ -224,17 +162,18 @@
         bybox_height: Union[float, None] = None,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
         count_any: bool = False,
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+    ]: ...
     async def geosearchstore(
         self,
         destination: str,
         source: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         frommember: Union[str, None] = None,
         fromlonlat_longitude: Union[float, None] = None,
@@ -242,582 +181,350 @@
         byradius: Union[float, None] = None,
         bybox_width: Union[float, None] = None,
         bybox_height: Union[float, None] = None,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
         count_any: bool = False,
         storedist: bool = False,
-    ) -> int:
-        ...
-
-    async def hdel(self, key: str, *fields: str) -> int:
-        ...
-
-    async def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def hget(self, key: str, field: str) -> Union[str, None]:
-        ...
-
-    async def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]:
-        ...
-
-    async def hincrby(self, key: str, field: str, increment: int) -> int:
-        ...
-
+    ) -> int: ...
+    async def hdel(self, key: str, *fields: str) -> int: ...
+    async def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]: ...
+    async def hget(self, key: str, field: str) -> Union[str, None]: ...
+    async def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]: ...
+    async def hincrby(self, key: str, field: str, increment: int) -> int: ...
     async def hincrbyfloat(
         self, key: str, field: str, increment: float
-    ) -> Union[str, float]:
-        ...
-
-    async def hkeys(self, key: str) -> List[str]:
-        ...
-
-    async def hlen(self, key: str) -> int:
-        ...
-
-    async def hmget(self, key: str, *fields: str) -> List[Union[str, None]]:
-        ...
-
-    async def hmset(self, key: str, field_value_pairs: Dict) -> str:
-        ...
-
+    ) -> Union[str, float]: ...
+    async def hkeys(self, key: str) -> List[str]: ...
+    async def hlen(self, key: str) -> int: ...
+    async def hmget(self, key: str, *fields: str) -> List[Union[str, None]]: ...
+    async def hmset(self, key: str, field_value_pairs: Dict) -> str: ...
     async def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
-    ):
-        ...
-
+    ): ...
     async def hscan(
         self,
         name: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Tuple[int, Dict[str, str]]:
-        ...
-
-    async def hset(self, name: str, key: Optional[str] = None, val: Optional[str] = None, field_value_pairs: Optional[Dict] = None) -> int:
-        ...
-
+    ) -> Tuple[int, Dict[str, str]]: ...
+    async def hset(
+        self,
+        name: str,
+        key: Optional[str] = None,
+        val: Optional[str] = None,
+        field_value_pairs: Optional[Dict] = None,
+    ) -> int: ...
     async def hsetnx(
         self, key: str, field: str, value: Any
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def hstrlen(self, key: str, field: str) -> int:
-        ...
-
-    async def hvals(self, key: str) -> List[str]:
-        ...
-
-    async def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def pfcount(self, *keys: str) -> int:
-        ...
-
-    async def pfmerge(self, destkey: str, *sourcekeys: str) -> str:
-        ...
-
-    async def lindex(self, key: str, index: int) -> Union[str, None]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    async def hstrlen(self, key: str, field: str) -> int: ...
+    async def hvals(self, key: str) -> List[str]: ...
+    async def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]: ...
+    async def pfcount(self, *keys: str) -> int: ...
+    async def pfmerge(self, destkey: str, *sourcekeys: str) -> str: ...
+    async def lindex(self, key: str, index: int) -> Union[str, None]: ...
     async def linsert(
-        self, key: str, position: Literal["BEFORE", "AFTER", "before", "after"], pivot: Any, element: Any
-    ) -> int:
-       ...
-
-    async def llen(self, key: str) -> int:
-        ...
-
+        self,
+        key: str,
+        position: Literal["BEFORE", "AFTER", "before", "after"],
+        pivot: Any,
+        element: Any,
+    ) -> int: ...
+    async def llen(self, key: str) -> int: ...
     async def lmove(
         self,
         source: str,
         destination: str,
         source_position: Literal["LEFT", "RIGHT"] = "LEFT",
         destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
-    ) -> Union[str, None]:
-        ...
-
+    ) -> Union[str, None]: ...
     async def lpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
     async def lpos(
         self,
         key: str,
         element: Any,
         rank: Union[int, None] = None,
         count: Union[int, None] = None,
         maxlen: Union[int, None] = None,
-    ) -> Union[(Union[int, None]), List[int]]:
-        ...
-
-    async def lpush(self, key: str, *elements: Any) -> int:
-        ...
-
-    async def lpushx(self, key: str, *elements: Any) -> int:
-        ...
-
-    async def lrange(self, key: str, start: int, stop: int) -> List[str]:
-        ...
-
-    async def lrem(self, key: str, count: int, element: Any) -> int:
-        ...
-
-    async def lset(self, key: str, index: int, element: Any) -> str:
-        ...
-
-    async def ltrim(self, key: str, start: int, stop: int) -> str:
-        ...
-
+    ) -> Union[(Union[int, None]), List[int]]: ...
+    async def lpush(self, key: str, *elements: Any) -> int: ...
+    async def lpushx(self, key: str, *elements: Any) -> int: ...
+    async def lrange(self, key: str, start: int, stop: int) -> List[str]: ...
+    async def lrem(self, key: str, count: int, element: Any) -> int: ...
+    async def lset(self, key: str, index: int, element: Any) -> str: ...
+    async def ltrim(self, key: str, start: int, stop: int) -> str: ...
     async def rpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
-    async def rpoplpush(self, source: str, destination: str) -> Union[str, None]:
-        ...
-
-    async def rpush(self, key: str, *elements: Any) -> int:
-        ...
-
-    async def rpushx(self, key: str, *elements: Any) -> int:
-        ...
-
-    async def publish(self, channel: str, message: str) -> int:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
+    async def rpoplpush(self, source: str, destination: str) -> Union[str, None]: ...
+    async def rpush(self, key: str, *elements: Any) -> int: ...
+    async def rpushx(self, key: str, *elements: Any) -> int: ...
+    async def publish(self, channel: str, message: str) -> int: ...
     async def eval(
         self,
         script: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
-    ) -> Any:
-        ...
-
+    ) -> Any: ...
     async def evalsha(
         self,
         sha1: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
-    ) -> Any:
-        ...
-
-    async def dbsize(self) -> int:
-        ...
-
-    async def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
-        ...
-
-    async def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
-        ...
-
-    async def time(self) -> Union[List[str], Dict[str, int]]:
-        ...
-
-    async def sadd(self, key: str, *members: Any) -> int:
-        ...
-
-    async def scard(self, key: str) -> int:
-        ...
-
-    async def sdiff(self, *keys: str) -> Set[str]:
-        ...
-
-    async def sdiffstore(self, destination: str, *keys: str) -> int:
-        ...
-
-    async def sinter(self, *keys: str) -> Set[str]:
-        ...
-
-    async def sinterstore(self, destination: str, *keys: str) -> int:
-        ...
-
-    async def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]:
-        ...
-
-    async def smembers(self, key: str) -> Set[str]:
-        ...
-
+    ) -> Any: ...
+    async def dbsize(self) -> int: ...
+    async def flushall(
+        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> Union[str, bool]: ...
+    async def flushdb(
+        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> Union[str, bool]: ...
+    async def time(self) -> Union[List[str], Dict[str, int]]: ...
+    async def sadd(self, key: str, *members: Any) -> int: ...
+    async def scard(self, key: str) -> int: ...
+    async def sdiff(self, *keys: str) -> Set[str]: ...
+    async def sdiffstore(self, destination: str, *keys: str) -> int: ...
+    async def sinter(self, *keys: str) -> Set[str]: ...
+    async def sinterstore(self, destination: str, *keys: str) -> int: ...
+    async def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]: ...
+    async def smismember(
+        self, key: str, *members: Any
+    ) -> Union[List[Literal[1, 0]], List[bool]]: ...
+    async def smembers(self, key: str) -> Set[str]: ...
     async def smove(
         self, source: str, destination: str, member: Any
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
     async def spop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
     async def srandmember(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
-    async def srem(self, key: str, *members: Any) -> int:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
+    async def srem(self, key: str, *members: Any) -> int: ...
     async def sscan(
         self,
         key: str,
         cursor: int = 0,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Tuple[int, List[str]]:
-        ...
-
-    async def sunion(self, *keys: str) -> Set[str]:
-        ...
-
-    async def sunionstore(self, destination: str, *keys: str) -> int:
-        ...
-
+    ) -> Tuple[int, List[str]]: ...
+    async def sunion(self, *keys: str) -> Set[str]: ...
+    async def sunionstore(self, destination: str, *keys: str) -> int: ...
     async def zadd(
         self,
         key: str,
         score_member_pairs: Dict,
         nx: bool = False,
         xx: bool = False,
         gt: bool = False,
         lt: bool = False,
         ch: bool = False,
         incr: bool = False,
-    ) -> Union[int, (Union[str, None, float])]:
-        ...
-    
-    async def zcard(self, key: str) -> int:
-        ...
-
+    ) -> Union[int, (Union[str, None, float])]: ...
+    async def zcard(self, key: str) -> int: ...
     async def zcount(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> int:
-        ...
-
+    ) -> int: ...
     def zdiff(
         self, keys: List[str], withscores: bool = False
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
-    async def zdiffstore(self, destination: str, keys: List[str]) -> int:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    async def zdiffstore(self, destination: str, keys: List[str]) -> int: ...
     async def zincrby(
         self, key: str, increment: float, member: str
-    ) -> Union[str, float]:
-        ...
-
+    ) -> Union[str, float]: ...
     async def zinter(
         self,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zinterstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
-    ) -> int:
-        ...
-
-    async def zlexcount(self, key: str, min_score: str, max_score: str) -> int:
-        ...
-
+    ) -> int: ...
+    async def zlexcount(self, key: str, min_score: str, max_score: str) -> int: ...
     async def zmscore(
         self, key: str, members: List[str]
-    ) -> Union[List[Union[str, None]], List[Union[float, None]]]:
-        ...
-
+    ) -> Union[List[Union[str, None]], List[Union[float, None]]]: ...
     async def zpopmax(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zpopmin(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrandmember(
         self, key: str, count: Union[int, None] = None, withscores: bool = False
-    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]:
-        ...
-
+    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]: ...
     async def zrange(
         self,
         key: str,
         start: FloatMinMax,
         stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
         withscores: bool = False,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrangebylex(
         self,
         key: str,
         min_score: str,
         max_score: str,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> List[Union[str, None]]:
-        ...
-
+    ) -> List[Union[str, None]]: ...
     async def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
         withscores: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrangestore(
         self,
         dst: str,
         src: str,
         start: FloatMinMax,
         stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> int:
-        ...
-
-    async def zrank(self, key: str, member: str) -> Union[int, None]:
-        ...
-
-    async def zrem(self, key: str, *members: str) -> int:
-        ...
-
-    async def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int:
-        ...
-
-    async def zremrangebyrank(self, key: str, start: int, stop: int) -> int:
-        ...
-
+    ) -> int: ...
+    async def zrank(self, key: str, member: str) -> Union[int, None]: ...
+    async def zrem(self, key: str, *members: str) -> int: ...
+    async def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int: ...
+    async def zremrangebyrank(self, key: str, start: int, stop: int) -> int: ...
     async def zremrangebyscore(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> int:
-        ...
-
+    ) -> int: ...
     async def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> List[str]:
-        ...
-
+    ) -> List[str]: ...
     async def zrevrangebyscore(
         self,
         key: str,
         max_score: FloatMinMax,
         min_score: FloatMinMax,
         withscores: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
-    async def zrevrank(self, key: str, member: str) -> Union[int, None]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    async def zrevrank(self, key: str, member: str) -> Union[int, None]: ...
     async def zscan(
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Tuple[int, List[Tuple[str, float]]]:
-        ...
-
-    async def zscore(self, key: str, member: str) -> Union[str, None, float]:
-        ...
-
+    ) -> Tuple[int, List[Tuple[str, float]]]: ...
+    async def zscore(self, key: str, member: str) -> Union[str, None, float]: ...
     def zunion(
         self,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zunionstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
-    ) -> int:
-        ...
-
-    async def append(self, key: str, value: Any) -> int:
-        ...
-
-    async def decr(self, key: str) -> int:
-        ...
-
-    async def decrby(self, key: str, decrement: int) -> int:
-        ...
-
-    async def get(self, key: str) -> Union[str, None]:
-        ...
-
-    async def getdel(self, key: str) -> Union[str, None]:
-        ...
-
+    ) -> int: ...
+    async def append(self, key: str, value: Any) -> int: ...
+    async def decr(self, key: str) -> int: ...
+    async def decrby(self, key: str, decrement: int) -> int: ...
+    async def get(self, key: str) -> Union[str, None]: ...
+    async def getdel(self, key: str) -> Union[str, None]: ...
     async def getex(
         self,
         key: str,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         persist: Union[bool, None] = None,
-    ) -> Union[str, None]:
-        ...
-
-    async def getrange(self, key: str, start: int, end: int) -> str:
-        ...
-
-    async def getset(self, key: str, value: Any) -> Union[str, None]:
-        ...
-
-    async def incr(self, key: str) -> int:
-        ...
-
-    async def incrby(self, key: str, increment: int) -> int:
-        ...
-
-    async def incrbyfloat(self, key: str, increment: float) -> Union[str, float]:
-        ...
-
-    async def mget(self, *keys: str) -> List[Union[str, None]]:
-        ...
-
-    async def mset(self, key_value_pairs: Dict) -> Literal["OK"]:
-        ...
-
-    async def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]:
-        ...
-
-    async def psetex(self, key: str, milliseconds: int, value: Any) -> str:
-        ...
-
+    ) -> Union[str, None]: ...
+    async def getrange(self, key: str, start: int, end: int) -> str: ...
+    async def getset(self, key: str, value: Any) -> Union[str, None]: ...
+    async def incr(self, key: str) -> int: ...
+    async def incrby(self, key: str, increment: int) -> int: ...
+    async def incrbyfloat(self, key: str, increment: float) -> Union[str, float]: ...
+    async def mget(self, *keys: str) -> List[Union[str, None]]: ...
+    async def mset(self, key_value_pairs: Dict) -> Literal["OK"]: ...
+    async def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]: ...
+    async def psetex(self, key: str, milliseconds: int, value: Any) -> str: ...
     async def set(
         self,
         key: str,
         value: Any,
         nx: bool = False,
         xx: bool = False,
         get: bool = False,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         keepttl: bool = False,
-    ) -> Union[str, None]:
-        ...
-
-    async def setex(self, key: str, seconds: int, value: Any) -> str:
-        ...
-
-    async def setnx(self, key: str, value: Any) -> Literal[1, 0]:
-        ...
-    
-    async def setrange(self, key: str, offset: int, value: Any) -> int:
-        ...
-
-    async def strlen(self, key: str) -> int:
-        ...
-
-    async def substr(self, key: str, start: int, end: int) -> str:
-        ...
-    
-    def pubsub(self) -> "PubSub":
-        ...
-
-    def script(self) -> "Script":
-        ...
-
+    ) -> Union[str, None]: ...
+    async def setex(self, key: str, seconds: int, value: Any) -> str: ...
+    async def setnx(self, key: str, value: Any) -> Literal[1, 0]: ...
+    async def setrange(self, key: str, offset: int, value: Any) -> int: ...
+    async def strlen(self, key: str) -> int: ...
+    async def substr(self, key: str, start: int, end: int) -> str: ...
+    async def script_exists(self, *sha1: str) -> Union[List[int], List[bool]]: ...
+    async def script_flush(
+        self, mode: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> Union[str, bool]: ...
+    async def script_load(self, script: str) -> str: ...
+
+    # async def pubsub_channels(self, pattern: Union[str, None] = None) -> List[str]:
+    #     ...
+
+    # async def pubsub_numpat(self) -> int:
+    #     ...
+
+    # async def pubsub_numsub(
+    #     self, *channels: str
+    # ) -> Union[List[Union[str, int]], Dict[str, int]]:
+    #     ...
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: AsyncCommands, key: str):
-        ...
-
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands":
-        ...
-
-    def set(self, encoding: str, offset: BitFieldOffset, value: int) -> "BitFieldCommands":
-        ...
-
-    def incrby(self, encoding: str, offset: BitFieldOffset, increment: int) -> "BitFieldCommands":
-        ...
-
-    def overflow(self, overflow: Literal["WRAP", "SAT", "FAIL"]) -> "BitFieldCommands":
-        ...
-
-    async def execute(self) -> List:
-        ...
-
+    def __init__(self, client: AsyncCommands, key: str): ...
+    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands": ...
+    def set(
+        self, encoding: str, offset: BitFieldOffset, value: int
+    ) -> "BitFieldCommands": ...
+    def incrby(
+        self, encoding: str, offset: BitFieldOffset, increment: int
+    ) -> "BitFieldCommands": ...
+    def overflow(
+        self, overflow: Literal["WRAP", "SAT", "FAIL"]
+    ) -> "BitFieldCommands": ...
+    async def execute(self) -> List: ...
 
 class BitFieldRO:
-    def __init__(self, client: AsyncCommands, key: str):
-        ...
-
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO":
-        ...
-
-    async def execute(self) -> List:
-        ...
-
-
-class PubSub:
-    def __init__(self, client: AsyncCommands):
-        ...
-
-    async def channels(self, pattern: Union[str, None] = None) -> List[str]:
-        ...
-
-    async def numpat(self) -> int:
-        ...
-
-    async def numsub(
-        self, *channels: str
-    ) -> Union[List[Union[str, int]], Dict[str, int]]:
-        ...
-
-
-class Script:
-    def __init__(self, client: AsyncCommands):
-        ...
-
-    async def exists(self, *sha1: str) -> Union[List[Literal[1, 0]], List[bool]]:
-        ...
-
-    async def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
-        ...
-
-    async def load(self, script: str) -> str:
-        ...
+    def __init__(self, client: AsyncCommands, key: str): ...
+    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO": ...
+    async def execute(self) -> List: ...
```

### Comparing `upstash_redis-0.13.3/upstash_redis/commands/commands.py` & `upstash_redis-0.14.0/upstash_redis/commands/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from upstash_redis.typing import CommandsProtocol, ResponseType
 
 from upstash_redis.utils.exception import (
     handle_geosearch_exceptions,
     handle_non_deprecated_zrange_exceptions,
     handle_zrangebylex_exceptions,
     handle_georadius_write_exceptions,
@@ -181,17 +180,15 @@
         :return: A bool if "format_return" is True.
         """
 
         command: List = ["EXPIRE", key, seconds]
 
         return self.run(command)
 
-    def expireat(
-        self, key: str, unix_time_seconds: int
-    ) -> ResponseType:
+    def expireat(self, key: str, unix_time_seconds: int) -> ResponseType:
         """
         See https://redis.io/commands/expireat
 
         :return: A bool if "format_return" is True.
         """
 
         command: List = ["EXPIREAT", key, unix_time_seconds]
@@ -225,17 +222,15 @@
         :return: A bool if "format_return" is True.
         """
 
         command: List = ["PEXPIRE", key, milliseconds]
 
         return self.run(command)
 
-    def pexpireat(
-        self, key: str, unix_time_milliseconds: int
-    ) -> ResponseType:
+    def pexpireat(self, key: str, unix_time_milliseconds: int) -> ResponseType:
         """
         See https://redis.io/commands/pexpireat
 
         :return: A bool if "format_return" is True.
         """
 
         command: List = ["PEXPIREAT", key, unix_time_milliseconds]
@@ -307,15 +302,14 @@
 
         if scan_type is not None:
             command.extend(["TYPE", scan_type])
 
         # The raw result is composed of the new cursor and the List of elements.
         return self.run(command)
 
-
     def touch(self, *keys: str) -> ResponseType:
         """
         See https://redis.io/commands/touch
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
@@ -401,28 +395,26 @@
         See https://redis.io/commands/geodist
 
         :return: A float value if "format_return" is True.
         """
 
         command: List = ["GEODIST", key, member1, member2, unit]
 
-        return self.run(command)        
+        return self.run(command)
 
     def geohash(self, key: str, *members: str) -> ResponseType:
         """
         See https://redis.io/commands/geohash
         """
 
         command: List = ["GEOHASH", key, *members]
 
         return self.run(command)
 
-    def geopos(
-        self, key: str, *members: str
-    ) -> ResponseType:
+    def geopos(self, key: str, *members: str) -> ResponseType:
         """
         See https://redis.io/commands/geopos
 
         :return: A List of Dicts with either None or the longitude and latitude if "format_return" is True.
         """
 
         command: List = ["GEOPOS", key, *members]
@@ -446,15 +438,15 @@
         storedist: Union[str, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/georadius
 
         :param count_any: replacement for "ANY"
 
-        :return: A List of Dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         handle_georadius_write_exceptions(
             withdist, withhash, withcoord, count, count_any, store, storedist
         )
 
         command: List = ["GEORADIUS", key, longitude, latitude, radius, unit]
@@ -500,15 +492,15 @@
         sort: Union[Literal["ASC", "DESC"], None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/georadius_ro
 
         :param count_any: replacement for "ANY"
 
-        :return: A List of Dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         if count_any and count is None:
             raise Exception('"count_any" can only be used together with "count".')
 
         command: List = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
 
@@ -528,15 +520,14 @@
 
         if sort:
             command.append(sort)
 
         # If none of the additional properties are requested, the result will be "List[str]".
         return self.run(command)
 
-
     def georadiusbymember(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
@@ -549,15 +540,15 @@
         storedist: Union[str, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/georadiusbymember
 
         :param count_any: replacement for "ANY"
 
-        :return: A List of Dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         handle_georadius_write_exceptions(
             withdist, withhash, withcoord, count, count_any, store, storedist
         )
 
         command: List = ["GEORADIUSBYMEMBER", key, member, radius, unit]
@@ -602,15 +593,15 @@
         sort: Union[Literal["ASC", "DESC"], None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/georadiusbymember_ro
 
         :param count_any: replacement for "ANY"
 
-        :return: A List of Dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         if count_any and count is None:
             raise Exception('"count_any" can only be used together with "count".')
 
         command: List = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
 
@@ -652,15 +643,15 @@
         withcoord: bool = False,
     ) -> ResponseType:
         """
         See https://redis.io/commands/geosearch
 
         :param count_any: replacement for "ANY"
 
-        :return: A List of Dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         handle_geosearch_exceptions(
             frommember,
             fromlonlat_longitude,
             fromlonlat_latitude,
             byradius,
@@ -816,17 +807,15 @@
         See https://redis.io/commands/hincrby
         """
 
         command: List = ["HINCRBY", key, field, increment]
 
         return self.run(command)
 
-    def hincrbyfloat(
-        self, key: str, field: str, increment: float
-    ) -> ResponseType:
+    def hincrbyfloat(self, key: str, field: str, increment: float) -> ResponseType:
         """
         See https://redis.io/commands/hincrbyfloat
 
         :return: A float if "format_return" is True.
         """
 
         command: List = ["HINCRBYFLOAT", key, field, increment]
@@ -917,15 +906,21 @@
 
         if count is not None:
             command.extend(["COUNT", count])
 
         # The raw result is composed of the new cursor and the List of elements.
         return self.run(command)
 
-    def hset(self, name: str, key: Optional[str] = None, val: Optional[str] = None, field_value_pairs: Optional[Dict] = None) -> ResponseType:
+    def hset(
+        self,
+        name: str,
+        key: Optional[str] = None,
+        val: Optional[str] = None,
+        field_value_pairs: Optional[Dict] = None,
+    ) -> ResponseType:
         """
         See https://redis.io/commands/hset
         """
         command: List = ["HSET", name]
 
         if key is None and field_value_pairs is None:
             raise Exception("'hset' with no key value pairs")
@@ -935,17 +930,15 @@
 
         if field_value_pairs is not None:
             for field, value in field_value_pairs.items():
                 command.extend([field, value])
 
         return self.run(command)
 
-    def hsetnx(
-        self, key: str, field: str, value: Any
-    ) -> ResponseType:
+    def hsetnx(self, key: str, field: str, value: Any) -> ResponseType:
         """
         See https://redis.io/commands/hsetnx
 
         :return: A bool if "format_return" is True.
         """
 
         command: List = ["HSETNX", key, field, value]
@@ -1008,15 +1001,19 @@
         """
 
         command: List = ["LINDEX", key, index]
 
         return self.run(command)
 
     def linsert(
-        self, key: str, position: Literal["BEFORE", "AFTER", "before", "after"], pivot: Any, element: Any
+        self,
+        key: str,
+        position: Literal["BEFORE", "AFTER", "before", "after"],
+        pivot: Any,
+        element: Any,
     ) -> ResponseType:
         """
         See https://redis.io/commands/linsert
         """
 
         command: List = ["LINSERT", key, position, pivot, element]
 
@@ -1048,17 +1045,15 @@
             destination,
             source_position,
             destination_position,
         ]
 
         return self.run(command)
 
-    def lpop(
-        self, key: str, count: Union[int, None] = None
-    ) -> ResponseType:
+    def lpop(self, key: str, count: Union[int, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/lpop
 
         :param count: defaults to 1 on the server side
         """
 
         command: List = ["LPOP", key]
@@ -1149,17 +1144,15 @@
         See https://redis.io/commands/ltrim
         """
 
         command: List = ["LTRIM", key, start, stop]
 
         return self.run(command)
 
-    def rpop(
-        self, key: str, count: Union[int, None] = None
-    ) -> ResponseType:
+    def rpop(self, key: str, count: Union[int, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/rpop
 
         :param count: defaults to 1 on the server side
         """
 
         command: List = ["RPOP", key]
@@ -1264,27 +1257,31 @@
         See https://redis.io/commands/dbsize
         """
 
         command: List = ["DBSIZE"]
 
         return self.run(command)
 
-    def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> ResponseType:
+    def flushall(
+        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> ResponseType:
         """
         See https://redis.io/commands/flushall
         """
 
         command: List = ["FLUSHALL"]
 
         if mode:
             command.append(mode)
 
         return self.run(command)
 
-    def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> ResponseType:
+    def flushdb(
+        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> ResponseType:
         """
         See https://redis.io/commands/flushdb
         """
 
         command: List = ["FLUSHDB"]
 
         if mode:
@@ -1388,46 +1385,54 @@
         See https://redis.io/commands/smembers
         """
 
         command: List = ["SMEMBERS", key]
 
         return self.run(command)
 
-    def smove(
-        self, source: str, destination: str, member: Any
-    ) -> ResponseType:
+    def smismember(self, key: str, *members: Any) -> ResponseType:
+        """
+        See https://redis.io/commands/smismember
+
+        :return: A bool list if self.format_return is True.
+        """
+
+        if len(members) == 0:
+            raise Exception("At least one member must be removed.")
+
+        command: List = ["SMISMEMBER", key, *members]
+
+        return self.run(command)
+
+    def smove(self, source: str, destination: str, member: Any) -> ResponseType:
         """
         See https://redis.io/commands/smove
 
         :return: A bool if self.format_return is True.
         """
 
         command: List = ["SMOVE", source, destination, member]
 
         return self.run(command)
 
-    def spop(
-        self, key: str, count: Union[int, None] = None
-    ) -> ResponseType:
+    def spop(self, key: str, count: Union[int, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/spop
 
         :param count: defaults to 1 on the server side
         """
 
         command: List = ["SPOP", key]
 
         if count is not None:
             command.append(count)
 
         return self.run(command)
 
-    def srandmember(
-        self, key: str, count: Union[int, None] = None
-    ) -> ResponseType:
+    def srandmember(self, key: str, count: Union[int, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/srandmember
 
         :param count: defaults to 1 on the server side
         """
 
         command: List = ["SRANDMEMBER", key]
@@ -1579,17 +1584,15 @@
         return self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
     whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
-    def zdiff(
-        self, keys: List[str], withscores: bool = False
-    ) -> ResponseType:
+    def zdiff(self, keys: List[str], withscores: bool = False) -> ResponseType:
         """
         See https://redis.io/commands/zdiff
 
         The number of keys is calculated automatically.
 
         :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
@@ -1614,17 +1617,15 @@
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["ZDIFFSTORE", destination, len(keys), *keys]
 
         return self.run(command)
 
-    def zincrby(
-        self, key: str, increment: float, member: str
-    ) -> ResponseType:
+    def zincrby(self, key: str, increment: float, member: str) -> ResponseType:
         """
         See https://redis.io/commands/zincrby
 
         :return: A float if "format_return" is True.
         """
 
         command: List = ["ZINCRBY", key, increment, member]
@@ -1708,33 +1709,29 @@
                 "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
             )
 
         command: List = ["ZLEXCOUNT", key, min_score, max_score]
 
         return self.run(command)
 
-    def zmscore(
-        self, key: str, members: List[str]
-    ) -> ResponseType:
+    def zmscore(self, key: str, members: List[str]) -> ResponseType:
         """
         See https://redis.io/commands/zmscore
 
         :return: A List of float or None values if "format_return" is True.
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be specified.")
 
         command: List = ["ZMSCORE", key, *members]
 
         return self.run(command)
 
-    def zpopmax(
-        self, key: str, count: Union[int, None] = None
-    ) -> ResponseType:
+    def zpopmax(self, key: str, count: Union[int, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/zpopmax
 
         :param count: defaults to 1 on the server side
 
         :return: A Dict of member-score pairs if "format_return" is True.
         """
@@ -1742,17 +1739,15 @@
         command: List = ["ZPOPMAX", key]
 
         if count is not None:
             command.append(count)
 
         return self.run(command)
 
-    def zpopmin(
-        self, key: str, count: Union[int, None] = None
-    ) -> ResponseType:
+    def zpopmin(self, key: str, count: Union[int, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/zpopmin
 
         :param count: defaults to 1 on the server side
 
         :return: A Dict of member-score pairs if "format_return" is True.
         """
@@ -2237,15 +2232,17 @@
         pxat: Union[int, None] = None,
         persist: Union[bool, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/getex
         """
 
-        if (ex or px or exat or pxat or persist) and not number_are_not_none(ex, px, exat, pxat, persist, number=1):
+        if (ex or px or exat or pxat or persist) and not number_are_not_none(
+            ex, px, exat, pxat, persist, number=1
+        ):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         command: List = ["GETEX", key]
 
         if ex is not None:
             command.extend(["EX", ex])
 
@@ -2371,15 +2368,17 @@
         """
         See https://redis.io/commands/set
         """
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
 
-        if (ex or px or exat or pxat or keepttl) and not number_are_not_none(ex, px, exat, pxat, keepttl, number=1):
+        if (ex or px or exat or pxat or keepttl) and not number_are_not_none(
+            ex, px, exat, pxat, keepttl, number=1
+        ):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         if nx and get:
             raise Exception('"nx" and "get" are mutually exclusive.')
 
         command: List = ["SET", key, value]
 
@@ -2449,28 +2448,85 @@
         """
         See https://redis.io/commands/substr
         """
 
         command: List = ["SUBSTR", key, start, end]
 
         return self.run(command)
-    
-    def pubsub(self) -> "PubSub":
+
+    def script_exists(self, *sha1: str) -> ResponseType:
+        """
+        See https://redis.io/commands/script-exists
+
+        :return: A List of bools if "format_return" is True.
+        """
+
+        if len(sha1) == 0:
+            raise Exception("At least one sha1 digests must be provided.")
+
+        command: List = ["SCRIPT", "EXISTS", *sha1]
+
+        return self.run(command)
+
+    def script_flush(
+        self, mode: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> ResponseType:
         """
-        See https://redis.io/commands/pubsub
+        See https://redis.io/commands/script-flush
         """
 
-        return PubSub(client=self)
+        command: List = ["SCRIPT", "FLUSH"]
 
-    def script(self) -> "Script":
+        if mode:
+            command.append(mode)
+
+        return self.run(command)
+
+    def script_load(self, script: str) -> ResponseType:
         """
-        See https://redis.io/commands/script
+        See https://redis.io/commands/script-load
         """
 
-        return Script(client=self)
+        command: List = ["SCRIPT", "LOAD", script]
+
+        return self.run(command)
+
+    # def pubsub_channels(self, pattern: Union[str, None] = None) -> ResponseType:
+    #     """
+    #     See https://redis.io/commands/pubsub-channels
+    #     """
+
+    #     command: List = ["PUBSUB", "CHANNELS"]
+
+    #     if pattern is not None:
+    #         command.append(pattern)
+
+    #     return self.run(command)
+
+    # def pubsub_numpat(self) -> ResponseType:
+    #     """
+    #     See https://redis.io/commands/pubsub-numpat
+    #     """
+
+    #     command: List = ["PUBSUB", "NUMPAT"]
+
+    #     return self.run(command)
+
+    # def pubsub_numsub(
+    #     self, *channels: str
+    # ) -> ResponseType:
+    #     """
+    #     See https://redis.io/commands/pubsub-numsub
+
+    #     :return: A Dict with channel-number_of_subscribers pairs if "format_return" is True.
+    #     """
+
+    #     command: List = ["PUBSUB", "NUMSUB", *channels]
+
+    #     return self.run(command)
 
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
     def __init__(self, client: Commands, key: str):
         self.client = client
         self.command: List = ["BITFIELD", key]
@@ -2483,27 +2539,31 @@
         """
 
         _command = ["GET", encoding, offset]
         self.command.extend(_command)
 
         return self
 
-    def set(self, encoding: str, offset: BitFieldOffset, value: int) -> "BitFieldCommands":
+    def set(
+        self, encoding: str, offset: BitFieldOffset, value: int
+    ) -> "BitFieldCommands":
         """
         Set the specified bit field and returns its old value.
 
         Source: https://redis.io/commands/bitfield
         """
 
         _command = ["SET", encoding, offset, value]
         self.command.extend(_command)
 
         return self
 
-    def incrby(self, encoding: str, offset: BitFieldOffset, increment: int) -> "BitFieldCommands":
+    def incrby(
+        self, encoding: str, offset: BitFieldOffset, increment: int
+    ) -> "BitFieldCommands":
         """
         Increments or decrements (if a negative increment is given) the specified bit field and returns the new value.
 
         Source: https://redis.io/commands/bitfield
         """
 
         _command = ["INCRBY", encoding, offset, increment]
@@ -2549,92 +2609,14 @@
 
         return self
 
     def execute(self) -> ResponseType:
         return self.client.run(command=self.command)
 
 
-class PubSub:
-    def __init__(self, client: Commands):
-        self.client = client
-
-    def channels(self, pattern: Union[str, None] = None) -> ResponseType:
-        """
-        See https://redis.io/commands/pubsub-channels
-        """
-
-        command: List = ["PUBSUB", "CHANNELS"]
-
-        if pattern is not None:
-            command.append(pattern)
-
-        return self.client.run(command=command)
-
-    def numpat(self) -> ResponseType:
-        """
-        See https://redis.io/commands/pubsub-numpat
-        """
-
-        command: List = ["PUBSUB", "NUMPAT"]
-
-        return self.client.run(command=command)
-
-    def numsub(
-        self, *channels: str
-    ) -> ResponseType:
-        """
-        See https://redis.io/commands/pubsub-numsub
-
-        :return: A Dict with channel-number_of_subscribers pairs if "format_return" is True.
-        """
-
-        command: List = ["PUBSUB", "NUMSUB", *channels]
-
-        return self.client.run(command)
-
-class Script:
-    def __init__(self, client: Commands):
-        self.client = client
-
-    def exists(self, *sha1: str) -> ResponseType:
-        """
-        See https://redis.io/commands/script-exists
-
-        :return: A List of bools if "format_return" is True.
-        """
-
-        if len(sha1) == 0:
-            raise Exception("At least one sha1 digests must be provided.")
-
-        command: List = ["SCRIPT", "EXISTS", *sha1]
-
-        return self.client.run(command=command)
-
-    def flush(self, mode: Literal["ASYNC", "SYNC"]) -> ResponseType:
-        """
-        See https://redis.io/commands/script-flush
-        """
-
-        command: List = ["SCRIPT", "FLUSH"]
-
-        if mode:
-            command.append(mode)
-
-        return self.client.run(command=command)
-
-    def load(self, script: str) -> ResponseType:
-        """
-        See https://redis.io/commands/script-load
-        """
-
-        command: List = ["SCRIPT", "LOAD", script]
-
-        return self.client.run(command=command)
-
-
 """
 class ACL:
     def __init__(self, client: Commands):
         self.client = client
 
     async def cat(self, category: Union[str, None] = None) -> List[str]:
         # See https://redis.io/commands/acl-cat
@@ -2699,8 +2681,26 @@
         if count is not None:
             command.append(count)
 
         if reset:
             command.append("RESET")
 
         return await self.client.run(command=command)
+
+    async def save(self, count: Union[int, None] = None, reset: bool = False) -> List[str]:
+        # See https://redis.io/commands/acl-save
+
+        command: List = ["ACL", "SAVE"]
+
+        return await self.client.run(command=command)
+
+    async def setuser():
+        ...
+    
+    async def users():
+        ...
+
+    async def whoami():
+        ...
+
+
 """
```

### Comparing `upstash_redis-0.13.3/upstash_redis/commands/commands.pyi` & `upstash_redis-0.14.0/upstash_redis/commands/commands.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,84 @@
-
-from upstash_redis.schema.commands.returns import (
-    GeoMembersReturn,
-    FormattedGeoMembersReturn,
-)
-
 from upstash_redis.schema.commands.parameters import (
     BitFieldOffset,
     GeoMember,
     FloatMinMax,
 )
 
 from typing import Any, Iterable, Optional, Set, Tuple, Union, List, Literal, Dict
 
 class Commands:
     def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
-    ) -> int: 
-        ...
-
-    def bitfield(self, key: str) -> "BitFieldCommands":
-        ...
-
-    def bitfield_ro(self, key: str) -> "BitFieldRO":
-        ...
-
+    ) -> int: ...
+    def bitfield(self, key: str) -> "BitFieldCommands": ...
+    def bitfield_ro(self, key: str) -> "BitFieldRO": ...
     def bitop(
         self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *srckeys: str
-    ) -> int:
-        ...
-
+    ) -> int: ...
     def bitpos(
         self,
         key: str,
         bit: Literal[0, 1],
         start: Union[int, None] = None,
         end: Union[int, None] = None,
-    ) -> int:
-        ...
-
-    def getbit(self, key: str, offset: int) -> int:
-        ...
-
-    def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int:
-        ...
-
-    def ping(self, message: Union[str, None] = None) -> str:
-        ...
-
-    def echo(self, message: str) -> str:
-        ...
-    
+    ) -> int: ...
+    def getbit(self, key: str, offset: int) -> int: ...
+    def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int: ...
+    def ping(self, message: Union[str, None] = None) -> str: ...
+    def echo(self, message: str) -> str: ...
     def copy(
         self, source: str, destination: str, replace: bool = False
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def delete(self, *keys: str) -> int:
-        ...
-
-    def exists(self, *keys: str) -> int:
-        ...
-
-    def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    def delete(self, *keys: str) -> int: ...
+    def exists(self, *keys: str) -> int: ...
+    def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]: ...
     def expireat(
         self, key: str, unix_time_seconds: int
-    ) -> Union[Literal[1, 0], bool]:
-       ...
-
-    def keys(self, pattern: str) -> List[str]:
-        ...
-
-    def persist(self, key: str) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def pexpire(self, key: str, milliseconds: int) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    def keys(self, pattern: str) -> List[str]: ...
+    def persist(self, key: str) -> Union[Literal[1, 0], bool]: ...
+    def pexpire(self, key: str, milliseconds: int) -> Union[Literal[1, 0], bool]: ...
     def pexpireat(
         self, key: str, unix_time_milliseconds: int
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def pttl(self, key: str) -> int:
-        ...
-
-    def randomkey(self) -> Union[str, None]:
-        ...
-
-    def rename(self, key: str, newkey: str) -> str:
-        ...
-
-    def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    def pttl(self, key: str) -> int: ...
+    def randomkey(self) -> Union[str, None]: ...
+    def rename(self, key: str, newkey: str) -> str: ...
+    def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]: ...
     def scan(
         self,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         scan_type: Union[str, None] = None,
-    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]:
-        ...
-    
-    def touch(self, *keys: str) -> int:
-        ...
-
-    def ttl(self, key: str) -> int:
-        ...
-
-    def type(self, key: str) -> Union[str, None]:
-        ...
-
-    def unlink(self, *keys: str) -> int:
-        ...
-
+    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]: ...
+    def touch(self, *keys: str) -> int: ...
+    def ttl(self, key: str) -> int: ...
+    def type(self, key: str) -> Union[str, None]: ...
+    def unlink(self, *keys: str) -> int: ...
     def geoadd(
         self,
         key: str,
         *members: GeoMember,
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
-    ) -> int:
-        ...
-
+    ) -> int: ...
     def geodist(
         self,
         key: str,
         member1: str,
         member2: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M",
-    ) -> Union[str, float, None]:
-        ...
-
-    def geohash(self, key: str, *members: str) -> List[Union[str, None]]:
-        ...
-
+    ) -> Union[str, float, None]: ...
+    def geohash(self, key: str, *members: str) -> List[Union[str, None]]: ...
     def geopos(
         self, key: str, *members: str
-    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]:
-        ...
-
+    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]: ...
     def georadius(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
@@ -154,65 +86,71 @@
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn, int]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+        int,
+    ]: ...
     def georadius_ro(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+    ]: ...
     def georadiusbymember(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+        int,
+    ]: ...
     def georadiusbymember_ro(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
         count_any: bool = False,
         sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+    ]: ...
     def geosearch(
         self,
         key: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         frommember: Union[str, None] = None,
         fromlonlat_longitude: Union[float, None] = None,
         fromlonlat_latitude: Union[float, None] = None,
@@ -221,17 +159,18 @@
         bybox_height: Union[float, None] = None,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
         count_any: bool = False,
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
-    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
-        ...
-
+    ) -> Union[
+        List[Union[str, List[Union[str, List[str]]]]],
+        List[Dict[str, Union[str, float, int]]],
+    ]: ...
     def geosearchstore(
         self,
         destination: str,
         source: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
         frommember: Union[str, None] = None,
         fromlonlat_longitude: Union[float, None] = None,
@@ -239,584 +178,350 @@
         byradius: Union[float, None] = None,
         bybox_width: Union[float, None] = None,
         bybox_height: Union[float, None] = None,
         sort: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
         count_any: bool = False,
         storedist: bool = False,
-    ) -> int:
-        ...
-
-    def hdel(self, key: str, *fields: str) -> int:
-        ...
-
-    def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def hget(self, key: str, field: str) -> Union[str, None]:
-        ...
-
-    def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]:
-        ...
-
-    def hincrby(self, key: str, field: str, increment: int) -> int:
-        ...
-
+    ) -> int: ...
+    def hdel(self, key: str, *fields: str) -> int: ...
+    def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]: ...
+    def hget(self, key: str, field: str) -> Union[str, None]: ...
+    def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]: ...
+    def hincrby(self, key: str, field: str, increment: int) -> int: ...
     def hincrbyfloat(
         self, key: str, field: str, increment: float
-    ) -> Union[str, float]:
-        ...
-
-    def hkeys(self, key: str) -> List[str]:
-        ...
-
-    def hlen(self, key: str) -> int:
-        ...
-
-    def hmget(self, key: str, *fields: str) -> List[Union[str, None]]:
-        ...
-
-    def hmset(self, key: str, field_value_pairs: Dict) -> str:
-        ...
-
+    ) -> Union[str, float]: ...
+    def hkeys(self, key: str) -> List[str]: ...
+    def hlen(self, key: str) -> int: ...
+    def hmget(self, key: str, *fields: str) -> List[Union[str, None]]: ...
+    def hmset(self, key: str, field_value_pairs: Dict) -> str: ...
     def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
-    ):
-        ...
-
+    ): ...
     def hscan(
         self,
         name: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Tuple[int, Dict[str, str]]:
-        ...
-
-    def hset(self, name: str, key: Optional[str] = None, val: Optional[str] = None, field_value_pairs: Optional[Dict] = None) -> int:
-        ...
-
+    ) -> Tuple[int, Dict[str, str]]: ...
+    def hset(
+        self,
+        name: str,
+        key: Optional[str] = None,
+        val: Optional[str] = None,
+        field_value_pairs: Optional[Dict] = None,
+    ) -> int: ...
     def hsetnx(
         self, key: str, field: str, value: Any
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def hstrlen(self, key: str, field: str) -> int:
-        ...
-
-    def hvals(self, key: str) -> List[str]:
-        ...
-
-    def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def pfcount(self, *keys: str) -> int:
-        ...
-
-    def pfmerge(self, destkey: str, *sourcekeys: str) -> str:
-        ...
-
-    def lindex(self, key: str, index: int) -> Union[str, None]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
+    def hstrlen(self, key: str, field: str) -> int: ...
+    def hvals(self, key: str) -> List[str]: ...
+    def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]: ...
+    def pfcount(self, *keys: str) -> int: ...
+    def pfmerge(self, destkey: str, *sourcekeys: str) -> str: ...
+    def lindex(self, key: str, index: int) -> Union[str, None]: ...
     def linsert(
-        self, key: str, position: Literal["BEFORE", "AFTER", "before", "after"], pivot: Any, element: Any
-    ) -> int:
-       ...
-
-    def llen(self, key: str) -> int:
-        ...
-
+        self,
+        key: str,
+        position: Literal["BEFORE", "AFTER", "before", "after"],
+        pivot: Any,
+        element: Any,
+    ) -> int: ...
+    def llen(self, key: str) -> int: ...
     def lmove(
         self,
         source: str,
         destination: str,
         source_position: Literal["LEFT", "RIGHT"] = "LEFT",
         destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
-    ) -> Union[str, None]:
-        ...
-
+    ) -> Union[str, None]: ...
     def lpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
     def lpos(
         self,
         key: str,
         element: Any,
         rank: Union[int, None] = None,
         count: Union[int, None] = None,
         maxlen: Union[int, None] = None,
-    ) -> Union[(Union[int, None]), List[int]]:
-        ...
-
-    def lpush(self, key: str, *elements: Any) -> int:
-        ...
-
-    def lpushx(self, key: str, *elements: Any) -> int:
-        ...
-
-    def lrange(self, key: str, start: int, stop: int) -> List[str]:
-        ...
-
-    def lrem(self, key: str, count: int, element: Any) -> int:
-        ...
-
-    def lset(self, key: str, index: int, element: Any) -> str:
-        ...
-
-    def ltrim(self, key: str, start: int, stop: int) -> str:
-        ...
-
+    ) -> Union[(Union[int, None]), List[int]]: ...
+    def lpush(self, key: str, *elements: Any) -> int: ...
+    def lpushx(self, key: str, *elements: Any) -> int: ...
+    def lrange(self, key: str, start: int, stop: int) -> List[str]: ...
+    def lrem(self, key: str, count: int, element: Any) -> int: ...
+    def lset(self, key: str, index: int, element: Any) -> str: ...
+    def ltrim(self, key: str, start: int, stop: int) -> str: ...
     def rpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
-    def rpoplpush(self, source: str, destination: str) -> Union[str, None]:
-        ...
-
-    def rpush(self, key: str, *elements: Any) -> int:
-        ...
-
-    def rpushx(self, key: str, *elements: Any) -> int:
-        ...
-
-    def publish(self, channel: str, message: str) -> int:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
+    def rpoplpush(self, source: str, destination: str) -> Union[str, None]: ...
+    def rpush(self, key: str, *elements: Any) -> int: ...
+    def rpushx(self, key: str, *elements: Any) -> int: ...
+    def publish(self, channel: str, message: str) -> int: ...
     def eval(
         self,
         script: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
-    ) -> Any:
-        ...
-
+    ) -> Any: ...
     def evalsha(
         self,
         sha1: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
-    ) -> Any:
-        ...
-
-    def dbsize(self) -> int:
-        ...
-
-    def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
-        ...
-
-    def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
-        ...
-
-    def time(self) -> Union[List[str], Dict[str, int]]:
-        ...
-
-    def sadd(self, key: str, *members: Any) -> int:
-        ...
-
-    def scard(self, key: str) -> int:
-        ...
-
-    def sdiff(self, *keys: str) -> Set[str]:
-        ...
-
-    def sdiffstore(self, destination: str, *keys: str) -> int:
-        ...
-
-    def sinter(self, *keys: str) -> Set[str]:
-        ...
-
-    def sinterstore(self, destination: str, *keys: str) -> int:
-        ...
-
-    def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]:
-        ...
-
-    def smembers(self, key: str) -> Set[str]:
-        ...
-
+    ) -> Any: ...
+    def dbsize(self) -> int: ...
+    def flushall(
+        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> Union[str, bool]: ...
+    def flushdb(
+        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> Union[str, bool]: ...
+    def time(self) -> Union[List[str], Dict[str, int]]: ...
+    def sadd(self, key: str, *members: Any) -> int: ...
+    def scard(self, key: str) -> int: ...
+    def sdiff(self, *keys: str) -> Set[str]: ...
+    def sdiffstore(self, destination: str, *keys: str) -> int: ...
+    def sinter(self, *keys: str) -> Set[str]: ...
+    def sinterstore(self, destination: str, *keys: str) -> int: ...
+    def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]: ...
+    def smismember(
+        self, key: str, *members: Any
+    ) -> Union[List[Literal[1, 0]], List[bool]]: ...
+    def smembers(self, key: str) -> Set[str]: ...
     def smove(
         self, source: str, destination: str, member: Any
-    ) -> Union[Literal[1, 0], bool]:
-        ...
-
+    ) -> Union[Literal[1, 0], bool]: ...
     def spop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
     def srandmember(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]:
-        ...
-
-    def srem(self, key: str, *members: Any) -> int:
-        ...
-
+    ) -> Union[(Union[str, None]), List[str]]: ...
+    def srem(self, key: str, *members: Any) -> int: ...
     def sscan(
         self,
         key: str,
         cursor: int = 0,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Tuple[int, List[str]]:
-        ...
-
-    def sunion(self, *keys: str) -> Set[str]:
-        ...
-
-    def sunionstore(self, destination: str, *keys: str) -> int:
-        ...
-
+    ) -> Tuple[int, List[str]]: ...
+    def sunion(self, *keys: str) -> Set[str]: ...
+    def sunionstore(self, destination: str, *keys: str) -> int: ...
     def zadd(
         self,
         key: str,
         score_member_pairs: Dict,
         nx: bool = False,
         xx: bool = False,
         gt: bool = False,
         lt: bool = False,
         ch: bool = False,
         incr: bool = False,
-    ) -> Union[int, (Union[str, None, float])]:
-        ...
-    
-    def zcard(self, key: str) -> int:
-        ...
-
+    ) -> Union[int, (Union[str, None, float])]: ...
+    def zcard(self, key: str) -> int: ...
     def zcount(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> int:
-        ...
-
+    ) -> int: ...
     def zdiff(
         self, keys: List[str], withscores: bool = False
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
-    def zdiffstore(self, destination: str, keys: List[str]) -> int:
-        ...
-
-    def zincrby(
-        self, key: str, increment: float, member: str
-    ) -> Union[str, float]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zdiffstore(self, destination: str, keys: List[str]) -> int: ...
+    def zincrby(self, key: str, increment: float, member: str) -> Union[str, float]: ...
     def zinter(
         self,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zinterstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
-    ) -> int:
-        ...
-
-    def zlexcount(self, key: str, min_score: str, max_score: str) -> int:
-        ...
-
+    ) -> int: ...
+    def zlexcount(self, key: str, min_score: str, max_score: str) -> int: ...
     def zmscore(
         self, key: str, members: List[str]
-    ) -> Union[List[Union[str, None]], List[Union[float, None]]]:
-        ...
-
+    ) -> Union[List[Union[str, None]], List[Union[float, None]]]: ...
     def zpopmax(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zpopmin(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zrandmember(
         self, key: str, count: Union[int, None] = None, withscores: bool = False
-    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]:
-        ...
-
+    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]: ...
     def zrange(
         self,
         key: str,
         start: FloatMinMax,
         stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
         withscores: bool = False,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zrangebylex(
         self,
         key: str,
         min_score: str,
         max_score: str,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> List[Union[str, None]]:
-        ...
-
+    ) -> List[Union[str, None]]: ...
     def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
         withscores: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zrangestore(
         self,
         dst: str,
         src: str,
         start: FloatMinMax,
         stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> int:
-        ...
-
-    def zrank(self, key: str, member: str) -> Union[int, None]:
-        ...
-
-    def zrem(self, key: str, *members: str) -> int:
-        ...
-
-    def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int:
-        ...
-
-    def zremrangebyrank(self, key: str, start: int, stop: int) -> int:
-        ...
-
+    ) -> int: ...
+    def zrank(self, key: str, member: str) -> Union[int, None]: ...
+    def zrem(self, key: str, *members: str) -> int: ...
+    def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int: ...
+    def zremrangebyrank(self, key: str, start: int, stop: int) -> int: ...
     def zremrangebyscore(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> int:
-        ...
-
+    ) -> int: ...
     def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> List[str]:
-        ...
-
+    ) -> List[str]: ...
     def zrevrangebyscore(
         self,
         key: str,
         max_score: FloatMinMax,
         min_score: FloatMinMax,
         withscores: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
-    def zrevrank(self, key: str, member: str) -> Union[int, None]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zrevrank(self, key: str, member: str) -> Union[int, None]: ...
     def zscan(
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Tuple[int, List[Tuple[str, float]]]:
-        ...
-
-    def zscore(self, key: str, member: str) -> Union[str, None, float]:
-        ...
-
+    ) -> Tuple[int, List[Tuple[str, float]]]: ...
+    def zscore(self, key: str, member: str) -> Union[str, None, float]: ...
     def zunion(
         self,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[List[str], List[Tuple[str, float]]]:
-        ...
-
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
     def zunionstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
-    ) -> int:
-        ...
-
-    def append(self, key: str, value: Any) -> int:
-        ...
-
-    def decr(self, key: str) -> int:
-        ...
-
-    def decrby(self, key: str, decrement: int) -> int:
-        ...
-
-    def get(self, key: str) -> Union[str, None]:
-        ...
-
-    def getdel(self, key: str) -> Union[str, None]:
-        ...
-
+    ) -> int: ...
+    def append(self, key: str, value: Any) -> int: ...
+    def decr(self, key: str) -> int: ...
+    def decrby(self, key: str, decrement: int) -> int: ...
+    def get(self, key: str) -> Union[str, None]: ...
+    def getdel(self, key: str) -> Union[str, None]: ...
     def getex(
         self,
         key: str,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         persist: Union[bool, None] = None,
-    ) -> Union[str, None]:
-        ...
-
-    def getrange(self, key: str, start: int, end: int) -> str:
-        ...
-
-    def getset(self, key: str, value: Any) -> Union[str, None]:
-        ...
-
-    def incr(self, key: str) -> int:
-        ...
-
-    def incrby(self, key: str, increment: int) -> int:
-        ...
-
-    def incrbyfloat(self, key: str, increment: float) -> Union[str, float]:
-        ...
-
-    def mget(self, *keys: str) -> List[Union[str, None]]:
-        ...
-
-    def mset(self, key_value_pairs: Dict) -> Literal["OK"]:
-        ...
-
-    def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]:
-        ...
-
-    def psetex(self, key: str, milliseconds: int, value: Any) -> str:
-        ...
-
+    ) -> Union[str, None]: ...
+    def getrange(self, key: str, start: int, end: int) -> str: ...
+    def getset(self, key: str, value: Any) -> Union[str, None]: ...
+    def incr(self, key: str) -> int: ...
+    def incrby(self, key: str, increment: int) -> int: ...
+    def incrbyfloat(self, key: str, increment: float) -> Union[str, float]: ...
+    def mget(self, *keys: str) -> List[Union[str, None]]: ...
+    def mset(self, key_value_pairs: Dict) -> Literal["OK"]: ...
+    def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]: ...
+    def psetex(self, key: str, milliseconds: int, value: Any) -> str: ...
     def set(
         self,
         key: str,
         value: Any,
         nx: bool = False,
         xx: bool = False,
         get: bool = False,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         keepttl: bool = False,
-    ) -> Union[str, None]:
-        ...
-
-    def setex(self, key: str, seconds: int, value: Any) -> str:
-        ...
-
-    def setnx(self, key: str, value: Any) -> Literal[1, 0]:
-        ...
-    
-    def setrange(self, key: str, offset: int, value: Any) -> int:
-        ...
-
-    def strlen(self, key: str) -> int:
-        ...
-
-    def substr(self, key: str, start: int, end: int) -> str:
-        ...
-
-    def pubsub(self) -> "PubSub":
-        ...
-
-    def script(self) -> "Script":
-        ...
+    ) -> Union[str, None]: ...
+    def setex(self, key: str, seconds: int, value: Any) -> str: ...
+    def setnx(self, key: str, value: Any) -> Literal[1, 0]: ...
+    def setrange(self, key: str, offset: int, value: Any) -> int: ...
+    def strlen(self, key: str) -> int: ...
+    def substr(self, key: str, start: int, end: int) -> str: ...
+    def script_exists(self, *sha1: str) -> Union[List[int], List[bool]]: ...
+    def script_flush(
+        self, mode: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> Union[str, bool]: ...
+    def script_load(self, script: str) -> str: ...
+
+    # def pubsub_channels(self, pattern: Union[str, None] = None) -> List[str]:
+    #     ...
+
+    # def pubsub_numpat(self) -> int:
+    #     ...
+
+    # def pubsub_numsub(
+    #     self, *channels: str
+    # ) -> Union[List[Union[str, int]], Dict[str, int]]:
+    #     ...
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: Commands, key: str):
-        ...
-
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands":
-        ...
-
-    def set(self, encoding: str, offset: BitFieldOffset, value: int) -> "BitFieldCommands":
-        ...
-
-    def incrby(self, encoding: str, offset: BitFieldOffset, increment: int) -> "BitFieldCommands":
-        ...
-
-    def overflow(self, overflow: Literal["WRAP", "SAT", "FAIL"]) -> "BitFieldCommands":
-        ...
-
-    def execute(self) -> List:
-        ...
-
+    def __init__(self, client: Commands, key: str): ...
+    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands": ...
+    def set(
+        self, encoding: str, offset: BitFieldOffset, value: int
+    ) -> "BitFieldCommands": ...
+    def incrby(
+        self, encoding: str, offset: BitFieldOffset, increment: int
+    ) -> "BitFieldCommands": ...
+    def overflow(
+        self, overflow: Literal["WRAP", "SAT", "FAIL"]
+    ) -> "BitFieldCommands": ...
+    def execute(self) -> List: ...
 
 class BitFieldRO:
-    def __init__(self, client: Commands, key: str):
-        ...
-
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO":
-        ...
-
-    def execute(self) -> List:
-        ...
-
-
-class PubSub:
-    def __init__(self, client: Commands):
-        ...
-
-    def channels(self, pattern: Union[str, None] = None) -> List[str]:
-        ...
-
-    def numpat(self) -> int:
-        ...
-
-    def numsub(
-        self, *channels: str
-    ) -> Union[List[Union[str, int]], Dict[str, int]]:
-        ...
-
-
-class Script:
-    def __init__(self, client: Commands):
-        ...
-
-    def exists(self, *sha1: str) -> Union[List[Literal[1, 0]], List[bool]]:
-        ...
-
-    def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
-        ...
-
-    def load(self, script: str) -> str:
-        ...
-
+    def __init__(self, client: Commands, key: str): ...
+    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO": ...
+    def execute(self) -> List: ...
 
-# TODO: make sure all the relevant sorted set commands return tuples
+# TODO: make sure all the relevant sorted set commands return tuples
```

### Comparing `upstash_redis-0.13.3/upstash_redis/http/decode.py` & `upstash_redis-0.14.0/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.3/upstash_redis/http/execute.py` & `upstash_redis-0.14.0/upstash_redis/http/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,21 @@
     :param retries: how many times an HTTP request will be retried if it fails
     :param retry_interval: how many seconds will be waited between each retry
     :param allow_telemetry: whether anonymous telemetry can be collected
     """
 
     # Serialize the command; more specifically, write string-incompatible types as JSON strings.
     command = [
-        element if (isinstance(element, str) or isinstance(element, int) or isinstance(element, float)) else dumps(element)
+        element
+        if (
+            isinstance(element, str)
+            or isinstance(element, int)
+            or isinstance(element, float)
+        )
+        else dumps(element)
         for element in command
     ]
 
     for i in range(retries + 1):
         try:
             headers: Dict[str, str] = {"Authorization": f"Bearer {token}"}
 
@@ -94,17 +100,22 @@
     encoding: RESTEncoding,
     retries: int,
     retry_interval: int,
     command: List,
     allow_telemetry: bool,
     telemetry_data: Union[TelemetryData, None] = None,
 ) -> RESTResult:
-
     command = [
-        element if (isinstance(element, str) or isinstance(element, int) or isinstance(element, float)) else dumps(element)
+        element
+        if (
+            isinstance(element, str)
+            or isinstance(element, int)
+            or isinstance(element, float)
+        )
+        else dumps(element)
         for element in command
     ]
 
     for i in range(retries + 1):
         try:
             headers: Dict[str, str] = {"Authorization": f"Bearer {token}"}
```

### Comparing `upstash_redis-0.13.3/upstash_redis/schema/http.py` & `upstash_redis-0.14.0/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.3/upstash_redis/utils/exception.py` & `upstash_redis-0.14.0/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.3/upstash_redis/utils/format.py` & `upstash_redis-0.14.0/upstash_redis/utils/format.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-from upstash_redis.schema.commands.returns import (
-    GeoMembersReturn,
-    FormattedGeoMembersReturn,
-)
 from typing import Literal, Tuple, Union, List, Dict
 
 
 def _list_to_dict(raw: List, command=None) -> Dict:
     """
     Convert a list that contains ungrouped pairs as consecutive elements (usually field-value or similar) into a dict.
     """
 
     return {raw[iterator]: raw[iterator + 1] for iterator in range(0, len(raw), 2)}
 
 
 def format_geo_positions_return(
-    raw: List[Union[List[str], None]],
-    command = None
+    raw: List[Union[List[str], None]], command=None
 ) -> List[Union[Dict[str, float], None]]:
     """
     Format the raw output returned by "GEOPOS".
     """
 
     return [
         {"longitude": float(member[0]), "latitude": float(member[1])}
         if isinstance(member, List)
         else None
         for member in raw
     ]
 
 
 def format_geo_members_return(
-    raw: GeoMembersReturn,
+    raw: List[Union[str, List[Union[str, List[str]]]]],
     with_distance: Union[bool, None],
     with_hash: Union[bool, None],
     with_coordinates: Union[bool, None],
-) -> FormattedGeoMembersReturn:
+) -> List[Dict[str, Union[str, float, int]]]:
     """
     Format the raw output given by some Geo commands, usually the ones that return properties of members,
     when additional properties are requested.
 
     Note that the output's type might differ from the "GeoMember" type that represents the initial properties of
     a geo member.
 
@@ -48,15 +43,15 @@
      - the coordinates as:
         - the longitude
         - the latitude
 
     All represented as strings
     """
 
-    result: FormattedGeoMembersReturn = []
+    result: List[Dict[str, Union[str, float, int]]] = []
 
     for member in raw:
         formatted_member: Dict[str, Union[str, float, int]] = {"member": member[0]}
 
         if with_distance:
             formatted_member["distance"] = float(member[1])
 
@@ -83,15 +78,15 @@
             formatted_member["latitude"] = float(member[1][1])
 
         result.append(formatted_member)
 
     return result
 
 
-def format_hash_return(raw: List[str], command = None) -> Dict[str, str]:
+def format_hash_return(raw: List[str], command=None) -> Dict[str, str]:
     """
     Format the raw output given by Hash commands, usually the ones that return the field-value
     pairs of Hashes.
     """
 
     return _list_to_dict(raw=raw)
 
@@ -125,188 +120,214 @@
     Format the raw output given by Sorted Set commands, usually the ones that return the member-score
     pairs of Sorted Sets.
     """
     it = iter(raw)
     return list(zip(it, map(float, it)))
 
 
-def format_float_list(raw: List[Union[str, None]], command=None) -> List[Union[float, None]]:
+def format_float_list(
+    raw: List[Union[str, None]], command=None
+) -> List[Union[float, None]]:
     """
     Format a list of strings representing floats or None values.
     """
 
     return [float(value) if value is not None else None for value in raw]
 
 
-
 def to_set(res, command):
     return set(res)
 
+
 def ok_to_bool(res, command):
     return res == "OK"
 
+
 def to_bool(res, command):
     return bool(res)
 
+
+def list_to_bool_list(res, command):
+    return list(map(bool, res))
+
+
 def to_float(res, command):
     return float(res)
 
+
 def scan_formatter(res, command):
     return [int(res[0]), res[1]]
 
+
 def hscan_formatter(res, command):
     return [int(res[0]), format_hash_return(res[1])]
 
-def sscan_formatter(res, command): ## same with scan_formatter
+
+def sscan_formatter(res, command):  ## same with scan_formatter
     return [int(res[0]), res[1]]
 
-def zscan_formatter(res, command): ## same with scan_formatter
-    return [int(res[0]), format_sorted_set_return(res[1])] 
+
+def zscan_formatter(res, command):  ## same with scan_formatter
+    return [int(res[0]), format_sorted_set_return(res[1])]
+
 
 def zscore_formatter(res, command):
     return float(res) if res is not None else res
 
+
 def georadius_formatter(res, command):
-    withdist = "WITHDIST" in command 
+    withdist = "WITHDIST" in command
     withhash = "WITHHASH" in command
     withcoord = "WITHCOORD" in command
     if withdist or withhash or withcoord:
         return format_geo_members_return(res, withdist, withhash, withcoord)
 
     return res
 
+
 def hrandfield_formatter(res, command):
     withvalues = "WITHVALUES" in command
     if withvalues:
         return format_hash_return(res)
 
     return res
 
+
 def zadd_formatter(res, command):
     incr = "INCR" in command
     if incr:
         return float(res) if res is not None else res
 
     return res
 
+
 def zdiff_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zinter_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zrandmember_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zrange_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zrangebyscore_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zrevrange_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zrevrangebyscore_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
 
+
 def zunion_formatter(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
-    
+
     return res
-    
+
+
 class FormattedResponse:
     FORMATTERS = {
         "COPY": to_bool,
         "EXPIRE": to_bool,
         "EXPIREAT": to_bool,
         "PERSIST": to_bool,
         "PEXPIRE": to_bool,
         "PEXPIREAT": to_bool,
         "RENAMENX": to_bool,
         "SCAN": scan_formatter,
         "GEODIST": to_float,
         "GEOPOS": format_geo_positions_return,
         "GEORADIUS": georadius_formatter,
-        "GEORADIUS_RO": georadius_formatter, # same with the georadius, missing tests
-        "GEORADIUSBYMEMBER": georadius_formatter, # same with the georadius, missing tests
-        "GEORADIUSBYMEMBER_RO": georadius_formatter, # same with the georadius, missing tests
-        "GEOSEARCH": georadius_formatter, # same with the georadius, missing tests
-        "HEXISTS": to_bool, # missing test
-        "HGETALL": format_hash_return, # missing test
-        "HINCRBYFLOAT": to_float, # missing test
-        "HRANDFIELD": hrandfield_formatter, # missing test
-        "HSCAN": hscan_formatter, # missing test
-        "HSETNX": to_bool, # missing test
+        "GEORADIUS_RO": georadius_formatter,  # same with the georadius, missing tests
+        "GEORADIUSBYMEMBER": georadius_formatter,  # same with the georadius, missing tests
+        "GEORADIUSBYMEMBER_RO": georadius_formatter,  # same with the georadius, missing tests
+        "GEOSEARCH": georadius_formatter,  # same with the georadius, missing tests
+        "HEXISTS": to_bool,  # missing test
+        "HGETALL": format_hash_return,  # missing test
+        "HINCRBYFLOAT": to_float,  # missing test
+        "HRANDFIELD": hrandfield_formatter,  # missing test
+        "HSCAN": hscan_formatter,  # missing test
+        "HSETNX": to_bool,  # missing test
         "PFADD": to_bool,
-        "TIME": format_server_time_return, # missing test
-        "SISMEMBER": to_bool, # missing test
-        "SMOVE": to_bool, # missing test
-        "SSCAN": sscan_formatter, # missing test
-        "ZADD": zadd_formatter, # missing test
-        "ZDIFF": zdiff_formatter, # missing test
-        "ZINCRBY": to_float, # missing test
-        "ZINTER": zinter_formatter, # missing test
-        "ZMSCORE": format_float_list, # missing test
-        "ZPOPMAX": format_sorted_set_return, # missing test
-        "ZPOPMIN": format_sorted_set_return, # missing test
-        "ZRANDMEMBER": zrandmember_formatter, # missing test
-        "ZRANGE": zrange_formatter, # missing test
-        "ZRANGEBYSCORE": zrangebyscore_formatter, # missing test
-        "ZREVRANGE": zrevrange_formatter, # missing test
-        "ZREVRANGEBYSCORE": zrevrangebyscore_formatter, # missing test
-        "ZSCAN": zscan_formatter, # missing test
-        "ZSCORE": zscore_formatter, # missing test
-        "ZUNION": zunion_formatter, # missing test
-        "INCRBYFLOAT": to_float, # missing test
+        "TIME": format_server_time_return,  # missing test
+        "SISMEMBER": to_bool,  # missing test
+        "SMISMEMBER": list_to_bool_list,
+        "SMOVE": to_bool,  # missing test
+        "SSCAN": sscan_formatter,  # missing test
+        "ZADD": zadd_formatter,  # missing test
+        "ZDIFF": zdiff_formatter,  # missing test
+        "ZINCRBY": to_float,  # missing test
+        "ZINTER": zinter_formatter,  # missing test
+        "ZMSCORE": format_float_list,  # missing test
+        "ZPOPMAX": format_sorted_set_return,  # missing test
+        "ZPOPMIN": format_sorted_set_return,  # missing test
+        "ZRANDMEMBER": zrandmember_formatter,  # missing test
+        "ZRANGE": zrange_formatter,  # missing test
+        "ZRANGEBYSCORE": zrangebyscore_formatter,  # missing test
+        "ZREVRANGE": zrevrange_formatter,  # missing test
+        "ZREVRANGEBYSCORE": zrevrangebyscore_formatter,  # missing test
+        "ZSCAN": zscan_formatter,  # missing test
+        "ZSCORE": zscore_formatter,  # missing test
+        "ZUNION": zunion_formatter,  # missing test
+        "INCRBYFLOAT": to_float,  # missing test
         "PUBSUB NUMSUB": _list_to_dict,
-        "SCRIPT EXISTS": format_bool_list, # missing test
-
+        "SCRIPT EXISTS": format_bool_list,  # missing test
         "FLUSHALL": ok_to_bool,
         "FLUSHDB": ok_to_bool,
         "MSETNX": to_bool,
         "PSETEX": ok_to_bool,
         "SET": ok_to_bool,
         "SETEX": ok_to_bool,
         "SETNX": to_bool,
         "HMSET": ok_to_bool,
-
         "SMEMBERS": to_set,
         "SDIFF": to_set,
         "SINTER": to_set,
         "SUNION": to_set,
+        "SCRIPT FLUSH": ok_to_bool,
+        "SCRIPT EXISTS": list_to_bool_list,
     }
 
     # TODO: Check return_cursor stuff.
     # TODO: lots of duplicate formatters. unite them
     # TODO: all formatters should take `command` parameter
-    # TODO: check commands using format_sorted_set_return
+    # TODO: check commands using format_sorted_set_return
```

### Comparing `upstash_redis-0.13.3/PKG-INFO` & `upstash_redis-0.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.13.3
+Version: 0.14.0
 Summary: Serverless Redis Sdk from Upstash
 Author: Upstash
 Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


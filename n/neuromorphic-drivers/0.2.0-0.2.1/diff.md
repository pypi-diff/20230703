# Comparing `tmp/neuromorphic_drivers-0.2.0.tar.gz` & `tmp/neuromorphic_drivers-0.2.1.tar.gz`

## Comparing `neuromorphic_drivers-0.2.0.tar` & `neuromorphic_drivers-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/Cargo.toml
--rw-r--r--   0     1001      123    18887 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/de.rs
--rw-r--r--   0     1001      123     5021 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/error.rs
--rw-r--r--   0     1001      123    25754 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/format.rs
--rw-r--r--   0     1001      123    14340 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/lib.rs
--rw-r--r--   0     1001      123    14435 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/ser.rs
--rw-r--r--   0     1001      123    11374 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/trace.rs
--rw-r--r--   0     1001      123    10825 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/value.rs
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123       58 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1102 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/LICENSE
--rw-r--r--   0     1001      123      115 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/README.md
--rw-r--r--   0     1001      123    34780 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/build.rs
--rw-r--r--   0     1001      123      948 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123     2765 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/__init__.py
--rw-r--r--   0     1001      123      802 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/device.py
--rw-r--r--   0     1001      123     5842 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
--rw-r--r--   0     1001      123     6204 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
--rw-r--r--   0     1001      123     8330 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices_types.py
--rw-r--r--   0     1001      123      400 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/enums.py
--rw-r--r--   0     1001      123      680 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/unions.py
--rw-r--r--   0     1001      123     4481 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/mask.py
--rw-r--r--   0     1001      123       91 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/__init__.py
--rw-r--r--   0     1001      123    15358 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/binary.py
--rw-r--r--   0     1001      123     2296 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/bincode.py
--rw-r--r--   0     1001      123     1547 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/type.py
--rw-r--r--   0     1001      123     1091 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/status.py
--rw-r--r--   0     1001      123     1858 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/udev.py
--rw-r--r--   0     1001      123     4497 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/adapters.rs
--rw-r--r--   0     1001      123     1675 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/bytes.rs
--rw-r--r--   0     1001      123    14237 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     4091 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/structured_array.rs
--rw-r--r--   0     1001      123     6177 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/display.py
--rw-r--r--   0     1001      123     1961 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/external_synchronization.py
--rw-r--r--   0     1001      123      608 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/read_many.py
--rw-r--r--   0     1001      123      583 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/record_raw.py
--rw-r--r--   0     1001      123      336 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/test.py
--rw-r--r--   0     1001      123    19206 2023-07-02 21:13:23.000000 neuromorphic_drivers-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/Cargo.toml
+-rw-r--r--   0     1001      123    18887 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/de.rs
+-rw-r--r--   0     1001      123     5021 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/error.rs
+-rw-r--r--   0     1001      123    25754 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/format.rs
+-rw-r--r--   0     1001      123    14340 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/lib.rs
+-rw-r--r--   0     1001      123    14435 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/ser.rs
+-rw-r--r--   0     1001      123    11374 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/trace.rs
+-rw-r--r--   0     1001      123    10825 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/value.rs
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123       41 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/.gitignore
+-rw-r--r--   0     1001      123     1102 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/LICENSE
+-rw-r--r--   0     1001      123      115 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/README.md
+-rw-r--r--   0     1001      123    34780 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/build.rs
+-rw-r--r--   0     1001      123     1031 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123     2765 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/__init__.py
+-rw-r--r--   0     1001      123      802 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/device.py
+-rw-r--r--   0     1001      123     5781 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
+-rw-r--r--   0     1001      123     6143 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
+-rw-r--r--   0     1001      123     8269 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices_types.py
+-rw-r--r--   0     1001      123      400 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/enums.py
+-rw-r--r--   0     1001      123      701 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/unions.py
+-rw-r--r--   0     1001      123     4481 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/mask.py
+-rw-r--r--   0     1001      123       91 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/__init__.py
+-rw-r--r--   0     1001      123    15358 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/binary.py
+-rw-r--r--   0     1001      123     2296 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/bincode.py
+-rw-r--r--   0     1001      123     1547 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/type.py
+-rw-r--r--   0     1001      123     1091 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/status.py
+-rw-r--r--   0     1001      123     1858 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/udev.py
+-rw-r--r--   0     1001      123     4497 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/adapters.rs
+-rw-r--r--   0     1001      123     1675 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/bytes.rs
+-rw-r--r--   0     1001      123    14237 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     4091 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/src/structured_array.rs
+-rw-r--r--   0     1001      123     6177 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/display.py
+-rw-r--r--   0     1001      123     1961 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/external_synchronization.py
+-rw-r--r--   0     1001      123      608 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/read_many.py
+-rw-r--r--   0     1001      123      687 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/record_raw.py
+-rw-r--r--   0     1001      123      336 2023-07-02 23:55:56.000000 neuromorphic_drivers-0.2.1/tests/test.py
+-rw-r--r--   0     1001      123    19206 2023-07-02 23:56:13.000000 neuromorphic_drivers-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.1/PKG-INFO
```

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/de.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/de.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/error.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/error.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/format.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/format.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/lib.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/ser.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/ser.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/trace.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/trace.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/value.rs` & `neuromorphic_drivers-0.2.1/local_dependencies/reflect/src/value.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/LICENSE` & `neuromorphic_drivers-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/build.rs` & `neuromorphic_drivers-0.2.1/build.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/pyproject.toml` & `neuromorphic_drivers-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Neuromorphic devices drivers"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "International Centre for Neuromorphic Systems"},
     {name = "Alexandre Marcireau"},
 ]
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.8"
 dependencies = ["numpy>=1.24"]
 
 [project.urls]
 homepage = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 repository = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 documentation = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
@@ -20,20 +20,19 @@
 requires = ["maturin>=0.12", "numpy"]
 build-backend = "maturin"
 
 [tool.maturin]
 python-source = "python"
 
 [tool.black]
-extend-exclude = ".venv"
+extend-exclude = "python/neuromorphic_drivers/generated"
 
 [tool.pyright]
 typeCheckingMode = "basic"
-executionEnvironments = [
-    {root=".", venv=".venv"},
-]
+executionEnvironments = [{root = ".", venv = ".venv"}]
 
 [tool.isort]
 profile = "black"
+extend_skip = "python/neuromorphic_drivers/generated"
 
 [project.scripts]
 neuromorphic-drivers-install-udev-rules = "neuromorphic_drivers:install_udev_rules"
```

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/__init__.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/device.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/device.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,48 @@
 import dataclasses
 import enum
 import types
 import typing
 
 import numpy
 
-from ... import serde, status
+from ... import serde
+from ... import status
 from .. import enums
 
 
 @dataclasses.dataclass
 class Biases:
-    pr: serde.type.uint8 = 0x69
-    fo_p: serde.type.uint8 = 0x4A
-    fo_n: serde.type.uint8 = 0x00
+    pr: serde.type.uint8 = 0x7C
+    fo: serde.type.uint8 = 0x53
     hpf: serde.type.uint8 = 0x00
-    diff_on: serde.type.uint8 = 0x73
-    diff: serde.type.uint8 = 0x50
-    diff_off: serde.type.uint8 = 0x34
-    refr: serde.type.uint8 = 0x44
-    reqpuy: serde.type.uint8 = 0x94
-    blk: serde.type.uint8 = 0x78
+    diff_on: serde.type.uint8 = 0x66
+    diff: serde.type.uint8 = 0x4D
+    diff_off: serde.type.uint8 = 0x49
+    inv: serde.type.uint8 = 0x5B
+    refr: serde.type.uint8 = 0x14
+    reqpuy: serde.type.uint8 = 0x8C
+    reqpux: serde.type.uint8 = 0x7C
+    sendreqpdy: serde.type.uint8 = 0x94
+    unknown_1: serde.type.uint8 = 0x74
+    unknown_2: serde.type.uint8 = 0x51
 
     def serialize(self) -> bytes:
         return serde.bincode.serialize(self, Biases)
 
 
+class Clock(enum.Enum):
+    INTERNAL = 0
+    INTERNAL_WITH_OUTPUT_ENABLED = 1
+    EXTERNAL = 2
+
+    def serialize(self) -> bytes:
+        return serde.bincode.serialize(self, Clock)
+
+
 @dataclasses.dataclass
 class RateLimiter:
     reference_period_us: serde.type.uint16
     maximum_events_per_period: serde.type.uint32
 
     def serialize(self) -> bytes:
         return serde.bincode.serialize(self, RateLimiter)
@@ -73,22 +86,24 @@
         serde.type.uint64,
         serde.type.uint64,
         serde.type.uint64,
         serde.type.uint64,
         serde.type.uint64,
     ] = (0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0)
     mask_intersection_only: bool = False
+    enable_external_trigger: bool = True
+    clock: Clock = Clock.INTERNAL
     rate_limiter: typing.Optional[RateLimiter] = None
 
     def serialize(self) -> bytes:
         return serde.bincode.serialize(self, Configuration)
 
     @staticmethod
     def type() -> str:
-        return "prophesee_evk3_hd"
+        return "prophesee_evk4"
 
 
 @dataclasses.dataclass
 class UsbConfiguration:
     buffer_size: serde.type.uint64 = 131072
     ring_size: serde.type.uint64 = 4096
     transfer_queue_size: serde.type.uint64 = 32
@@ -115,26 +130,21 @@
         traceback: typing.Optional[types.TracebackType],
     ) -> bool:
         ...
 
     def __iter__(self) -> "Device":
         ...
 
-    def __next__(
-        self,
-    ) -> tuple[
-        status.StatusNonOptional,
-        dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]],
-    ]:
+    def __next__(self) -> tuple[status.StatusNonOptional, dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
@@ -154,26 +164,21 @@
         traceback: typing.Optional[types.TracebackType],
     ) -> bool:
         ...
 
     def __iter__(self) -> "DeviceOptional":
         ...
 
-    def __next__(
-        self,
-    ) -> tuple[
-        status.Status,
-        typing.Optional[dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]],
-    ]:
+    def __next__(self) -> tuple[status.Status, typing.Optional[dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
@@ -199,15 +204,15 @@
 
     def __next__(self) -> tuple[status.StatusNonOptional, bytes]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
@@ -233,15 +238,15 @@
 
     def __next__(self) -> tuple[status.Status, typing.Optional[bytes]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
```

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,47 +3,36 @@
 import dataclasses
 import enum
 import types
 import typing
 
 import numpy
 
-from ... import serde, status
+from ... import serde
+from ... import status
 from .. import enums
 
 
 @dataclasses.dataclass
 class Biases:
-    pr: serde.type.uint8 = 0x7C
-    fo: serde.type.uint8 = 0x53
+    pr: serde.type.uint8 = 0x69
+    fo_p: serde.type.uint8 = 0x4A
+    fo_n: serde.type.uint8 = 0x00
     hpf: serde.type.uint8 = 0x00
-    diff_on: serde.type.uint8 = 0x66
-    diff: serde.type.uint8 = 0x4D
-    diff_off: serde.type.uint8 = 0x49
-    inv: serde.type.uint8 = 0x5B
-    refr: serde.type.uint8 = 0x14
-    reqpuy: serde.type.uint8 = 0x8C
-    reqpux: serde.type.uint8 = 0x7C
-    sendreqpdy: serde.type.uint8 = 0x94
-    unknown_1: serde.type.uint8 = 0x74
-    unknown_2: serde.type.uint8 = 0x51
+    diff_on: serde.type.uint8 = 0x73
+    diff: serde.type.uint8 = 0x50
+    diff_off: serde.type.uint8 = 0x34
+    refr: serde.type.uint8 = 0x44
+    reqpuy: serde.type.uint8 = 0x94
+    blk: serde.type.uint8 = 0x78
 
     def serialize(self) -> bytes:
         return serde.bincode.serialize(self, Biases)
 
 
-class Clock(enum.Enum):
-    INTERNAL = 0
-    INTERNAL_WITH_OUTPUT_ENABLED = 1
-    EXTERNAL = 2
-
-    def serialize(self) -> bytes:
-        return serde.bincode.serialize(self, Clock)
-
-
 @dataclasses.dataclass
 class RateLimiter:
     reference_period_us: serde.type.uint16
     maximum_events_per_period: serde.type.uint32
 
     def serialize(self) -> bytes:
         return serde.bincode.serialize(self, RateLimiter)
@@ -85,24 +74,22 @@
         serde.type.uint64,
         serde.type.uint64,
         serde.type.uint64,
         serde.type.uint64,
         serde.type.uint64,
     ] = (0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0)
     mask_intersection_only: bool = False
-    enable_external_trigger: bool = True
-    clock: Clock = Clock.INTERNAL
     rate_limiter: typing.Optional[RateLimiter] = None
 
     def serialize(self) -> bytes:
         return serde.bincode.serialize(self, Configuration)
 
     @staticmethod
     def type() -> str:
-        return "prophesee_evk4"
+        return "prophesee_evk3_hd"
 
 
 @dataclasses.dataclass
 class UsbConfiguration:
     buffer_size: serde.type.uint64 = 131072
     ring_size: serde.type.uint64 = 4096
     transfer_queue_size: serde.type.uint64 = 32
@@ -129,26 +116,21 @@
         traceback: typing.Optional[types.TracebackType],
     ) -> bool:
         ...
 
     def __iter__(self) -> "Device":
         ...
 
-    def __next__(
-        self,
-    ) -> tuple[
-        status.StatusNonOptional,
-        dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]],
-    ]:
+    def __next__(self) -> tuple[status.StatusNonOptional, dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
@@ -168,26 +150,21 @@
         traceback: typing.Optional[types.TracebackType],
     ) -> bool:
         ...
 
     def __iter__(self) -> "DeviceOptional":
         ...
 
-    def __next__(
-        self,
-    ) -> tuple[
-        status.Status,
-        typing.Optional[dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]],
-    ]:
+    def __next__(self) -> tuple[status.Status, typing.Optional[dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
@@ -213,15 +190,15 @@
 
     def __next__(self) -> tuple[status.StatusNonOptional, bytes]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
@@ -247,15 +224,15 @@
 
     def __next__(self) -> tuple[status.Status, typing.Optional[bytes]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
-    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK4]:
+    def name(self) -> typing.Literal[enums.Name.PROPHESEE_EVK3_HD]:
         ...
 
     def properties(self) -> Properties:
         ...
 
     def serial(self) -> str:
         ...
```

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices_types.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/devices_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import types
 import typing
 
 import numpy
 
-from .. import device, status
+from .. import device
+from .. import status
 from .devices import prophesee_evk3_hd as prophesee_evk3_hd
 from .devices import prophesee_evk4 as prophesee_evk4
 from .enums import *
 from .unions import *
 
 
+
 class GenericDevice(typing.Protocol):
     def __enter__(self) -> "GenericDevice":
         ...
 
     def __exit__(
         self,
         exception_type: typing.Optional[typing.Type[BaseException]],
@@ -23,20 +25,15 @@
         traceback: typing.Optional[types.TracebackType],
     ) -> bool:
         ...
 
     def __iter__(self) -> "GenericDevice":
         ...
 
-    def __next__(
-        self,
-    ) -> tuple[
-        status.StatusNonOptional,
-        dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]],
-    ]:
+    def __next__(self) -> tuple[status.StatusNonOptional, dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
     def name(self) -> Name:
         ...
@@ -62,20 +59,15 @@
         traceback: typing.Optional[types.TracebackType],
     ) -> bool:
         ...
 
     def __iter__(self) -> "GenericDeviceOptional":
         ...
 
-    def __next__(
-        self,
-    ) -> tuple[
-        status.Status,
-        typing.Optional[dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]],
-    ]:
+    def __next__(self) -> tuple[status.Status, typing.Optional[dict[str, numpy.ndarray[typing.Any, numpy.dtype[numpy.void]]]]]:
         ...
 
     def clear_backlog(self, until: int):
         ...
 
     def name(self) -> Name:
         ...
```

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/unions.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/generated/unions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import typing
 
 from . import enums
-from .devices import prophesee_evk3_hd, prophesee_evk4
+from .devices import prophesee_evk3_hd
+from .devices import prophesee_evk4
+
 
 Properties = typing.Union[
     prophesee_evk3_hd.Properties,
     prophesee_evk4.Properties,
 ]
 
 Configuration = typing.Union[
```

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/mask.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/mask.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/binary.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/binary.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/bincode.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/bincode.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/type.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/serde/type.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/status.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/status.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/udev.py` & `neuromorphic_drivers-0.2.1/python/neuromorphic_drivers/udev.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/src/adapters.rs` & `neuromorphic_drivers-0.2.1/src/adapters.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/src/bytes.rs` & `neuromorphic_drivers-0.2.1/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/src/lib.rs` & `neuromorphic_drivers-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/src/structured_array.rs` & `neuromorphic_drivers-0.2.1/src/structured_array.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/tests/display.py` & `neuromorphic_drivers-0.2.1/tests/display.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/tests/external_synchronization.py` & `neuromorphic_drivers-0.2.1/tests/external_synchronization.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/tests/read_many.py` & `neuromorphic_drivers-0.2.1/tests/read_many.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.0/Cargo.lock` & `neuromorphic_drivers-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "bincode",
  "cc",
  "neuromorphic-drivers 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "numpy",
  "paste",
  "pyo3",
```

### Comparing `neuromorphic_drivers-0.2.0/PKG-INFO` & `neuromorphic_drivers-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromorphic_drivers
-Version: 0.2.0
+Version: 0.2.1
 Requires-Dist: numpy >=1.24
 License-File: LICENSE
 Summary: Neuromorphic devices drivers
 Author: International Centre for Neuromorphic Systems, Alexandre Marcireau
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/neuromorphicsystems/neuromorphic-rs/
```


# Comparing `tmp/ltcodecs-0.2.0.tar.gz` & `tmp/ltcodecs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltcodecs-0.2.0.tar", last modified: Tue Dec  6 19:01:56 2022, max compression
+gzip compressed data, was "ltcodecs-1.0.0.tar", last modified: Mon Jul  3 19:18:21 2023, max compression
```

## Comparing `ltcodecs-0.2.0.tar` & `ltcodecs-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 19:01:56.520509 ltcodecs-0.2.0/
--rw-rw-rw-   0        0        0     7651 2021-10-03 02:56:16.000000 ltcodecs-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      679 2022-12-06 19:01:56.520509 ltcodecs-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       92 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/README.md
--rw-rw-rw-   0        0        0      103 2021-10-03 02:56:16.000000 ltcodecs-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      752 2022-12-06 19:01:56.522509 ltcodecs-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-06 19:01:56.463515 ltcodecs-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-12-06 19:01:56.514512 ltcodecs-0.2.0/src/ltcodecs/
--rw-rw-rw-   0        0        0     2765 2022-12-06 18:58:16.000000 ltcodecs-0.2.0/src/ltcodecs/__init__.py
--rw-rw-rw-   0        0        0      517 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/bool_codec.py
--rw-rw-rw-   0        0        0      962 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/bytes_codec.py
--rw-rw-rw-   0        0        0     1515 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/ccl_latlon_bcd_codec.py
--rw-rw-rw-   0        0        0      689 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/ccl_latlon_codec.py
--rw-rw-rw-   0        0        0      376 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/field_codec.py
--rw-rw-rw-   0        0        0     1397 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/fixed_len_array_codec.py
--rw-rw-rw-   0        0        0     1888 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/fixedint_codec.py
--rw-rw-rw-   0        0        0     1542 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/float_codec.py
--rw-rw-rw-   0        0        0     1225 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/ieee_float_codec.py
--rw-rw-rw-   0        0        0     2540 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/linspace_float_codec.py
--rw-rw-rw-   0        0        0      595 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/padding_codec.py
--rw-rw-rw-   0        0        0     4311 2022-09-17 00:03:24.000000 ltcodecs-0.2.0/src/ltcodecs/ros_message_codec.py
--rw-rw-rw-   0        0        0     7716 2022-09-17 00:58:04.000000 ltcodecs-0.2.0/src/ltcodecs/ros_msg_field_codec.py
--rw-rw-rw-   0        0        0     1596 2022-09-16 23:13:06.000000 ltcodecs-0.2.0/src/ltcodecs/rostime_codec.py
--rw-rw-rw-   0        0        0     3459 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/string_codecs.py
--rw-rw-rw-   0        0        0     1903 2022-09-29 22:38:56.000000 ltcodecs-0.2.0/src/ltcodecs/string_enum_codec.py
--rw-rw-rw-   0        0        0     1737 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/variable_len_array_codec.py
--rw-rw-rw-   0        0        0     2224 2021-12-13 18:44:37.000000 ltcodecs-0.2.0/src/ltcodecs/varint_codec.py
-drwxrwxrwx   0        0        0        0 2022-12-06 19:01:56.519509 ltcodecs-0.2.0/src/ltcodecs.egg-info/
--rw-rw-rw-   0        0        0      679 2022-12-06 19:01:56.000000 ltcodecs-0.2.0/src/ltcodecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-12-06 19:01:56.000000 ltcodecs-0.2.0/src/ltcodecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-06 19:01:56.000000 ltcodecs-0.2.0/src/ltcodecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-06 19:01:56.000000 ltcodecs-0.2.0/src/ltcodecs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:18:21.399884 ltcodecs-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      661 2023-07-03 19:18:21.399884 ltcodecs-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-07-03 19:18:21.399884 ltcodecs-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:18:21.395884 ltcodecs-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:18:21.399884 ltcodecs-1.0.0/src/ltcodecs/
+-rw-rw-rw-   0 root         (0) root         (0)     2210 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/bool_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-07 21:37:10.000000 ltcodecs-1.0.0/src/ltcodecs/bytes_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/ccl_latlon_bcd_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/ccl_latlon_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/field_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/fixed_len_array_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2369 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/fixedint_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/float_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/ieee_float_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/linspace_float_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-09 15:34:23.000000 ltcodecs-1.0.0/src/ltcodecs/lzma_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/padding_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-06-07 17:55:48.000000 ltcodecs-1.0.0/src/ltcodecs/ros_message_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/ros_msg_field_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-06-07 20:48:56.000000 ltcodecs-1.0.0/src/ltcodecs/rostime_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/string_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/string_enum_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/variable_len_array_codec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2023-06-06 18:19:18.000000 ltcodecs-1.0.0/src/ltcodecs/varint_codec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:18:21.399884 ltcodecs-1.0.0/src/ltcodecs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-07-03 19:18:21.000000 ltcodecs-1.0.0/src/ltcodecs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      870 2023-07-03 19:18:21.000000 ltcodecs-1.0.0/src/ltcodecs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 19:18:21.000000 ltcodecs-1.0.0/src/ltcodecs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 19:18:21.000000 ltcodecs-1.0.0/src/ltcodecs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:18:21.399884 ltcodecs-1.0.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    10389 2023-06-21 15:43:47.000000 ltcodecs-1.0.0/tests/test_codecs.py
```

### Comparing `ltcodecs-0.2.0/LICENSE` & `ltcodecs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ltcodecs-0.2.0/PKG-INFO` & `ltcodecs-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: ltcodecs
-Version: 0.2.0
-Summary: LT Codecs
-Home-page: https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
-Author: whoi
-Author-email: egallimore@whoi.edu
-Project-URL: Bug Tracker, https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# LT Codecs
-
-The package was original part of ros_acomms under the field_codecs directory. 
+Metadata-Version: 2.1
+Name: ltcodecs
+Version: 1.0.0
+Summary: LT Codecs
+Home-page: https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
+Author: whoi
+Author-email: egallimore@whoi.edu
+Project-URL: Bug Tracker, https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LT Codecs
+
+The package was original part of ros_acomms under the field_codecs directory.
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/__init__.py` & `ltcodecs-1.0.0/src/ltcodecs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,51 +13,55 @@
 from .fixed_len_array_codec import FixedLenArrayCodec
 from .ros_msg_field_codec import RosMsgFieldCodec
 from .ccl_latlon_codec import CclLatLonCodec
 from .ccl_latlon_bcd_codec import CclLatLonBcdCodec
 from .padding_codec import PaddingCodec
 from .rostime_codec import RosTimeCodec
 from .ros_message_codec import RosMessageCodec
+from .lzma_codec import LzmaCodec
+from .exceptions import EncodingFailed
 
+field_codec_classes = {
+    "integer": VarintCodec,
+    "fixedint": FixedIntCodec,
+    "varint": VarintCodec,
+    "float": FloatCodec,
+    "linspace_float": LinspaceFloatCodec,
+    "linspace": LinspaceFloatCodec,
+    "uint8": UInt8Codec,
+    "uint16": UInt16Codec,
+    "uint32": UInt32Codec,
+    "uint64": UInt64Codec,
+    "int8": Int8Codec,
+    "int16": Int16Codec,
+    "int32": Int32Codec,
+    "int64": Int64Codec,
+    "float32": IeeeFloat32Codec,
+    "float64": IeeeFloat64Codec,
+    "bool": BoolCodec,
+    "string": AsciiStringCodec,
+    "ascii": AsciiStringCodec,
+    "bytes": BytesCodec,
+    "msg": RosMsgFieldCodec,
+    "ros_msg": RosMsgFieldCodec,
+    "variable_len_array": VariableLenArrayCodec,
+    "fixed_len_array": FixedLenArrayCodec,
+    "ccl_latlon": CclLatLonCodec,
+    "ccl_latlon_bcd": CclLatLonBcdCodec,
+    "pad": PaddingCodec,
+    "padding": PaddingCodec,
+    "time": RosTimeCodec,
+    "rostime": RosTimeCodec,
+    "string_enum": StringEnumCodec,
+    "lzma": LzmaCodec,
+}
+
+metadata_decoders = {
+    "src": "packet.src",
+    "dest": "packet.dest",
+    "dest_decoder": "packet.dest",
+    "toa": "cst.toa",
+    "snr_in": "cst.snr_in",
+}
 
-field_codec_classes = {'integer': VarintCodec,
-                       'fixedint': FixedIntCodec,
-                       'varint': VarintCodec,
-                       'float': FloatCodec,
-                       'linspace_float': LinspaceFloatCodec,
-                       'linspace': LinspaceFloatCodec,
-                       'uint8': UInt8Codec,
-                       'uint16': UInt16Codec,
-                       'uint32': UInt32Codec,
-                       'uint64': UInt64Codec,
-                       'int8': Int8Codec,
-                       'int16': Int16Codec,
-                       'int32': Int32Codec,
-                       'int64': Int64Codec,
-                       'float32': IeeeFloat32Codec,
-                       'float64': IeeeFloat64Codec,
-                       'bool': BoolCodec,
-                       'string': AsciiStringCodec,
-                       'ascii': AsciiStringCodec,
-                       'bytes': BytesCodec,
-                       'msg': RosMsgFieldCodec,
-                       'ros_msg': RosMsgFieldCodec,
-                       'variable_len_array': VariableLenArrayCodec,
-                       'fixed_len_array': FixedLenArrayCodec,
-                       'ccl_latlon': CclLatLonCodec,
-                       'ccl_latlon_bcd': CclLatLonBcdCodec,
-                       'pad': PaddingCodec,
-                       'padding': PaddingCodec,
-                       'time': RosTimeCodec,
-                       'rostime': RosTimeCodec,
-                       'string_enum': StringEnumCodec,
-                       }
-
-metadata_decoders = {'src': 'packet.src',
-                     'dest': 'packet.dest',
-                     'dest_decoder': 'packet.dest',
-                     'toa': 'cst.toa',
-                     'snr_in': 'cst.snr_in'}
-
-
-metadata_encoders = {'dest': 'packet.dest'}
 
+metadata_encoders = {"dest": "packet.dest"}
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/ccl_latlon_bcd_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/ccl_latlon_bcd_codec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,56 @@
+"""
+ltcodecs.ccl_latlon_bcd_codec
+-----------------------------
+
+This module contains the the ccl latlon bcd codec
+"""
+
+from __future__ import annotations
 from bitstring import ConstBitStream, Bits
 from .field_codec import FieldCodec
 from math import modf, copysign
 
 
 class CclLatLonBcdCodec(FieldCodec):
-    ''' This codec is horrifically inefficient, but included for compatibility with messages like MDAT_RANGER '''
+    """This codec is horrifically inefficient, but included for compatibility with messages like MDAT_RANGER"""
+
     def __init__(self, lat_not_lon=True, **kwargs):
         self.lat_not_lon = lat_not_lon
-        pass
 
-    def encode(self, value: float):
+    def encode(self, value: float) -> tuple[Bits, float]:
         sign = copysign(1, value)
         abs_value = abs(value)
         frac, degrees = modf(abs_value)
         degrees = int(degrees)
         minutes = frac * 60
         dec_min = int(minutes * 10000)
 
         if self.lat_not_lon:
-            sign_char = 'a' if sign > 0 else 'c'
+            sign_char = "a" if sign > 0 else "c"
         else:
-            sign_char = 'b' if sign > 0 else 'd'
+            sign_char = "b" if sign > 0 else "d"
 
-        hex_string = "{:03d}{}{:06d}".format(degrees, sign_char, dec_min)
+        hex_string = f"{degrees:03d}{sign_char}{dec_min:06d}"
         encoded_value = sign * (degrees + (dec_min / 10000) / 60)
         encoded_bits = Bits(hex=hex_string)
 
         return encoded_bits, encoded_value
 
-    def decode(self, bits_to_decode: ConstBitStream):
-        string_bytes = bits_to_decode.read('bytes:5')
-        hex_string = ''.join('{:02x}'.format(x) for x in string_bytes)
+    def decode(self, bits_to_decode: ConstBitStream) -> float:
+        string_bytes = bits_to_decode.read("bytes:5")
+        hex_string = "".join(f"{x:02x}" for x in string_bytes)
 
         degrees = int(hex_string[0:3])
-        direction = 1 if hex_string[3] in ('a', 'b') else -1
-        minutes = float(hex_string[4:10]) / 10000.
+        direction = 1 if hex_string[3] in ("a", "b") else -1
+        minutes = float(hex_string[4:10]) / 10000.0
 
         value = direction * (degrees + (minutes / 60))
         return value
 
     @property
-    def max_length_bits(self):
+    def max_length_bits(self) -> int:
         return 40
 
     @property
-    def min_length_bits(self):
-        return 40
+    def min_length_bits(self) -> int:
+        return 40
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/fixed_len_array_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/variable_len_array_codec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,73 @@
+"""
+variable_len_array_codec.py
+---------------------------
+
+module for VariableLenArrayCodec
+"""
+
+from __future__ import annotations
+from typing import Any
 from bitstring import BitArray, ConstBitStream
 from .field_codec import FieldCodec
+from .varint_codec import VarintCodec
 import ltcodecs as ltcodecs
-from typing import List
+from .exceptions import EncodingFailed
 
 
-class FixedLenArrayCodec(FieldCodec):
-    def __init__(self, element_type: str, length: int, element_params=None, **kwargs):
-        self.length = length
+class VariableLenArrayCodec(FieldCodec):
+    """
+    codec for variable-length array
+    """
+
+    def __init__(
+        self, element_type: str, max_length: int, element_params=None, **kwargs
+    ) -> None:
+        self.max_length = max_length
+        self.length_codec = VarintCodec(min_value=0, max_value=self.max_length)
+        print("element_type", element_type)
         if element_params:
-            self.element_field_codec = ltcodecs.field_codec_classes[element_type](**element_params)
+            self.element_field_codec = ltcodecs.field_codec_classes[element_type](
+                **element_params
+            )
         else:
             self.element_field_codec = ltcodecs.field_codec_classes[element_type]()
 
-    def encode(self, value: List):
-        value = value[0:self.length]
-        value_bits = BitArray()
+    def encode(self, value: list) -> tuple[BitArray, list[Any]]:
+        """
+        encodes list of elements
+        """
+
+        value = value[0 : self.max_length]
+        length_bits, _ = self.length_codec.encode(len(value))
+        value_bits = BitArray(length_bits)
         encoded_value_list = []
         for element in value:
-            element_bits, element_value = self.element_field_codec.encode(element)
+            (
+                element_bits,
+                element_value,
+            ) = self.element_field_codec.encode(element)
+
             value_bits.append(element_bits)
             encoded_value_list.append(element_value)
         return value_bits, encoded_value_list
 
-    def decode(self, bits_to_decode: ConstBitStream):
+    def decode(self, bits_to_decode: ConstBitStream) -> list:
+        """
+        decodes list of elements from bits
+        """
+        num_elements = self.length_codec.decode(bits_to_decode)
         decoded_list = []
-        for i in range(self.length):
+        for i in range(num_elements):
             element = self.element_field_codec.decode(bits_to_decode)
             decoded_list.append(element)
         return decoded_list
 
     @property
-    def min_length_bits(self):
-        return self.length * self.element_field_codec.max_length_bits
+    def min_length_bits(self) -> int:
+        return self.length_codec.max_length_bits
 
     @property
-    def max_length_bits(self):
-        return self.length * self.element_field_codec.max_length_bits
+    def max_length_bits(self) -> int:
+        return self.length_codec.max_length_bits + (
+            self.max_length * self.element_field_codec.max_length_bits
+        )
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/fixedint_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/fixedint_codec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,108 @@
-from bitstring import ConstBitStream, Bits
-from .field_codec import FieldCodec
+"""
+ltcodecs.fixedint_codec
+-----------------------
+
+This module contains classes for fixed width integer codecs
+"""
+
 from .varint_codec import VarintCodec
-from math import ceil, log2
 
 
 class FixedIntCodec(VarintCodec):
-    def __init__(self, num_bits: int, signed: bool = False, min_value: int = None, resolution: int = 1,
-                 little_endian: bool = False, **kwargs):
+    """
+    FixedIntCodec base class
+    """
+
+    def __init__(
+        self,
+        num_bits: int,
+        signed: bool = False,
+        min_value: int = None,
+        resolution: int = 1,
+        little_endian: bool = False,
+        **kwargs
+    ):
         self.num_bits = num_bits
         if min_value:
             self.min_value = int(min_value)
         else:
             if signed:
-                self.min_value = -1 * resolution * 2**(self.num_bits - 1)
+                self.min_value = -1 * resolution * 2 ** (self.num_bits - 1)
             else:
                 self.min_value = 0
         self.max_value = self.min_value + (2**self.num_bits * resolution)
         self.resolution = int(resolution)
         self.signed = signed
         self.little_endian = little_endian
 
 
-
-
 class Int8Codec(FixedIntCodec):
+    """
+    metaclass for int8 codec
+    """
+
     def __init__(self, **kwargs):
         super(Int8Codec, self).__init__(num_bits=8, signed=True)
 
 
 class Int16Codec(FixedIntCodec):
+    """
+    metaclass for int16 codec
+    """
+
     def __init__(self, **kwargs):
         super(Int16Codec, self).__init__(num_bits=16, signed=True)
 
 
 class Int32Codec(FixedIntCodec):
+    """
+    metaclass for int32 codec
+    """
+
     def __init__(self, **kwargs):
         super(Int32Codec, self).__init__(num_bits=32, signed=True)
 
 
 class Int64Codec(FixedIntCodec):
+    """
+    metaclass for int64 codec
+    """
+
     def __init__(self, **kwargs):
         super(Int64Codec, self).__init__(num_bits=64, signed=True)
 
 
 class UInt8Codec(FixedIntCodec):
+    """
+    metaclass for uint8 codec
+    """
+
     def __init__(self, **kwargs):
         super(UInt8Codec, self).__init__(num_bits=8, signed=False)
 
 
 class UInt16Codec(FixedIntCodec):
+    """
+    metaclass for uint16 codec
+    """
+
     def __init__(self, **kwargs):
         super(UInt16Codec, self).__init__(num_bits=16, signed=False)
 
 
 class UInt32Codec(FixedIntCodec):
+    """
+    metaclass for uint32 codec
+    """
+
     def __init__(self, **kwargs):
         super(UInt32Codec, self).__init__(num_bits=32, signed=False)
 
 
 class UInt64Codec(FixedIntCodec):
+    """
+    metaclass for uint64 codec
+    """
+
     def __init__(self, **kwargs):
-        super(UInt32Codec, self).__init__(num_bits=64, signed=False)
+        super(UInt32Codec, self).__init__(num_bits=64, signed=False)
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/float_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/float_codec.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,73 @@
+"""
+ltcodecs.float_codec
+-----------------------------
+
+This module contains the the float codec
+"""
+
+from __future__ import annotations
 from bitstring import ConstBitStream, Bits
 from .field_codec import FieldCodec
 from math import ceil, log2
 
 
 class FloatCodec(FieldCodec):
-    def __init__(self, min_value: float, max_value: float, precision: int, **kwargs):
+    """
+    codec for floating point numbers
+    """
+
+    def __init__(
+        self, min_value: float, max_value: float, precision: int, **kwargs
+    ) -> None:
         self.max_value = float(max_value)
         self.min_value = float(min_value)
         self.precision = int(precision)
 
-        self.value_range = int(round(max_value - min_value, precision) * 10 ** precision)
+        self.value_range = int(
+            round(max_value - min_value, precision) * 10**precision
+        )
         self.num_bits = ceil(log2(self.value_range))
-        #print("Float codec: precision {} num_bits {}".format(precision, self.num_bits))
 
-    def encode(self, value: float):
+    def encode(self, value: float) -> tuple[Bits, float]:
+        """
+        encode a float
+
+        :param value: the value to encode
+        """
         value = float(value)
         if value < self.min_value:
             value = self.min_value
         elif value > self.max_value:
             value = self.max_value
 
-        encoded_value = int(round(value - self.min_value, self.precision) * 10 ** self.precision)
-        #print(value, self.min_value, self.precision)
-        rounded_value = round(value - self.min_value, self.precision) + self.min_value  # Used only for validation
+        encoded_value = int(
+            round(value - self.min_value, self.precision) * 10**self.precision
+        )
+        # print(value, self.min_value, self.precision)
+        rounded_value = (
+            round(value - self.min_value, self.precision) + self.min_value
+        )  # Used only for validation
         encoded_bits = Bits(uint=encoded_value, length=self.num_bits)
 
         return encoded_bits, rounded_value
 
-    def decode(self, bits_to_decode: ConstBitStream):
-        float_offset = bits_to_decode.read('uint:{}'.format(self.num_bits)) / 10 ** self.precision
+    def decode(self, bits_to_decode: ConstBitStream) -> float:
+        """
+        decode a float
+
+        :param bits_to_decode: the bitstream to decode
+        """
+
+        float_offset = (
+            bits_to_decode.read(f"uint:{self.num_bits}") / 10**self.precision
+        )
         value = self.min_value + float_offset
         return value
 
     @property
-    def max_length_bits(self):
+    def max_length_bits(self) -> int:
         return self.num_bits
 
     @property
-    def min_length_bits(self):
-        return self.num_bits
+    def min_length_bits(self) -> int:
+        return self.num_bits
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/ieee_float_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/ieee_float_codec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,71 @@
+"""
+ltcodecs.ieee_float_codec
+-------------------------
+
+ieee_float_codec encodes and decodes IEEE floating point numbers
+"""
+
+from __future__ import annotations
 from bitstring import ConstBitStream, Bits
 from .field_codec import FieldCodec
-from math import ceil, log2
 
 
 class IeeeFloatCodec(FieldCodec):
+    """
+    codec for IEEE floating point numbers
+    """
+
     def __init__(self, num_bits=32, **kwargs):
         if num_bits not in (32, 64):
-            raise ValueError("Only 32 or 64 bit widths are supported for IEEE floating point codecs")
+            raise ValueError(
+                "Only 32 or 64 bit widths are supported for IEEE floating point codecs"
+            )
         self.num_bits = num_bits
 
-    def encode(self, value: float):
+    def encode(self, value: float) -> tuple[Bits, float]:
+        """
+        encode value
+
+        :param value: the value to encode
+        """
+
         value = float(value)
         encoded_bits = Bits(float=value, length=self.num_bits)
         encoded_value = encoded_bits.float
-        ## print("encode varint {} bits as {}".format(num_bits, encoded_bits))
         return encoded_bits, encoded_value
 
     def decode(self, bits_to_decode: ConstBitStream):
-        value = bits_to_decode.read('floatbe:{}'.format(self.num_bits))
+        """
+        decode value
+
+        :param bits_to_decode: the bitstream to decode
+        """
+
+        value = bits_to_decode.read(f"floatbe:{self.num_bits}")
         return value
 
     @property
     def max_length_bits(self):
         return self.num_bits
 
     @property
     def min_length_bits(self):
         return self.num_bits
 
 
 class IeeeFloat32Codec(IeeeFloatCodec):
+    """
+    metaclass for IEEE 32 bit floating point numbers
+    """
+
     def __init__(self, **kwargs):
         super(IeeeFloat32Codec, self).__init__(num_bits=32)
 
 
 class IeeeFloat64Codec(IeeeFloatCodec):
+    """
+    metaclass for IEEE 64 bit floating point numbers
+    """
+
     def __init__(self, **kwargs):
-        super(IeeeFloat64Codec, self).__init__(num_bits=64)
+        super(IeeeFloat64Codec, self).__init__(num_bits=64)
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/linspace_float_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/linspace_float_codec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,90 @@
+"""
+ltcodecs.linspace_float_codec
+-----------------------------
+
+This module contains the the linspace float codec
+"""
+
+from __future__ import annotations
+from math import ceil, log2
 from bitstring import ConstBitStream, Bits
+
 from .field_codec import FieldCodec
-from math import ceil, log2
 
 
 class LinspaceFloatCodec(FieldCodec):
-    def __init__(self, min_value: float, max_value: float,
-                 resolution: float = None, num_values: int = None, num_bits: int = None, **kwargs):
+    """
+    LinspaceFloatCodec
+    """
+
+    def __init__(
+        self,
+        min_value: float,
+        max_value: float,
+        resolution: float = None,
+        num_values: int = None,
+        num_bits: int = None,
+        **kwargs,
+    ):
         self.max_value = float(max_value)
         self.min_value = float(min_value)
         self.value_range = max_value - min_value
         if num_values or num_bits:
             if resolution:
-                raise ValueError("LinspaceFloatCodec supports setting only one of num_values, num_bits, or resolution.")
+                raise ValueError(
+                    "LinspaceFloatCodec supports setting only one of num_values, num_bits, or resolution."
+                )
             if num_bits:
                 if num_values:
-                    raise ValueError("LinspaceFloatCodec supports setting either num_values or num_bits, not both.")
+                    raise ValueError(
+                        "LinspaceFloatCodec supports setting either num_values or num_bits, not both."
+                    )
                 if num_bits < 1:
-                    raise ValueError("LinspaceFloatCodec requires at least 1 bit (num_bits >= 1), you specified num_bits={}".format(num_bits))
-                num_values = 2 ** num_bits
+                    raise ValueError(
+                        f"LinspaceFloatCodec requires at least 1 bit (num_bits >= 1), you specified num_bits={num_bits}"
+                    )
+                num_values = 2**num_bits
             if num_values < 2:
                 raise ValueError(
-                    "LinspaceFloatCodec requires at least 2 values (num_values >= 2), you specified num_values={}".format(
-                        num_values))
+                    f"LinspaceFloatCodec requires at least 2 values (num_values >= 2), you specified num_values={num_values}"
+                )
             resolution = self.value_range / (num_values - 1)
 
         self.resolution = float(resolution)
 
         self.num_values = self.value_range // self.resolution + 1
         # if the max value isn't an integer multiple of the resolution from the min value, it won't be encoded.
         self.num_bits = ceil(log2(self.num_values))
 
-    def encode(self, value: float):
+    def encode(self, value: float) -> tuple[Bits, float]:
+        """
+        encode value
+
+        :param value: the value to encode
+        """
         value = float(value)
         if value < self.min_value:
             value = self.min_value
         elif value > self.max_value:
             value = self.max_value
         offset = value - self.min_value
         discretized_offset = int(offset // self.resolution)
         encoded_value = self.min_value + (discretized_offset * self.resolution)
         encoded_bits = Bits(uint=discretized_offset, length=self.num_bits)
-        ## print("encode varint {} bits as {}".format(num_bits, encoded_bits))
         return encoded_bits, encoded_value
 
-    def decode(self, bits_to_decode: ConstBitStream):
-        discretized_offset = bits_to_decode.read('uint:{}'.format(self.num_bits))
+    def decode(self, bits_to_decode: ConstBitStream) -> float:
+        """
+        decode bits_to_decode into a value
+        """
+        discretized_offset = bits_to_decode.read(f"uint:{self.num_bits}")
         value = self.min_value + (discretized_offset * self.resolution)
         return value
 
     @property
-    def max_length_bits(self):
+    def max_length_bits(self) -> int:
         return self.num_bits
 
     @property
-    def min_length_bits(self):
-        return self.num_bits
+    def min_length_bits(self) -> int:
+        return self.num_bits
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/ros_message_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/ros_message_codec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,134 @@
+"""
+ltcodecs.ros_message_codec
+--------------------------
+
+This module contains the the ROS message codec
+"""
+
+from __future__ import annotations
+from typing import Any
 import ltcodecs as ltcodecs
 import msgpack
 from crccheck.crc import Crc8SaeJ1850, Crc32Iscsi
 from bitstring import Bits, ConstBitStream
 from copy import copy
 import operator
 from std_msgs.msg import Header
 import rospy
 
+
 class RosMessageCodec(object):
+    """
+    RosMessageCodec
+    """
+
     def __init__(self, ros_type, fields_dict: dict = None, checksum=None):
         self.ros_type = ros_type
         self.packet_codec = None
         self.checksum = checksum
-        
+
         if fields_dict:
             self.metadata_encoder_fields = {}
 
             for field_name, field_params in fields_dict.items():
                 # We only support a few metadata fields for encoding
-                codec_name = field_params.get('codec', 'auto')
+                codec_name = field_params.get("codec", "auto")
 
             for field_name, field_params in fields_dict.items():
                 # We only support a few metadata fields for encoding
-                codec_name = field_params.get('codec', 'auto')
+                codec_name = field_params.get("codec", "auto")
                 if codec_name in (ltcodecs.metadata_encoders.keys()):
                     self.metadata_encoder_fields[field_name] = codec_name
         else:
             self.metadata_encoder_fields = None
 
-        self.root_field_codec = ltcodecs.RosMsgFieldCodec(ros_type=ros_type, fields=fields_dict)
-        
-    def encode(self, ros_msg):
+        self.root_field_codec = ltcodecs.RosMsgFieldCodec(
+            ros_type=ros_type, fields=fields_dict
+        )
+
+    def encode(self, ros_msg: rospy.AnyMsg) -> tuple[Bits, dict[Any]]:
+        """
+        Encode a ROS message into a bitstream and metadata dictionary
+
+        :param ros_msg: ROS message to encode
+        """
         encoded_bits, encoded_dict = self.root_field_codec.encode(ros_msg)
 
         if self.checksum:
             msgpack_bytes = msgpack.packb(encoded_dict)
-            if self.checksum == 'crc8':
+            if self.checksum == "crc8":
                 calculated_crc = Crc8SaeJ1850.calc(msgpack_bytes)
                 encoded_bits.append(Bits(uint=calculated_crc, length=8))
-            elif self.checksum == 'crc32':
+            elif self.checksum == "crc32":
                 calculated_crc = Crc32Iscsi.calc(msgpack_bytes)
                 encoded_bits.append(Bits(uint=calculated_crc, length=32))
-            #print("Encoded CRC: {}".format(hex(calculated_crc)))
 
         metadata_dict = self._encode_metadata(ros_msg)
 
         return encoded_bits, metadata_dict
 
-    def decode(self, bits_to_decode: ConstBitStream, received_packet = None):
-        rospy.loginfo("Decoding ROS message {}".format(self.ros_type))
+    def decode(
+        self, bits_to_decode: ConstBitStream, received_packet=None
+    ) -> rospy.AnyMsg:
+        """
+        Decode a ROS message from a bitstream
+
+        :param bits_to_decode: Bitstream to decode
+        """
+
+        rospy.loginfo(f"Decoding ROS message {self.ros_type}")
         # Now, check CRC, if required.
         if self.checksum:
             # We need to decode this as a dict separately, so we need a new copy of the received bitstream.
             bits_copy = copy(bits_to_decode)
             bits_copy.pos = bits_to_decode.pos
             decoded_dict = self.root_field_codec.decode_as_dict(bits_copy)
 
         ros_msg = self.root_field_codec.decode(bits_to_decode, metadata=received_packet)
 
         if self.checksum:
             msgpack_bytes = msgpack.packb(decoded_dict)
-            # print("Msgpack length: {} bytes".format(len(msgpack_bytes)))
-            if self.checksum == 'crc8':
+            if self.checksum == "crc8":
                 calculated_crc = Crc8SaeJ1850.calc(msgpack_bytes)
                 # Next 8 bits of message are CRC
-                received_crc = bits_to_decode.read('uint:8')
-            elif self.checksum == 'crc32':
+                received_crc = bits_to_decode.read("uint:8")
+            elif self.checksum == "crc32":
                 calculated_crc = Crc32Iscsi.calc(msgpack_bytes)
-                received_crc = bits_to_decode.read('uint:32')
+                received_crc = bits_to_decode.read("uint:32")
 
-            #print("Received CRC: {}".format(hex(received_crc)))
             if calculated_crc != received_crc:
                 raise ValueError("Message CRC Mismatch")
 
-        rospy.loginfo("ROS Message: {}".format(ros_msg))
+        rospy.loginfo(f"ROS Message: {ros_msg}")
         return ros_msg
 
-    def _encode_metadata(self, ros_msg):
-        # Look through the fields dict for one of the magic keywords specified in field_codecs.py
+    def _encode_metadata(self, ros_msg) -> dict[Any]:
+        """Look through the fields dict for one of the magic keywords specified in field_codecs.py"""
+
         if self.metadata_encoder_fields:
             metadata_dict = {}
             for field_name, codec in self.metadata_encoder_fields.items():
                 metadata_dict[field_name] = getattr(ros_msg, codec)
             return metadata_dict
         else:
             return None
 
     @property
-    def max_length_bits(self):
-        if self.checksum == 'crc8':
+    def max_length_bits(self) -> int:
+        if self.checksum == "crc8":
             checksum_len = 8
-        elif self.checksum == 'crc32': 
+        elif self.checksum == "crc32":
             checksum_len = 32
         else:
             checksum_len = 0
         return self.root_field_codec.max_length_bits + checksum_len
 
     @property
-    def min_length_bits(self):
-        if self.checksum == 'crc8':
+    def min_length_bits(self) -> int:
+        if self.checksum == "crc8":
             checksum_len = 8
-        elif self.checksum == 'crc32':
+        elif self.checksum == "crc32":
             checksum_len = 32
         else:
             checksum_len = 0
         return self.root_field_codec.min_length_bits + checksum_len
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/ros_msg_field_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/ros_msg_field_codec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,44 @@
+"""
+ltcodecs.ros_msg_codec
+----------------------
+
+This module contains the the field codec which is used to encode and decode ROS messages.
+"""
+
+from __future__ import annotations
 import re
 from bitstring import ConstBitStream, BitArray
-from .field_codec import FieldCodec
-import ltcodecs as ltcodecs
-from rospy import AnyMsg
-from typing import Union
 import operator
+
+from rospy import AnyMsg
+from typing import Union, Any
 import roslib.message
 
+import ltcodecs as ltcodecs
+
+from .field_codec import FieldCodec
+from .exceptions import EncodingFailed
+
 
 class RosMsgFieldCodec(FieldCodec):
-    def __init__(self, ros_type: Union[str, AnyMsg], fields: dict = None, **kwargs):
+    """
+    field codec for ROS messages
+    """
+
+    def __init__(
+        self, ros_type: Union[str, AnyMsg], fields: dict = None, **kwargs
+    ) -> None:
         self.fields = fields
         self.ros_type = ros_type
 
         if isinstance(ros_type, str):
             msg_class = roslib.message.get_message_class(ros_type)
             if not msg_class:
-                raise TypeError('Invalid ROS type "{}" for message codec {}'.format(ros_type, id))
+                raise TypeError(f'Invalid ROS type "{ros_type}" for message codec {id}')
         else:
             msg_class = ros_type
         self.ros_msg_class = msg_class
 
         self.field_codecs = {}
         # Handle the case where we have to infer the field list from the ROS msg, since the user didn't specify one.
         if not self.fields:
@@ -29,82 +47,106 @@
 
             slots = dict(zip(slot_names, slot_types))
 
             new_fields = dict.fromkeys(slot_names)
             for field_name in new_fields:
                 msg_type = slots[field_name]
                 if msg_type in ltcodecs.field_codec_classes:
-                    field_params = {'codec': msg_type}
+                    field_params = {"codec": msg_type}
                 else:
                     # There are two cases here: arrays or nested ROS messages
-                    if msg_type.endswith(']'):
+                    if msg_type.endswith("]"):
                         # either a variable or fixed length array
-                        matched = re.match(r'(?P<element_type>.*)\[(?P<array_len>\d*)\]', msg_type)
-                        if matched['array_len']:
-                            array_len = int(matched['array_len'])
-                            field_params = {'codec': 'fixed_len_array',
-                                            'length': array_len}
+                        matched = re.match(
+                            r"(?P<element_type>.*)\[(?P<array_len>\d*)\]", msg_type
+                        )
+                        if matched["array_len"]:
+                            array_len = int(matched["array_len"])
+                            field_params = {
+                                "codec": "fixed_len_array",
+                                "length": array_len,
+                            }
                         else:
-                            field_params = {'codec': 'variable_len_array',
-                                            'max_length': 10}  # TODO: maybe take this as a parameter?
+                            field_params = {
+                                "codec": "variable_len_array",
+                                "max_length": 10,
+                            }  # TODO: maybe take this as a parameter?
                         # and the element type is either a standard type or a ROS message
-                        if matched['element_type'] in ltcodecs.field_codec_classes:
-                            field_params['element_type'] = matched['element_type']
+                        if matched["element_type"] in ltcodecs.field_codec_classes:
+                            field_params["element_type"] = matched["element_type"]
                         else:
-                            field_params['element_type'] = 'msg'
-                            field_params['element_params'] = {'ros_type': matched['element_type']}
+                            field_params["element_type"] = "msg"
+                            field_params["element_params"] = {
+                                "ros_type": matched["element_type"]
+                            }
                     else:
                         # It's a nested ROS message
-                        field_params = {'codec': 'msg',
-                                        'ros_type': msg_type}
+                        field_params = {"codec": "msg", "ros_type": msg_type}
 
                 new_fields[field_name] = field_params
 
             self.fields = new_fields
 
         # Now, build the list of codec classes for each field
         self.field_codecs = {}
         for field_name, field_params in self.fields.items():
             # print(field_name, field_params['codec'])
             # print(field_codecs.field_codec_classes[field_params['codec']])
             try:
-                if field_params['codec'] not in ltcodecs.metadata_decoders.keys():
-                    self.field_codecs[field_name] = ltcodecs.field_codec_classes[field_params['codec']](**field_params)
+                if field_params["codec"] not in ltcodecs.metadata_decoders.keys():
+                    self.field_codecs[field_name] = ltcodecs.field_codec_classes[
+                        field_params["codec"]
+                    ](**field_params)
                 else:
                     # The metadata codec is a string, which we use for a lookup later.
-                    self.field_codecs[field_name] = field_params['codec']
-            except KeyError as e:
-                raise KeyError("Error parsing codec config for {}.  Got params:\n{}\nError: {}".format(field_name,
-                                                                                                       field_params,
-                                                                                                       e))
+                    self.field_codecs[field_name] = field_params["codec"]
+            except KeyError as err:
+                raise KeyError(
+                    f"Error parsing codec config for {field_name}.  Got params:\n{field_params}\nError: {err}"
+                ) from err
+
+    def encode(self, message: AnyMsg, metadata=None) -> tuple[BitArray, dict[Any]]:
+        """
+        encode a ROS message
 
-    def encode(self, message: AnyMsg, metadata=None):
+        :param message: the message to encode
+        """
         # ROS messages use __slots__, so we can't use __dict__ or vars() to get the attributes as a dict
         message_dict = {}
         for field in message.__slots__:
             message_dict[field] = getattr(message, field)
 
         encoded_bits = BitArray()
         encoded_dict = {}
         for field_name, field_params in self.fields.items():
             try:
                 field_codec = self.field_codecs[field_name]
                 # Note that metadata encoding is done at the ros_msg_codec level, not here
                 if not field_codec or isinstance(field_codec, str):
                     continue
-                field_bits, encoded_dict[field_name] = field_codec.encode(message_dict[field_name])
+                (
+                    field_bits,
+                    encoded_dict[field_name],
+                ) = field_codec.encode(message_dict[field_name])
+
                 encoded_bits.append(field_bits)
-            except Exception as e:
-                #print("Codec: {}, max len bits {}".format(field_codec, field_codec.max_length_bits))
-                raise Exception('Error encoding field "{}" with codec {} (max len bits {})'.format(field_name,
-                                    field_codec, field_codec.max_length_bits)).with_traceback(e.__traceback__)
+            except Exception as err:
+                raise EncodingFailed(
+                    f'Error encoding field "{field_name}" with codec {field_codec} (max len bits {field_codec.max_length_bits})'
+                ) from err
         return encoded_bits, encoded_dict
 
-    def decode(self, bits_to_decode: ConstBitStream, metadata=None):
-        # We go through the bits in sequence until we are decoded.
+    def decode(self, bits_to_decode: ConstBitStream, metadata=None) -> AnyMsg:
+        """
+        decode a ROS message
+
+        :param bits_to_decode: the bits to decode
+        """
+
+        # go through the bits in sequence until we are decoded.
         # The ConstBitStream has an internal read pointer.
         decoded_message = {}
         for field_name, field_params in self.fields.items():
             field_codec = self.field_codecs[field_name]
             if not field_codec:
                 continue
 
@@ -118,37 +160,41 @@
                         value = operator.attrgetter(metadata_attribute)(metadata)
                         decoded_message[field_name] = value
                         continue
                 except KeyError:
                     # if we don't recognize the metadata codec, just keep going
                     continue
 
-            ## print("Ros decode field {}".format(field_name))
             # pass metadata only to nested ros msg fields
             if isinstance(field_codec, type(self)):
-                decoded_message[field_name] = field_codec.decode(bits_to_decode, metadata=metadata)
+                decoded_message[field_name] = field_codec.decode(
+                    bits_to_decode, metadata=metadata
+                )
             else:
                 decoded_message[field_name] = field_codec.decode(bits_to_decode)
-        ## print("Ros decode got {}".format(decoded_message))
         return self.ros_msg_class(**decoded_message)
 
-    def decode_as_dict(self, bits_to_decode: ConstBitStream):
-        # This function is used to generate an object that we can use for calculating CRCs in the message codec
+    def decode_as_dict(self, bits_to_decode: ConstBitStream) -> dict[Any]:
+        """This function is used to generate an object that we can use for calculating CRCs in the message codec
+        It seems like a bit of a hack, but the alternative would require adding a second return value to every field
+        decoder.  Since this only affects ROS messages, this keeps the bloat down.
+
+        :param bits_to_decode: the bits to decode
+        """
         # It seems like a bit of a hack, but the alternative would require adding a second return value to every field
         # decoder.  Since this only affects ROS messages, this keeps the bloat down.
         decoded_message = {}
         for field_name, field_params in self.fields.items():
             field_codec = self.field_codecs[field_name]
-            if hasattr(field_codec, 'decode_as_dict'):
+            if hasattr(field_codec, "decode_as_dict"):
                 decoded_message[field_name] = field_codec.decode_as_dict(bits_to_decode)
             else:
                 decoded_message[field_name] = field_codec.decode(bits_to_decode)
-        ## print("Ros decode got {}".format(decoded_message))
         return decoded_message
 
     @property
-    def min_length_bits(self):
+    def min_length_bits(self) -> int:
         return sum([c.min_length_bits for c in self.field_codecs.values()])
 
     @property
-    def max_length_bits(self):
+    def max_length_bits(self) -> int:
         return sum([c.max_length_bits for c in self.field_codecs.values()])
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/string_codecs.py` & `ltcodecs-1.0.0/src/ltcodecs/string_codecs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,124 @@
-from sys import byteorder
+"""
+ltcodecs.string_codecs
+----------------------
+
+This module contains codecs for encoding and decoding strings.
+"""
+
+from __future__ import annotations
 from bitstring import BitArray, Bits, ConstBitStream, offsetcopy
 from .varint_codec import VarintCodec
 from .field_codec import FieldCodec
 
-def to_sixbit_ascii(character: str):
+
+def to_sixbit_ascii(character: str) -> int:
+    """
+    return the sixbit code corresponding to the ascii character
+
+    :param character: the character to convert
+    """
     upper_character = character.upper()
-    ascii_code = int(upper_character.encode('ascii')[0])
+    ascii_code = int(upper_character.encode("ascii")[0])
 
-    if ascii_code >= 0x40 and ascii_code <= 0x5f:
+    if ascii_code >= 0x40 and ascii_code <= 0x5F:
         sixbit_code = ascii_code - 0x40
-    elif ascii_code >= 0x20 and ascii_code <= 0x3f:
+    elif ascii_code >= 0x20 and ascii_code <= 0x3F:
         sixbit_code = ascii_code
     else:
-        sixbit_code = 0x3f  # out of bounds values are encoded as '?'
+        sixbit_code = 0x3F  # out of bounds values are encoded as '?'
 
     return sixbit_code
 
 
-def from_sixbit_ascii(sixbit_code: int):
-    if sixbit_code <= 0x1f:
-        ascii_code = sixbit_code + 0x40
-    # Other characters map directly
-    else:
-        ascii_code = sixbit_code
+def from_sixbit_ascii(sixbit_code: int) -> str:
+    """
+    return the ascii character corresponding to the sixbit code
+
+    :param sixbit_code: the sixbit code to convert
+    """
+    ascii_code = sixbit_code + 0x40 if sixbit_code <= 0x1F else sixbit_code
 
-    return bytes([ascii_code]).decode('ascii')
+    return bytes([ascii_code]).decode("ascii")
 
 
 class AsciiStringCodec(FieldCodec):
-    def __init__(self, max_length: int = 128, bits_per_char: int = 7, tail=False, **kwargs):
+    """
+    codec for encoding and decoding ascii strings
+    """
+
+    def __init__(
+        self, max_length: int = 128, bits_per_char: int = 7, tail=False, **kwargs
+    ) -> None:
         self.max_length = int(max_length)
         self.bits_per_char = bits_per_char
         self.tail = tail
         self.string_len_codec = VarintCodec(min_value=0, max_value=max_length)
 
-    def encode(self, value: str):
+    def encode(self, value: str) -> tuple[Bits, str]:
+        """
+        encode a string into a bitstream
+
+        :param value: the string to encode
+        """
         if not self.tail:
-            value = value[0:self.max_length]
+            value = value[0 : self.max_length]
         else:
-            value = value[-self.max_length:]
+            value = value[-self.max_length :]
         length_bits, _ = self.string_len_codec.encode(len(value))
         encoded_bits = BitArray()
         encoded_bits.append(length_bits)
 
-        string_bytes = value.encode('ascii')
+        string_bytes = value.encode("ascii")
         if self.bits_per_char == 7:
             compressed_bytes = bytearray()
             for sb in string_bytes:
-                if sb > 0x7f:
+                if sb > 0x7F:
                     # Replace out of bounds values with "?"
-                    sb = 0x3f
+                    sb = 0x3F
                 compressed_bytes.append(sb)
                 encoded_bits.append(Bits(bytes=[sb], length=7, offset=1))
         elif self.bits_per_char == 6:
             compressed_bytes = bytearray()
             for sb in string_bytes:
                 sixbit_value = to_sixbit_ascii(sb)
-                compressed_byte = from_sixbit_ascii(sixbit_value).encode('ascii')
+                compressed_byte = from_sixbit_ascii(sixbit_value).encode("ascii")
                 compressed_bytes.extend(compressed_byte)
                 encoded_bits.append(Bits(bytes=[sixbit_value], length=6, offset=2))
         else:
             encoded_bits.append(Bits(bytes=value))
             compressed_bytes = string_bytes
 
-        compressed_string = compressed_bytes.decode('ascii')
+        compressed_string = compressed_bytes.decode("ascii")
         return encoded_bits, compressed_string
 
-    def decode(self, encoded_bits: ConstBitStream):
+    def decode(self, encoded_bits: ConstBitStream) -> str:
+        """
+        decode a string from a bitstream
+
+        :param encoded_bits: the bitstream to decode
+        """
         num_chars = self.string_len_codec.decode(encoded_bits)
         if self.bits_per_char == 7:
             string_bytes = bytearray()
             for i in range(num_chars):
-                char_byte = encoded_bits.read('uint:7').to_bytes(1, 'big')[0]
+                char_byte = encoded_bits.read("uint:7").to_bytes(1, "big")[0]
                 string_bytes.append(char_byte)
         elif self.bits_per_char == 6:
             new_string = ""
             for i in range(num_chars):
-                sixbit_code = encoded_bits.read('uint:6').to_bytes(1, 'big')[0]
-                new_string.append(from_sixbit_ascii(sixbit_code))
+                sixbit_code = encoded_bits.read("uint:6").to_bytes(1, "big")[0]
+                new_string += from_sixbit_ascii(sixbit_code)
             return new_string
         else:
-            string_bytes = encoded_bits.read('bytes:{}'.format(num_chars))
-        return string_bytes.decode('ascii')
+            string_bytes = encoded_bits.read(f"bytes:{num_chars}")
+        return string_bytes.decode("ascii")
 
     @property
-    def max_length_bits(self):
-        return self.string_len_codec.max_length_bits + (self.max_length * self.bits_per_char)
+    def max_length_bits(self) -> int:
+        return self.string_len_codec.max_length_bits + (
+            self.max_length * self.bits_per_char
+        )
 
     @property
-    def min_length_bits(self):
-        return self.string_len_codec.max_length_bits
+    def min_length_bits(self) -> int:
+        return self.string_len_codec.max_length_bits
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/variable_len_array_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/bytes_codec.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,57 @@
-from bitstring import BitArray, ConstBitStream
+"""
+ltcodecs.bytes_codec
+---------------------
+
+This module contains the BytesCodec class, which is used to encode and decode bytes.
+"""
+
+from __future__ import annotations
+from bitstring import BitArray, ConstBitStream, Bits
 from .field_codec import FieldCodec
 from .varint_codec import VarintCodec
-import ltcodecs as ltcodecs
-from typing import List
+from .exceptions import EncodingFailed
+
 
+class BytesCodec(FieldCodec):
+    """
+    codec for bytes
+    """
 
-class VariableLenArrayCodec(FieldCodec):
-    def __init__(self, element_type: str, max_length: int, element_params=None, **kwargs):
+    def __init__(self, max_length: int, fail_on_overflow=False, **kwargs) -> None:
         self.max_length = max_length
         self.length_codec = VarintCodec(min_value=0, max_value=self.max_length)
-        print('element_type', element_type)
-        if element_params:
-            self.element_field_codec = ltcodecs.field_codec_classes[element_type](**element_params)
-        else:
-            self.element_field_codec = ltcodecs.field_codec_classes[element_type]()
+        self.fail_on_overflow = fail_on_overflow
 
-    def encode(self, value: List):
-        value = value[0:self.max_length]
+    def encode(self, value: bytes) -> tuple[Bits, bytes]:
+        """
+        encode bytes
+
+        :param value: the bytes to encode
+        """
+        if self.fail_on_overflow and len(value) > self.max_length:
+            raise EncodingFailed(
+                f"BytesCodec: value with length {len(value)} is too long to encode (codec max_length={self.max_length}"
+            )
+        value = value[0 : self.max_length]
         length_bits, _ = self.length_codec.encode(len(value))
-        value_bits = BitArray(length_bits)
-        encoded_value_list = []
-        for element in value:
-            element_bits, element_value = self.element_field_codec.encode(element)
-            value_bits.append(element_bits)
-            encoded_value_list.append(element_value)
-        return value_bits, encoded_value_list
-
-    def decode(self, bits_to_decode: ConstBitStream):
-        num_elements = self.length_codec.decode(bits_to_decode)
-        decoded_list = []
-        for i in range(num_elements):
-            element = self.element_field_codec.decode(bits_to_decode)
-            decoded_list.append(element)
-        return decoded_list
+        value_bits = BitArray(bytes=value)
+        value_bits.prepend(length_bits)
+        return value_bits, value
+
+    def decode(self, bits_to_decode: ConstBitStream) -> bytes:
+        """
+        decode bytes
+
+        :param bits_to_decode: the bits to decode
+        """
+        num_bytes = self.length_codec.decode(bits_to_decode)
+        value = bits_to_decode.read("bytes:" + str(num_bytes))
+        return value
 
     @property
-    def min_length_bits(self):
+    def min_length_bits(self) -> int:
         return self.length_codec.max_length_bits
 
     @property
-    def max_length_bits(self):
-        return self.length_codec.max_length_bits + (self.max_length * self.element_field_codec.max_length_bits)
+    def max_length_bits(self) -> int:
+        return self.length_codec.max_length_bits + (8 * self.max_length)
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs/varint_codec.py` & `ltcodecs-1.0.0/src/ltcodecs/varint_codec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,84 @@
+"""
+ltcodecs.varint_codec
+---------------------
+
+This module contains the VarintCodec class, which is used to encode and decode variable-length integers.
+"""
+
+from __future__ import annotations
+
+from math import ceil, log2
+
 from bitstring import ConstBitStream, Bits
 from .field_codec import FieldCodec
-from math import ceil, log2
 
 
 class VarintCodec(FieldCodec):
-    def __init__(self, min_value: int, max_value: int, resolution: int = 1, little_endian: bool = False, **kwargs):
+    """
+    codec for variable-length integers
+    """
+
+    def __init__(
+        self,
+        min_value: int,
+        max_value: int,
+        resolution: int = 1,
+        little_endian: bool = False,
+        **kwargs,
+    ) -> None:
         self.max_value = int(max_value)
         self.min_value = int(min_value)
         self.resolution = int(resolution)
 
         self.value_range = max_value - min_value
         num_values = (self.value_range // self.resolution) + 1
         self.num_bits = ceil(log2(num_values))
         self.little_endian = little_endian
 
-    def encode(self, value: int):
+    def encode(self, value: int) -> tuple[Bits, int]:
+        """
+        turns int into variable-length int
+
+        :param value: int to encode
+        """
         value = int(value)
         if value < self.min_value:
             value = self.min_value
         elif value > self.max_value:
             value = self.max_value
         offset = value - self.min_value
         discretized_offset = offset // self.resolution
         encoded_value = self.min_value + (discretized_offset * self.resolution)
         if self.little_endian:
             encoded_bits = Bits(uintle=discretized_offset, length=self.num_bits)
         else:
             encoded_bits = Bits(uint=discretized_offset, length=self.num_bits)
-        ## print("encode varint {} bits as {}".format(num_bits, encoded_bits))
         return encoded_bits, encoded_value
 
-    def decode(self, bits_to_decode: ConstBitStream):
+    def decode(self, bits_to_decode: ConstBitStream) -> int:
+        """
+        decodes encoded varint
+
+        :param bits_to_decode: ConstBitStream to decode
+        """
         if self.little_endian:
-            discretized_offset = bits_to_decode.read('uintle:{}'.format(self.num_bits))
+            discretized_offset = bits_to_decode.read(f"uintle:{self.num_bits}")
         else:
-            discretized_offset = bits_to_decode.read('uint:{}'.format(self.num_bits))
+            discretized_offset = bits_to_decode.read(f"uint:{self.num_bits}")
 
         value = self.min_value + (discretized_offset * self.resolution)
         return value
 
     @property
-    def max_length_bits(self):
+    def max_length_bits(self) -> int:
         return self.num_bits
 
     @property
-    def min_length_bits(self):
+    def min_length_bits(self) -> int:
         return self.num_bits
 
-    def __repr__(self):
-        return "VarintCodec {:x}: min_value={}, max_value={}, resolution={}".format(id(self),
-                                                                                    self.min_value,
-                                                                                    self.max_value,
-                                                                                    self.resolution)
+    def __repr__(self) -> str:
+        """
+        returns string representation of VarintCodec
+        """
+        return f"VarintCodec {id(self):x}: min_value={self.min_value}, max_value={self.max_value}, resolution={self.resolution}"
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs.egg-info/PKG-INFO` & `ltcodecs-1.0.0/src/ltcodecs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: ltcodecs
-Version: 0.2.0
-Summary: LT Codecs
-Home-page: https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
-Author: whoi
-Author-email: egallimore@whoi.edu
-Project-URL: Bug Tracker, https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# LT Codecs
-
-The package was original part of ros_acomms under the field_codecs directory. 
+Metadata-Version: 2.1
+Name: ltcodecs
+Version: 1.0.0
+Summary: LT Codecs
+Home-page: https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
+Author: whoi
+Author-email: egallimore@whoi.edu
+Project-URL: Bug Tracker, https://git.whoi.edu/acomms/ros_acomms/tree/master/src/acomms_codecs
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LT Codecs
+
+The package was original part of ros_acomms under the field_codecs directory.
```

### Comparing `ltcodecs-0.2.0/src/ltcodecs.egg-info/SOURCES.txt` & `ltcodecs-1.0.0/src/ltcodecs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 pyproject.toml
 setup.cfg
 src/ltcodecs/__init__.py
 src/ltcodecs/bool_codec.py
 src/ltcodecs/bytes_codec.py
 src/ltcodecs/ccl_latlon_bcd_codec.py
 src/ltcodecs/ccl_latlon_codec.py
+src/ltcodecs/exceptions.py
 src/ltcodecs/field_codec.py
 src/ltcodecs/fixed_len_array_codec.py
 src/ltcodecs/fixedint_codec.py
 src/ltcodecs/float_codec.py
 src/ltcodecs/ieee_float_codec.py
 src/ltcodecs/linspace_float_codec.py
+src/ltcodecs/lzma_codec.py
 src/ltcodecs/padding_codec.py
 src/ltcodecs/ros_message_codec.py
 src/ltcodecs/ros_msg_field_codec.py
 src/ltcodecs/rostime_codec.py
 src/ltcodecs/string_codecs.py
 src/ltcodecs/string_enum_codec.py
 src/ltcodecs/variable_len_array_codec.py
 src/ltcodecs/varint_codec.py
 src/ltcodecs.egg-info/PKG-INFO
 src/ltcodecs.egg-info/SOURCES.txt
 src/ltcodecs.egg-info/dependency_links.txt
-src/ltcodecs.egg-info/top_level.txt
+src/ltcodecs.egg-info/top_level.txt
+tests/test_codecs.py
```


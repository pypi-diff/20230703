# Comparing `tmp/nanopb-0.4.8.dev1406.tar.gz` & `tmp/nanopb-0.4.8.dev1410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanopb-0.4.8.dev1406.tar", max compression
+gzip compressed data, was "nanopb-0.4.8.dev1410.tar", max compression
```

## Comparing `nanopb-0.4.8.dev1406.tar` & `nanopb-0.4.8.dev1410.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4366 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/README.md
--rw-r--r--   0        0        0        0 2023-05-22 02:33:00.226176 nanopb-0.4.8.dev1406/nanopb/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 02:33:00.226176 nanopb-0.4.8.dev1406/nanopb/generator/__init__.py
--rwxr-xr-x   0        0        0   106424 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/nanopb_generator.py
--rwxr-xr-x   0        0        0      460 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/nanopb_generator.py2
--rw-r--r--   0        0        0     5820 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/platformio_generator.py
--rw-r--r--   0        0        0      126 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/proto/Makefile
--rw-r--r--   0        0        0     4565 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/proto/__init__.py
--rw-r--r--   0        0        0     3318 2023-05-22 02:33:00.254177 nanopb-0.4.8.dev1406/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2121 2023-05-22 02:33:00.374178 nanopb-0.4.8.dev1406/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2023 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/proto/_utils.py
--rw-r--r--   0        0        0    36277 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/proto/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     6923 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/proto/nanopb.proto
--rw-r--r--   0        0        0     4551 2023-05-22 02:33:00.386178 nanopb-0.4.8.dev1406/nanopb/generator/proto/nanopb_pb2.py
--rwxr-xr-x   0        0        0     1577 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/protoc
--rwxr-xr-x   0        0        0      374 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/protoc-gen-nanopb
--rwxr-xr-x   0        0        0      554 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/protoc-gen-nanopb-py2
--rw-r--r--   0        0        0      449 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/protoc-gen-nanopb.bat
--rw-r--r--   0        0        0      302 2023-05-17 05:04:33.000000 nanopb-0.4.8.dev1406/nanopb/generator/protoc.bat
--rw-r--r--   0        0        0     1065 2023-05-22 02:33:00.418178 nanopb-0.4.8.dev1406/pyproject.toml
--rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 nanopb-0.4.8.dev1406/PKG-INFO
+-rw-r--r--   0        0        0     4366 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 02:35:49.772655 nanopb-0.4.8.dev1410/nanopb/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 02:35:49.772655 nanopb-0.4.8.dev1410/nanopb/generator/__init__.py
+-rwxr-xr-x   0        0        0   107186 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/nanopb_generator.py
+-rwxr-xr-x   0        0        0      460 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/nanopb_generator.py2
+-rw-r--r--   0        0        0     5820 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/platformio_generator.py
+-rw-r--r--   0        0        0      126 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/proto/Makefile
+-rw-r--r--   0        0        0     4565 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/proto/__init__.py
+-rw-r--r--   0        0        0     3318 2023-07-03 02:35:49.820658 nanopb-0.4.8.dev1410/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2121 2023-07-03 02:35:49.944665 nanopb-0.4.8.dev1410/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2023 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/proto/_utils.py
+-rw-r--r--   0        0        0    36277 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/proto/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     6923 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/proto/nanopb.proto
+-rw-r--r--   0        0        0     4690 2023-07-03 02:35:49.964666 nanopb-0.4.8.dev1410/nanopb/generator/proto/nanopb_pb2.py
+-rwxr-xr-x   0        0        0     1577 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/protoc
+-rwxr-xr-x   0        0        0      374 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/protoc-gen-nanopb
+-rwxr-xr-x   0        0        0      554 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/protoc-gen-nanopb-py2
+-rw-r--r--   0        0        0      449 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/protoc-gen-nanopb.bat
+-rw-r--r--   0        0        0      302 2023-06-26 06:08:25.000000 nanopb-0.4.8.dev1410/nanopb/generator/protoc.bat
+-rw-r--r--   0        0        0     1065 2023-07-03 02:35:49.996668 nanopb-0.4.8.dev1410/pyproject.toml
+-rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 nanopb-0.4.8.dev1410/PKG-INFO
```

### Comparing `nanopb-0.4.8.dev1406/README.md` & `nanopb-0.4.8.dev1410/README.md`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/nanopb_generator.py` & `nanopb-0.4.8.dev1410/nanopb/generator/nanopb_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,19 @@
     FieldD.TYPE_SFIXED32:   ('int32_t',  'SFIXED32',    4,  4),
     FieldD.TYPE_SFIXED64:   ('int64_t',  'SFIXED64',    8,  8),
     FieldD.TYPE_SINT32:     ('int32_t',  'SINT32',      5,  4),
     FieldD.TYPE_SINT64:     ('int64_t',  'SINT64',     10,  8),
     FieldD.TYPE_UINT32:     ('uint32_t', 'UINT32',      5,  4),
     FieldD.TYPE_UINT64:     ('uint64_t', 'UINT64',     10,  8),
 
-    # Integer size override options
+    # Integer size override option
+    (FieldD.TYPE_ENUM,    nanopb_pb2.IS_8):   ('uint8_t', 'ENUM',  4,  1),
+    (FieldD.TYPE_ENUM,   nanopb_pb2.IS_16):   ('uint16_t', 'ENUM',  4,  2),
+    (FieldD.TYPE_ENUM,   nanopb_pb2.IS_32):   ('uint32_t', 'ENUM',  4,  4),
+    (FieldD.TYPE_ENUM,   nanopb_pb2.IS_64):   ('uint64_t', 'ENUM',  4,  8),
     (FieldD.TYPE_INT32,   nanopb_pb2.IS_8):   ('int8_t',   'INT32', 10,  1),
     (FieldD.TYPE_INT32,  nanopb_pb2.IS_16):   ('int16_t',  'INT32', 10,  2),
     (FieldD.TYPE_INT32,  nanopb_pb2.IS_32):   ('int32_t',  'INT32', 10,  4),
     (FieldD.TYPE_INT32,  nanopb_pb2.IS_64):   ('int64_t',  'INT32', 10,  8),
     (FieldD.TYPE_SINT32,  nanopb_pb2.IS_8):   ('int8_t',  'SINT32',  2,  1),
     (FieldD.TYPE_SINT32, nanopb_pb2.IS_16):   ('int16_t', 'SINT32',  3,  2),
     (FieldD.TYPE_SINT32, nanopb_pb2.IS_32):   ('int32_t', 'SINT32',  5,  4),
@@ -427,15 +431,26 @@
     def __str__(self):
         leading_comment, trailing_comment = self.get_comments()
 
         result = ''
         if leading_comment:
             result = '%s\n' % leading_comment
 
-        result += 'typedef enum %s {' % Globals.naming_style.enum_name(self.names)
+        result += 'typedef enum %s' % Globals.naming_style.enum_name(self.names)
+
+        # Override the enum size if user wants to use smaller integers
+        if (FieldD.TYPE_ENUM, self.options.int_size) in datatypes:
+            self.ctype, self.pbtype, self.enc_size, self.data_item_size = datatypes[(FieldD.TYPE_ENUM, self.options.int_size)]
+            result += '\n#ifdef __cplusplus\n'
+            result += ' : ' + self.ctype + '\n'
+            result += '#endif\n'
+            result += '{'
+        else:
+            result += ' {'
+
         if trailing_comment:
             result += " " + trailing_comment
 
         result += "\n"
 
         enum_length = len(self.values)
         enum_values = []
```

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/platformio_generator.py` & `nanopb-0.4.8.dev1410/nanopb/generator/platformio_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/__init__.py` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed May 17 05:04:33 2023 UTC, .py size: 4565 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6160 6464 d511 0000  U.......a`dd....
+00000000: 550d 0d0a 0000 0000 592b 9964 d511 0000  U.......Y+.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a03 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6404 6405 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
```

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed May 17 05:04:33 2023 UTC, .py size: 2023 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6160 6464 e707 0000  U.......a`dd....
+00000000: 550d 0d0a 0000 0000 592b 9964 e707 0000  U.......Y+.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 8400 5a04 6404  d.l.Z.d.d...Z.d.
 00000050: 6405 8400 5a05 6406 6407 8400 5a06 6507  d...Z.d.d...Z.e.
 00000060: 6408 6b02 723e 6506 8300 0100 6401 5300  d.k.r>e.....d.S.
 00000070: 2909 e900 0000 004e 6300 0000 0000 0000  )......Nc.......
```

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/_utils.py` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/_utils.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/google/protobuf/descriptor.proto` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/nanopb.proto` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/nanopb.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/proto/nanopb_pb2.py` & `nanopb-0.4.8.dev1410/nanopb/generator/proto/nanopb_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: nanopb.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cnanopb.proto\x1a google/protobuf/descriptor.proto\"\xa4\x07\n\rNanoPBOptions\x12\x10\n\x08max_size\x18\x01 \x01(\x05\x12\x12\n\nmax_length\x18\x0e \x01(\x05\x12\x11\n\tmax_count\x18\x02 \x01(\x05\x12&\n\x08int_size\x18\x07 \x01(\x0e\x32\x08.IntSize:\nIS_DEFAULT\x12$\n\x04type\x18\x03 \x01(\x0e\x32\n.FieldType:\nFT_DEFAULT\x12\x18\n\nlong_names\x18\x04 \x01(\x08:\x04true\x12\x1c\n\rpacked_struct\x18\x05 \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0bpacked_enum\x18\n \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0cskip_message\x18\x06 \x01(\x08:\x05\x66\x61lse\x12\x18\n\tno_unions\x18\x08 \x01(\x08:\x05\x66\x61lse\x12\r\n\x05msgid\x18\t \x01(\r\x12\x1e\n\x0f\x61nonymous_oneof\x18\x0b \x01(\x08:\x05\x66\x61lse\x12\x15\n\x06proto3\x18\x0c \x01(\x08:\x05\x66\x61lse\x12#\n\x14proto3_singular_msgs\x18\x15 \x01(\x08:\x05\x66\x61lse\x12\x1d\n\x0e\x65num_to_string\x18\r \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0c\x66ixed_length\x18\x0f \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0b\x66ixed_count\x18\x10 \x01(\x08:\x05\x66\x61lse\x12\x1e\n\x0fsubmsg_callback\x18\x16 \x01(\x08:\x05\x66\x61lse\x12/\n\x0cmangle_names\x18\x11 \x01(\x0e\x32\x11.TypenameMangling:\x06M_NONE\x12(\n\x11\x63\x61llback_datatype\x18\x12 \x01(\t:\rpb_callback_t\x12\x34\n\x11\x63\x61llback_function\x18\x13 \x01(\t:\x19pb_default_field_callback\x12\x30\n\x0e\x64\x65scriptorsize\x18\x14 \x01(\x0e\x32\x0f.DescriptorSize:\x07\x44S_AUTO\x12\x1a\n\x0b\x64\x65\x66\x61ult_has\x18\x17 \x01(\x08:\x05\x66\x61lse\x12\x0f\n\x07include\x18\x18 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x1a \x03(\t\x12\x0f\n\x07package\x18\x19 \x01(\t\x12\x41\n\rtype_override\x18\x1b \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.Type\x12\x19\n\x0bsort_by_tag\x18\x1c \x01(\x08:\x04true\x12.\n\rfallback_type\x18\x1d \x01(\x0e\x32\n.FieldType:\x0b\x46T_CALLBACK*i\n\tFieldType\x12\x0e\n\nFT_DEFAULT\x10\x00\x12\x0f\n\x0b\x46T_CALLBACK\x10\x01\x12\x0e\n\nFT_POINTER\x10\x04\x12\r\n\tFT_STATIC\x10\x02\x12\r\n\tFT_IGNORE\x10\x03\x12\r\n\tFT_INLINE\x10\x05*D\n\x07IntSize\x12\x0e\n\nIS_DEFAULT\x10\x00\x12\x08\n\x04IS_8\x10\x08\x12\t\n\x05IS_16\x10\x10\x12\t\n\x05IS_32\x10 \x12\t\n\x05IS_64\x10@*Z\n\x10TypenameMangling\x12\n\n\x06M_NONE\x10\x00\x12\x13\n\x0fM_STRIP_PACKAGE\x10\x01\x12\r\n\tM_FLATTEN\x10\x02\x12\x16\n\x12M_PACKAGE_INITIALS\x10\x03*E\n\x0e\x44\x65scriptorSize\x12\x0b\n\x07\x44S_AUTO\x10\x00\x12\x08\n\x04\x44S_1\x10\x01\x12\x08\n\x04\x44S_2\x10\x02\x12\x08\n\x04\x44S_4\x10\x04\x12\x08\n\x04\x44S_8\x10\x08:E\n\x0enanopb_fileopt\x12\x1c.google.protobuf.FileOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:G\n\rnanopb_msgopt\x12\x1f.google.protobuf.MessageOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:E\n\x0enanopb_enumopt\x12\x1c.google.protobuf.EnumOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:>\n\x06nanopb\x12\x1d.google.protobuf.FieldOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptionsB\x1a\n\x18\x66i.kapsi.koti.jpa.nanopb')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nanopb_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nanopb_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.FileOptions.RegisterExtension(nanopb_fileopt)
   google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(nanopb_msgopt)
   google_dot_protobuf_dot_descriptor__pb2.EnumOptions.RegisterExtension(nanopb_enumopt)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(nanopb)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030fi.kapsi.koti.jpa.nanopb'
-  _FIELDTYPE._serialized_start=985
-  _FIELDTYPE._serialized_end=1090
-  _INTSIZE._serialized_start=1092
-  _INTSIZE._serialized_end=1160
-  _TYPENAMEMANGLING._serialized_start=1162
-  _TYPENAMEMANGLING._serialized_end=1252
-  _DESCRIPTORSIZE._serialized_start=1254
-  _DESCRIPTORSIZE._serialized_end=1323
-  _NANOPBOPTIONS._serialized_start=51
-  _NANOPBOPTIONS._serialized_end=983
+  _globals['_FIELDTYPE']._serialized_start=985
+  _globals['_FIELDTYPE']._serialized_end=1090
+  _globals['_INTSIZE']._serialized_start=1092
+  _globals['_INTSIZE']._serialized_end=1160
+  _globals['_TYPENAMEMANGLING']._serialized_start=1162
+  _globals['_TYPENAMEMANGLING']._serialized_end=1252
+  _globals['_DESCRIPTORSIZE']._serialized_start=1254
+  _globals['_DESCRIPTORSIZE']._serialized_end=1323
+  _globals['_NANOPBOPTIONS']._serialized_start=51
+  _globals['_NANOPBOPTIONS']._serialized_end=983
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/protoc` & `nanopb-0.4.8.dev1410/nanopb/generator/protoc`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/nanopb/generator/protoc-gen-nanopb-py2` & `nanopb-0.4.8.dev1410/nanopb/generator/protoc-gen-nanopb-py2`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1406/pyproject.toml` & `nanopb-0.4.8.dev1410/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanopb"
-version = "0.4.8-dev1406"
+version = "0.4.8-dev1410"
 description = "Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system."
 authors = ["Petteri Aimonen <jpa@npb.mail.kapsi.fi>"]
 license = "Zlib"
 repository = "https://github.com/nanopb/nanopb/"
 readme = "README.md"
 homepage = "https://jpa.kapsi.fi/nanopb/"
 documentation = "https://jpa.kapsi.fi/nanopb/docs/index.html"
```

### Comparing `nanopb-0.4.8.dev1406/PKG-INFO` & `nanopb-0.4.8.dev1410/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanopb
-Version: 0.4.8.dev1406
+Version: 0.4.8.dev1410
 Summary: Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system.
 Home-page: https://jpa.kapsi.fi/nanopb/
 License: Zlib
 Keywords: protobuf,protoc
 Author: Petteri Aimonen
 Author-email: jpa@npb.mail.kapsi.fi
 Requires-Python: >=2.7
```


# Comparing `tmp/avro-1.9.1.tar.gz` & `tmp/avro-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/avro-1.9.1.tar", last modified: Mon Sep  2 07:40:28 2019, max compression
+gzip compressed data, was "dist/avro-1.9.2.tar", last modified: Wed Feb 12 13:51:51 2020, max compression
```

## Comparing `avro-1.9.1.tar` & `avro-1.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 fokkodriesprong   (501) staff       (20)        0 2019-09-02 07:40:28.000000 avro-1.9.1/
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)      313 2019-09-02 07:40:28.000000 avro-1.9.1/PKG-INFO
-drwxr-xr-x   0 fokkodriesprong   (501) staff       (20)        0 2019-09-02 07:40:28.000000 avro-1.9.1/test/
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     1494 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_ipc.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     3590 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_tether_task.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    12341 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_protocol.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     7474 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_script.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     5935 2019-08-28 09:35:21.000000 avro-1.9.1/test/test_tether_word_count.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     7206 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_datafile.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    13874 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_io.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     1466 2019-08-28 09:35:18.000000 avro-1.9.1/test/test_datafile_interop.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    21167 2019-08-28 09:35:17.000000 avro-1.9.1/test/test_schema.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     6026 2019-08-28 09:35:18.000000 avro-1.9.1/test/test_tether_task_runner.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     1722 2019-08-28 09:35:18.000000 avro-1.9.1/setup.py
-drwxr-xr-x   0 fokkodriesprong   (501) staff       (20)        0 2019-09-02 07:40:28.000000 avro-1.9.1/scripts/
--rwxr-xr-x   0 fokkodriesprong   (501) staff       (20)     7976 2019-08-28 09:35:18.000000 avro-1.9.1/scripts/avro
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)       38 2019-09-02 07:40:28.000000 avro-1.9.1/setup.cfg
-drwxr-xr-x   0 fokkodriesprong   (501) staff       (20)        0 2019-09-02 07:40:28.000000 avro-1.9.1/avro.egg-info/
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)      313 2019-09-02 07:40:28.000000 avro-1.9.1/avro.egg-info/PKG-INFO
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)      632 2019-09-02 07:40:28.000000 avro-1.9.1/avro.egg-info/SOURCES.txt
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)       24 2019-09-02 07:40:28.000000 avro-1.9.1/avro.egg-info/requires.txt
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)        5 2019-09-02 07:40:28.000000 avro-1.9.1/avro.egg-info/top_level.txt
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)        1 2019-09-02 07:40:28.000000 avro-1.9.1/avro.egg-info/dependency_links.txt
-drwxr-xr-x   0 fokkodriesprong   (501) staff       (20)        0 2019-09-02 07:40:28.000000 avro-1.9.1/src/
-drwxr-xr-x   0 fokkodriesprong   (501) staff       (20)        0 2019-09-02 07:40:28.000000 avro-1.9.1/src/avro/
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    12138 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/datafile.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    11361 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/LICENSE
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    18065 2019-08-28 09:35:18.000000 avro-1.9.1/src/avro/ipc.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     7859 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/protocol.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     1124 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/constants.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    43444 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/io.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)      869 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/__init__.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)      167 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/NOTICE
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     7830 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/txipc.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     5226 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/tool.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)     1296 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/timezones.py
--rw-r--r--   0 fokkodriesprong   (501) staff       (20)    30743 2019-08-28 09:35:17.000000 avro-1.9.1/src/avro/schema.py
+drwxr-xr-x   0 rskraba   (1000) rskraba   (1000)        0 2020-02-12 13:51:51.000000 avro-1.9.2/
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)       38 2020-02-12 13:51:51.000000 avro-1.9.2/setup.cfg
+drwxr-xr-x   0 rskraba   (1000) rskraba   (1000)        0 2020-02-12 13:51:51.000000 avro-1.9.2/src/
+drwxr-xr-x   0 rskraba   (1000) rskraba   (1000)        0 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro/
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     4917 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/tool.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)      958 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/__init__.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     7878 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/protocol.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)      167 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/NOTICE
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    42201 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/io.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    30856 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/schema.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    18123 2020-02-07 08:53:28.000000 avro-1.9.2/src/avro/ipc.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     1346 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/timezones.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     1212 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/constants.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    12998 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/datafile.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    11361 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/LICENSE
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     7885 2020-02-07 08:39:02.000000 avro-1.9.2/src/avro/txipc.py
+drwxr-xr-x   0 rskraba   (1000) rskraba   (1000)        0 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro.egg-info/
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)       47 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro.egg-info/requires.txt
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)        5 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro.egg-info/top_level.txt
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)      652 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro.egg-info/SOURCES.txt
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)        1 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro.egg-info/dependency_links.txt
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)      339 2020-02-12 13:51:51.000000 avro-1.9.2/src/avro.egg-info/PKG-INFO
+drwxr-xr-x   0 rskraba   (1000) rskraba   (1000)        0 2020-02-12 13:51:51.000000 avro-1.9.2/scripts/
+-rwxr-xr-x   0 rskraba   (1000) rskraba   (1000)     7983 2020-02-07 08:53:28.000000 avro-1.9.2/scripts/avro
+drwxr-xr-x   0 rskraba   (1000) rskraba   (1000)        0 2020-02-12 13:51:51.000000 avro-1.9.2/test/
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    22159 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_schema.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     1588 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_ipc.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     6077 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_tether_task_runner.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    14158 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_io.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)    12434 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_protocol.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     5727 2020-02-07 08:53:28.000000 avro-1.9.2/test/test_tether_word_count.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     7138 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_script.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     1868 2020-02-07 08:53:28.000000 avro-1.9.2/test/test_datafile_interop.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     7211 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_datafile.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     3769 2020-02-07 08:39:02.000000 avro-1.9.2/test/test_tether_task.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)     2450 2020-02-12 13:42:45.000000 avro-1.9.2/setup.py
+-rw-r--r--   0 rskraba   (1000) rskraba   (1000)      339 2020-02-12 13:51:51.000000 avro-1.9.2/PKG-INFO
```

### Comparing `avro-1.9.1/test/test_ipc.py` & `avro-1.9.2/test/test_ipc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -9,26 +12,30 @@
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """
 There are currently no IPC tests within python, in part because there are no
 servers yet available.
 """
+
+from __future__ import absolute_import, division, print_function
+
 import unittest
 
 import set_avro_test_path
-
 # This test does import this code, to make sure it at least passes
 # compilation.
 from avro import ipc
 
+
 class TestIPC(unittest.TestCase):
   def test_placeholder(self):
     pass
 
   def test_server_with_path(self):
     client_with_custom_path = ipc.HTTPTransceiver('apache.org', 80, '/service/article')
     self.assertEqual('/service/article', client_with_custom_path.req_resource)
```

### Comparing `avro-1.9.1/test/test_tether_task.py` & `avro-1.9.2/test/test_tether_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -10,68 +13,71 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
+from __future__ import absolute_import, division, print_function
 
 import os
+import StringIO
 import subprocess
 import sys
 import time
 import unittest
 
+import avro.tether.tether_task
+import avro.tether.util
+import mock_tether_parent
 import set_avro_test_path
+from avro import io as avio
+from avro import schema, tether
+from word_count_task import WordCountTask
+
 
 class TestTetherTask(unittest.TestCase):
   """
   TODO: We should validate the the server response by looking at stdout
   """
   def test1(self):
     """
     Test that the thether_task is working. We run the mock_tether_parent in a separate
     subprocess
     """
-    from avro import tether
-    from avro import io as avio
-    from avro import schema
-    from avro.tether import HTTPRequestor,inputProtocol, find_port
-
-    import StringIO
-    import mock_tether_parent
-    from word_count_task import WordCountTask
-
     task=WordCountTask()
 
     proc=None
     try:
       # launch the server in a separate process
       # env["AVRO_TETHER_OUTPUT_PORT"]=output_port
       env=dict()
       env["PYTHONPATH"]=':'.join(sys.path)
-      server_port=find_port()
+      server_port = avro.tether.util.find_port()
 
       pyfile=mock_tether_parent.__file__
       proc=subprocess.Popen(["python", pyfile,"start_server","{0}".format(server_port)])
-      input_port=find_port()
+      input_port = avro.tether.util.find_port()
 
-      print "Mock server started process pid={0}".format(proc.pid)
+      print("Mock server started process pid={0}".format(proc.pid))
       # Possible race condition? open tries to connect to the subprocess before the subprocess is fully started
       # so we give the subprocess time to start up
       time.sleep(1)
       task.open(input_port,clientPort=server_port)
 
       # TODO: We should validate that open worked by grabbing the STDOUT of the subproces
       # and ensuring that it outputted the correct message.
 
       #***************************************************************
       # Test the mapper
-      task.configure(tether.TaskType.MAP,str(task.inschema),str(task.midschema))
+      task.configure(
+        avro.tether.tether_task.TaskType.MAP,
+        str(task.inschema),
+        str(task.midschema)
+      )
 
       # Serialize some data so we can send it to the input function
       datum="This is a line of text"
       writer = StringIO.StringIO()
       encoder = avio.BinaryEncoder(writer)
       datum_writer = avio.DatumWriter(task.inschema)
       datum_writer.write(datum, encoder)
@@ -79,15 +85,19 @@
       writer.seek(0)
       data=writer.read()
 
       # Call input to simulate calling map
       task.input(data,1)
 
       # Test the reducer
-      task.configure(tether.TaskType.REDUCE,str(task.midschema),str(task.outschema))
+      task.configure(
+        avro.tether.tether_task.TaskType.REDUCE,
+        str(task.midschema),
+        str(task.outschema)
+      )
 
       # Serialize some data so we can send it to the input function
       datum={"key":"word","value":2}
       writer = StringIO.StringIO()
       encoder = avio.BinaryEncoder(writer)
       datum_writer = avio.DatumWriter(task.midschema)
       datum_writer.write(datum, encoder)
@@ -109,8 +119,8 @@
       # close the process
       if not(proc is None):
         proc.kill()
 
       pass
 
 if __name__ == '__main__':
-  unittest.main()
+  unittest.main()
```

### Comparing `avro-1.9.1/test/test_protocol.py` & `avro-1.9.2/test/test_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-Test the protocol parsing logic.
-"""
+
+"""Test the protocol parsing logic."""
+
+from __future__ import absolute_import, division, print_function
+
 import unittest
+
 from avro import protocol
 
+
 class ExampleProtocol(object):
   def __init__(self, protocol_string, valid, name='', comment=''):
     self._protocol_string = protocol_string
     self._valid = valid
     self._name = name or protocol_string # default to schema_string for name
     self._comment = comment
 
@@ -148,28 +155,28 @@
     """, True),
 ExampleProtocol("""\
 {"namespace": "org.apache.avro.test.namespace",
  "protocol": "TestImplicitNamespace",
 
  "types": [
      {"name": "org.apache.avro.test.util.MD5", "type": "fixed", "size": 16},
-     {"name": "ReferencedRecord", "type": "record", 
+     {"name": "ReferencedRecord", "type": "record",
        "fields": [ {"name": "foo", "type": "string"} ] },
      {"name": "TestRecord", "type": "record",
       "fields": [ {"name": "hash", "type": "org.apache.avro.test.util.MD5"},
                   {"name": "unqalified", "type": "ReferencedRecord"} ]
      },
      {"name": "TestError",
       "type": "error", "fields": [ {"name": "message", "type": "string"} ]
      }
  ],
 
  "messages": {
      "echo": {
-         "request": [{"name": "qualified", 
+         "request": [{"name": "qualified",
              "type": "org.apache.avro.test.namespace.TestRecord"}],
          "response": "TestRecord"
      },
 
      "error": {
          "request": [],
          "response": "null",
@@ -182,31 +189,31 @@
     """, True),
 ExampleProtocol("""\
 {"namespace": "org.apache.avro.test.namespace",
  "protocol": "TestNamespaceTwo",
 
  "types": [
      {"name": "org.apache.avro.test.util.MD5", "type": "fixed", "size": 16},
-     {"name": "ReferencedRecord", "type": "record", 
-       "namespace": "org.apache.avro.other.namespace", 
+     {"name": "ReferencedRecord", "type": "record",
+       "namespace": "org.apache.avro.other.namespace",
        "fields": [ {"name": "foo", "type": "string"} ] },
      {"name": "TestRecord", "type": "record",
       "fields": [ {"name": "hash", "type": "org.apache.avro.test.util.MD5"},
-                  {"name": "qualified", 
-                    "type": "org.apache.avro.other.namespace.ReferencedRecord"} 
+                  {"name": "qualified",
+                    "type": "org.apache.avro.other.namespace.ReferencedRecord"}
                 ]
      },
      {"name": "TestError",
       "type": "error", "fields": [ {"name": "message", "type": "string"} ]
      }
  ],
 
  "messages": {
      "echo": {
-         "request": [{"name": "qualified", 
+         "request": [{"name": "qualified",
              "type": "org.apache.avro.test.namespace.TestRecord"}],
          "response": "TestRecord"
      },
 
      "error": {
          "request": [],
          "response": "null",
@@ -219,27 +226,27 @@
     """, True),
 ExampleProtocol("""\
 {"namespace": "org.apache.avro.test.namespace",
  "protocol": "TestValidRepeatedName",
 
  "types": [
      {"name": "org.apache.avro.test.util.MD5", "type": "fixed", "size": 16},
-     {"name": "ReferencedRecord", "type": "record", 
-       "namespace": "org.apache.avro.other.namespace", 
+     {"name": "ReferencedRecord", "type": "record",
+       "namespace": "org.apache.avro.other.namespace",
        "fields": [ {"name": "foo", "type": "string"} ] },
-     {"name": "ReferencedRecord", "type": "record", 
+     {"name": "ReferencedRecord", "type": "record",
        "fields": [ {"name": "bar", "type": "double"} ] },
      {"name": "TestError",
       "type": "error", "fields": [ {"name": "message", "type": "string"} ]
      }
  ],
 
  "messages": {
      "echo": {
-         "request": [{"name": "qualified", 
+         "request": [{"name": "qualified",
              "type": "ReferencedRecord"}],
          "response": "org.apache.avro.other.namespace.ReferencedRecord"
      },
 
      "error": {
          "request": [],
          "response": "null",
@@ -252,26 +259,26 @@
     """, True),
 ExampleProtocol("""\
 {"namespace": "org.apache.avro.test.namespace",
  "protocol": "TestInvalidRepeatedName",
 
  "types": [
      {"name": "org.apache.avro.test.util.MD5", "type": "fixed", "size": 16},
-     {"name": "ReferencedRecord", "type": "record", 
+     {"name": "ReferencedRecord", "type": "record",
        "fields": [ {"name": "foo", "type": "string"} ] },
-     {"name": "ReferencedRecord", "type": "record", 
+     {"name": "ReferencedRecord", "type": "record",
        "fields": [ {"name": "bar", "type": "double"} ] },
      {"name": "TestError",
       "type": "error", "fields": [ {"name": "message", "type": "string"} ]
      }
  ],
 
  "messages": {
      "echo": {
-         "request": [{"name": "qualified", 
+         "request": [{"name": "qualified",
              "type": "ReferencedRecord"}],
          "response": "org.apache.avro.other.namespace.ReferencedRecord"
      },
 
      "error": {
          "request": [],
          "response": "null",
@@ -346,33 +353,33 @@
 
 class TestProtocol(unittest.TestCase):
   def test_parse(self):
     num_correct = 0
     for example in EXAMPLES:
       try:
         protocol.parse(example.protocol_string)
-        if example.valid: 
+        if example.valid:
           num_correct += 1
         else:
           self.fail("Parsed invalid protocol: %s" % (example.name,))
-      except Exception, e:
-        if not example.valid: 
+      except Exception as e:
+        if not example.valid:
           num_correct += 1
         else:
           self.fail("Coudl not parse valid protocol: %s" % (example.name,))
 
     fail_msg = "Parse behavior correct on %d out of %d protocols." % \
       (num_correct, len(EXAMPLES))
     self.assertEqual(num_correct, len(EXAMPLES), fail_msg)
 
   def test_inner_namespace_set(self):
-    print ''
-    print 'TEST INNER NAMESPACE'
-    print '==================='
-    print ''
+    print('')
+    print('TEST INNER NAMESPACE')
+    print('===================')
+    print('')
     proto = protocol.parse(HELLO_WORLD.protocol_string)
     self.assertEqual(proto.namespace, "com.acme")
     greeting_type = proto.types_dict['Greeting']
     self.assertEqual(greeting_type.namespace, 'com.acme')
 
   def test_inner_namespace_not_rendered(self):
     proto = protocol.parse(HELLO_WORLD.protocol_string)
@@ -382,57 +389,56 @@
     self.assertFalse('namespace' in proto.to_json()['types'][0])
 
   def test_valid_cast_to_string_after_parse(self):
     """
     Test that the string generated by an Avro Protocol object
     is, in fact, a valid Avro protocol.
     """
-    print ''
-    print 'TEST CAST TO STRING'
-    print '==================='
-    print ''
+    print('')
+    print('TEST CAST TO STRING')
+    print('===================')
+    print('')
 
     num_correct = 0
     for example in VALID_EXAMPLES:
       protocol_data = protocol.parse(example.protocol_string)
       try:
-        try:
-          protocol.parse(str(protocol_data))
-          debug_msg = "%s: STRING CAST SUCCESS" % example.name
-          num_correct += 1
-        except:
-          debug_msg = "%s: STRING CAST FAILURE" % example.name
-      finally:
-        print debug_msg
+        protocol.parse(str(protocol_data))
+      except (ValueError, ProtocolParseException):
+        debug_msg = "%s: STRING CAST FAILURE" % example.name
+      else:
+        debug_msg = "%s: STRING CAST SUCCESS" % example.name
+        num_correct += 1
+      print(debug_msg)
 
     fail_msg = "Cast to string success on %d out of %d protocols" % \
       (num_correct, len(VALID_EXAMPLES))
     self.assertEqual(num_correct, len(VALID_EXAMPLES), fail_msg)
 
   def test_equivalence_after_round_trip(self):
     """
     1. Given a string, parse it to get Avro protocol "original".
     2. Serialize "original" to a string and parse that string
          to generate Avro protocol "round trip".
     3. Ensure "original" and "round trip" protocols are equivalent.
     """
-    print ''
-    print 'TEST ROUND TRIP'
-    print '==============='
-    print ''
+    print('')
+    print('TEST ROUND TRIP')
+    print('===============')
+    print('')
 
     num_correct = 0
     for example in VALID_EXAMPLES:
       original_protocol = protocol.parse(example.protocol_string)
       round_trip_protocol = protocol.parse(str(original_protocol))
 
       if original_protocol == round_trip_protocol:
         num_correct += 1
         debug_msg = "%s: ROUND TRIP SUCCESS" % example.name
-      else:       
+      else:
         self.fail("Round trip failure: %s %s %s", (example.name, example.protocol_string, str(original_protocol)))
 
     fail_msg = "Round trip success on %d out of %d protocols" % \
       (num_correct, len(VALID_EXAMPLES))
     self.assertEqual(num_correct, len(VALID_EXAMPLES), fail_msg)
 
 if __name__ == '__main__':
```

### Comparing `avro-1.9.1/test/test_script.py` & `avro-1.9.2/test/test_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,44 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import unittest
+
+from __future__ import absolute_import, division, print_function
+
 import csv
+import json
+import unittest
 from cStringIO import StringIO
-try:
-    import json
-except ImportError:
-    import simplejson as json
+from operator import itemgetter
+from os import remove
+from os.path import dirname, isfile, join
+from subprocess import check_call, check_output
 from tempfile import NamedTemporaryFile
+
 import avro.schema
-from avro.io import DatumWriter
 from avro.datafile import DataFileWriter
-from os.path import dirname, join, isfile
-from os import remove
-from operator import itemgetter
+from avro.io import DatumWriter
 
 NUM_RECORDS = 7
 
-try:
-    from subprocess import check_output
-except ImportError:
-    from subprocess import Popen, PIPE
-
-    def check_output(args):
-        pipe = Popen(args, stdout=PIPE)
-        if pipe.wait() != 0:
-            raise ValueError
-        return pipe.stdout.read()
-
-try:
-    from subprocess import check_call
-except ImportError:
-    def check_call(args, **kw):
-        pipe = Popen(args, **kw)
-        assert pipe.wait() == 0
 
 SCHEMA = '''
 {
     "namespace": "test.avro",
         "name": "LooneyTunes",
         "type": "record",
         "fields": [
@@ -138,15 +126,15 @@
     def test_help(self):
         # Just see we have these
         self._run("-h")
         self._run("--help")
 
     def test_json_pretty(self):
         out = self._run("--format", "json-pretty", "-n", "1", raw=1)
-        assert out.strip() == _JSON_PRETTY.strip()
+        self.assertEqual(out.strip(), _JSON_PRETTY.strip())
 
     def test_version(self):
         check_output([SCRIPT, "cat", "--version"])
 
     def test_files(self):
         out = self._run(self.avro_file)
         assert len(out) == 2 * NUM_RECORDS
```

### Comparing `avro-1.9.1/test/test_tether_word_count.py` & `avro-1.9.2/test/test_tether_word_count.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -10,54 +13,54 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import inspect
+from __future__ import absolute_import, division, print_function
+
+import os
+import shutil
 import subprocess
 import sys
-import time
+import tempfile
 import unittest
-import os
 
+import avro
+import avro.datafile
+import avro.io
+import avro.schema
+import avro.tether.tether_task_runner
 import set_avro_test_path
 
+
 class TestTetherWordCount(unittest.TestCase):
-  """ unittest for a python tethered map-reduce job.
-  """
+  """unittest for a python tethered map-reduce job."""
 
   def _write_lines(self,lines,fname):
     """
     Write the lines to an avro file named fname
 
     Parameters
     --------------------------------------------------------
     lines - list of strings to write
     fname - the name of the file to write to.
     """
-    import avro.io as avio
-    from avro.datafile import DataFileReader,DataFileWriter
-    from avro import schema
-
     #recursively make all directories
     dparts=fname.split(os.sep)[:-1]
     for i in range(len(dparts)):
       pdir=os.sep+os.sep.join(dparts[:i+1])
       if not(os.path.exists(pdir)):
         os.mkdir(pdir)
 
 
     with file(fname,'w') as hf:
       inschema="""{"type":"string"}"""
-      writer=DataFileWriter(hf,avio.DatumWriter(inschema),writers_schema=schema.parse(inschema))
-
-      #encoder = avio.BinaryEncoder(writer)
-      #datum_writer = avio.DatumWriter()
+      writer = avro.datafile.DataFileWriter(hf, avro.io.DatumWriter(inschema), writers_schema=avro.schema.parse(inschema))
       for datum in lines:
         writer.append(datum)
 
       writer.close()
 
 
 
@@ -67,40 +70,29 @@
     """
     counts={}
 
     for line in lines:
       words=line.split()
 
       for w in words:
-        if not(counts.has_key(w.strip())):
+        if not(w.strip() in counts):
           counts[w.strip()]=0
 
         counts[w.strip()]=counts[w.strip()]+1
 
     return counts
 
   def test1(self):
     """
     Run a tethered map-reduce job.
 
     Assumptions: 1) bash is available in /bin/bash
     """
-    from word_count_task import WordCountTask
-    from avro.tether import tether_task_runner
-    from avro.datafile import DataFileReader
-    from avro.io import DatumReader
-    import avro
-
-    import subprocess
-    import StringIO
-    import shutil
-    import tempfile
-    import inspect
-
     proc=None
+    exfile = None
 
     try:
 
 
       # TODO we use the tempfile module to generate random names
       # for the files
       base_dir = "/tmp/test_tether_word_count"
@@ -142,72 +134,72 @@
 
       outpath = os.path.join(base_dir, "out")
 
       args=[]
 
       args.append("java")
       args.append("-jar")
-      args.append(os.path.abspath("/avro/lang/py/../java/tools/target/avro-tools-1.9.1.jar"))
+      args.append(os.path.abspath("/home/rskraba/avro/lang/py/../java/tools/target/avro-tools-1.9.2.jar"))
 
 
       args.append("tether")
       args.extend(["--in",inpath])
       args.extend(["--out",outpath])
       args.extend(["--outschema",outschema])
       args.extend(["--protocol","http"])
 
       # form the arguments for the subprocess
       subargs=[]
 
-      srcfile=inspect.getsourcefile(tether_task_runner)
+      srcfile = avro.tether.tether_task_runner.__file__
 
       # Create a shell script to act as the program we want to execute
       # We do this so we can set the python path appropriately
       script="""#!/bin/bash
 export PYTHONPATH={0}
 python -m avro.tether.tether_task_runner word_count_task.WordCountTask
 """
       # We need to make sure avro is on the path
       # getsourcefile(avro) returns .../avro/__init__.py
-      asrc=inspect.getsourcefile(avro)
+      asrc = avro.__file__
       apath=asrc.rsplit(os.sep,2)[0]
 
       # path to where the tests lie
       tpath=os.path.split(__file__)[0]
 
       exhf=tempfile.NamedTemporaryFile(mode='w',prefix="exec_word_count_",delete=False)
       exfile=exhf.name
       exhf.write(script.format((os.pathsep).join([apath,tpath]),srcfile))
       exhf.close()
 
       # make it world executable
-      os.chmod(exfile,0755)
+      os.chmod(exfile,0o755)
 
       args.extend(["--program",exfile])
 
-      print "Command:\n\t{0}".format(" ".join(args))
+      print("Command:\n\t{0}".format(" ".join(args)))
       proc=subprocess.Popen(args)
 
 
       proc.wait()
 
       # read the output
       with file(os.path.join(outpath,"part-00000.avro")) as hf:
-        reader=DataFileReader(hf, DatumReader())
+        reader = avro.datafile.DataFileReader(hf, avro.io.DatumReader())
         for record in reader:
           self.assertEqual(record["value"],true_counts[record["key"]])
 
         reader.close()
 
     except Exception as e:
       raise
     finally:
       # close the process
       if proc is not None and proc.returncode is None:
         proc.kill()
       if os.path.exists(base_dir):
         shutil.rmtree(base_dir)
-      if os.path.exists(exfile):
+      if exfile is not None and os.path.exists(exfile):
         os.remove(exfile)
 
 if __name__== "__main__":
   unittest.main()
```

### Comparing `avro-1.9.1/test/test_datafile.py` & `avro-1.9.2/test/test_datafile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from __future__ import absolute_import, division, print_function
+
 import os
 import unittest
 
 import set_avro_test_path
-
-from avro import schema
-from avro import io
-from avro import datafile
+from avro import datafile, io, schema
 
 SCHEMAS_TO_VALIDATE = (
   ('"null"', None),
   ('"boolean"', True),
   ('"string"', unicode('adsfasdf09809dsf-=adsf')),
   ('"bytes"', '12345abcd'),
   ('"int"', 1234),
@@ -55,33 +58,38 @@
 
 FILENAME = 'test_datafile.out'
 CODECS_TO_VALIDATE = ('null', 'deflate')
 try:
   import snappy
   CODECS_TO_VALIDATE += ('snappy',)
 except ImportError:
-  print 'Snappy not present, will skip testing it.'
+  print('Snappy not present, will skip testing it.')
+try:
+  import zstandard
+  CODECS_TO_VALIDATE += ('zstandard',)
+except ImportError:
+  print('Zstandard not present, will skip testing it.')
 
 # TODO(hammer): clean up written files with ant, not os.remove
 class TestDataFile(unittest.TestCase):
   def test_round_trip(self):
-    print ''
-    print 'TEST ROUND TRIP'
-    print '==============='
-    print ''
+    print('')
+    print('TEST ROUND TRIP')
+    print('===============')
+    print('')
     correct = 0
     for i, (example_schema, datum) in enumerate(SCHEMAS_TO_VALIDATE):
       for codec in CODECS_TO_VALIDATE:
-        print ''
-        print 'SCHEMA NUMBER %d' % (i + 1)
-        print '================'
-        print ''
-        print 'Schema: %s' % example_schema
-        print 'Datum: %s' % datum
-        print 'Codec: %s' % codec
+        print('')
+        print('SCHEMA NUMBER %d' % (i + 1))
+        print('================')
+        print('')
+        print('Schema: %s' % example_schema)
+        print('Datum: %s' % datum)
+        print('Codec: %s' % codec)
 
         # write data in binary to file 10 times
         writer = open(FILENAME, 'wb')
         datum_writer = io.DatumWriter()
         schema_object = schema.parse(example_schema)
         dfw = datafile.DataFileWriter(writer, datum_writer, schema_object, codec=codec)
         for i in range(10):
@@ -92,38 +100,38 @@
         reader = open(FILENAME, 'rb')
         datum_reader = io.DatumReader()
         dfr = datafile.DataFileReader(reader, datum_reader)
         round_trip_data = []
         for datum in dfr:
           round_trip_data.append(datum)
 
-        print 'Round Trip Data: %s' % round_trip_data
-        print 'Round Trip Data Length: %d' % len(round_trip_data)
+        print('Round Trip Data: %s' % round_trip_data)
+        print('Round Trip Data Length: %d' % len(round_trip_data))
         is_correct = [datum] * 10 == round_trip_data
         if is_correct: correct += 1
-        print 'Correct Round Trip: %s' % is_correct
-        print ''
+        print('Correct Round Trip: %s' % is_correct)
+        print('')
     os.remove(FILENAME)
     self.assertEquals(correct, len(CODECS_TO_VALIDATE)*len(SCHEMAS_TO_VALIDATE))
 
   def test_append(self):
-    print ''
-    print 'TEST APPEND'
-    print '==========='
-    print ''
+    print('')
+    print('TEST APPEND')
+    print('===========')
+    print('')
     correct = 0
     for i, (example_schema, datum) in enumerate(SCHEMAS_TO_VALIDATE):
       for codec in CODECS_TO_VALIDATE:
-        print ''
-        print 'SCHEMA NUMBER %d' % (i + 1)
-        print '================'
-        print ''
-        print 'Schema: %s' % example_schema
-        print 'Datum: %s' % datum
-        print 'Codec: %s' % codec
+        print('')
+        print('SCHEMA NUMBER %d' % (i + 1))
+        print('================')
+        print('')
+        print('Schema: %s' % example_schema)
+        print('Datum: %s' % datum)
+        print('Codec: %s' % codec)
 
         # write data in binary to file once
         writer = open(FILENAME, 'wb')
         datum_writer = io.DatumWriter()
         schema_object = schema.parse(example_schema)
         dfw = datafile.DataFileWriter(writer, datum_writer, schema_object, codec=codec)
         dfw.append(datum)
@@ -140,31 +148,25 @@
         reader = open(FILENAME, 'rb')
         datum_reader = io.DatumReader()
         dfr = datafile.DataFileReader(reader, datum_reader)
         appended_data = []
         for datum in dfr:
           appended_data.append(datum)
 
-        print 'Appended Data: %s' % appended_data
-        print 'Appended Data Length: %d' % len(appended_data)
+        print('Appended Data: %s' % appended_data)
+        print('Appended Data Length: %d' % len(appended_data))
         is_correct = [datum] * 10 == appended_data
         if is_correct: correct += 1
-        print 'Correct Appended: %s' % is_correct
-        print ''
+        print('Correct Appended: %s' % is_correct)
+        print('')
     os.remove(FILENAME)
     self.assertEquals(correct, len(CODECS_TO_VALIDATE)*len(SCHEMAS_TO_VALIDATE))
 
   def test_context_manager(self):
-    # Context manager was introduced as a first class
-    # member only in Python 2.6 and above.
-    import sys
-    if sys.version_info < (2,6):
-      print 'Skipping context manager tests on this Python version.'
-      return
-    # Test the writer with a 'with' statement.
+    """Test the writer with a 'with' statement."""
     writer = open(FILENAME, 'wb')
     datum_writer = io.DatumWriter()
     sample_schema, sample_datum = SCHEMAS_TO_VALIDATE[1]
     schema_object = schema.parse(sample_schema)
     with datafile.DataFileWriter(writer, datum_writer, schema_object) as dfw:
       dfw.append(sample_datum)
     self.assertTrue(writer.closed)
```

### Comparing `avro-1.9.1/test/test_io.py` & `avro-1.9.2/test/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,46 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import unittest
 
+from __future__ import absolute_import, division, print_function
+
+import datetime
+import unittest
+from binascii import hexlify
 from decimal import Decimal
 
+import set_avro_test_path
+from avro import io, schema, timezones
+
 try:
   from cStringIO import StringIO
 except ImportError:
   from StringIO import StringIO
-from binascii import hexlify
-import datetime
 
-import set_avro_test_path
-
-from avro import schema
-from avro import io
-from avro import timezones
 
 SCHEMAS_TO_VALIDATE = (
   ('"null"', None),
   ('"boolean"', True),
-  ('"string"', unicode('adsfasdf09809dsf-=adsf')),
+  ('"string"', u'adsfasdf09809dsf-=adsf'),
   ('"bytes"', '12345abcd'),
   ('"int"', 1234),
   ('"long"', 1234),
   ('"float"', 1234.0),
   ('"double"', 1234.0),
   ('{"type": "fixed", "name": "Test", "size": 1}', 'B'),
   ('{"type": "fixed", "logicalType": "decimal", "name": "Test", "size": 8, "precision": 5, "scale": 4}',
@@ -75,14 +78,17 @@
     '{"type": "long", "logicalType": "timestamp-micros"}',
     datetime.datetime(9999, 12, 31, 23, 59, 59, 999999, tzinfo=timezones.utc)
   ),
   (
     '{"type": "long", "logicalType": "timestamp-micros"}',
     datetime.datetime(2000, 1, 18, 2, 2, 1, 123499, tzinfo=timezones.tst)
   ),
+  ('{"type": "string", "logicalType": "uuid"}', u'12345abcd'),
+  ('{"type": "string", "logicalType": "unknown-logical-type"}', u'12345abcd'),
+  ('{"type": "string", "logicalType": "timestamp-millis"}', u'12345abcd'),
   ("""\
    {"type": "record",
     "name": "Test",
     "fields": [{"name": "f", "type": "long"}]}
    """, {'f': 5}),
   ("""\
    {"type": "record",
@@ -110,15 +116,15 @@
 
 DEFAULT_VALUE_EXAMPLES = (
   ('"null"', 'null', None),
   ('"boolean"', 'true', True),
   ('"string"', '"foo"', u'foo'),
   ('"bytes"', '"\u00FF\u00FF"', u'\xff\xff'),
   ('"int"', '5', 5),
-  ('"long"', '5', 5L),
+  ('"long"', '5', 5),
   ('"float"', '1.1', 1.1),
   ('"double"', '1.1', 1.1),
   ('{"type": "fixed", "name": "F", "size": 2}', '"\u00FF\u00FF"', u'\xff\xff'),
   ('{"type": "enum", "name": "F", "symbols": ["FOO", "BAR"]}', '"FOO"', 'FOO'),
   ('{"type": "array", "items": "int"}', '[1, 2, 3]', [1, 2, 3]),
   ('{"type": "map", "values": "int"}', '{"a": 1, "b": 2}', {'a': 1, 'b': 2}),
   ('["int", "null"]', '5', 5),
@@ -146,18 +152,18 @@
   bytes.append(hexlify(current_byte))
   while (ord(current_byte) & 0x80) != 0:
     current_byte = reader.read(1)
     bytes.append(hexlify(current_byte))
   return ' '.join(bytes)
 
 def print_test_name(test_name):
-  print ''
-  print test_name
-  print '=' * len(test_name)
-  print ''
+  print('')
+  print(test_name)
+  print('=' * len(test_name))
+  print('')
 
 def write_datum(datum, writers_schema):
   writer = StringIO()
   encoder = io.BinaryEncoder(writer)
   datum_writer = io.DatumWriter(writers_schema)
   datum_writer.write(datum, encoder)
   return writer, encoder, datum_writer
@@ -168,33 +174,33 @@
   datum_reader = io.DatumReader(writers_schema, readers_schema)
   return datum_reader.read(decoder)
 
 def check_binary_encoding(number_type):
   print_test_name('TEST BINARY %s ENCODING' % number_type.upper())
   correct = 0
   for datum, hex_encoding in BINARY_ENCODINGS:
-    print 'Datum: %d' % datum
-    print 'Correct Encoding: %s' % hex_encoding
+    print('Datum: %d' % datum)
+    print('Correct Encoding: %s' % hex_encoding)
 
     writers_schema = schema.parse('"%s"' % number_type.lower())
     writer, encoder, datum_writer = write_datum(datum, writers_schema)
     writer.seek(0)
     hex_val = avro_hexlify(writer)
 
-    print 'Read Encoding: %s' % hex_val
+    print('Read Encoding: %s' % hex_val)
     if hex_encoding == hex_val: correct += 1
-    print ''
+    print('')
   return correct
 
 def check_skip_number(number_type):
   print_test_name('TEST SKIP %s' % number_type.upper())
   correct = 0
   for value_to_skip, hex_encoding in BINARY_ENCODINGS:
     VALUE_TO_READ = 6253
-    print 'Value to Skip: %d' % value_to_skip
+    print('Value to Skip: %d' % value_to_skip)
 
     # write the value to skip and a known value
     writers_schema = schema.parse('"%s"' % number_type.lower())
     writer, encoder, datum_writer = write_datum(value_to_skip, writers_schema)
     datum_writer.write(VALUE_TO_READ, encoder)
 
     # skip the value
@@ -202,47 +208,47 @@
     decoder = io.BinaryDecoder(reader)
     decoder.skip_long()
 
     # read data from string buffer
     datum_reader = io.DatumReader(writers_schema)
     read_value = datum_reader.read(decoder)
 
-    print 'Read Value: %d' % read_value
+    print('Read Value: %d' % read_value)
     if read_value == VALUE_TO_READ: correct += 1
-    print ''
+    print('')
   return correct
-    
+
 class TestIO(unittest.TestCase):
   #
   # BASIC FUNCTIONALITY
   #
 
   def test_validate(self):
     print_test_name('TEST VALIDATE')
     passed = 0
     for example_schema, datum in SCHEMAS_TO_VALIDATE:
-      print 'Schema: %s' % example_schema
-      print 'Datum: %s' % datum
+      print('Schema: %s' % example_schema)
+      print('Datum: %s' % datum)
       validated = io.validate(schema.parse(example_schema), datum)
-      print 'Valid: %s' % validated
+      print('Valid: %s' % validated)
       if validated: passed += 1
     self.assertEquals(passed, len(SCHEMAS_TO_VALIDATE))
 
   def test_round_trip(self):
     print_test_name('TEST ROUND TRIP')
     correct = 0
     for example_schema, datum in SCHEMAS_TO_VALIDATE:
-      print 'Schema: %s' % example_schema
-      print 'Datum: %s' % datum
+      print('Schema: %s' % example_schema)
+      print('Datum: %s' % datum)
 
       writers_schema = schema.parse(example_schema)
       writer, encoder, datum_writer = write_datum(datum, writers_schema)
       round_trip_datum = read_datum(writer, writers_schema)
 
-      print 'Round Trip Datum: %s' % round_trip_datum
+      print('Round Trip Datum: %s' % round_trip_datum)
       if isinstance(round_trip_datum, Decimal):
         round_trip_datum = round_trip_datum.to_eng_string()
         datum = str(datum)
       elif isinstance(round_trip_datum, datetime.datetime):
         datum = datum.astimezone(tz=timezones.utc)
       if datum == round_trip_datum:
         correct += 1
@@ -281,16 +287,16 @@
     for i, ws in enumerate(promotable_schemas):
       writers_schema = schema.parse(ws)
       datum_to_write = 219
       for rs in promotable_schemas[i + 1:]:
         readers_schema = schema.parse(rs)
         writer, enc, dw = write_datum(datum_to_write, writers_schema)
         datum_read = read_datum(writer, writers_schema, readers_schema)
-        print 'Writer: %s Reader: %s' % (writers_schema, readers_schema)
-        print 'Datum Read: %s' % datum_read
+        print('Writer: %s Reader: %s' % (writers_schema, readers_schema))
+        print('Datum Read: %s' % datum_read)
         if datum_read != datum_to_write: incorrect += 1
     self.assertEquals(incorrect, 0)
 
   def test_unknown_symbol(self):
     print_test_name('TEST UNKNOWN SYMBOL')
     writers_schema = schema.parse("""\
       {"type": "enum", "name": "Test",
@@ -318,15 +324,15 @@
         {"type": "record", "name": "Test",
          "fields": [{"name": "H", "type": %s, "default": %s}]}
         """ % (field_type, default_json))
       datum_to_read = {'H': default_datum}
 
       writer, encoder, datum_writer = write_datum(datum_to_write, writers_schema)
       datum_read = read_datum(writer, writers_schema, readers_schema)
-      print 'Datum Read: %s' % datum_read
+      print('Datum Read: %s' % datum_read)
       if datum_to_read == datum_read: correct += 1
     self.assertEquals(correct, len(DEFAULT_VALUE_EXAMPLES))
 
   def test_no_default_value(self):
     print_test_name('TEST NO DEFAULT VALUE')
     writers_schema = LONG_RECORD_SCHEMA
     datum_to_write = LONG_RECORD_DATUM
@@ -350,15 +356,15 @@
       {"type": "record", "name": "Test",
        "fields": [{"name": "E", "type": "int"},
                   {"name": "F", "type": "int"}]}""")
     datum_to_read = {'E': 5, 'F': 6}
 
     writer, encoder, datum_writer = write_datum(datum_to_write, writers_schema)
     datum_read = read_datum(writer, writers_schema, readers_schema)
-    print 'Datum Read: %s' % datum_read
+    print('Datum Read: %s' % datum_read)
     self.assertEquals(datum_to_read, datum_read)
 
   def test_field_order(self):
     print_test_name('TEST FIELD ORDER')
     writers_schema = LONG_RECORD_SCHEMA
     datum_to_write = LONG_RECORD_DATUM
 
@@ -366,15 +372,15 @@
       {"type": "record", "name": "Test",
        "fields": [{"name": "F", "type": "int"},
                   {"name": "E", "type": "int"}]}""")
     datum_to_read = {'E': 5, 'F': 6}
 
     writer, encoder, datum_writer = write_datum(datum_to_write, writers_schema)
     datum_read = read_datum(writer, writers_schema, readers_schema)
-    print 'Datum Read: %s' % datum_read
+    print('Datum Read: %s' % datum_read)
     self.assertEquals(datum_to_read, datum_read)
 
   def test_type_exception(self):
     print_test_name('TEST TYPE EXCEPTION')
     writers_schema = schema.parse("""\
       {"type": "record", "name": "Test",
        "fields": [{"name": "F", "type": "int"},
```

### Comparing `avro-1.9.1/test/test_datafile_interop.py` & `avro-1.9.2/test/test_datafile_interop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,54 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from __future__ import absolute_import, division, print_function
+
 import os
 import unittest
 
 import set_avro_test_path
+from avro import datafile, io
 
-from avro import io
-from avro import datafile
 
 class TestDataFileInterop(unittest.TestCase):
   def test_interop(self):
-    print ''
-    print 'TEST INTEROP'
-    print '============'
-    print ''
-    for f in os.listdir('/avro/lang/py/../../build/interop/data'):
-      print 'READING %s' % f
-      print ''
-
-      # read data in binary from file
-      reader = open(os.path.join('/avro/lang/py/../../build/interop/data', f), 'rb')
-      datum_reader = io.DatumReader()
-      dfr = datafile.DataFileReader(reader, datum_reader)
-      for datum in dfr:
-        assert datum is not None
+    print()
+    print('TEST INTEROP')
+    print('============')
+    print()
+    for f in os.listdir('/home/rskraba/avro/lang/py/../../build/interop/data'):
+      base_ext = os.path.splitext(os.path.basename(f))[0].split('_', 1)
+      if len(base_ext) < 2 or base_ext[1] in datafile.VALID_CODECS:
+        print('READING %s' % f)
+        print('')
+
+        # read data in binary from file
+        reader = open(os.path.join('/home/rskraba/avro/lang/py/../../build/interop/data', f), 'rb')
+        datum_reader = io.DatumReader()
+        dfr = datafile.DataFileReader(reader, datum_reader)
+        i = 0
+        for i, datum in enumerate(dfr, 1):
+          assert datum is not None
+        assert i > 0
+      else:
+        print('SKIPPING %s due to an unsupported codec' % f)
+        print('')
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `avro-1.9.1/test/test_schema.py` & `avro-1.9.2/test/test_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,382 +1,244 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-Test the schema parsing logic.
-"""
-import unittest
 
-from avro.schema import SchemaParseException, AvroException
+"""Test the schema parsing logic."""
 
-import set_avro_test_path
+from __future__ import absolute_import, division, print_function
+
+import json
+import unittest
 
+import set_avro_test_path
 from avro import schema
+from avro.schema import AvroException, SchemaParseException
 
-def print_test_name(test_name):
-  print ''
-  print test_name
-  print '=' * len(test_name)
-  print ''
-
-class ExampleSchema(object):
-  def __init__(self, schema_string, valid, name='', comment=''):
-    self._schema_string = schema_string
-    self._valid = valid
-    self._name = name or schema_string # default to schema_string for name
+
+class TestSchema(object):
+  """A proxy for a schema string that provides useful test metadata."""
+
+  def __init__(self, data, name='', comment=''):
+    if not isinstance(data, basestring):
+      data = json.dumps(data)
+    self.data = data
+    self.name = name or data  # default to data for name
     self.comment = comment
 
-  @property
-  def schema_string(self):
-    return self._schema_string
-
-  @property
-  def valid(self):
-    return self._valid
-
-  @property
-  def name(self):
-    return self._name
+  def parse(self):
+    return schema.parse(str(self))
+
+  def __str__(self):
+    return str(self.data)
+
+
+class ValidTestSchema(TestSchema):
+  """A proxy for a valid schema string that provides useful test metadata."""
+  valid = True
 
-#
-# Example Schemas
-#
 
-def make_primitive_examples():
-  examples = []
-  for type in schema.PRIMITIVE_TYPES:
-    examples.append(ExampleSchema('"%s"' % type, True))
-    examples.append(ExampleSchema('{"type": "%s"}' % type, True))
-  return examples
-
-PRIMITIVE_EXAMPLES = [
-  ExampleSchema('"True"', False),
-  ExampleSchema('True', False),
-  ExampleSchema('{"no_type": "test"}', False),
-  ExampleSchema('{"type": "panther"}', False),
-] + make_primitive_examples()
+class InvalidTestSchema(ValidTestSchema):
+  """A proxy for an invalid schema string that provides useful test metadata."""
+  valid = False
+
+
+PRIMITIVE_EXAMPLES = ([
+  InvalidTestSchema('"True"'),
+  InvalidTestSchema('True'),
+  InvalidTestSchema('{"no_type": "test"}'),
+  InvalidTestSchema('{"type": "panther"}'),
+] + [ValidTestSchema('"{}"'.format(t)) for t in schema.PRIMITIVE_TYPES]
+  + [ValidTestSchema({"type": t}) for t in schema.PRIMITIVE_TYPES])
 
 FIXED_EXAMPLES = [
-  ExampleSchema('{"type": "fixed", "name": "Test", "size": 1}', True),
-  ExampleSchema("""\
-    {"type": "fixed",
-     "name": "MyFixed",
-     "namespace": "org.apache.hadoop.avro",
-     "size": 1}
-    """, True),
-  ExampleSchema("""\
-    {"type": "fixed",
-     "name": "Missing size"}
-    """, False),
-  ExampleSchema("""\
-    {"type": "fixed",
-     "size": 314}
-    """, False),
+  ValidTestSchema({"type": "fixed", "name": "Test", "size": 1}),
+  ValidTestSchema({"type": "fixed", "name": "MyFixed", "size": 1,
+                   "namespace": "org.apache.hadoop.avro"}),
+  InvalidTestSchema({"type": "fixed", "name": "Missing size"}),
+  InvalidTestSchema({"type": "fixed", "size": 314}),
 ]
 
 ENUM_EXAMPLES = [
-  ExampleSchema('{"type": "enum", "name": "Test", "symbols": ["A", "B"]}', True),
-  ExampleSchema("""\
-    {"type": "enum",
-     "name": "Status",
-     "symbols": "Normal Caution Critical"}
-    """, False),
-  ExampleSchema("""\
-    {"type": "enum",
-     "name": [ 0, 1, 1, 2, 3, 5, 8 ],
-     "symbols": ["Golden", "Mean"]}
-    """, False),
-  ExampleSchema("""\
-    {"type": "enum",
-     "symbols" : ["I", "will", "fail", "no", "name"]}
-    """, False),
-  ExampleSchema("""\
-    {"type": "enum",
-     "name": "Test"
-     "symbols" : ["AA", "AA"]}
-    """, False),
+  ValidTestSchema({"type": "enum", "name": "Test", "symbols": ["A", "B"]}),
+  InvalidTestSchema({"type": "enum", "name": "Status", "symbols": "Normal Caution Critical"}),
+  InvalidTestSchema({"type": "enum", "name": [0, 1, 1, 2, 3, 5, 8],
+                     "symbols": ["Golden", "Mean"]}),
+  InvalidTestSchema({"type": "enum", "symbols" : ["I", "will", "fail", "no", "name"]}),
+  InvalidTestSchema({"type": "enum", "name": "Test", "symbols": ["AA", "AA"]}),
 ]
 
 ARRAY_EXAMPLES = [
-  ExampleSchema('{"type": "array", "items": "long"}', True),
-  ExampleSchema("""\
-    {"type": "array",
-     "items": {"type": "enum", "name": "Test", "symbols": ["A", "B"]}}
-    """, True),
+  ValidTestSchema({"type": "array", "items": "long"}),
+  ValidTestSchema({"type": "array",
+                   "items": {"type": "enum", "name": "Test", "symbols": ["A", "B"]}}),
 ]
 
 MAP_EXAMPLES = [
-  ExampleSchema('{"type": "map", "values": "long"}', True),
-  ExampleSchema("""\
-    {"type": "map",
-     "values": {"type": "enum", "name": "Test", "symbols": ["A", "B"]}}
-    """, True),
+  ValidTestSchema({"type": "map", "values": "long"}),
+  ValidTestSchema({"type": "map",
+                   "values": {"type": "enum", "name": "Test", "symbols": ["A", "B"]}}),
 ]
 
 UNION_EXAMPLES = [
-  ExampleSchema('["string", "null", "long"]', True),
-  ExampleSchema('["null", "null"]', False),
-  ExampleSchema('["long", "long"]', False),
-  ExampleSchema("""\
-    [{"type": "array", "items": "long"}
-     {"type": "array", "items": "string"}]
-    """, False),
+  ValidTestSchema(["string", "null", "long"]),
+  InvalidTestSchema(["null", "null"]),
+  InvalidTestSchema(["long", "long"]),
+  InvalidTestSchema([{"type": "array", "items": "long"},
+                     {"type": "array", "items": "string"}]),
 ]
 
 RECORD_EXAMPLES = [
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "Test",
-     "fields": [{"name": "f",
-                 "type": "long"}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "error",
-     "name": "Test",
-     "fields": [{"name": "f",
-                 "type": "long"}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "Node",
-     "fields": [{"name": "label", "type": "string"},
-                {"name": "children",
-                 "type": {"type": "array", "items": "Node"}}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "Lisp",
-     "fields": [{"name": "value",
-                 "type": ["null", "string",
-                          {"type": "record",
-                           "name": "Cons",
-                           "fields": [{"name": "car", "type": "Lisp"},
-                                      {"name": "cdr", "type": "Lisp"}]}]}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "HandshakeRequest",
-     "namespace": "org.apache.avro.ipc",
-     "fields": [{"name": "clientHash",
-                 "type": {"type": "fixed", "name": "MD5", "size": 16}},
-                {"name": "clientProtocol", "type": ["null", "string"]},
-                {"name": "serverHash", "type": "MD5"},
-                {"name": "meta", 
-                 "type": ["null", {"type": "map", "values": "bytes"}]}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "HandshakeResponse",
-     "namespace": "org.apache.avro.ipc",
-     "fields": [{"name": "match",
-                 "type": {"type": "enum",
-                          "name": "HandshakeMatch",
-                          "symbols": ["BOTH", "CLIENT", "NONE"]}},
-                {"name": "serverProtocol", "type": ["null", "string"]},
-                {"name": "serverHash",
-                 "type": ["null",
-                          {"name": "MD5", "size": 16, "type": "fixed"}]},
-                {"name": "meta",
-                 "type": ["null", {"type": "map", "values": "bytes"}]}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "Interop",
-     "namespace": "org.apache.avro",
-     "fields": [{"name": "intField", "type": "int"},
-                {"name": "longField", "type": "long"},
-                {"name": "stringField", "type": "string"},
-                {"name": "boolField", "type": "boolean"},
-                {"name": "floatField", "type": "float"},
-                {"name": "doubleField", "type": "double"},
-                {"name": "bytesField", "type": "bytes"},
-                {"name": "nullField", "type": "null"},
-                {"name": "arrayField",
-                 "type": {"type": "array", "items": "double"}},
-                {"name": "mapField",
-                 "type": {"type": "map",
-                          "values": {"name": "Foo",
-                                     "type": "record",
-                                     "fields": [{"name": "label",
-                                                 "type": "string"}]}}},
-                {"name": "unionField",
-                 "type": ["boolean",
-                          "double",
-                          {"type": "array", "items": "bytes"}]},
-                {"name": "enumField",
-                 "type": {"type": "enum",
-                          "name": "Kind",
-                          "symbols": ["A", "B", "C"]}},
-                {"name": "fixedField",
-                 "type": {"type": "fixed", "name": "MD5", "size": 16}},
-                {"name": "recordField",
-                 "type": {"type": "record",
-                          "name": "Node",
-                          "fields": [{"name": "label", "type": "string"},
-                                     {"name": "children",
-                                      "type": {"type": "array",
-                                               "items": "Node"}}]}}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "ipAddr",
-     "fields": [{"name": "addr", 
-                 "type": [{"name": "IPv6", "type": "fixed", "size": 16},
-                          {"name": "IPv4", "type": "fixed", "size": 4}]}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "Address",
-     "fields": [{"type": "string"},
-                {"type": "string", "name": "City"}]}
-    """, False),
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "Event",
-     "fields": [{"name": "Sponsor"},
-                {"name": "City", "type": "string"}]}
-    """, False),
-  ExampleSchema("""\
-    {"type": "record",
-     "fields": "His vision, from the constantly passing bars,"
-     "name", "Rainer"}
-    """, False),
-  ExampleSchema("""\
-    {"name": ["Tom", "Jerry"],
-     "type": "record",
-     "fields": [{"name": "name", "type": "string"}]}
-    """, False),
+  ValidTestSchema({"type": "record", "name": "Test", "fields": [{"name": "f", "type": "long"}]}),
+  ValidTestSchema({"type": "error", "name": "Test", "fields": [{"name": "f", "type": "long"}]}),
+  ValidTestSchema({"type": "record", "name": "Node",
+                   "fields": [
+                     {"name": "label", "type": "string"},
+                     {"name": "children", "type": {"type": "array", "items": "Node"}}]}),
+  ValidTestSchema({"type": "record", "name": "Lisp",
+                   "fields": [{"name": "value",
+                               "type": ["null", "string",
+                                        {"type": "record", "name": "Cons",
+                                         "fields": [{"name": "car", "type": "Lisp"},
+                                                    {"name": "cdr", "type": "Lisp"}]}]}]}),
+  ValidTestSchema({"type": "record", "name": "HandshakeRequest",
+                   "namespace": "org.apache.avro.ipc",
+                   "fields": [{"name": "clientHash",
+                               "type": {"type": "fixed", "name": "MD5", "size": 16}},
+                              {"name": "clientProtocol", "type": ["null", "string"]},
+                              {"name": "serverHash", "type": "MD5"},
+                              {"name": "meta",
+                               "type": ["null", {"type": "map", "values": "bytes"}]}]}),
+  ValidTestSchema({"type": "record", "name": "HandshakeResponse",
+                   "namespace": "org.apache.avro.ipc",
+                   "fields": [{"name": "match",
+                               "type": {"type": "enum", "name": "HandshakeMatch",
+                                        "symbols": ["BOTH", "CLIENT", "NONE"]}},
+                              {"name": "serverProtocol", "type": ["null", "string"]},
+                              {"name": "serverHash",
+                               "type": ["null", {"name": "MD5", "size": 16, "type": "fixed"}]},
+                              {"name": "meta",
+                               "type": ["null", {"type": "map", "values": "bytes"}]}]}),
+  ValidTestSchema({"type": "record",
+                   "name": "Interop",
+                   "namespace": "org.apache.avro",
+                   "fields": [{"name": "intField", "type": "int"},
+                              {"name": "longField", "type": "long"},
+                              {"name": "stringField", "type": "string"},
+                              {"name": "boolField", "type": "boolean"},
+                              {"name": "floatField", "type": "float"},
+                              {"name": "doubleField", "type": "double"},
+                              {"name": "bytesField", "type": "bytes"},
+                              {"name": "nullField", "type": "null"},
+                              {"name": "arrayField", "type": {"type": "array", "items": "double"}},
+                              {"name": "mapField",
+                               "type": {"type": "map",
+                                        "values": {"name": "Foo",
+                                                   "type": "record",
+                                                   "fields": [{"name": "label", "type": "string"}]}}},
+                              {"name": "unionField",
+                               "type": ["boolean", "double", {"type": "array", "items": "bytes"}]},
+                              {"name": "enumField",
+                               "type": {"type": "enum", "name": "Kind", "symbols": ["A", "B", "C"]}},
+                              {"name": "fixedField",
+                               "type": {"type": "fixed", "name": "MD5", "size": 16}},
+                              {"name": "recordField",
+                               "type": {"type": "record", "name": "Node",
+                                        "fields": [{"name": "label", "type": "string"},
+                                                   {"name": "children",
+                                                    "type": {"type": "array",
+                                                             "items": "Node"}}]}}]}),
+  ValidTestSchema({"type": "record", "name": "ipAddr",
+                   "fields": [{"name": "addr", "type": [{"name": "IPv6", "type": "fixed", "size": 16},
+                                                        {"name": "IPv4", "type": "fixed", "size": 4}]}]}),
+  InvalidTestSchema({"type": "record", "name": "Address",
+                     "fields": [{"type": "string"}, {"type": "string", "name": "City"}]}),
+  InvalidTestSchema({"type": "record", "name": "Event",
+                     "fields": [{"name": "Sponsor"}, {"name": "City", "type": "string"}]}),
+  InvalidTestSchema({"type": "record", "name": "Rainer",
+                     "fields": "His vision, from the constantly passing bars"}),
+  InvalidTestSchema({"name": ["Tom", "Jerry"], "type": "record",
+                     "fields": [{"name": "name", "type": "string"}]}),
 ]
 
 DOC_EXAMPLES = [
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "TestDoc",
-     "doc":  "Doc string",
-     "fields": [{"name": "name", "type": "string", 
-                 "doc" : "Doc String"}]}
-    """, True),
-  ExampleSchema("""\
-    {"type": "enum", "name": "Test", "symbols": ["A", "B"],
-     "doc": "Doc String"}
-    """, True),
+  ValidTestSchema({"type": "record", "name": "TestDoc", "doc": "Doc string",
+                   "fields": [{"name": "name", "type": "string", "doc" : "Doc String"}]}),
+  ValidTestSchema({"type": "enum", "name": "Test", "symbols": ["A", "B"], "doc": "Doc String"}),
 ]
 
 OTHER_PROP_EXAMPLES = [
-  ExampleSchema("""\
-    {"type": "record",
-     "name": "TestRecord",
-     "cp_string": "string",
-     "cp_int": 1,
-     "cp_array": [ 1, 2, 3, 4],
-     "fields": [ {"name": "f1", "type": "string", "cp_object": {"a":1,"b":2} },
-                 {"name": "f2", "type": "long", "cp_null": null} ]}
-    """, True),
-  ExampleSchema("""\
-     {"type": "map", "values": "long", "cp_boolean": true}
-    """, True),
-  ExampleSchema("""\
-    {"type": "enum",
-     "name": "TestEnum",
-     "symbols": [ "one", "two", "three" ],
-     "cp_float" : 1.0 }
-    """,True),
-  ExampleSchema("""\
-    {"type": "long",
-     "date": "true"}
-    """, True)
+  ValidTestSchema({"type": "record", "name": "TestRecord", "cp_string": "string",
+                   "cp_int": 1, "cp_array": [1, 2, 3, 4],
+                   "fields": [{"name": "f1", "type": "string", "cp_object": {"a": 1,"b": 2}},
+                              {"name": "f2", "type": "long", "cp_null": None}]}),
+  ValidTestSchema({"type": "map", "values": "long", "cp_boolean": True}),
+  ValidTestSchema({"type": "enum", "name": "TestEnum",
+                   "symbols": ["one", "two", "three"], "cp_float": 1.0}),
 ]
 
 DECIMAL_LOGICAL_TYPE = [
-  ExampleSchema("""{
-  "type": "fixed",
-  "logicalType": "decimal",
-  "name": "TestDecimal",
-  "precision": 4,
-  "size": 10,
-  "scale": 2}""", True),
-  ExampleSchema("""{
-  "type": "bytes",
-  "logicalType": "decimal",
-  "precision": 4,
-  "scale": 2}""", True)
+  ValidTestSchema({"type": "fixed", "logicalType": "decimal", "name": "TestDecimal", "precision": 4, "size": 10, "scale": 2}),
+  ValidTestSchema({"type": "bytes", "logicalType": "decimal", "precision": 4, "scale": 2}),
+  InvalidTestSchema({"type": "fixed", "logicalType": "decimal", "name": "TestDecimal2", "precision": 2, "scale": 2, "size": -2}),
 ]
 
 DATE_LOGICAL_TYPE = [
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "date"} """, True),
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "date1"} """, False),
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "date"} """, False),
+  ValidTestSchema({"type": "int", "logicalType": "date"})
 ]
 
 TIMEMILLIS_LOGICAL_TYPE = [
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "time-millis"} """, True),
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "time-milis"} """, False),
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "time-millis"} """, False),
+  ValidTestSchema({"type": "int", "logicalType": "time-millis"})
 ]
 
 TIMEMICROS_LOGICAL_TYPE = [
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "time-micros"} """, True),
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "time-micro"} """, False),
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "time-micros"} """, False),
+  ValidTestSchema({"type": "long", "logicalType": "time-micros"})
 ]
 
 TIMESTAMPMILLIS_LOGICAL_TYPE = [
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "timestamp-millis"} """, True),
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "timestamp-milis"} """, False),
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "timestamp-millis"} """, False),
+  ValidTestSchema({"type": "long", "logicalType": "timestamp-millis"})
 ]
 
 TIMESTAMPMICROS_LOGICAL_TYPE = [
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "timestamp-micros"} """, True),
-  ExampleSchema("""{
-  "type": "long",
-  "logicalType": "timestamp-micro"} """, False),
-  ExampleSchema("""{
-  "type": "int",
-  "logicalType": "timestamp-micros"} """, False),
+  ValidTestSchema({"type": "long", "logicalType": "timestamp-micros"})
 ]
 
+IGNORED_LOGICAL_TYPE = [
+  ValidTestSchema({"type": "string", "logicalType": "uuid"}),
+  ValidTestSchema({"type": "string", "logicalType": "unknown-logical-type"}),
+  ValidTestSchema({"type": "bytes", "logicalType": "decimal", "precision": 2, "scale": -2}),
+  ValidTestSchema({"type": "bytes", "logicalType": "decimal", "precision": -2, "scale": 2}),
+  ValidTestSchema({"type": "bytes", "logicalType": "decimal", "precision": 2, "scale": 3}),
+  ValidTestSchema({"type": "fixed", "logicalType": "decimal", "name": "TestIgnored", "precision": -10, "scale": 2, "size": 5}),
+  ValidTestSchema({"type": "fixed", "logicalType": "decimal", "name": "TestIgnored2", "precision": 2, "scale": 3, "size": 2}),
+  ValidTestSchema({"type": "int", "logicalType": "date1"}),
+  ValidTestSchema({"type": "long", "logicalType": "date"}),
+  ValidTestSchema({"type": "int", "logicalType": "time-milis"}),
+  ValidTestSchema({"type": "long", "logicalType": "time-millis"}),
+  ValidTestSchema({"type": "long", "logicalType": "time-micro"}),
+  ValidTestSchema({"type": "int", "logicalType": "time-micros"}),
+  ValidTestSchema({"type": "long", "logicalType": "timestamp-milis"}),
+  ValidTestSchema({"type": "int", "logicalType": "timestamp-millis"}),
+  ValidTestSchema({"type": "long", "logicalType": "timestamp-micro"}),
+  ValidTestSchema({"type": "int", "logicalType": "timestamp-micros"})
+]
 
 EXAMPLES = PRIMITIVE_EXAMPLES
 EXAMPLES += FIXED_EXAMPLES
 EXAMPLES += ENUM_EXAMPLES
 EXAMPLES += ARRAY_EXAMPLES
 EXAMPLES += MAP_EXAMPLES
 EXAMPLES += UNION_EXAMPLES
@@ -384,91 +246,33 @@
 EXAMPLES += DOC_EXAMPLES
 EXAMPLES += DECIMAL_LOGICAL_TYPE
 EXAMPLES += DATE_LOGICAL_TYPE
 EXAMPLES += TIMEMILLIS_LOGICAL_TYPE
 EXAMPLES += TIMEMICROS_LOGICAL_TYPE
 EXAMPLES += TIMESTAMPMILLIS_LOGICAL_TYPE
 EXAMPLES += TIMESTAMPMICROS_LOGICAL_TYPE
+EXAMPLES += IGNORED_LOGICAL_TYPE
 
 VALID_EXAMPLES = [e for e in EXAMPLES if e.valid]
+INVALID_EXAMPLES = [e for e in EXAMPLES if not e.valid]
 
-# TODO(hammer): refactor into harness for examples
-# TODO(hammer): pretty-print detailed output
-# TODO(hammer): make verbose flag
-# TODO(hammer): show strack trace to user
-# TODO(hammer): use logging module?
 class TestSchema(unittest.TestCase):
+  """Miscellaneous tests for schema"""
 
   def test_correct_recursive_extraction(self):
+    """A recursive reference within a schema should be the same type every time."""
     s = schema.parse('{"type": "record", "name": "X", "fields": [{"name": "y", "type": {"type": "record", "name": "Y", "fields": [{"name": "Z", "type": "X"}]}}]}')
     t = schema.parse(str(s.fields[0].type))
     # If we've made it this far, the subschema was reasonably stringified; it ccould be reparsed.
     self.assertEqual("X", t.fields[0].type.name)
 
-  def test_parse(self):
-    correct = 0
-    for example in EXAMPLES:
-      try:
-        schema.parse(example.schema_string)
-        if example.valid:
-          correct += 1
-        else:
-          self.fail("Invalid schema was parsed: " + example.schema_string)
-      except:
-        if not example.valid: 
-          correct += 1
-        else:
-          self.fail("Valid schema failed to parse: " + example.schema_string)
-
-    fail_msg = "Parse behavior correct on %d out of %d schemas." % \
-      (correct, len(EXAMPLES))
-    self.assertEqual(correct, len(EXAMPLES), fail_msg)
-
-  def test_valid_cast_to_string_after_parse(self):
-    """
-    Test that the string generated by an Avro Schema object
-    is, in fact, a valid Avro schema.
-    """
-    print_test_name('TEST CAST TO STRING AFTER PARSE')
-    correct = 0
-    for example in VALID_EXAMPLES:
-      schema_data = schema.parse(example.schema_string)
-      schema.parse(str(schema_data))
-      correct += 1
-
-    fail_msg = "Cast to string success on %d out of %d schemas" % \
-      (correct, len(VALID_EXAMPLES))
-    self.assertEqual(correct, len(VALID_EXAMPLES), fail_msg)
-
-  def test_equivalence_after_round_trip(self):
-    """
-    1. Given a string, parse it to get Avro schema "original".
-    2. Serialize "original" to a string and parse that string
-         to generate Avro schema "round trip".
-    3. Ensure "original" and "round trip" schemas are equivalent.
-    """
-    print_test_name('TEST ROUND TRIP')
-    correct = 0
-    for example in VALID_EXAMPLES:
-      original_schema = schema.parse(example.schema_string)
-      round_trip_schema = schema.parse(str(original_schema))
-      if original_schema == round_trip_schema:
-        correct += 1
-        debug_msg = "%s: ROUND TRIP SUCCESS" % example.name
-      else:       
-        debug_msg = "%s: ROUND TRIP FAILURE" % example.name
-        self.fail("Round trip failure: %s, %s, %s" % (example.name, original_schema, str(original_schema)))
-
-    fail_msg = "Round trip success on %d out of %d schemas" % \
-      (correct, len(VALID_EXAMPLES))
-    self.assertEqual(correct, len(VALID_EXAMPLES), fail_msg)
-
   # TODO(hammer): more tests
   def test_fullname(self):
-    """
+    """Test schema full names
+
     The fullname is determined in one of the following ways:
      * A name and namespace are both specified.  For example,
        one might use "name": "X", "namespace": "org.foo"
        to indicate the fullname "org.foo.X".
      * A fullname is specified.  If the name specified contains
        a dot, then it is assumed to be a fullname, and any
        namespace also specified is ignored.  For example,
@@ -487,24 +291,23 @@
     the enclosing definition.
 
     Primitive type names have no namespace and their names may
     not be defined in any namespace.  A schema may only contain
     multiple definitions of a fullname if the definitions are
     equivalent.
     """
-    print_test_name('TEST FULLNAME')
 
-    # name and namespace specified    
+    # name and namespace specified
     fullname = schema.Name('a', 'o.a.h', None).fullname
     self.assertEqual(fullname, 'o.a.h.a')
 
     # fullname and namespace specified
     fullname = schema.Name('a.b.c.d', 'o.a.h', None).fullname
     self.assertEqual(fullname, 'a.b.c.d')
-    
+
     # name and default namespace specified
     fullname = schema.Name('a', None, 'b.c.d').fullname
     self.assertEqual(fullname, 'b.c.d.a')
 
     # fullname and default namespace specified
     fullname = schema.Name('a.b.c.d', None, 'o.a.h').fullname
     self.assertEqual(fullname, 'a.b.c.d')
@@ -513,141 +316,191 @@
     fullname = schema.Name('a.b.c.d', 'o.a.a', 'o.a.h').fullname
     self.assertEqual(fullname, 'a.b.c.d')
 
     # name, namespace, default namespace specified
     fullname = schema.Name('a', 'o.a.a', 'o.a.h').fullname
     self.assertEqual(fullname, 'o.a.a.a')
 
-  def test_doc_attributes(self):
-    print_test_name('TEST DOC ATTRIBUTES')
-    correct = 0
-    for example in DOC_EXAMPLES:
-      original_schema = schema.parse(example.schema_string)
-      if original_schema.doc is not None:
-        correct += 1
-      if original_schema.type == 'record':
-        for f in original_schema.fields:
-          if f.doc is None:
-            self.fail("Failed to preserve 'doc' in fields: " + example.schema_string)
-    self.assertEqual(correct,len(DOC_EXAMPLES))
-
-  def test_other_attributes(self):
-    print_test_name('TEST OTHER ATTRIBUTES')
-    correct = 0
-    props = {}
-    for example in OTHER_PROP_EXAMPLES:
-      original_schema = schema.parse(example.schema_string)
-      round_trip_schema = schema.parse(str(original_schema))
-      self.assertEqual(original_schema.other_props,round_trip_schema.other_props)
-      if original_schema.type == "record":
-        field_props = 0
-        for f in original_schema.fields:
-          if f.other_props:
-            props.update(f.other_props)
-            field_props += 1
-        self.assertEqual(field_props,len(original_schema.fields))
-      if original_schema.other_props:
-        props.update(original_schema.other_props)
-        correct += 1
-    for k in props:
-      v = props[k]
-      if k == "cp_boolean":
-        self.assertEqual(type(v), bool)
-      elif k == "cp_int":
-        self.assertEqual(type(v), int)
-      elif k == "cp_object":
-        self.assertEqual(type(v), dict)
-      elif k == "cp_float":
-        self.assertEqual(type(v), float)
-      elif k == "cp_array":
-        self.assertEqual(type(v), list)
-    self.assertEqual(correct,len(OTHER_PROP_EXAMPLES))
-
   def test_exception_is_not_swallowed_on_parse_error(self):
-    print_test_name('TEST EXCEPTION NOT SWALLOWED ON PARSE ERROR')
-
+    """A specific exception message should appear on a json parse error."""
     try:
         schema.parse('/not/a/real/file')
         caught_exception = False
-    except schema.SchemaParseException, e:
+    except schema.SchemaParseException as e:
         expected_message = 'Error parsing JSON: /not/a/real/file, error = ' \
                            'No JSON object could be decoded'
         self.assertEqual(expected_message, e.args[0])
         caught_exception = True
 
     self.assertTrue(caught_exception, 'Exception was not caught')
 
-  def test_decimal_invalid_schema(self):
-    invalid_schemas = [
-      ExampleSchema("""{
-      "type": "bytes",
+  def test_decimal_valid_type(self):
+    fixed_decimal_schema = ValidTestSchema({
+      "type": "fixed",
       "logicalType": "decimal",
-      "precision": 2,
-      "scale": -2}""", True),
+      "name": "TestDecimal",
+      "precision": 4,
+      "scale": 2,
+      "size": 2})
 
-      ExampleSchema("""{
+    bytes_decimal_schema = ValidTestSchema({
       "type": "bytes",
       "logicalType": "decimal",
-      "precision": -2,
-      "scale": 2}""", True),
+      "precision": 4})
 
-      ExampleSchema("""{
-      "type": "bytes",
-      "logicalType": "decimal",
-      "precision": 2,
-      "scale": 3}""", True),
+    fixed_decimal = fixed_decimal_schema.parse()
+    self.assertEqual(4, fixed_decimal.get_prop('precision'))
+    self.assertEqual(2, fixed_decimal.get_prop('scale'))
+    self.assertEqual(2, fixed_decimal.get_prop('size'))
 
-      ExampleSchema("""{
+    bytes_decimal = bytes_decimal_schema.parse()
+    self.assertEqual(4, bytes_decimal.get_prop('precision'))
+    self.assertEqual(0, bytes_decimal.get_prop('scale'))
+
+  def test_fixed_decimal_valid_max_precision(self):
+    # An 8 byte number can represent any 18 digit number.
+    fixed_decimal_schema = ValidTestSchema({
       "type": "fixed",
       "logicalType": "decimal",
       "name": "TestDecimal",
-      "precision": -10,
-      "scale": 2,
-      "size": 5}""", True),
-
-
-      ExampleSchema("""{
+      "precision": 18,
+      "scale": 0,
+      "size": 8})
+
+    fixed_decimal = fixed_decimal_schema.parse()
+    self.assertIsInstance(fixed_decimal, schema.FixedSchema)
+    self.assertIsInstance(fixed_decimal, schema.DecimalLogicalSchema)
+
+  def test_fixed_decimal_invalid_max_precision(self):
+    # An 8 byte number can't represent every 19 digit number, so the logical
+    # type is not applied.
+    fixed_decimal_schema = ValidTestSchema({
       "type": "fixed",
       "logicalType": "decimal",
       "name": "TestDecimal",
-      "precision": 2,
-      "scale": 3,
-      "size": 2}""", True)
-    ]
-
-    for invalid_schema in invalid_schemas:
-      self.assertRaises(SchemaParseException, schema.parse, invalid_schema.schema_string)
-
-    fixed_invalid_schema_size = ExampleSchema("""{
-                                "type": "fixed",
-                                "logicalType": "decimal",
-                                "name": "TestDecimal",
-                                "precision": 2,
-                                "scale": 2,
-                                "size": -2}""", True)
-    self.assertRaises(AvroException, schema.parse, fixed_invalid_schema_size.schema_string)
+      "precision": 19,
+      "scale": 0,
+      "size": 8})
+
+    fixed_decimal = fixed_decimal_schema.parse()
+    self.assertIsInstance(fixed_decimal, schema.FixedSchema)
+    self.assertNotIsInstance(fixed_decimal, schema.DecimalLogicalSchema)
+
+class SchemaParseTestCase(unittest.TestCase):
+  """Enable generating parse test cases over all the valid and invalid example schema."""
+
+  def __init__(self, test_schema):
+    """Ignore the normal signature for unittest.TestCase because we are generating
+    many test cases from this one class. This is safe as long as the autoloader
+    ignores this class. The autoloader will ignore this class as long as it has
+    no methods starting with `test_`.
+    """
+    super(SchemaParseTestCase, self).__init__(
+        'parse_valid' if test_schema.valid else 'parse_invalid')
+    self.test_schema = test_schema
 
-  def test_decimal_valid_type(self):
-    fixed_decimal_schema = ExampleSchema("""{
-    "type": "fixed",
-    "logicalType": "decimal",
-    "name": "TestDecimal",
-    "precision": 4,
-    "scale": 2,
-    "size": 2}""", True)
-
-    bytes_decimal_schema = ExampleSchema("""{
-    "type": "bytes",
-    "logicalType": "decimal",
-    "precision": 4}""", True)
+  def parse_valid(self):
+    """Parsing a valid schema should not error."""
+    try:
+      self.test_schema.parse()
+    except (schema.AvroException, schema.SchemaParseException):
+      self.fail("Valid schema failed to parse: {!s}".format(self.test_schema))
 
-    fixed_decimal = schema.parse(fixed_decimal_schema.schema_string)
-    self.assertEqual(4, fixed_decimal.get_prop('precision'))
-    self.assertEqual(2, fixed_decimal.get_prop('scale'))
-    self.assertEqual(2, fixed_decimal.get_prop('size'))
+  def parse_invalid(self):
+    """Parsing an invalid schema should error."""
+    try:
+      self.test_schema.parse()
+    except (schema.AvroException, schema.SchemaParseException):
+      pass
+    else:
+      self.fail("Invalid schema should not have parsed: {!s}".format(self.test_schema))
+
+class RoundTripParseTestCase(unittest.TestCase):
+  """Enable generating round-trip parse test cases over all the valid test schema."""
+
+  def __init__(self, test_schema):
+    """Ignore the normal signature for unittest.TestCase because we are generating
+    many test cases from this one class. This is safe as long as the autoloader
+    ignores this class. The autoloader will ignore this class as long as it has
+    no methods starting with `test_`.
+    """
+    super(RoundTripParseTestCase, self).__init__('parse_round_trip')
+    self.test_schema = test_schema
 
-    bytes_decimal = schema.parse(bytes_decimal_schema.schema_string)
-    self.assertEqual(4, bytes_decimal.get_prop('precision'))
-    self.assertEqual(0, bytes_decimal.get_prop('scale'))
+  def parse_round_trip(self):
+    """The string of a Schema should be parseable to the same Schema."""
+    parsed = self.test_schema.parse()
+    round_trip = schema.parse(str(parsed))
+    self.assertEqual(parsed, round_trip)
+
+class DocAttributesTestCase(unittest.TestCase):
+  """Enable generating document attribute test cases over all the document test schema."""
+
+  def __init__(self, test_schema):
+    """Ignore the normal signature for unittest.TestCase because we are generating
+    many test cases from this one class. This is safe as long as the autoloader
+    ignores this class. The autoloader will ignore this class as long as it has
+    no methods starting with `test_`.
+    """
+    super(DocAttributesTestCase, self).__init__('check_doc_attributes')
+    self.test_schema = test_schema
+
+  def check_doc_attributes(self):
+    """Documentation attributes should be preserved."""
+    sch = self.test_schema.parse()
+    self.assertIsNotNone(sch.doc, "Failed to preserve 'doc' in schema: {!s}".format(self.test_schema))
+    if sch.type == 'record':
+      for f in sch.fields:
+        self.assertIsNotNone(f.doc, "Failed to preserve 'doc' in fields: {!s}".format(self.test_schema))
+
+
+class OtherAttributesTestCase(unittest.TestCase):
+  """Enable generating attribute test cases over all the other-prop test schema."""
+  _type_map = {
+    "cp_array": list,
+    "cp_boolean": bool,
+    "cp_float": float,
+    "cp_int": int,
+    "cp_null": type(None),
+    "cp_object": dict,
+    "cp_string": basestring,
+  }
+
+  def __init__(self, test_schema):
+    """Ignore the normal signature for unittest.TestCase because we are generating
+    many test cases from this one class. This is safe as long as the autoloader
+    ignores this class. The autoloader will ignore this class as long as it has
+    no methods starting with `test_`.
+    """
+    super(OtherAttributesTestCase, self).__init__('check_attributes')
+    self.test_schema = test_schema
+
+  def _check_props(self, props):
+    for k, v in props.items():
+      self.assertIsInstance(v, self._type_map[k])
+
+  def check_attributes(self):
+    """Other attributes and their types on a schema should be preserved."""
+    sch = self.test_schema.parse()
+    round_trip = schema.parse(str(sch))
+    self.assertEqual(sch.other_props, round_trip.other_props,
+                     "Properties were not preserved in a round-trip parse.")
+    self._check_props(sch.other_props)
+    if sch.type == "record":
+      field_props = [f.other_props for f in sch.fields if f.other_props]
+      self.assertEqual(len(field_props), len(sch.fields))
+      for p in field_props:
+        self._check_props(p)
+
+
+def load_tests(loader, default_tests, pattern):
+  """Generate test cases across many test schema."""
+  suite = unittest.TestSuite()
+  suite.addTests(loader.loadTestsFromTestCase(TestSchema))
+  suite.addTests(SchemaParseTestCase(ex) for ex in EXAMPLES)
+  suite.addTests(RoundTripParseTestCase(ex) for ex in VALID_EXAMPLES)
+  suite.addTests(DocAttributesTestCase(ex) for ex in DOC_EXAMPLES)
+  suite.addTests(OtherAttributesTestCase(ex) for ex in OTHER_PROP_EXAMPLES)
+  return suite
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `avro-1.9.1/test/test_tether_task_runner.py` & `avro-1.9.2/test/test_tether_task_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -10,68 +13,73 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import absolute_import, division, print_function
+
+import logging
 import os
+import StringIO
 import subprocess
 import sys
 import time
 import unittest
 
+import avro.tether.tether_task
+import avro.tether.tether_task_runner
+import avro.tether.util
+import mock_tether_parent
 import set_avro_test_path
+from avro import io as avio
+from word_count_task import WordCountTask
 
 
 class TestTetherTaskRunner(unittest.TestCase):
-  """ unit test for a tethered task runner.
-  """
+  """unit test for a tethered task runner."""
 
   def test1(self):
-    from word_count_task import WordCountTask
-    from avro.tether import TaskRunner, find_port,HTTPRequestor,inputProtocol, TaskType
-    from avro import io as avio
-    import mock_tether_parent
-    import subprocess
-    import StringIO
-    import logging
-
     # set the logging level to debug so that debug messages are printed
     logging.basicConfig(level=logging.DEBUG)
 
     proc=None
     try:
       # launch the server in a separate process
       env=dict()
       env["PYTHONPATH"]=':'.join(sys.path)
-      parent_port=find_port()
+      parent_port = avro.tether.util.find_port()
 
       pyfile=mock_tether_parent.__file__
       proc=subprocess.Popen(["python", pyfile,"start_server","{0}".format(parent_port)])
-      input_port=find_port()
+      input_port = avro.tether.util.find_port()
 
-      print "Mock server started process pid={0}".format(proc.pid)
+      print("Mock server started process pid={0}".format(proc.pid))
       # Possible race condition? open tries to connect to the subprocess before the subprocess is fully started
       # so we give the subprocess time to start up
       time.sleep(1)
 
-      runner=TaskRunner(WordCountTask())
+      runner = avro.tether.tether_task_runner.TaskRunner(WordCountTask())
 
       runner.start(outputport=parent_port,join=False)
 
-      # Test sending various messages to the server and ensuring they are
-      # processed correctly
-      requestor=HTTPRequestor("localhost",runner.server.server_address[1],inputProtocol)
+      # Test sending various messages to the server and ensuring they are processed correctly
+      requestor = avro.tether.tether_task.HTTPRequestor(
+          "localhost", runner.server.server_address[1], avro.tether.tether_task.inputProtocol)
 
       # TODO: We should validate that open worked by grabbing the STDOUT of the subproces
       # and ensuring that it outputted the correct message.
 
       # Test the mapper
-      requestor.request("configure",{"taskType":TaskType.MAP,"inSchema":str(runner.task.inschema),"outSchema":str(runner.task.midschema)})
+      requestor.request("configure", {
+        "taskType": avro.tether.tether_task.TaskType.MAP,
+        "inSchema": str(runner.task.inschema),
+        "outSchema": str(runner.task.midschema)
+      })
 
       # Serialize some data so we can send it to the input function
       datum="This is a line of text"
       writer = StringIO.StringIO()
       encoder = avio.BinaryEncoder(writer)
       datum_writer = avio.DatumWriter(runner.task.inschema)
       datum_writer.write(datum, encoder)
@@ -79,16 +87,20 @@
       writer.seek(0)
       data=writer.read()
 
 
       # Call input to simulate calling map
       requestor.request("input",{"data":data,"count":1})
 
-      #Test the reducer
-      requestor.request("configure",{"taskType":TaskType.REDUCE,"inSchema":str(runner.task.midschema),"outSchema":str(runner.task.outschema)})
+      # Test the reducer
+      requestor.request("configure", {
+        "taskType": avro.tether.tether_task.TaskType.REDUCE,
+        "inSchema": str(runner.task.midschema),
+        "outSchema": str(runner.task.outschema)}
+      )
 
       #Serialize some data so we can send it to the input function
       datum={"key":"word","value":2}
       writer = StringIO.StringIO()
       encoder = avio.BinaryEncoder(writer)
       datum_writer = avio.DatumWriter(runner.task.midschema)
       datum_writer.write(datum, encoder)
@@ -129,53 +141,44 @@
 
   def test2(self):
     """
     In this test we want to make sure that when we run "tether_task_runner.py"
     as our main script everything works as expected. We do this by using subprocess to run it
     in a separate thread.
     """
-    from word_count_task import WordCountTask
-    from avro.tether import TaskRunner, find_port,HTTPRequestor,inputProtocol, TaskType
-    from avro.tether import tether_task_runner
-    from avro import io as avio
-    import mock_tether_parent
-    import subprocess
-    import StringIO
-
-
     proc=None
 
     runnerproc=None
     try:
       #launch the server in a separate process
       env=dict()
       env["PYTHONPATH"]=':'.join(sys.path)
-      parent_port=find_port()
+      parent_port = avro.tether.util.find_port()
 
       pyfile=mock_tether_parent.__file__
       proc=subprocess.Popen(["python", pyfile,"start_server","{0}".format(parent_port)])
 
       #Possible race condition? when we start tether_task_runner it will call
       # open tries to connect to the subprocess before the subprocess is fully started
       #so we give the subprocess time to start up
       time.sleep(1)
 
 
       #start the tether_task_runner in a separate process
       env={"AVRO_TETHER_OUTPUT_PORT":"{0}".format(parent_port)}
       env["PYTHONPATH"]=':'.join(sys.path)
 
-      runnerproc=subprocess.Popen(["python",tether_task_runner.__file__,"word_count_task.WordCountTask"],env=env)
+      runnerproc = subprocess.Popen(["python", avro.tether.tether_task_runner.__file__, "word_count_task.WordCountTask"],env=env)
 
       #possible race condition wait for the process to start
       time.sleep(1)
 
 
 
-      print "Mock server started process pid={0}".format(proc.pid)
+      print("Mock server started process pid={0}".format(proc.pid))
       #Possible race condition? open tries to connect to the subprocess before the subprocess is fully started
       #so we give the subprocess time to start up
       time.sleep(1)
 
 
     except Exception as e:
       raise
```

### Comparing `avro-1.9.1/scripts/avro` & `avro-1.9.2/scripts/avro`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Command line utlity for reading and writing Avro files."""
 
-from avro.io import DatumReader, DatumWriter
-from avro.datafile import DataFileReader, DataFileWriter
-import avro.schema
+"""Command line utility for reading and writing Avro files."""
+
+from __future__ import absolute_import, division, print_function
 
-try:
-    import json
-except ImportError:
-    import simplejson as json
 import csv
-from sys import stdout, stdin
-from itertools import ifilter, imap
+import json
 from functools import partial
+from itertools import ifilter, imap
 from os.path import splitext
+from sys import stdin, stdout
+
+import avro.schema
+from avro.datafile import DataFileReader, DataFileWriter
+from avro.io import DatumReader, DatumWriter
+
 
 class AvroError(Exception):
     pass
 
 def print_json(row):
     print(json.dumps(row))
 
@@ -50,17 +51,17 @@
 def print_csv(row):
     # We sort the keys to the fields will be in the same place
     # FIXME: Do we want to do it in schema order?
     _write_row([_encode(row[key]) for key in sorted(row)])
 
 def select_printer(format):
     return {
-        "json" : print_json,
-        "json-pretty" : print_json_pretty,
-        "csv" : print_csv
+        "json": print_json,
+        "json-pretty": print_json_pretty,
+        "csv": print_csv
     }[format]
 
 def record_match(expr, record):
     return eval(expr, None, {"r" : record})
 
 def parse_fields(fields):
     fields = fields or ''
@@ -100,15 +101,15 @@
         if i >= opts.count:
             break
         printer(record)
 
 def print_schema(avro):
     schema = avro.meta["avro.schema"]
     # Pretty print
-    print json.dumps(json.loads(schema), indent=4)
+    print(json.dumps(json.loads(schema), indent=4))
 
 def cat(opts, args):
     if not args:
         raise AvroError("No files to show")
 
     for filename in args:
         try:
@@ -205,15 +206,15 @@
 def main(argv=None):
     import sys
     from optparse import OptionParser, OptionGroup
 
     argv = argv or sys.argv
 
     parser = OptionParser(description="Display/write for Avro files",
-                      version="1.9.1",
+                      version="1.9.2",
                       usage="usage: %prog cat|write [options] FILE [FILE...]")
     # cat options
 
     cat_options = OptionGroup(parser, "cat options")
     cat_options.add_option("-n", "--count", default=float("Infinity"),
                     help="number of records to print", type=int)
     cat_options.add_option("-s", "--skip", help="number of records to skip",
@@ -255,8 +256,7 @@
     except AvroError, e:
         parser.error("%s" % e) # Will exit
     except Exception, e:
         raise SystemExit("panic: %s" % e)
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `avro-1.9.1/src/avro/datafile.py` & `avro-1.9.2/src/avro/datafile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -9,29 +12,39 @@
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-Read/Write Avro File Object Containers.
-"""
+
+"""Read/Write Avro File Object Containers."""
+
+from __future__ import absolute_import, division, print_function
+
+import os
+import random
 import zlib
+
+from avro import io, schema
+
 try:
   from cStringIO import StringIO
 except ImportError:
   from StringIO import StringIO
-from avro import schema
-from avro import io
 try:
   import snappy
   has_snappy = True
 except ImportError:
   has_snappy = False
+try:
+  import zstandard as zstd
+  has_zstandard = True
+except ImportError:
+  has_zstandard = False
 #
 # Constants
 #
 
 VERSION = 1
 MAGIC = 'Obj' + chr(VERSION)
 MAGIC_SIZE = len(MAGIC)
@@ -43,14 +56,16 @@
    {"name": "magic", "type": {"type": "fixed", "name": "magic", "size": %d}},
    {"name": "meta", "type": {"type": "map", "values": "bytes"}},
    {"name": "sync", "type": {"type": "fixed", "name": "sync", "size": %d}}]}
 """ % (MAGIC_SIZE, SYNC_SIZE))
 VALID_CODECS = ['null', 'deflate']
 if has_snappy:
     VALID_CODECS.append('snappy')
+if has_zstandard:
+    VALID_CODECS.append('zstandard')
 VALID_ENCODINGS = ['binary'] # not used yet
 
 CODEC_KEY = "avro.codec"
 SCHEMA_KEY = "avro.schema"
 
 #
 # Exceptions
@@ -94,15 +109,15 @@
       self._sync_marker = DataFileWriter.generate_sync_marker()
       self.set_meta('avro.codec', codec)
       self.set_meta('avro.schema', str(writers_schema))
       self.datum_writer.writers_schema = writers_schema
     else:
       # open writer for reading to collect metadata
       dfr = DataFileReader(writer, io.DatumReader())
-      
+
       # TODO(hammer): collect arbitrary metadata
       # collect metadata
       self._sync_marker = dfr.sync_marker
       self.set_meta('avro.codec', dfr.get_meta('avro.codec'))
 
       # get schema used to write existing file
       schema_from_file = dfr.get_meta('avro.schema')
@@ -166,33 +181,36 @@
         # The first two characters and last character are zlib
         # wrappers around deflate data.
         compressed_data = zlib.compress(uncompressed_data)[2:-1]
         compressed_data_length = len(compressed_data)
       elif self.get_meta(CODEC_KEY) == 'snappy':
         compressed_data = snappy.compress(uncompressed_data)
         compressed_data_length = len(compressed_data) + 4 # crc32
+      elif self.get_meta(CODEC_KEY) == 'zstandard':
+        compressed_data = zstd.ZstdCompressor().compress(uncompressed_data)
+        compressed_data_length = len(compressed_data)
       else:
         fail_msg = '"%s" codec is not supported.' % self.get_meta(CODEC_KEY)
         raise DataFileException(fail_msg)
 
       # Write length of block
       self.encoder.write_long(compressed_data_length)
 
       # Write block
       self.writer.write(compressed_data)
-      
+
       # Write CRC32 checksum for Snappy
       if self.get_meta(CODEC_KEY) == 'snappy':
         self.encoder.write_crc32(uncompressed_data)
 
       # write sync marker
       self.writer.write(self.sync_marker)
 
       # reset buffer
-      self.buffer_writer.truncate(0) 
+      self.buffer_writer.truncate(0)
       self.block_count = 0
 
   def append(self, datum):
     """Append a datum to the file."""
     self.datum_writer.write(datum, self.buffer_encoder)
     self.block_count += 1
 
@@ -224,15 +242,15 @@
   # TODO(hammer): allow user to specify expected schema?
   # TODO(hammer): allow user to specify the encoder
   def __init__(self, reader, datum_reader):
     self._reader = reader
     self._raw_decoder = io.BinaryDecoder(reader)
     self._datum_decoder = None # Maybe reset at every block.
     self._datum_reader = datum_reader
-    
+
     # read the header: magic, meta, sync
     self._read_header()
 
     # ensure codec is valid
     self.codec = self.get_meta('avro.codec')
     if self.codec is None:
       self.codec = "null"
@@ -288,15 +306,15 @@
     return file_length
 
   def is_EOF(self):
     return self.reader.tell() == self.file_length
 
   def _read_header(self):
     # seek to the beginning of the file to get magic block
-    self.reader.seek(0, 0) 
+    self.reader.seek(0, 0)
 
     # read header into a dict
     header = self.datum_reader.read_data(
       META_SCHEMA, META_SCHEMA, self.raw_decoder)
 
     # check magic number
     if header.get('magic') != MAGIC:
@@ -327,14 +345,26 @@
     elif self.codec == 'snappy':
       # Compressed data includes a 4-byte CRC32 checksum
       length = self.raw_decoder.read_long()
       data = self.raw_decoder.read(length - 4)
       uncompressed = snappy.decompress(data)
       self._datum_decoder = io.BinaryDecoder(StringIO(uncompressed))
       self.raw_decoder.check_crc32(uncompressed);
+    elif self.codec == 'zstandard':
+      length = self.raw_decoder.read_long()
+      data = self.raw_decoder.read(length)
+      uncompressed = bytearray()
+      dctx = zstd.ZstdDecompressor()
+      with dctx.stream_reader(StringIO(data)) as reader:
+        while True:
+          chunk = reader.read(16384)
+          if not chunk:
+            break
+          uncompressed.extend(chunk)
+      self._datum_decoder = io.BinaryDecoder(StringIO(uncompressed))
     else:
       raise DataFileException("Unknown codec: %r" % self.codec)
 
   def _skip_sync(self):
     """
     Read the length of the sync marker; if it matches the sync marker,
     return True. Otherwise, seek back to where we started and return False.
@@ -355,22 +385,20 @@
         raise StopIteration
       elif self._skip_sync():
         if self.is_EOF(): raise StopIteration
         self._read_block_header()
       else:
         self._read_block_header()
 
-    datum = self.datum_reader.read(self.datum_decoder) 
+    datum = self.datum_reader.read(self.datum_decoder)
     self.block_count -= 1
     return datum
 
   def close(self):
     """Close this reader."""
     self.reader.close()
 
 def generate_sixteen_random_bytes():
   try:
-    import os
     return os.urandom(16)
-  except:
-    import random
-    return [ chr(random.randrange(256)) for i in range(16) ]
+  except NotImplementedError:
+    return bytes(random.randrange(256) for i in range(16))
```

### Comparing `avro-1.9.1/src/avro/LICENSE` & `avro-1.9.2/src/avro/LICENSE`

 * *Files identical despite different names*

### Comparing `avro-1.9.1/src/avro/ipc.py` & `avro-1.9.2/src/avro/ipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-Support for inter-process calls.
-"""
+
+"""Support for inter-process calls."""
+
+from __future__ import absolute_import, division, print_function
+
 import httplib
+
+from avro import io, protocol, schema
+
 try:
   from cStringIO import StringIO
 except ImportError:
   from StringIO import StringIO
-from avro import io
-from avro import protocol
-from avro import schema
 
 #
 # Constants
 #
 
 # Handshake schema is pulled in during build
 HANDSHAKE_REQUEST_SCHEMA = schema.parse("""
@@ -211,15 +216,15 @@
   def read_call_response(self, message_name, decoder):
     """
     The format of a call response is:
       * response metadata, a map with values of type bytes
       * a one-byte error flag boolean, followed by either:
         o if the error flag is false,
           the message response, serialized per the message's response schema.
-        o if the error flag is true, 
+        o if the error flag is true,
           the error, serialized per the message's error union schema.
     """
     # response metadata
     response_metadata = META_READER.read(decoder)
 
     # remote response schema
     remote_message_schema = self.remote_protocol.messages.get(message_name)
@@ -289,19 +294,19 @@
     """
     buffer_reader = StringIO(call_request)
     buffer_decoder = io.BinaryDecoder(buffer_reader)
     buffer_writer = StringIO()
     buffer_encoder = io.BinaryEncoder(buffer_writer)
     error = None
     response_metadata = {}
-    
+
     try:
       remote_protocol = self.process_handshake(buffer_decoder, buffer_encoder)
       # handshake failure
-      if remote_protocol is None:  
+      if remote_protocol is None:
         return buffer_writer.getvalue()
 
       # read request using remote protocol
       request_metadata = META_READER.read(buffer_decoder)
       remote_message_name = buffer_decoder.read_utf8()
 
       # get remote and local request schemas so we can do
@@ -318,29 +323,29 @@
       readers_schema = local_message.request
       request = self.read_request(writers_schema, readers_schema,
                                   buffer_decoder)
 
       # perform server logic
       try:
         response = self.invoke(local_message, request)
-      except AvroRemoteException, e:
+      except AvroRemoteException as e:
         error = e
-      except Exception, e:
+      except Exception as e:
         error = AvroRemoteException(str(e))
 
       # write response using local protocol
       META_WRITER.write(response_metadata, buffer_encoder)
       buffer_encoder.write_boolean(error is not None)
       if error is None:
         writers_schema = local_message.response
         self.write_response(writers_schema, response, buffer_encoder)
       else:
         writers_schema = local_message.errors
         self.write_error(writers_schema, error, buffer_encoder)
-    except schema.AvroException, e:
+    except schema.AvroException as e:
       error = AvroRemoteException(str(e))
       buffer_encoder = io.BinaryEncoder(StringIO())
       META_WRITER.write(response_metadata, buffer_encoder)
       buffer_encoder.write_boolean(True)
       self.write_error(SYSTEM_ERROR_SCHEMA, error, buffer_encoder)
     return buffer_writer.getvalue()
 
@@ -504,8 +509,7 @@
 
   def close(self):
     self.conn.close()
 
 #
 # Server Implementations (none yet)
 #
-
```

### Comparing `avro-1.9.1/src/avro/protocol.py` & `avro-1.9.2/src/avro/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-Protocol implementation.
-"""
+
+"""Protocol implementation."""
+
+from __future__ import absolute_import, division, print_function
+
+import json
+
+from avro import schema
+
 try:
   from hashlib import md5
 except ImportError:
   from md5 import md5
-try:
-  import json
-except ImportError:
-  import simplejson as json
-from avro import schema
+
 
 #
 # Constants
 #
 
 # TODO(hammer): confirmed 'fixed' with Doug
 VALID_TYPE_SCHEMA_TYPES = ('enum', 'record', 'error', 'fixed')
@@ -55,15 +57,15 @@
         raise ProtocolParseException(fail_msg)
       type_objects.append(type_object)
     return type_objects
 
   def _parse_messages(self, messages, names):
     message_objects = {}
     for name, body in messages.iteritems():
-      if message_objects.has_key(name):
+      if name in message_objects:
         fail_msg = 'Message name "%s" repeated.' % name
         raise ProtocolParseException(fail_msg)
       try:
         request = body.get('request')
         response = body.get('response')
         errors = body.get('errors')
       except AttributeError:
@@ -212,12 +214,12 @@
     raise ProtocolParseException('Not a JSON object: %s' % json_data)
   return Protocol(name, namespace, types, messages)
 
 def parse(json_string):
   """Constructs the Protocol from the JSON text."""
   try:
     json_data = json.loads(json_string)
-  except:
+  except ValueError:
     raise ProtocolParseException('Error parsing JSON: %s' % json_string)
 
   # construct the Avro Protocol object
   return make_avpr_object(json_data)
```

### Comparing `avro-1.9.1/src/avro/constants.py` & `avro-1.9.2/src/avro/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Contains Constants for Python Avro
-"""
+"""Contains Constants for Python Avro"""
+
+from __future__ import absolute_import, division, print_function
 
 DATE = "date"
 DECIMAL = "decimal"
 TIMESTAMP_MICROS = "timestamp-micros"
 TIMESTAMP_MILLIS = "timestamp-millis"
 TIME_MICROS = "time-micros"
 TIME_MILLIS = "time-millis"
```

### Comparing `avro-1.9.1/src/avro/io.py` & `avro-1.9.2/src/avro/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """
 Input/Output utilities, including:
 
  * i/o-specific constants
  * i/o-specific exceptions
  * schema validation
  * leaf value encoding and decoding
@@ -30,31 +34,27 @@
   * Schema maps are implemented as dict.
   * Schema strings are implemented as unicode.
   * Schema bytes are implemented as str.
   * Schema ints are implemented as int.
   * Schema longs are implemented as long.
   * Schema floats are implemented as float.
   * Schema doubles are implemented as float.
-  * Schema booleans are implemented as bool. 
+  * Schema booleans are implemented as bool.
 """
+
+from __future__ import absolute_import, division, print_function
+
+import datetime
+import json
 import struct
-from avro import schema
-from avro import constants
-from avro import timezones
 import sys
 from binascii import crc32
-import datetime
-
-from decimal import Decimal
-from decimal import getcontext
+from decimal import Decimal, getcontext
 
-try:
-	import json
-except ImportError:
-	import simplejson as json
+from avro import constants, schema, timezones
 
 #
 # Constants
 #
 
 INT_MIN_VALUE = -(1 << 31)
 INT_MAX_VALUE = (1 << 31) - 1
@@ -70,23 +70,22 @@
       self.format = format
     def pack(self, *args):
       return struct.pack(self.format, *args)
     def unpack(self, *args):
       return struct.unpack(self.format, *args)
   struct_class = SimpleStruct
 
-STRUCT_INT = struct_class('!I')             # big-endian unsigned int
-STRUCT_LONG = struct_class('!Q')            # big-endian unsigned long long
-STRUCT_FLOAT = struct_class('!f')           # big-endian float
-STRUCT_DOUBLE = struct_class('!d')          # big-endian double
+STRUCT_FLOAT = struct_class('<f')           # big-endian float
+STRUCT_DOUBLE = struct_class('<d')          # big-endian double
 STRUCT_CRC32 = struct_class('>I')           # big-endian unsigned int
 STRUCT_SIGNED_SHORT = struct_class('>h')    # big-endian signed short
 STRUCT_SIGNED_INT = struct_class('>i')      # big-endian signed int
 STRUCT_SIGNED_LONG = struct_class('>q')     # big-endian signed long
 
+
 #
 # Exceptions
 #
 
 class AvroTypeException(schema.AvroException):
   """Raised when datum is not an example of schema."""
   def __init__(self, expected_schema, datum):
@@ -102,73 +101,67 @@
     if writers_schema: fail_msg += "\nWriter's Schema: %s" % pretty_writers
     if readers_schema: fail_msg += "\nReader's Schema: %s" % pretty_readers
     schema.AvroException.__init__(self, fail_msg)
 
 #
 # Validate
 #
-
 def _is_timezone_aware_datetime(dt):
   return dt.tzinfo is not None and dt.tzinfo.utcoffset(dt) is not None
 
+_valid = {
+  'null': lambda s, d: d is None,
+  'boolean': lambda s, d: isinstance(d, bool),
+  'string': lambda s, d: isinstance(d, basestring),
+  'bytes': lambda s, d: ((isinstance(d, str)) or
+                         (isinstance(d, Decimal) and
+                          getattr(s, 'logical_type', None) == constants.DECIMAL)),
+  'int': lambda s, d: ((isinstance(d, (int, long))) and (INT_MIN_VALUE <= d <= INT_MAX_VALUE) or
+                       (isinstance(d, datetime.date) and
+                        getattr(s, 'logical_type', None) == constants.DATE) or
+                       (isinstance(d, datetime.time) and
+                        getattr(s, 'logical_type', None) == constants.TIME_MILLIS)),
+  'long': lambda s, d: ((isinstance(d, (int, long))) and (LONG_MIN_VALUE <= d <= LONG_MAX_VALUE) or
+                        (isinstance(d, datetime.time) and
+                         getattr(s, 'logical_type', None) == constants.TIME_MICROS) or
+                        (isinstance(d, datetime.date) and
+                         _is_timezone_aware_datetime(d) and
+                        getattr(s, 'logical_type', None) in (constants.TIMESTAMP_MILLIS,
+                                                             constants.TIMESTAMP_MICROS))),
+  'float': lambda s, d: isinstance(d, (int, long, float)),
+  'fixed': lambda s, d: ((isinstance(d, str) and len(d) == s.size) or
+                         (isinstance(d, Decimal) and
+                          getattr(s, 'logical_type', None) == constants.DECIMAL)),
+  'enum': lambda s, d: d in s.symbols,
+  'array': lambda s, d: isinstance(d, list) and all(validate(s.items, item) for item in d),
+  'map': lambda s, d: (isinstance(d, dict) and all(isinstance(key, basestring) for key in d)
+                       and all(validate(s.values, value) for value in d.values())),
+  'union': lambda s, d: any(validate(branch, d) for branch in s.schemas),
+  'record': lambda s, d: (isinstance(d, dict)
+                          and all(validate(f.type, d.get(f.name)) for f in s.fields)
+                          and {f.name for f in s.fields}.issuperset(d.keys())),
+}
+_valid['double'] = _valid['float']
+_valid['error_union'] = _valid['union']
+_valid['error'] = _valid['request'] = _valid['record']
+
+
 def validate(expected_schema, datum):
-  """Determine if a python datum is an instance of a schema."""
-  schema_type = expected_schema.type
-  if schema_type == 'null':
-    return datum is None
-  elif schema_type == 'boolean':
-    return isinstance(datum, bool)
-  elif schema_type == 'string':
-    return isinstance(datum, basestring)
-  elif schema_type == 'bytes':
-    if (hasattr(expected_schema, 'logical_type') and
-            expected_schema.logical_type == 'decimal'):
-      return isinstance(datum, Decimal)
-    return isinstance(datum, str)
-  elif schema_type == 'int':
-    if hasattr(expected_schema, 'logical_type'):
-      if expected_schema.logical_type == constants.DATE:
-        return isinstance(datum, datetime.date)
-      elif expected_schema.logical_type == constants.TIME_MILLIS:
-        return isinstance(datum, datetime.time)
-    return (isinstance(datum, (int, long))
-            and INT_MIN_VALUE <= datum <= INT_MAX_VALUE)
-  elif schema_type == 'long':
-    if hasattr(expected_schema, 'logical_type'):
-      if expected_schema.logical_type == constants.TIME_MICROS:
-        return isinstance(datum, datetime.time)
-      elif expected_schema.logical_type in [constants.TIMESTAMP_MILLIS, constants.TIMESTAMP_MICROS]:
-        return isinstance(datum, datetime.datetime) and _is_timezone_aware_datetime(datum)
-    return (isinstance(datum, (int, long))
-            and LONG_MIN_VALUE <= datum <= LONG_MAX_VALUE)
-  elif schema_type in ['float', 'double']:
-    return (isinstance(datum, int) or isinstance(datum, long)
-            or isinstance(datum, float))
-  # Check for int, float, long and decimal
-  elif schema_type == 'fixed':
-    if (hasattr(expected_schema, 'logical_type') and
-                    expected_schema.logical_type == 'decimal'):
-      return isinstance(datum, Decimal)
-    return isinstance(datum, str) and len(datum) == expected_schema.size
-  elif schema_type == 'enum':
-    return datum in expected_schema.symbols
-  elif schema_type == 'array':
-    return (isinstance(datum, list) and
-      False not in [validate(expected_schema.items, d) for d in datum])
-  elif schema_type == 'map':
-    return (isinstance(datum, dict) and
-      False not in [isinstance(k, basestring) for k in datum.keys()] and
-      False not in
-        [validate(expected_schema.values, v) for v in datum.values()])
-  elif schema_type in ['union', 'error_union']:
-    return True in [validate(s, datum) for s in expected_schema.schemas]
-  elif schema_type in ['record', 'error', 'request']:
-    return (isinstance(datum, dict) and
-      False not in
-        [validate(f.type, datum.get(f.name)) for f in expected_schema.fields])
+  """Determines if a python datum is an instance of a schema.
+
+  Args:
+    expected_schema: Schema to validate against.
+    datum: Datum to validate.
+  Returns:
+    True if the datum is an instance of the schema.
+  """
+  try:
+    return _valid[expected_schema.type](expected_schema, datum)
+  except KeyError:
+    raise AvroTypeException('Unknown Avro schema type: %r' % schema_type)
 
 #
 # Decoder/Encoder
 #
 
 class BinaryDecoder(object):
   """Read leaf values."""
@@ -191,15 +184,15 @@
     """
     null is written as zero bytes
     """
     return None
 
   def read_boolean(self):
     """
-    a boolean is written as a single byte 
+    a boolean is written as a single byte
     whose value is either 0 (false) or 1 (true).
     """
     return ord(self.read(1)) == 1
 
   def read_int(self):
     """
     int and long values are written using variable-length, zig-zag coding.
@@ -222,35 +215,23 @@
 
   def read_float(self):
     """
     A float is written as 4 bytes.
     The float is converted into a 32-bit integer using a method equivalent to
     Java's floatToIntBits and then encoded in little-endian format.
     """
-    bits = (((ord(self.read(1)) & 0xffL)) |
-      ((ord(self.read(1)) & 0xffL) <<  8) |
-      ((ord(self.read(1)) & 0xffL) << 16) |
-      ((ord(self.read(1)) & 0xffL) << 24))
-    return STRUCT_FLOAT.unpack(STRUCT_INT.pack(bits))[0]
+    return STRUCT_FLOAT.unpack(self.read(4))[0]
 
   def read_double(self):
     """
     A double is written as 8 bytes.
     The double is converted into a 64-bit integer using a method equivalent to
     Java's doubleToLongBits and then encoded in little-endian format.
     """
-    bits = (((ord(self.read(1)) & 0xffL)) |
-      ((ord(self.read(1)) & 0xffL) <<  8) |
-      ((ord(self.read(1)) & 0xffL) << 16) |
-      ((ord(self.read(1)) & 0xffL) << 24) |
-      ((ord(self.read(1)) & 0xffL) << 32) |
-      ((ord(self.read(1)) & 0xffL) << 40) |
-      ((ord(self.read(1)) & 0xffL) << 48) |
-      ((ord(self.read(1)) & 0xffL) << 56))
-    return STRUCT_DOUBLE.unpack(STRUCT_LONG.pack(bits))[0]
+    return STRUCT_DOUBLE.unpack(self.read(8))[0]
 
   def read_decimal_from_bytes(self, precision, scale):
     """
     Decimal bytes are decoded as signed short, int or long depending on the
     size of bytes.
     """
     size = self.read_long()
@@ -281,15 +262,15 @@
     getcontext().prec = precision
     scaled_datum = Decimal(unscaled_datum).scaleb(-scale)
     getcontext().prec = original_prec
     return scaled_datum
 
   def read_bytes(self):
     """
-    Bytes are encoded as a long followed by that many bytes of data. 
+    Bytes are encoded as a long followed by that many bytes of data.
     """
     return self.read(self.read_long())
 
   def read_utf8(self):
     """
     A string is encoded as a long followed by
     that many bytes of UTF-8 encoded character data.
@@ -317,41 +298,41 @@
       minute=minutes,
       second=seconds,
       microsecond=microseconds
     )
 
   def read_time_millis_from_int(self):
     """
-    int is decoded as python time object which represents 
+    int is decoded as python time object which represents
     the number of milliseconds after midnight, 00:00:00.000.
     """
     milliseconds = self.read_int()
     return self._build_time_object(milliseconds, 1000)
 
   def read_time_micros_from_long(self):
     """
-    long is decoded as python time object which represents 
+    long is decoded as python time object which represents
     the number of microseconds after midnight, 00:00:00.000000.
     """
     microseconds = self.read_long()
     return self._build_time_object(microseconds, 1)
 
   def read_timestamp_millis_from_long(self):
     """
-    long is decoded as python datetime object which represents 
+    long is decoded as python datetime object which represents
     the number of milliseconds from the unix epoch, 1 January 1970.
     """
     timestamp_millis = self.read_long()
     timedelta = datetime.timedelta(microseconds=timestamp_millis * 1000)
-    unix_epoch_datetime = datetime.datetime(1970, 1, 1, 0, 0, 0, 0, tzinfo=timezones.utc) 
+    unix_epoch_datetime = datetime.datetime(1970, 1, 1, 0, 0, 0, 0, tzinfo=timezones.utc)
     return unix_epoch_datetime + timedelta
 
   def read_timestamp_micros_from_long(self):
     """
-    long is decoded as python datetime object which represents 
+    long is decoded as python datetime object which represents
     the number of microseconds from the unix epoch, 1 January 1970.
     """
     timestamp_micros = self.read_long()
     timedelta = datetime.timedelta(microseconds=timestamp_micros)
     unix_epoch_datetime = datetime.datetime(1970, 1, 1, 0, 0, 0, 0, tzinfo=timezones.utc)
     return unix_epoch_datetime + timedelta
 
@@ -406,28 +387,28 @@
     self.writer.write(datum)
 
   def write_null(self, datum):
     """
     null is written as zero bytes
     """
     pass
-  
+
   def write_boolean(self, datum):
     """
-    a boolean is written as a single byte 
+    a boolean is written as a single byte
     whose value is either 0 (false) or 1 (true).
     """
     if datum:
       self.write(chr(1))
     else:
       self.write(chr(0))
 
   def write_int(self, datum):
     """
-    int and long values are written using variable-length, zig-zag coding.    
+    int and long values are written using variable-length, zig-zag coding.
     """
     self.write_long(datum);
 
   def write_long(self, datum):
     """
     int and long values are written using variable-length, zig-zag coding.
     """
@@ -439,35 +420,23 @@
 
   def write_float(self, datum):
     """
     A float is written as 4 bytes.
     The float is converted into a 32-bit integer using a method equivalent to
     Java's floatToIntBits and then encoded in little-endian format.
     """
-    bits = STRUCT_INT.unpack(STRUCT_FLOAT.pack(datum))[0]
-    self.write(chr((bits) & 0xFF))
-    self.write(chr((bits >> 8) & 0xFF))
-    self.write(chr((bits >> 16) & 0xFF))
-    self.write(chr((bits >> 24) & 0xFF))
+    self.write(STRUCT_FLOAT.pack(datum))
 
   def write_double(self, datum):
     """
     A double is written as 8 bytes.
     The double is converted into a 64-bit integer using a method equivalent to
     Java's doubleToLongBits and then encoded in little-endian format.
     """
-    bits = STRUCT_LONG.unpack(STRUCT_DOUBLE.pack(datum))[0]
-    self.write(chr((bits) & 0xFF))
-    self.write(chr((bits >> 8) & 0xFF))
-    self.write(chr((bits >> 16) & 0xFF))
-    self.write(chr((bits >> 24) & 0xFF))
-    self.write(chr((bits >> 32) & 0xFF))
-    self.write(chr((bits >> 40) & 0xFF))
-    self.write(chr((bits >> 48) & 0xFF))
-    self.write(chr((bits >> 56) & 0xFF))
+    self.write(STRUCT_DOUBLE.pack(datum))
 
   def write_decimal_bytes(self, datum, scale):
     """
     Decimal in bytes are encoded as long. Since size of packed value in bytes for
     signed long is 8, 8 bytes are written.
     """
     sign, digits, exp = datum.as_tuple()
@@ -523,23 +492,23 @@
     if sign:
       unscaled_datum = (1 << bits_req) - unscaled_datum
       unscaled_datum = mask | unscaled_datum
       for index in range(size-1, -1, -1):
         bits_to_write = unscaled_datum >> (8 * index)
         self.write(chr(bits_to_write & 0xff))
     else:
-      for i in range(offset_bits/8):
+      for i in range(offset_bits // 8):
         self.write(chr(0))
       for index in range(bytes_req-1, -1, -1):
         bits_to_write = unscaled_datum >> (8 * index)
         self.write(chr(bits_to_write & 0xff))
 
   def write_bytes(self, datum):
     """
-    Bytes are encoded as a long followed by that many bytes of data. 
+    Bytes are encoded as a long followed by that many bytes of data.
     """
     self.write_long(len(datum))
     self.write(struct.pack('%ds' % len(datum), datum))
 
   def write_utf8(self, datum):
     """
     A string is encoded as a long followed by
@@ -623,40 +592,40 @@
     r_type = readers_schema.type
     if 'union' in [w_type, r_type] or 'error_union' in [w_type, r_type]:
       return True
     elif (w_type in schema.PRIMITIVE_TYPES and r_type in schema.PRIMITIVE_TYPES
           and w_type == r_type):
       return True
     elif (w_type == r_type == 'record' and
-          DatumReader.check_props(writers_schema, readers_schema, 
+          DatumReader.check_props(writers_schema, readers_schema,
                                   ['fullname'])):
       return True
     elif (w_type == r_type == 'error' and
-          DatumReader.check_props(writers_schema, readers_schema, 
+          DatumReader.check_props(writers_schema, readers_schema,
                                   ['fullname'])):
       return True
     elif (w_type == r_type == 'request'):
       return True
-    elif (w_type == r_type == 'fixed' and 
-          DatumReader.check_props(writers_schema, readers_schema, 
+    elif (w_type == r_type == 'fixed' and
+          DatumReader.check_props(writers_schema, readers_schema,
                                   ['fullname', 'size'])):
       return True
-    elif (w_type == r_type == 'enum' and 
-          DatumReader.check_props(writers_schema, readers_schema, 
+    elif (w_type == r_type == 'enum' and
+          DatumReader.check_props(writers_schema, readers_schema,
                                   ['fullname'])):
       return True
-    elif (w_type == r_type == 'map' and 
+    elif (w_type == r_type == 'map' and
           DatumReader.check_props(writers_schema.values,
                                   readers_schema.values, ['type'])):
       return True
-    elif (w_type == r_type == 'array' and 
+    elif (w_type == r_type == 'array' and
           DatumReader.check_props(writers_schema.items,
                                   readers_schema.items, ['type'])):
       return True
-    
+
     # Handle schema promotion
     if w_type == 'int' and r_type in ['long', 'float', 'double']:
       return True
     elif w_type == 'long' and r_type in ['float', 'double']:
       return True
     elif w_type == 'float' and r_type == 'double':
       return True
@@ -665,26 +634,26 @@
   def __init__(self, writers_schema=None, readers_schema=None):
     """
     As defined in the Avro specification, we call the schema encoded
     in the data the "writer's schema", and the schema expected by the
     reader the "reader's schema".
     """
     self._writers_schema = writers_schema
-    self._readers_schema = readers_schema 
+    self._readers_schema = readers_schema
 
   # read/write properties
   def set_writers_schema(self, writers_schema):
     self._writers_schema = writers_schema
   writers_schema = property(lambda self: self._writers_schema,
                             set_writers_schema)
   def set_readers_schema(self, readers_schema):
     self._readers_schema = readers_schema
   readers_schema = property(lambda self: self._readers_schema,
                             set_readers_schema)
-  
+
   def read(self, decoder):
     if self.readers_schema is None:
       self.readers_schema = self.writers_schema
     return self.read_data(self.writers_schema, self.readers_schema, decoder)
 
   def read_data(self, writers_schema, readers_schema, decoder):
     # schema matching
@@ -714,21 +683,21 @@
         return decoder.read_date_from_int()
       elif (hasattr(writers_schema, 'logical_type') and
         writers_schema.logical_type == constants.TIME_MILLIS):
         return decoder.read_time_millis_from_int()
       else:
         return decoder.read_int()
     elif writers_schema.type == 'long':
-      if (hasattr(writers_schema, 'logical_type') and 
+      if (hasattr(writers_schema, 'logical_type') and
           writers_schema.logical_type == constants.TIME_MICROS):
         return decoder.read_time_micros_from_long()
-      elif (hasattr(writers_schema, 'logical_type') and 
+      elif (hasattr(writers_schema, 'logical_type') and
             writers_schema.logical_type == constants.TIMESTAMP_MILLIS):
         return decoder.read_timestamp_millis_from_long()
-      elif (hasattr(writers_schema, 'logical_type') and 
+      elif (hasattr(writers_schema, 'logical_type') and
             writers_schema.logical_type == constants.TIMESTAMP_MICROS):
         return decoder.read_timestamp_micros_from_long()
       else:
         return decoder.read_long()
     elif writers_schema.type == 'float':
       return decoder.read_float()
     elif writers_schema.type == 'double':
@@ -918,15 +887,15 @@
     # schema resolution
     index_of_schema = int(decoder.read_long())
     if index_of_schema >= len(writers_schema.schemas):
       fail_msg = "Can't access branch index %d for union with %d branches"\
                  % (index_of_schema, len(writers_schema.schemas))
       raise SchemaResolutionException(fail_msg, writers_schema, readers_schema)
     selected_writers_schema = writers_schema.schemas[index_of_schema]
-    
+
     # read data
     return self.read_data(selected_writers_schema, readers_schema, decoder)
 
   def skip_union(self, writers_schema, decoder):
     index_of_schema = int(decoder.read_long())
     if index_of_schema >= len(writers_schema.schemas):
       fail_msg = "Can't access branch index %d for union with %d branches"\
@@ -946,15 +915,15 @@
      * schemas for fields with the same name in both records are resolved
        recursively.
      * if the writer's record contains a field with a name not present in the
        reader's record, the writer's value for that field is ignored.
      * if the reader's record schema has a field that contains a default value,
        and writer's schema does not have a field with the same name, then the
        reader should use the default value from its field.
-     * if the reader's record schema has a field with no default value, and 
+     * if the reader's record schema has a field with no default value, and
        writer's schema does not have a field with the same name, then the
        field's value is unset.
     """
     # schema resolution
     readers_fields_dict = readers_schema.fields_dict
     read_record = {}
     for field in writers_schema.fields:
@@ -965,15 +934,15 @@
       else:
         self.skip_data(field.type, decoder)
 
     # fill in default values
     if len(readers_fields_dict) > len(read_record):
       writers_fields_dict = writers_schema.fields_dict
       for field_name, field in readers_fields_dict.items():
-        if not writers_fields_dict.has_key(field_name):
+        if field_name not in writers_fields_dict:
           if field.has_default:
             field_val = self._read_default_value(field.type, field.default)
             read_record[field.name] = field_val
           else:
             fail_msg = 'No default value for field %s' % field_name
             raise SchemaResolutionException(fail_msg, writers_schema,
                                             readers_schema)
@@ -1036,15 +1005,15 @@
   writers_schema = property(lambda self: self._writers_schema,
                             set_writers_schema)
 
   def write(self, datum, encoder):
     # validate datum
     if not validate(self.writers_schema, datum):
       raise AvroTypeException(self.writers_schema, datum)
-    
+
     self.write_data(self.writers_schema, datum, encoder)
 
   def write_data(self, writers_schema, datum, encoder):
     # function dispatch to write datum
     if writers_schema.type == 'null':
       encoder.write_null(datum)
     elif writers_schema.type == 'boolean':
```

### Comparing `avro-1.9.1/src/avro/__init__.py` & `avro-1.9.2/src/avro/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__all__ = ['schema', 'io', 'datafile', 'protocol', 'ipc', 'constants', 'timezones']
+from __future__ import absolute_import, division, print_function
 
+__all__ = ['schema', 'io', 'datafile', 'protocol', 'ipc', 'constants', 'timezones']
```

### Comparing `avro-1.9.1/src/avro/txipc.py` & `avro-1.9.2/src/avro/txipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -11,29 +12,32 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-try:
-  from cStringIO import StringIO
-except ImportError:
-  from StringIO import StringIO
-from avro import ipc
-from avro import io
+
+from __future__ import absolute_import, division, print_function
 
 from zope.interface import implements
 
+from avro import io, ipc
+from twisted.internet.defer import Deferred, maybeDeferred
+from twisted.internet.protocol import Protocol
+from twisted.web import resource, server
 from twisted.web.client import Agent
 from twisted.web.http_headers import Headers
-from twisted.internet.defer import maybeDeferred, Deferred
 from twisted.web.iweb import IBodyProducer
-from twisted.web import resource, server
-from twisted.internet.protocol import Protocol
+
+try:
+  from cStringIO import StringIO
+except ImportError:
+  from StringIO import StringIO
+
 
 class TwistedRequestor(ipc.BaseRequestor):
   """A Twisted-compatible requestor. Returns a Deferred that will fire with the
      returning value, instead of blocking until the request completes."""
   def _process_handshake(self, call_response, message_name, request_datum):
     # process the handshake and call response
     buffer_decoder = io.BinaryDecoder(StringIO(call_response))
```

### Comparing `avro-1.9.1/src/avro/tool.py` & `avro-1.9.2/src/avro/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-#! /usr/bin/env python
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """
 Command-line tool
 
 NOTE: The API for the command-line tool is experimental.
 """
+
+from __future__ import absolute_import, division, print_function
+
 import sys
-from BaseHTTPServer import HTTPServer, BaseHTTPRequestHandler
+import threading
 import urlparse
-from avro import io
-from avro import datafile
-from avro import protocol
-from avro import ipc
+from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer
+
+from avro import datafile, io, ipc, protocol
+
 
 class GenericResponder(ipc.Responder):
   def __init__(self, proto, msg, datum):
     proto_json = file(proto, 'r').read()
     ipc.Responder.__init__(self, protocol.parse(proto_json))
     self.msg = msg
     self.datum = datum
 
   def invoke(self, message, request):
     if message.name == self.msg:
-      print >> sys.stderr, "Message: %s Datum: %s" % (message.name, self.datum)
+      print("Message: %s Datum: %s" % (message.name, self.datum), file=sys.stderr)
       # server will shut down after processing a single Avro request
       global server_should_shutdown
       server_should_shutdown = True
       return self.datum
 
 class GenericHandler(BaseHTTPRequestHandler):
   def do_POST(self):
@@ -50,111 +56,96 @@
     resp_body = self.responder.respond(call_request)
     self.send_response(200)
     self.send_header('Content-Type', 'avro/binary')
     self.end_headers()
     resp_writer = ipc.FramedWriter(self.wfile)
     resp_writer.write_framed_message(resp_body)
     if server_should_shutdown:
-      print >> sys.stderr, "Shutting down server."
-      self.server.force_stop()
-
-class StoppableHTTPServer(HTTPServer):
-  """HTTPServer.shutdown added in Python 2.6. FML."""
-  stopped = False
-  allow_reuse_address = True
-  def __init__(self, *args, **kw):
-    HTTPServer.__init__(self, *args, **kw)
-    self.allow_reuse_address = True
-
-  def serve_forever(self):
-    while not self.stopped:
-      self.handle_request()
-
-  def force_stop(self):
-    self.server_close()
-    self.stopped = True
-    self.serve_forever()
+      print("Shutting down server.", file=sys.stderr)
+      quitter = threading.Thread(target=self.server.shutdown)
+      quitter.daemon = True
+      quitter.start()
 
 def run_server(uri, proto, msg, datum):
   url_obj = urlparse.urlparse(uri)
   server_addr = (url_obj.hostname, url_obj.port)
   global responder
   global server_should_shutdown
   server_should_shutdown = False
   responder = GenericResponder(proto, msg, datum)
-  server = StoppableHTTPServer(server_addr, GenericHandler)
-  print "Port: %s" % server.server_port
+  server = HTTPServer(server_addr, GenericHandler)
+  print("Port: %s" % server.server_port)
   sys.stdout.flush()
   server.allow_reuse_address = True
-  print >> sys.stderr, "Starting server."
+  print("Starting server.", file=sys.stderr)
   server.serve_forever()
 
 def send_message(uri, proto, msg, datum):
   url_obj = urlparse.urlparse(uri)
   client = ipc.HTTPTransceiver(url_obj.hostname, url_obj.port)
   proto_json = file(proto, 'r').read()
   requestor = ipc.Requestor(protocol.parse(proto_json), client)
-  print requestor.request(msg, datum)
+  print(requestor.request(msg, datum))
 
 def file_or_stdin(f):
   if f == "-":
     return sys.stdin
   else:
     return file(f)
 
 def main(args=sys.argv):
   if len(args) == 1:
-    print "Usage: %s [dump|rpcreceive|rpcsend]" % args[0]
+    print("Usage: %s [dump|rpcreceive|rpcsend]" % args[0])
     return 1
 
   if args[1] == "dump":
     if len(args) != 3:
-      print "Usage: %s dump input_file" % args[0]
+      print("Usage: %s dump input_file" % args[0])
       return 1
     for d in datafile.DataFileReader(file_or_stdin(args[2]), io.DatumReader()):
-      print repr(d)
+      print(repr(d))
   elif args[1] == "rpcreceive":
     usage_str = "Usage: %s rpcreceive uri protocol_file " % args[0]
     usage_str += "message_name (-data d | -file f)"
     if len(args) not in [5, 7]:
-      print usage_str
+      print(usage_str)
       return 1
     uri, proto, msg = args[2:5]
     datum = None
     if len(args) > 5:
       if args[5] == "-file":
         reader = open(args[6], 'rb')
         datum_reader = io.DatumReader()
         dfr = datafile.DataFileReader(reader, datum_reader)
-        datum = dfr.next()
+        datum = next(dfr)
       elif args[5] == "-data":
-        print "JSON Decoder not yet implemented."
+        print("JSON Decoder not yet implemented.")
         return 1
       else:
-        print usage_str
+        print(usage_str)
         return 1
     run_server(uri, proto, msg, datum)
   elif args[1] == "rpcsend":
     usage_str = "Usage: %s rpcsend uri protocol_file " % args[0]
     usage_str += "message_name (-data d | -file f)"
     if len(args) not in [5, 7]:
-      print usage_str
+      print(usage_str)
       return 1
     uri, proto, msg = args[2:5]
     datum = None
     if len(args) > 5:
       if args[5] == "-file":
         reader = open(args[6], 'rb')
         datum_reader = io.DatumReader()
         dfr = datafile.DataFileReader(reader, datum_reader)
-        datum = dfr.next()
+        datum = next(dfr)
       elif args[5] == "-data":
-        print "JSON Decoder not yet implemented."
+        print("JSON Decoder not yet implemented.")
         return 1
       else:
-        print usage_str
+        print(usage_str)
         return 1
     send_message(uri, proto, msg, datum)
   return 0
-  
+
 if __name__ == "__main__":
   sys.exit(main(sys.argv))
```

### Comparing `avro-1.9.1/src/avro/timezones.py` & `avro-1.9.2/src/avro/timezones.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-# 
+#
 # https://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from datetime import datetime
-from datetime import timedelta
-from datetime import tzinfo
+from __future__ import absolute_import, division, print_function
+
+from datetime import datetime, timedelta, tzinfo
 
 
 class UTCTzinfo(tzinfo):
   def utcoffset(self, dt):
     return timedelta(0)
 
   def tzname(self, dt):
```

### Comparing `avro-1.9.1/src/avro/schema.py` & `avro-1.9.2/src/avro/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+
+##
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -9,14 +12,15 @@
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """
 Contains the Schema classes.
 
 A schema may be one of:
   A record, mapping field names to field value data;
   An error, equivalent to a record;
   An enum, containing one of a small set of symbols;
@@ -29,21 +33,20 @@
   A 32-bit signed int;
   A 64-bit signed long;
   A 32-bit floating-point float;
   A 64-bit floating-point double;
   A boolean; or
   Null.
 """
-from math import floor
-from math import log10
 
-try:
-  import json
-except ImportError:
-  import simplejson as json
+from __future__ import absolute_import, division, print_function
+
+import json
+import math
+import sys
 
 from avro import constants
 
 #
 # Constants
 #
 
@@ -230,19 +233,19 @@
   """Track name set and default namespace during parsing."""
   def __init__(self, default_namespace=None):
       self.names = {}
       self.default_namespace = default_namespace
 
   def has_name(self, name_attr, space_attr):
       test = Name(name_attr, space_attr, self.default_namespace).fullname
-      return self.names.has_key(test)
+      return test in self.names
 
   def get_name(self, name_attr, space_attr):
       test = Name(name_attr, space_attr, self.default_namespace).fullname
-      if not self.names.has_key(test):
+      if test not in self.names:
           return None
       return self.names[test]
 
   def prune_namespace(self, properties):
     """given a properties, return properties with namespace removed if
     it matches the own default namespace"""
     if self.default_namespace is None:
@@ -269,15 +272,15 @@
       @return: the Name that was just added.
     """
     to_add = Name(name_attr, space_attr, self.default_namespace)
 
     if to_add.fullname in VALID_TYPES:
       fail_msg = '%s is a reserved type name.' % to_add.fullname
       raise SchemaParseException(fail_msg)
-    elif self.names.has_key(to_add.fullname):
+    elif to_add.fullname in self.names:
       fail_msg = 'The name "%s" is already in use.' % to_add.fullname
       raise SchemaParseException(fail_msg)
 
     self.names[to_add.fullname] = new_schema
     return to_add
 
 class NamedSchema(Schema):
@@ -328,16 +331,15 @@
     self.logical_type = logical_type
 
 #
 # Decimal logical schema
 #
 
 class DecimalLogicalSchema(LogicalSchema):
-  def __init__(self, precision, scale=0):
-    max_precision = self._max_precision()
+  def __init__(self, precision, scale=0, max_precision=0):
     if not isinstance(precision, int) or precision <= 0:
       raise SchemaParseException("""Precision is required for logical type
                                 DECIMAL and must be a positive integer but
                                 is %s.""" % precision)
     elif precision > max_precision:
       raise SchemaParseException("Cannot store precision digits. Max is %s"
                                  %(max_precision))
@@ -347,17 +349,14 @@
 
     elif scale > precision:
       raise SchemaParseException("Invalid DECIMAL scale %s. Cannot be greater than precision %s"
                                  %(scale, precision))
 
     super(DecimalLogicalSchema, self).__init__('decimal')
 
-  def _max_precision(self):
-    raise NotImplementedError()
-
 
 class Field(object):
   def __init__(self, type, name, has_default, default=None,
                order=None,names=None, doc=None, other_props=None):
     # Ensure valid ctor args
     if not name:
       fail_msg = 'Fields must have a non-empty name.'
@@ -376,15 +375,15 @@
 
     if (isinstance(type, basestring) and names is not None
         and names.has_name(type, None)):
       type_schema = names.get_name(type, None)
     else:
       try:
         type_schema = make_avsc_object(type, names)
-      except Exception, e:
+      except Exception as e:
         fail_msg = 'Type property "%s" not a valid Avro schema: %s' % (type, e)
         raise SchemaParseException(fail_msg)
     self.set_prop('type', type_schema)
     self.set_prop('name', name)
     self.type = type_schema
     self.name = name
     # TODO(hammer): check to ensure default is valid
@@ -449,27 +448,23 @@
 
 #
 # Decimal Bytes Type
 #
 
 class BytesDecimalSchema(PrimitiveSchema, DecimalLogicalSchema):
   def __init__(self, precision, scale=0, other_props=None):
-    DecimalLogicalSchema.__init__(self, precision, scale)
+    DecimalLogicalSchema.__init__(self, precision, scale, max_precision=((1 << 31) - 1))
     PrimitiveSchema.__init__(self, 'bytes', other_props)
     self.set_prop('precision', precision)
     self.set_prop('scale', scale)
 
   # read-only properties
   precision = property(lambda self: self.get_prop('precision'))
   scale = property(lambda self: self.get_prop('scale'))
 
-  def _max_precision(self):
-    # Considering the max 32 bit integer value
-    return (1 << 31) - 1
-
   def to_json(self, names=None):
     return self.props
 
   def __eq__(self, that):
     return self.props == that.props
 
 
@@ -507,26 +502,24 @@
 
 #
 # Decimal Fixed Type
 #
 
 class FixedDecimalSchema(FixedSchema, DecimalLogicalSchema):
   def __init__(self, size, name, precision, scale=0, namespace=None, names=None, other_props=None):
+    max_precision = math.floor(math.log10(2) * (8 * size - 1))
+    DecimalLogicalSchema.__init__(self, precision, scale, max_precision)
     FixedSchema.__init__(self, name, namespace, size, names, other_props)
-    DecimalLogicalSchema.__init__(self, precision, scale)
     self.set_prop('precision', precision)
     self.set_prop('scale', scale)
 
   # read-only properties
   precision = property(lambda self: self.get_prop('precision'))
   scale = property(lambda self: self.get_prop('scale'))
 
-  def _max_precision(self):
-    return round(floor(log10(pow(2, (8 * self.size - 1)) - 1)))
-
   def to_json(self, names=None):
     return self.props
 
   def __eq__(self, that):
     return self.props == that.props
 
 
@@ -577,15 +570,15 @@
     # Add class members
 
     if isinstance(items, basestring) and names.has_name(items, None):
       items_schema = names.get_name(items, None)
     else:
       try:
         items_schema = make_avsc_object(items, names)
-      except SchemaParseException, e:
+      except SchemaParseException as e:
         fail_msg = 'Items schema (%s) not a valid Avro schema: %s (known names: %s)' % (items, e, names.names.keys())
         raise SchemaParseException(fail_msg)
 
     self.set_prop('items', items_schema)
 
   # read-only properties
   items = property(lambda self: self.get_prop('items'))
@@ -609,17 +602,18 @@
 
     # Add class members
     if isinstance(values, basestring) and names.has_name(values, None):
       values_schema = names.get_name(values, None)
     else:
       try:
         values_schema = make_avsc_object(values, names)
-      except:
-        fail_msg = 'Values schema not a valid Avro schema.'
-        raise SchemaParseException(fail_msg)
+      except SchemaParseException:
+        raise
+      except Exception:
+        raise SchemaParseException('Values schema is not a valid Avro schema.')
 
     self.set_prop('values', values_schema)
 
   # read-only properties
   values = property(lambda self: self.get_prop('values'))
 
   def to_json(self, names=None):
@@ -650,15 +644,15 @@
     schema_objects = []
     for schema in schemas:
       if isinstance(schema, basestring) and names.has_name(schema, None):
         new_schema = names.get_name(schema, None)
       else:
         try:
           new_schema = make_avsc_object(schema, names)
-        except Exception, e:
+        except Exception as e:
           raise SchemaParseException('Union item must be a valid Avro schema: %s' % str(e))
       # check the new schema
       if (new_schema.type in VALID_TYPES and new_schema.type not in NAMED_TYPES
           and new_schema.type in [schema.type for schema in schema_objects]):
         raise SchemaParseException('%s type already in Union' % new_schema.type)
       elif new_schema.type == 'union':
         raise SchemaParseException('Unions cannot contain other unions.')
@@ -706,15 +700,15 @@
       if callable(getattr(field, 'get', None)):
         type = field.get('type')
         name = field.get('name')
 
         # null values can have a default value of None
         has_default = False
         default = None
-        if field.has_key('default'):
+        if 'default' in field:
           has_default = True
           default = field.get('default')
 
         order = field.get('order')
         doc = field.get('doc')
         other_props = get_other_props(field, FIELD_RESERVED_PROPS)
         new_field = Field(type, name, has_default, default, order, names, doc,
@@ -874,79 +868,89 @@
 
   def __eq__(self, that):
     return self.props == that.props
 
 #
 # Module Methods
 #
-def get_other_props(all_props,reserved_props):
+def get_other_props(all_props, reserved_props):
   """
   Retrieve the non-reserved properties from a dictionary of properties
   @args reserved_props: The set of reserved properties to exclude
   """
   if callable(getattr(all_props, 'items', None)):
-    return dict([(k,v) for (k,v) in all_props.items() if k not in
-                 reserved_props ])
+    return {k: v for k, v in all_props.items() if k not in reserved_props}
 
+def make_bytes_decimal_schema(other_props):
+  """Make a BytesDecimalSchema from just other_props."""
+  return BytesDecimalSchema(other_props.get('precision'), other_props.get('scale', 0))
+
+def make_logical_schema(logical_type, type_, other_props):
+  """Map the logical types to the appropriate literal type and schema class."""
+  logical_types = {
+    constants.DATE: ('int', DateSchema),
+    # Fixed decimal schema is handled before we get here.
+    constants.DECIMAL: ('bytes', make_bytes_decimal_schema),
+    constants.TIMESTAMP_MICROS: ('long', TimestampMicrosSchema),
+    constants.TIMESTAMP_MILLIS: ('long', TimestampMillisSchema),
+    constants.TIME_MICROS: ('long', TimeMicrosSchema),
+    constants.TIME_MILLIS: ('int', TimeMillisSchema),
+  }
+  literal_type, schema_type = logical_types.get(logical_type, (None, None))
+  try:
+    if literal_type == type_:
+      return schema_type(other_props)
+  except SchemaParseException:
+    pass
+  return None
 
 def make_avsc_object(json_data, names=None):
   """
   Build Avro Schema from data parsed out of JSON string.
 
-  @arg names: A Name object (tracks seen names and default space)
+  @arg names: A Names object (tracks seen names and default space)
   """
-  if names == None:
+  if names is None:
     names = Names()
 
   # JSON object (non-union)
   if callable(getattr(json_data, 'get', None)):
     type = json_data.get('type')
     other_props = get_other_props(json_data, SCHEMA_RESERVED_PROPS)
-    logical_type = None
-    if 'logicalType' in json_data:
-      logical_type = json_data.get('logicalType')
-      if logical_type not in constants.SUPPORTED_LOGICAL_TYPE:
-        raise SchemaParseException("Currently does not support %s logical type" % logical_type)
-    if type in PRIMITIVE_TYPES:
-      if type == 'int' and logical_type == constants.DATE:
-        return DateSchema(other_props)
-      if type == 'int' and logical_type == constants.TIME_MILLIS:
-        return TimeMillisSchema(other_props=other_props)
-      if type == 'long' and logical_type == constants.TIME_MICROS:
-        return TimeMicrosSchema(other_props=other_props)
-      if type == 'long' and logical_type == constants.TIMESTAMP_MILLIS:
-        return TimestampMillisSchema(other_props=other_props)
-      if type == 'long' and logical_type == constants.TIMESTAMP_MICROS:
-        return TimestampMicrosSchema(other_props=other_props)
-      if type == 'bytes' and logical_type == constants.DECIMAL:
-          precision = json_data.get('precision')
-          scale = 0 if json_data.get('scale') is None else json_data.get('scale')
-          return BytesDecimalSchema(precision, scale, other_props)
-      return PrimitiveSchema(type, other_props)
-    elif type in NAMED_TYPES:
+    logical_type = json_data.get('logicalType')
+    if logical_type:
+      logical_schema = make_logical_schema(logical_type, type, other_props or {})
+      if logical_schema is not None:
+        return logical_schema
+    if type in NAMED_TYPES:
       name = json_data.get('name')
       namespace = json_data.get('namespace', names.default_namespace)
       if type == 'fixed':
         size = json_data.get('size')
         if logical_type == 'decimal':
           precision = json_data.get('precision')
           scale = 0 if json_data.get('scale') is None else json_data.get('scale')
-          return FixedDecimalSchema(size, name, precision, scale, namespace, names, other_props)
+          try:
+            return FixedDecimalSchema(size, name, precision, scale, namespace, names, other_props)
+          except (AvroException, SchemaParseException):
+            pass
         return FixedSchema(name, namespace, size, names, other_props)
       elif type == 'enum':
         symbols = json_data.get('symbols')
         doc = json_data.get('doc')
         return EnumSchema(name, namespace, symbols, names, doc, other_props)
       elif type in ['record', 'error']:
         fields = json_data.get('fields')
         doc = json_data.get('doc')
         return RecordSchema(name, namespace, fields, names, type, doc, other_props)
       else:
         raise SchemaParseException('Unknown Named Type: %s' % type)
-    elif type in VALID_TYPES:
+    if type in PRIMITIVE_TYPES:
+      return PrimitiveSchema(type, other_props)
+    if type in VALID_TYPES:
       if type == 'array':
         items = json_data.get('items')
         return ArraySchema(items, names, other_props)
       elif type == 'map':
         values = json_data.get('values')
         return MapSchema(values, names, other_props)
       elif type == 'error_union':
@@ -971,17 +975,20 @@
 
 # TODO(hammer): make method for reading from a file?
 def parse(json_string):
   """Constructs the Schema from the JSON text."""
   # parse the JSON
   try:
     json_data = json.loads(json_string)
-  except Exception, e:
-    import sys
-    raise SchemaParseException('Error parsing JSON: %s, error = %s'
-                               % (json_string, e)), None, sys.exc_info()[2]
+  except Exception as e:
+    msg = 'Error parsing JSON: {}, error = {}'.format(json_string, e)
+    new_exception = SchemaParseException(msg)
+    traceback = sys.exc_info()[2]
+    if not hasattr(new_exception, 'with_traceback'):
+      raise (new_exception, None, traceback)  # Python 2 syntax
+    raise new_exception.with_traceback(traceback)
 
   # Initialize the names object
   names = Names()
 
   # construct the Avro Schema object
   return make_avsc_object(json_data, names)
```


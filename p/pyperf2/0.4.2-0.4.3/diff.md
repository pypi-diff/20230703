# Comparing `tmp/pyperf2-0.4.2-py3-none-any.whl.zip` & `tmp/pyperf2-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11511 bytes, number of entries: 6
--rw-r--r--  2.0 unx    26586 b- defN 23-Jul-03 08:44 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-03 08:46 pyperf2-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3340 b- defN 23-Jul-03 08:46 pyperf2-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 08:46 pyperf2-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-03 08:46 pyperf2-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-03 08:46 pyperf2-0.4.2.dist-info/RECORD
-6 files, 41846 bytes uncompressed, 10677 bytes compressed:  74.5%
+Zip file size: 11525 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26635 b- defN 23-Jul-03 08:59 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-03 09:00 pyperf2-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3340 b- defN 23-Jul-03 09:00 pyperf2-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 09:00 pyperf2-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-03 09:00 pyperf2-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-03 09:00 pyperf2-0.4.3.dist-info/RECORD
+6 files, 41895 bytes uncompressed, 10691 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.4.2.dist-info/LICENSE
+Filename: pyperf2-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.4.2.dist-info/METADATA
+Filename: pyperf2-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.4.2.dist-info/WHEEL
+Filename: pyperf2-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.4.2.dist-info/top_level.txt
+Filename: pyperf2-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.4.2.dist-info/RECORD
+Filename: pyperf2-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -9,15 +9,15 @@
 import pyjq
 import copy
 from decimal import Decimal
 from pprint import pprint, pformat
 import logging
 import datetime
 from pyroute2 import netns
-
+import atexit
 
 def output_reader(proc, outq, parent):
     for line in iter(proc.stdout.readline, b""):
         outq.put(line.decode("utf-8"))
 
         # print("{0} {1}".format(parent.name,line.decode('utf-8')))
 
@@ -66,14 +66,16 @@
             self.expected_interval_packets = int(
                 Decimal(self.report_interval) * Decimal(self.bandwidth[:-3])
             )
         else:
             self.expected_interval_packets = None
         self._log = logging.getLogger("")
         self._current_event_number = 0
+        atexit.register(self.stop)
+
 
     def __del__(self):
         try:
             self._raw_log_filehandler.close()
         except:
             pass
```

## Comparing `pyperf2-0.4.2.dist-info/LICENSE` & `pyperf2-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.4.2.dist-info/METADATA` & `pyperf2-0.4.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```


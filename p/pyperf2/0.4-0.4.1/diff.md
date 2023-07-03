# Comparing `tmp/pyperf2-0.4-py3-none-any.whl.zip` & `tmp/pyperf2-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11468 bytes, number of entries: 6
--rw-r--r--  2.0 unx    26391 b- defN 23-Jun-26 06:20 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3338 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      453 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/RECORD
-6 files, 41639 bytes uncompressed, 10654 bytes compressed:  74.4%
+Zip file size: 11494 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26438 b- defN 23-Jul-03 08:11 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-03 08:13 pyperf2-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3340 b- defN 23-Jul-03 08:13 pyperf2-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 08:13 pyperf2-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-03 08:13 pyperf2-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-03 08:13 pyperf2-0.4.1.dist-info/RECORD
+6 files, 41698 bytes uncompressed, 10660 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.4.dist-info/LICENSE
+Filename: pyperf2-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.4.dist-info/METADATA
+Filename: pyperf2-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.4.dist-info/WHEEL
+Filename: pyperf2-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.4.dist-info/top_level.txt
+Filename: pyperf2-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.4.dist-info/RECORD
+Filename: pyperf2-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -599,18 +599,19 @@
             )
 
         self._output_reader_thread.start()
         self._running = True
         self.status = "running"
         time.sleep(0.2)
 
-        self._cleanup_timer_thread = threading.Timer(
-            int(self.test_duration) + 10, self.stop
-        )
-        self._cleanup_timer_thread.start()
+        if self.test_duration:
+            self._cleanup_timer_thread = threading.Timer(
+                int(self.test_duration) + 10, self.stop
+            )
+            self._cleanup_timer_thread.start()
 
         if self._proc.poll() is not None:
             self.stop()
             return False
 
         return True
```

## Comparing `pyperf2-0.4.dist-info/LICENSE` & `pyperf2-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.4.dist-info/METADATA` & `pyperf2-0.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.4
+Version: 0.4.1
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```


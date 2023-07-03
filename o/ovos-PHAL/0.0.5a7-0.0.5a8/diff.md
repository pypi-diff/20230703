# Comparing `tmp/ovos_PHAL-0.0.5a7-py3-none-any.whl.zip` & `tmp/ovos_PHAL-0.0.5a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9582 bytes, number of entries: 12
--rw-r--r--  2.0 unx      148 b- defN 23-Jul-03 21:22 ovos_PHAL/__init__.py
--rw-r--r--  2.0 unx      651 b- defN 23-Jul-03 21:22 ovos_PHAL/__main__.py
--rw-r--r--  2.0 unx     2628 b- defN 23-Jul-03 21:22 ovos_PHAL/admin.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Jul-03 21:22 ovos_PHAL/detection.py
--rw-r--r--  2.0 unx     3047 b- defN 23-Jul-03 21:22 ovos_PHAL/service.py
--rw-r--r--  2.0 unx      177 b- defN 23-Jul-03 21:22 ovos_PHAL/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Jul-03 21:22 ovos_PHAL-0.0.5a7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1249 b- defN 23-Jul-03 21:22 ovos_PHAL-0.0.5a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 21:22 ovos_PHAL-0.0.5a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       94 b- defN 23-Jul-03 21:22 ovos_PHAL-0.0.5a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-03 21:22 ovos_PHAL-0.0.5a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-03 21:22 ovos_PHAL-0.0.5a7.dist-info/RECORD
-12 files, 21848 bytes uncompressed, 7958 bytes compressed:  63.6%
+Zip file size: 9581 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      148 b- defN 23-Jul-03 21:23 ovos_PHAL/__init__.py
+-rw-r--r--  2.0 unx      651 b- defN 23-Jul-03 21:23 ovos_PHAL/__main__.py
+-rw-r--r--  2.0 unx     2628 b- defN 23-Jul-03 21:23 ovos_PHAL/admin.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-Jul-03 21:23 ovos_PHAL/detection.py
+-rw-r--r--  2.0 unx     3047 b- defN 23-Jul-03 21:23 ovos_PHAL/service.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jul-03 21:23 ovos_PHAL/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jul-03 21:23 ovos_PHAL-0.0.5a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1249 b- defN 23-Jul-03 21:23 ovos_PHAL-0.0.5a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 21:23 ovos_PHAL-0.0.5a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       94 b- defN 23-Jul-03 21:23 ovos_PHAL-0.0.5a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-03 21:23 ovos_PHAL-0.0.5a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-03 21:23 ovos_PHAL-0.0.5a8.dist-info/RECORD
+12 files, 21848 bytes uncompressed, 7957 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: ovos_PHAL/service.py
 Comment: 
 
 Filename: ovos_PHAL/version.py
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a7.dist-info/LICENSE
+Filename: ovos_PHAL-0.0.5a8.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a7.dist-info/METADATA
+Filename: ovos_PHAL-0.0.5a8.dist-info/METADATA
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a7.dist-info/WHEEL
+Filename: ovos_PHAL-0.0.5a8.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a7.dist-info/entry_points.txt
+Filename: ovos_PHAL-0.0.5a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a7.dist-info/top_level.txt
+Filename: ovos_PHAL-0.0.5a8.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a7.dist-info/RECORD
+Filename: ovos_PHAL-0.0.5a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_PHAL/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 5
-VERSION_ALPHA = 7
+VERSION_ALPHA = 8
 # END_VERSION_BLOCK
```

## Comparing `ovos_PHAL-0.0.5a7.dist-info/LICENSE` & `ovos_PHAL-0.0.5a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_PHAL-0.0.5a7.dist-info/METADATA` & `ovos_PHAL-0.0.5a8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL
-Version: 0.0.5a7
+Version: 0.0.5a8
 Summary: Plugin based Hardware Abstraction Layer for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL
 Author: jarbasAi
 Author-email: jarbasai@mailfence.com
 License: apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```


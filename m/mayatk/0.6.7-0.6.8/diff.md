# Comparing `tmp/mayatk-0.6.7.tar.gz` & `tmp/mayatk-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayatk-0.6.7.tar", last modified: Wed Jun 28 02:20:01 2023, max compression
+gzip compressed data, was "mayatk-0.6.8.tar", last modified: Mon Jul  3 15:10:24 2023, max compression
```

## Comparing `mayatk-0.6.7.tar` & `mayatk-0.6.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 02:20:01.272482 mayatk-0.6.7/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.7/LICENSE
--rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1246 2023-06-28 02:20:01.272482 mayatk-0.6.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-28 02:20:01.225393 mayatk-0.6.7/mayatk/
--rw-rw-rw-   0        0        0     4335 2023-06-28 02:19:57.000000 mayatk-0.6.7/mayatk/__init__.py
--rw-rw-rw-   0        0        0     8065 2023-06-27 21:45:31.000000 mayatk-0.6.7/mayatk/cam_utils.py
--rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.7/mayatk/cam_utils.py.bak
--rw-rw-rw-   0        0        0    64432 2023-06-28 00:14:46.000000 mayatk-0.6.7/mayatk/cmpt_utils.py
--rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.7/mayatk/cmpt_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-28 02:20:01.259189 mayatk-0.6.7/mayatk/display_utils/
--rw-rw-rw-   0        0        0      397 2023-06-25 00:47:10.000000 mayatk-0.6.7/mayatk/display_utils/__init__.py
--rw-rw-rw-   0        0        0     7746 2023-06-27 21:52:32.000000 mayatk-0.6.7/mayatk/display_utils/exploded_view.py
--rw-rw-rw-   0        0        0    30701 2023-06-28 01:35:20.000000 mayatk-0.6.7/mayatk/edit_utils.py
--rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.7/mayatk/macro_utils.py
--rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.7/mayatk/mash_utils.py
--rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.7/mayatk/mash_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-28 02:20:01.262838 mayatk-0.6.7/mayatk/mat_utils/
--rw-rw-rw-   0        0        0      337 2023-06-25 00:47:26.000000 mayatk-0.6.7/mayatk/mat_utils/__init__.py
--rw-rw-rw-   0        0        0     8911 2023-06-28 02:10:10.000000 mayatk-0.6.7/mayatk/mat_utils/mat_utils.py
--rw-rw-rw-   0        0        0    17681 2023-06-27 21:41:18.000000 mayatk-0.6.7/mayatk/mat_utils/stingray_arnold_shader.py
--rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.7/mayatk/misc_utils.py.bak
--rw-rw-rw-   0        0        0    27018 2023-06-27 22:30:12.000000 mayatk-0.6.7/mayatk/node_utils.py
--rw-rw-rw-   0        0        0    13327 2023-06-28 00:05:16.000000 mayatk-0.6.7/mayatk/project_utils.py
--rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.7/mayatk/project_utils.py.bak
--rw-rw-rw-   0        0        0    18251 2023-06-27 23:39:34.000000 mayatk-0.6.7/mayatk/rig_utils.py
--rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.7/mayatk/rig_utils.py.bak
--rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.7/mayatk/script_utils.py
--rw-rw-rw-   0        0        0    15184 2023-06-27 22:23:17.000000 mayatk-0.6.7/mayatk/utils.py
--rw-rw-rw-   0        0        0    31389 2023-06-27 23:49:44.000000 mayatk-0.6.7/mayatk/xform_utils.py
--rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.7/mayatk/xform_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-28 02:20:01.256183 mayatk-0.6.7/mayatk.egg-info/
--rw-rw-rw-   0        0        0     1246 2023-06-28 02:20:00.000000 mayatk-0.6.7/mayatk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.7/mayatk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1006 2023-06-28 02:20:01.000000 mayatk-0.6.7/mayatk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.7/mayatk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-28 02:20:00.000000 mayatk-0.6.7/mayatk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-28 02:20:00.000000 mayatk-0.6.7/mayatk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 02:20:01.273483 mayatk-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1442 2023-06-28 02:16:01.000000 mayatk-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 02:20:01.271482 mayatk-0.6.7/test/
--rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.7/test/__init__.py
--rw-rw-rw-   0        0        0    26026 2023-06-28 00:01:13.000000 mayatk-0.6.7/test/cmpt_utils_test.py
--rw-rw-rw-   0        0        0     7676 2023-06-28 00:35:52.000000 mayatk-0.6.7/test/edit_utils_test.py
--rw-rw-rw-   0        0        0     4505 2023-06-28 02:10:41.000000 mayatk-0.6.7/test/mat_utils_test.py
--rw-rw-rw-   0        0        0     7396 2023-06-28 00:17:04.000000 mayatk-0.6.7/test/node_utils_test.py
--rw-rw-rw-   0        0        0     5086 2023-06-28 01:40:55.000000 mayatk-0.6.7/test/rig_utils_test.py
--rw-rw-rw-   0        0        0     2068 2023-06-28 01:24:21.000000 mayatk-0.6.7/test/run_tests.py
--rw-rw-rw-   0        0        0     7022 2023-06-28 00:34:32.000000 mayatk-0.6.7/test/utils_test.py
--rw-rw-rw-   0        0        0     7298 2023-06-28 01:39:40.000000 mayatk-0.6.7/test/xform_utils_test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.561608 mayatk-0.6.8/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1246 2023-07-03 15:10:24.560606 mayatk-0.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.520828 mayatk-0.6.8/mayatk/
+-rw-rw-rw-   0        0        0     4335 2023-07-03 15:10:21.000000 mayatk-0.6.8/mayatk/__init__.py
+-rw-rw-rw-   0        0        0     8065 2023-06-27 21:45:31.000000 mayatk-0.6.8/mayatk/cam_utils.py
+-rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.8/mayatk/cam_utils.py.bak
+-rw-rw-rw-   0        0        0    64489 2023-06-29 16:12:36.000000 mayatk-0.6.8/mayatk/cmpt_utils.py
+-rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.8/mayatk/cmpt_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.546613 mayatk-0.6.8/mayatk/display_utils/
+-rw-rw-rw-   0        0        0      397 2023-06-25 00:47:10.000000 mayatk-0.6.8/mayatk/display_utils/__init__.py
+-rw-rw-rw-   0        0        0     7746 2023-06-27 21:52:32.000000 mayatk-0.6.8/mayatk/display_utils/exploded_view.py
+-rw-rw-rw-   0        0        0    30701 2023-06-28 01:35:20.000000 mayatk-0.6.8/mayatk/edit_utils.py
+-rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.8/mayatk/macro_utils.py
+-rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.8/mayatk/mash_utils.py
+-rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.8/mayatk/mash_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.549613 mayatk-0.6.8/mayatk/mat_utils/
+-rw-rw-rw-   0        0        0      337 2023-06-25 00:47:26.000000 mayatk-0.6.8/mayatk/mat_utils/__init__.py
+-rw-rw-rw-   0        0        0     8911 2023-06-28 02:10:10.000000 mayatk-0.6.8/mayatk/mat_utils/mat_utils.py
+-rw-rw-rw-   0        0        0    17681 2023-06-27 21:41:18.000000 mayatk-0.6.8/mayatk/mat_utils/stingray_arnold_shader.py
+-rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.8/mayatk/misc_utils.py.bak
+-rw-rw-rw-   0        0        0    27018 2023-06-27 22:30:12.000000 mayatk-0.6.8/mayatk/node_utils.py
+-rw-rw-rw-   0        0        0    13177 2023-06-28 22:54:55.000000 mayatk-0.6.8/mayatk/project_utils.py
+-rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.8/mayatk/project_utils.py.bak
+-rw-rw-rw-   0        0        0    18251 2023-06-27 23:39:34.000000 mayatk-0.6.8/mayatk/rig_utils.py
+-rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.8/mayatk/rig_utils.py.bak
+-rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.8/mayatk/script_utils.py
+-rw-rw-rw-   0        0        0    15184 2023-06-27 22:23:17.000000 mayatk-0.6.8/mayatk/utils.py
+-rw-rw-rw-   0        0        0    31389 2023-06-27 23:49:44.000000 mayatk-0.6.8/mayatk/xform_utils.py
+-rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.8/mayatk/xform_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.545608 mayatk-0.6.8/mayatk.egg-info/
+-rw-rw-rw-   0        0        0     1246 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.8/mayatk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1006 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.8/mayatk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:10:24.561608 mayatk-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-06-28 02:16:01.000000 mayatk-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.560606 mayatk-0.6.8/test/
+-rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.8/test/__init__.py
+-rw-rw-rw-   0        0        0    26026 2023-06-28 00:01:13.000000 mayatk-0.6.8/test/cmpt_utils_test.py
+-rw-rw-rw-   0        0        0     7676 2023-06-28 00:35:52.000000 mayatk-0.6.8/test/edit_utils_test.py
+-rw-rw-rw-   0        0        0     4505 2023-06-28 02:10:41.000000 mayatk-0.6.8/test/mat_utils_test.py
+-rw-rw-rw-   0        0        0     7396 2023-06-28 00:17:04.000000 mayatk-0.6.8/test/node_utils_test.py
+-rw-rw-rw-   0        0        0     5086 2023-06-28 01:40:55.000000 mayatk-0.6.8/test/rig_utils_test.py
+-rw-rw-rw-   0        0        0     2068 2023-06-28 01:24:21.000000 mayatk-0.6.8/test/run_tests.py
+-rw-rw-rw-   0        0        0     7022 2023-06-28 00:34:32.000000 mayatk-0.6.8/test/utils_test.py
+-rw-rw-rw-   0        0        0     7298 2023-06-28 01:39:40.000000 mayatk-0.6.8/test/xform_utils_test.py
```

### Comparing `mayatk-0.6.7/LICENSE` & `mayatk-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/PKG-INFO` & `mayatk-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.6.7
+Version: 0.6.8
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mayatk-0.6.7/mayatk/__init__.py` & `mayatk-0.6.8/mayatk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "mayatk"
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 
 
 # Define dictionaries to map class names, method names, class method names, and sub-modules to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
 SUBMODULE_TO_MODULE = {}
```

### Comparing `mayatk-0.6.7/mayatk/cam_utils.py` & `mayatk-0.6.8/mayatk/cam_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/cam_utils.py.bak` & `mayatk-0.6.8/mayatk/cam_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/cmpt_utils.py` & `mayatk-0.6.8/mayatk/cmpt_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1033,22 +1033,22 @@
         import math
 
         if not isinstance(edge, pm.general.MeshEdge):
             raise TypeError(f"Input must be a MeshEdge, got {type(edge)}.")
 
         # Get the faces connected by the edge
         connected_faces = list(edge.connectedFaces())
+        if len(connected_faces) != 2:
+            return 0
 
         # Get the normals of the faces
         normal1 = cls.get_normal(connected_faces[0])
         normal2 = cls.get_normal(connected_faces[1])
-
         # Calculate the angle between the normals
         angle = normal1.angle(normal2)
-
         # Convert the angle from radians to degrees
         angle = math.degrees(angle)
 
         return angle
 
     @classmethod
     def average_normals(cls, objects, by_uv_shell=False):
```

### Comparing `mayatk-0.6.7/mayatk/cmpt_utils.py.bak` & `mayatk-0.6.8/mayatk/cmpt_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/display_utils/exploded_view.py` & `mayatk-0.6.8/mayatk/display_utils/exploded_view.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/edit_utils.py` & `mayatk-0.6.8/mayatk/edit_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/macro_utils.py` & `mayatk-0.6.8/mayatk/macro_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/mash_utils.py` & `mayatk-0.6.8/mayatk/mash_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/mash_utils.py.bak` & `mayatk-0.6.8/mayatk/mash_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/mat_utils/mat_utils.py` & `mayatk-0.6.8/mayatk/mat_utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/mat_utils/stingray_arnold_shader.py` & `mayatk-0.6.8/mayatk/mat_utils/stingray_arnold_shader.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/misc_utils.py.bak` & `mayatk-0.6.8/mayatk/misc_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/node_utils.py` & `mayatk-0.6.8/mayatk/node_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/project_utils.py` & `mayatk-0.6.8/mayatk/project_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import os
 
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
-from pythontk import FileUtils
+import pythontk as ptk
 
 
 class ProjectUtils:
     """ """
 
     @staticmethod
     def get_recent_files(index=None, format="standard"):
@@ -38,34 +38,34 @@
             get_recent_files(format='standard|timestamp') --> Returns a dictionary with standard paths as keys and timestamped paths as values.
         """
         files = pm.optionVar(query="RecentFilesList")
         if not files:
             return []
 
         result = [
-            FileUtils.format_path(f)
+            ptk.format_path(f)
             for f in reversed(files)
-            if FileUtils.is_valid(f) and "Autosave" not in f
+            if ptk.is_valid(f) and "Autosave" not in f
         ]
 
         if index is not None:
             try:
                 result = result[index]
             except (IndexError, TypeError):
                 print(f"Incorrect index or slice. Returning empty list.")
                 return []
 
         format = format.split("|")
         if len(format) == 2 and "timestamp" in format and "standard" in format:
             if format[0] == "timestamp":
-                result = {FileUtils.time_stamp(res): res for res in result}
+                result = {ptk.time_stamp(res): res for res in result}
             else:
-                result = {res: FileUtils.time_stamp(res) for res in result}
+                result = {res: ptk.time_stamp(res) for res in result}
         elif "timestamp" in format:
-            result = [FileUtils.time_stamp(res) for res in result]
+            result = [ptk.time_stamp(res) for res in result]
         # else return the standard format
 
         return result
 
     @staticmethod
     def get_recent_projects(index=None, format="standard"):
         """
@@ -91,33 +91,31 @@
             get_recent_projects(format='timestamp') --> Returns all recent projects in timestamp format.
             get_recent_projects(format='standard|timestamp') --> Returns a dictionary with standard paths as keys and timestamped paths as values.
         """
         files = pm.optionVar(query="RecentProjectsList")
         if not files:
             return []
 
-        result = [
-            FileUtils.format_path(f) for f in reversed(files) if FileUtils.is_valid(f)
-        ]
+        result = [ptk.format_path(f) for f in reversed(files) if ptk.is_valid(f)]
 
         if index is not None:
             try:
                 result = result[index]
             except (IndexError, TypeError):
                 print("Incorrect index or slice. Returning empty list.")
                 return []
 
         format = format.split("|")
         if len(format) == 2 and "timestamp" in format and "standard" in format:
             if format[0] == "timestamp":
-                result = {FileUtils.time_stamp(res): res for res in result}
+                result = {ptk.time_stamp(res): res for res in result}
             else:
-                result = {res: FileUtils.time_stamp(res) for res in result}
+                result = {res: ptk.time_stamp(res) for res in result}
         elif "timestamp" in format:
-            result = [FileUtils.time_stamp(res) for res in result]
+            result = [ptk.time_stamp(res) for res in result]
         # else return the standard format
 
         return result
 
     @staticmethod
     def get_recent_autosave(index=None, format="standard"):
         """
@@ -159,31 +157,31 @@
 
         files = itertools.chain(
             glob.iglob(os.path.join(autosave_dir, "*.mb")),
             glob.iglob(os.path.join(autosave_dir, "*.ma")),
         )
 
         for file in files:
-            result.append(FileUtils.format_path(file))
+            result.append(ptk.format_path(file))
 
         if index is not None:
             try:
                 result = result[index]
             except (IndexError, TypeError):
                 print("Incorrect index or slice. Returning empty list.")
                 return []
 
         format = format.split("|")
         if len(format) == 2 and "timestamp" in format and "standard" in format:
             if format[0] == "timestamp":
-                result = {FileUtils.time_stamp(res): res for res in result}
+                result = {ptk.time_stamp(res): res for res in result}
             else:
-                result = {res: FileUtils.time_stamp(res) for res in result}
+                result = {res: ptk.time_stamp(res) for res in result}
         elif "timestamp" in format:
-            result = [FileUtils.time_stamp(res) for res in result]
+            result = [ptk.time_stamp(res) for res in result]
         # else return the standard format
 
         return result
 
     @staticmethod
     def get_workspace_scenes(fullPath=True):
         """Get a list of maya scene files from the current workspace directory.
@@ -192,19 +190,19 @@
             fullPath (bool): Return the full path instead of just the filename.
 
         Returns:
             (list)
         """
         workspace_dir = str(pm.workspace(q=True, rd=1))  # get current project path.
 
-        files = FileUtils.get_dir_contents(
+        files = ptk.get_dir_contents(
             workspace_dir, "filepaths", inc_files=("*.mb", "*.ma")
         )
         # Replace any backslashes with forward slashes.
-        result = [FileUtils.format_path(f) for f in files]
+        result = [ptk.format_path(f) for f in files]
 
         if not fullPath:
             result = [f.split("\\")[-1] for f in result]
 
         return result
 
     @staticmethod
@@ -316,17 +314,17 @@
 #     """
 # dir1 = str(pm.workspace(q=True, rd=1)) + "autosave"  # current project path.
 # # get autosave dir path from env variable.
 # dir2 = os.environ.get("MAYA_AUTOSAVE_FOLDER")
 # if dir2 is not None:  # Check if the environment variable exists
 #     dir2 = dir2.split(";")[0]
 
-#     result = FileUtils.get_dir_contents(dir1, "filepaths", inc_files=("*.mb", "*.ma"))
+#     result = ptk.get_dir_contents(dir1, "filepaths", inc_files=("*.mb", "*.ma"))
 #     if dir2 is not None:  # Add the files from the second directory if it exists
-#         result += FileUtils.get_dir_contents(dir2, "filepaths", inc_files=("*.mb", "*.ma"))
+#         result += ptk.get_dir_contents(dir2, "filepaths", inc_files=("*.mb", "*.ma"))
 #     # # Replace any backslashes with forward slashes and reverse the list.
-#     # result = [FileUtils.format_path(f) for f in list(reversed(files))]
+#     # result = [ptk.format_path(f) for f in list(reversed(files))]
 
 #     if timestamp:  # attach modified timestamp
-#         result = FileUtils.time_stamp(result, sort=True)
+#         result = ptk.time_stamp(result, sort=True)
 
 #     return result
```

### Comparing `mayatk-0.6.7/mayatk/project_utils.py.bak` & `mayatk-0.6.8/mayatk/project_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/rig_utils.py` & `mayatk-0.6.8/mayatk/rig_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/rig_utils.py.bak` & `mayatk-0.6.8/mayatk/rig_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/script_utils.py` & `mayatk-0.6.8/mayatk/script_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/utils.py` & `mayatk-0.6.8/mayatk/utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/xform_utils.py` & `mayatk-0.6.8/mayatk/xform_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk/xform_utils.py.bak` & `mayatk-0.6.8/mayatk/xform_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk.egg-info/PKG-INFO` & `mayatk-0.6.8/mayatk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.6.7
+Version: 0.6.8
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mayatk-0.6.7/mayatk.egg-info/PKG-INFO.bak` & `mayatk-0.6.8/mayatk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk.egg-info/SOURCES.txt` & `mayatk-0.6.8/mayatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/mayatk.egg-info/SOURCES.txt.bak` & `mayatk-0.6.8/mayatk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/setup.py` & `mayatk-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/__init__.py` & `mayatk-0.6.8/test/__init__.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/cmpt_utils_test.py` & `mayatk-0.6.8/test/cmpt_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/edit_utils_test.py` & `mayatk-0.6.8/test/edit_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/mat_utils_test.py` & `mayatk-0.6.8/test/mat_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/node_utils_test.py` & `mayatk-0.6.8/test/node_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/rig_utils_test.py` & `mayatk-0.6.8/test/rig_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/run_tests.py` & `mayatk-0.6.8/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/utils_test.py` & `mayatk-0.6.8/test/utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.7/test/xform_utils_test.py` & `mayatk-0.6.8/test/xform_utils_test.py`

 * *Files identical despite different names*


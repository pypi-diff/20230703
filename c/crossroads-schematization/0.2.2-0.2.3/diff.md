# Comparing `tmp/crossroads-schematization-0.2.2.tar.gz` & `tmp/crossroads-schematization-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.2.2.tar", last modified: Thu Jun 29 12:41:53 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.3.tar", last modified: Mon Jul  3 14:59:08 2023, max compression
```

## Comparing `crossroads-schematization-0.2.2.tar` & `crossroads-schematization-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.2/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.2/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.472530 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1104 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.472530 crossroads-schematization-0.2.2/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-29 12:38:10.000000 crossroads-schematization-0.2.2/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     7159 2023-06-29 12:41:17.000000 crossroads-schematization-0.2.2/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.2/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    28261 2023-06-29 12:29:38.000000 crossroads-schematization-0.2.2/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.2/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.2/crschem/resources/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.2/crschem/resources/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.2/crschem/resources/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.2/crschem/resources/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.2/crschem/resources/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.2/crschem/resources/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.2/crschem/resources/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.2/crschem/resources/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.2/crschem/resources/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.2/crschem/resources/style-96.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.2.2/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.2/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.2/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.2/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.3/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.3/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.469362 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1104 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.469362 crossroads-schematization-0.2.3/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-03 14:58:46.000000 crossroads-schematization-0.2.3/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7465 2023-07-03 14:58:16.000000 crossroads-schematization-0.2.3/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.3/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    29411 2023-07-03 14:56:56.000000 crossroads-schematization-0.2.3/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.3/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.3/crschem/resources/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.3/crschem/resources/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.3/crschem/resources/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.3/crschem/resources/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.3/crschem/resources/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.3/crschem/resources/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.3/crschem/resources/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.3/crschem/resources/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.3/crschem/resources/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.3/crschem/resources/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.2.3/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.3/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.3/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.3/setup.py
```

### Comparing `crossroads-schematization-0.2.2/PKG-INFO` & `crossroads-schematization-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.2
+Version: 0.2.3
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.2/README.md` & `crossroads-schematization-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.3/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.2
+Version: 0.2.3
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.2/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.2.3/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/cmd.py` & `crossroads-schematization-0.2.3/crschem/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
     group_output.add_argument('--display-preview', help='display a preview of the crossroad schematization', action='store_true')
     group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif, shp)', type=FileOpener('w'))
     group_output.add_argument('--dpi', help='dpi for tif export', type=int, choices=[96, 300], default=300)
+    group_output.add_argument('--layout', help='Map layout.', type=lambda s: cs.CrossroadSchematization.Layout[s], choices=list(cs.CrossroadSchematization.Layout))
+    group_output.add_argument('--margin', help='Margin in cm. Default: 1.0cm', type=float, default=1)
 
     group_preview = parser.add_argument_group("Preview options", "Parameters used by the preview display")
     group_preview.add_argument('--osm', help='display OpenStreetMap network', action='store_true')
     group_preview.add_argument('--branches', help='display branches', action='store_true')
     group_preview.add_argument('--sidewalks-on-branches', help='display sidewalks only on branches', action='store_true')
     group_preview.add_argument('--exact-islands', help='display exact shape of the islands', action='store_true')
     group_preview.add_argument("--non-reachable-islands", help="display non reachable islands.", action='store_true')
@@ -102,15 +104,15 @@
 
             if args.output.filename.endswith(".pdf"):
                 print("Exporting as pdf:", args.output.filename)
                 print("!! Legacy export")
                 crschem.toPdf(args.output.filename, args.log_files)
             elif args.output.filename.endswith(".tif"):
                 print("Exporting as tif:", args.output.filename)
-                crschem.toTif(args.output.filename, args.log_files, resolution=args.dpi)
+                crschem.toTif(args.output.filename, args.log_files, resolution=args.dpi, layout=args.layout, margin=args.margin)
             elif args.output.filename.endswith(".svg"):
                 print("Exporting as svg:", args.output.filename)
                 print("!! Legacy export")
                 crschem.toSvg(args.output.filename, args.non_reachable_islands)
             elif args.output.filename.endswith(".geojson"):
                 print("Exporting as geojson:", args.output.filename)
                 crschem.toGeojson(args.output.filename, args.non_reachable_islands)
```

### Comparing `crossroads-schematization-0.2.2/crschem/crossroad.py` & `crossroads-schematization-0.2.3/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.3/crschem/crossroad_schematization.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,21 +13,49 @@
 import shutil
 import mapnik
 import mapnik.printing
 from mapnik.printing.conversions import m2px
 import sys
 from osgeo import gdal, osr
 import tempfile
+from enum import Enum
 
 from . import utils as u
 from . import processing as p
 from . import crossroad as c
 
+
+
 class CrossroadSchematization:
 
+    class Layout(Enum):
+        A5_portrait = 0
+        A5_landscape = 1
+        A4_portrait = 2
+        A4_landscape = 3
+        
+        def __str__(self):
+                return self.name
+
+        def width(self, margin = 0.01):
+            if self == CrossroadSchematization.Layout.A5_landscape or self == CrossroadSchematization.Layout.A4_portrait:
+                return 0.21 - margin * 2
+            elif self == CrossroadSchematization.Layout.A5_portrait:
+                return 0.1485 - margin * 2
+            else: # self == Layout.A4_landscape
+                return 0.297 - margin * 2
+
+        def height(self, margin = 0.01):
+            if self == CrossroadSchematization.Layout.A5_portrait or self == CrossroadSchematization.Layout.A4_landscape:
+                return 0.21 - margin * 2
+            elif self == CrossroadSchematization.Layout.A5_landscape:
+                return 0.1485 - margin * 2
+            else: # self == Layout.A4_portrait
+                return 0.297 - margin * 2
+
     node_tags_to_keep = [
         # general informations
         'highway',
         # crosswalk informations
         'crossing',
         'tactile_paving',
         # traffic signals informations
@@ -474,17 +502,17 @@
 
 
 
     def toPdf(self, filename, log_files = False):
         self.to_printable_internal(filename, log_files)
 
 
-    def toTifInternal(self, dirName, filename, log_files, resolution, scale):
-        widthMeter = 0.2
-        heightMeter = 0.14
+    def toTifInternal(self, dirName, filename, log_files, resolution, scale, layout, marginCM):
+        widthMeter = layout.width(marginCM / 100)
+        heightMeter = layout.height(marginCM / 100)
 
         # scale (ie 1cm in the map is scale "scale" * 1 cm in reality)
         scale = 400
 
         width = int(m2px(widthMeter, resolution))
         height = int(m2px(heightMeter, resolution))
 
@@ -544,15 +572,15 @@
         sr = osr.SpatialReference()
         sr.SetFromUserInput(pseudo_mercator.params())
         wkt = sr.ExportToWkt()
         ds.SetProjection(wkt)
 
 
 
-    def toTif(self, filename, log_files = False, resolution = 300, scale = 400):
+    def toTif(self, filename, log_files = False, resolution = 300, scale = 400, layout=Layout.A5_portrait, margin=1):
         # first export to shapefiles in a temporary directory
         dirName = tempfile.mkdtemp()
         if log_files:
             print('Temporary directory (styling):', dirName)
         self.toShapefiles(dirName + "/crossroad.shp")
 
         # then move style file (xml) in this directory
@@ -564,15 +592,15 @@
                         "island-" + str(resolution) + "-white.svg"]:
                 shutil.copy(os.path.dirname(__file__) + "/resources/" + f, dirName)
         else:
             print("not supported DPI")
             return
 
         # finally render the image
-        self.toTifInternal(dirName, filename, log_files, resolution, scale)
+        self.toTifInternal(dirName, filename, log_files, resolution, scale, layout, margin)
 
         # then delete the temporary directory
         if not log_files:
             shutil.rmtree(dirName)
         
 
     def toSvg(self, filename, only_reachable_islands = False):
```

### Comparing `crossroads-schematization-0.2.2/crschem/processing.py` & `crossroads-schematization-0.2.3/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/crossing-3-300.svg` & `crossroads-schematization-0.2.3/crschem/resources/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/crossing-3-96.svg` & `crossroads-schematization-0.2.3/crschem/resources/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/island-300-white.svg` & `crossroads-schematization-0.2.3/crschem/resources/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/island-300.svg` & `crossroads-schematization-0.2.3/crschem/resources/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/island-96-white.svg` & `crossroads-schematization-0.2.3/crschem/resources/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/island-96.svg` & `crossroads-schematization-0.2.3/crschem/resources/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/point-300.svg` & `crossroads-schematization-0.2.3/crschem/resources/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/point-96.svg` & `crossroads-schematization-0.2.3/crschem/resources/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-areas.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-crossings.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-crossings.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-islands.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-islands.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-space.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-nodes.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-polylines-space.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-polylines-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.2.3/crschem/resources/rendering-polylines.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/style-300.xml` & `crossroads-schematization-0.2.3/crschem/resources/style-300.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/style-96.xml` & `crossroads-schematization-0.2.3/crschem/resources/style-96.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.2.3/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/crschem/utils.py` & `crossroads-schematization-0.2.3/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.2/setup.py` & `crossroads-schematization-0.2.3/setup.py`

 * *Files identical despite different names*


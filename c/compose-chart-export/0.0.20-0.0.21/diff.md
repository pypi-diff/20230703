# Comparing `tmp/compose_chart_export-0.0.20-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13386 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 06:58 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-05 06:58 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14564 b- defN 23-Jun-05 06:58 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4974 b- defN 23-Jun-05 06:58 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2285 b- defN 23-Jun-05 06:58 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9602 b- defN 23-Jun-05 06:58 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2365 b- defN 23-Jun-05 06:58 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 06:58 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      626 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/RECORD
-13 files, 38437 bytes uncompressed, 11330 bytes compressed:  70.5%
+Zip file size: 13383 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 08:46 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-03 08:46 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14564 b- defN 23-Jul-03 08:46 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4974 b- defN 23-Jul-03 08:46 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-Jul-03 08:46 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9602 b- defN 23-Jul-03 08:46 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-Jul-03 08:46 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Jul-03 08:46 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      626 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/RECORD
+13 files, 38437 bytes uncompressed, 11327 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.20.dist-info/METADATA
+Filename: compose_chart_export-0.0.21.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.20.dist-info/WHEEL
+Filename: compose_chart_export-0.0.21.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.20.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.21.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.20.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.21.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.20.dist-info/RECORD
+Filename: compose_chart_export-0.0.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `compose_chart_export-0.0.20.dist-info/METADATA` & `compose_chart_export-0.0.21.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.20
+Version: 0.0.21
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.20)
-Requires-Dist: model-lib (==0.0.20)
-Requires-Dist: pydantic (>=1.10.2)
+Requires-Dist: docker-compose-parser (==0.0.21)
+Requires-Dist: model-lib (==0.0.21)
+Requires-Dist: pydantic (==1.10.2)
 Requires-Dist: semver (==2.13.0)
 Requires-Dist: typing-extensions (>=4.3.0)
-Requires-Dist: zero-3rdparty (==0.0.20)
+Requires-Dist: zero-3rdparty (==0.0.21)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

## Comparing `compose_chart_export-0.0.20.dist-info/RECORD` & `compose_chart_export-0.0.21.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 compose_chart_export/chart_export.py,sha256=lRtxzU3Ac2SfOAxZmSv9ml0KsDM4tHx5ois0BOFF9dc,2517
 compose_chart_export/chart_file_templates.py,sha256=sQMgnbhaCgppTOO5XZD72YbshNJS90INvCENukeNY3w,14564
 compose_chart_export/chart_mods.py,sha256=6eaO7tuccQWcZDc_yoi3p7aIOO2YQ4vAb2aqKZ5qBzc,4974
 compose_chart_export/chart_read.py,sha256=5A7mcFdq1lnD7fitj5-evHE9A0zJ6aAlY0KEYPmeRZo,2285
 compose_chart_export/compose_export.py,sha256=9CLgDO88kYyR55TcHxhGsgaA4xbyj2f-mSXINYRP55w,9602
 compose_chart_export/ports.py,sha256=ubPaqe31gwDqPj8s4Bd6pZf8qB02hylpoQpYpbFkYwc,2365
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.20.dist-info/METADATA,sha256=nuys7GXtj31MjHpzgOic_SVIOhYUMSPmEkV1NNUQfL0,626
-compose_chart_export-0.0.20.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.20.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.20.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.20.dist-info/RECORD,,
+compose_chart_export-0.0.21.dist-info/METADATA,sha256=pt0BWsJQthTslawgiE7Vn6xjWQD2vveJcPrtoLg0jeE,626
+compose_chart_export-0.0.21.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.21.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.21.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.21.dist-info/RECORD,,
```


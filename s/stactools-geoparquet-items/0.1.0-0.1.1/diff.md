# Comparing `tmp/stactools-geoparquet-items-0.1.0.tar.gz` & `tmp/stactools-geoparquet-items-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-geoparquet-items-0.1.0.tar", last modified: Fri Jun 30 21:44:23 2023, max compression
+gzip compressed data, was "stactools-geoparquet-items-0.1.1.tar", last modified: Mon Jul  3 21:34:49 2023, max compression
```

## Comparing `stactools-geoparquet-items-0.1.0.tar` & `stactools-geoparquet-items-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-30 21:44:06.000000 stactools-geoparquet-items-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-30 21:44:06.000000 stactools-geoparquet-items-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-30 21:44:06.000000 stactools-geoparquet-items-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/src/stactools/geoparquet_items/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 21:44:06.000000 stactools-geoparquet-items-0.1.0/src/stactools/geoparquet_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-30 21:44:06.000000 stactools-geoparquet-items-0.1.0/src/stactools/geoparquet_items/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:44:23.467285 stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 21:44:23.000000 stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 21:44:23.000000 stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:44:23.000000 stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 21:44:23.000000 stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 21:44:23.000000 stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.619260 stactools-geoparquet-items-0.1.1/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/top_level.txt
```

### Comparing `stactools-geoparquet-items-0.1.0/LICENSE` & `stactools-geoparquet-items-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.1.0/PKG-INFO` & `stactools-geoparquet-items-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-geoparquet-items-0.1.0/README.md` & `stactools-geoparquet-items-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.1.0/setup.cfg` & `stactools-geoparquet-items-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.1.0/src/stactools/geoparquet_items/commands.py` & `stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import os
 
 import click
 import requests
 import stac_geoparquet
 from click import Command, Group
-from pystac import Asset, Collection
 
 logger = logging.getLogger(__name__)
 
 
 def create_geoparquetitems_command(cli: Group) -> Command:
     """Creates the stactools-geoparquet-items command line utility."""
 
@@ -58,20 +57,27 @@
         if len(items) > 0:
             df = stac_geoparquet.to_geodataframe(items)
             df.to_parquet(destination)
         else:
             raise Exception("No items found")
 
         if len(collection) > 0:
-            stac_collection = Collection.from_file(collection)
-            asset = Asset(
-                href=destination,
-                media_type="application/x-parquet",
-                roles=["stac-items"],
-                title="GeoParquet STAC Items",
-            )
-            stac_collection.add_asset("geoparquet-items", asset)
-            stac_collection.save_object(dest_href=collection)
+            with open(collection, 'r+') as f:
+                collection_json = json.load(f)
+                if "assets" not in collection_json:
+                    collection_json["assets"] = {}
+                
+                basepath = os.path.abspath(os.path.dirname(collection))
+                collection_json["assets"]["geoparquet-items"] = {
+                    "href": os.path.relpath(destination, basepath),
+                    "type": "application/x-parquet",
+                    "roles": ["stac-items"],
+                    "title": "GeoParquet STAC Items",
+                }
+
+                f.seek(0)
+                json.dump(collection_json, f, indent = 2)
+                f.truncate()
 
         return None
 
     return geoparquetitems
```

### Comparing `stactools-geoparquet-items-0.1.0/src/stactools_geoparquet_items.egg-info/PKG-INFO` & `stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
```


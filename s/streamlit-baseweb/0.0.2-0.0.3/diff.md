# Comparing `tmp/streamlit_baseweb-0.0.2.tar.gz` & `tmp/streamlit_baseweb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_baseweb-0.0.2.tar", last modified: Mon Jul  3 17:42:48 2023, max compression
+gzip compressed data, was "streamlit_baseweb-0.0.3.tar", last modified: Mon Jul  3 18:05:13 2023, max compression
```

## Comparing `streamlit_baseweb-0.0.2.tar` & `streamlit_baseweb-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 17:42:48.054383 streamlit_baseweb-0.0.2/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       44 2023-07-03 17:33:16.000000 streamlit_baseweb-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3871 2023-07-03 17:42:48.052454 streamlit_baseweb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1965 2023-07-03 17:37:38.000000 streamlit_baseweb-0.0.2/README.md
--rw-rw-rw-   0        0        0      892 2023-07-03 17:41:14.000000 streamlit_baseweb-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 17:42:48.054383 streamlit_baseweb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-03 17:41:09.000000 streamlit_baseweb-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:42:48.042592 streamlit_baseweb-0.0.2/streamlit_baseweb/
--rw-rw-rw-   0        0        0     2225 2023-07-03 17:37:38.000000 streamlit_baseweb-0.0.2/streamlit_baseweb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:42:48.051489 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/
--rw-rw-rw-   0        0        0     3871 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.460961 streamlit_baseweb-0.0.3/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-07-03 17:54:39.000000 streamlit_baseweb-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3871 2023-07-03 18:05:13.459962 streamlit_baseweb-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1965 2023-07-03 17:37:38.000000 streamlit_baseweb-0.0.3/README.md
+-rw-rw-rw-   0        0        0      892 2023-07-03 17:49:44.000000 streamlit_baseweb-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 18:05:13.460961 streamlit_baseweb-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-03 17:49:44.000000 streamlit_baseweb-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.414646 streamlit_baseweb-0.0.3/streamlit_baseweb/
+-rw-rw-rw-   0        0        0     2215 2023-07-03 18:04:03.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.402594 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.434649 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/
+-rw-rw-rw-   0        0        0      859 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1870 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/index.html
+-rw-rw-rw-   0        0        0      564 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js
+-rw-rw-rw-   0        0        0     1183 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.403595 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.457468 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/
+-rw-rw-rw-   0        0        0   700106 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1996642 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map
+-rw-rw-rw-   0        0        0     1488 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js
+-rw-rw-rw-   0        0        0     4819 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map
+-rw-rw-rw-   0        0        0     1590 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js
+-rw-rw-rw-   0        0        0     8309 2023-07-03 16:11:57.000000 streamlit_baseweb-0.0.3/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map
+drwxrwxrwx   0        0        0        0 2023-07-03 18:05:13.425648 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/
+-rw-rw-rw-   0        0        0     3871 2023-07-03 18:05:13.000000 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2023-07-03 18:05:13.000000 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 18:05:13.000000 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-03 18:05:13.000000 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-03 18:05:13.000000 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-03 18:05:13.000000 streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/top_level.txt
```

### Comparing `streamlit_baseweb-0.0.2/LICENSE` & `streamlit_baseweb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.0.2/PKG-INFO` & `streamlit_baseweb-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_baseweb
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_baseweb-0.0.2/README.md` & `streamlit_baseweb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.0.2/pyproject.toml` & `streamlit_baseweb-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_baseweb"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Streamlit implementation of the Base Web library."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `streamlit_baseweb-0.0.2/setup.py` & `streamlit_baseweb-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_baseweb",
-    version="0.0.2",
+    version="0.0.3",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the Base Web library.",
     long_description="https://baseweb.design/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/baseweb_components",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_baseweb-0.0.2/streamlit_baseweb/__init__.py` & `streamlit_baseweb-0.0.3/streamlit_baseweb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if not _RELEASE:
     _base_web_modal = components.declare_component(
         "base_web_modal", url="http://localhost:3000",
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    modal_dir = os.path.join(parent_dir, "baseweb_components/modal/frontend/build")
+    modal_dir = os.path.join(parent_dir, "streamlit_baseweb/modal/build")
     _base_web_modal = components.declare_component("base_web_modal", path=modal_dir)
 
 
 def base_web_modal(
     title: str,
     body: str,
     is_open: bool = True,
```

### Comparing `streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/PKG-INFO` & `streamlit_baseweb-0.0.3/streamlit_baseweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-baseweb
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


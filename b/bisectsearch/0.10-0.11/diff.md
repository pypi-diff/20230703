# Comparing `tmp/bisectsearch-0.10.tar.gz` & `tmp/bisectsearch-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisectsearch-0.10.tar", last modified: Mon Jul  3 02:32:41 2023, max compression
+gzip compressed data, was "bisectsearch-0.11.tar", last modified: Mon Jul  3 02:34:28 2023, max compression
```

## Comparing `bisectsearch-0.10.tar` & `bisectsearch-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 02:32:41.442887 bisectsearch-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-03 02:32:36.000000 bisectsearch-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      107 2023-07-03 02:32:35.000000 bisectsearch-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3251 2023-07-03 02:32:41.442887 bisectsearch-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2023-07-03 02:30:52.000000 bisectsearch-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 02:32:41.439895 bisectsearch-0.10/bisectsearch/
--rw-rw-rw-   0        0        0     2616 2023-07-03 02:30:52.000000 bisectsearch-0.10/bisectsearch/README.MD
--rw-rw-rw-   0        0        0     2734 2023-07-03 02:27:35.000000 bisectsearch-0.10/bisectsearch/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-03 02:32:40.000000 bisectsearch-0.10/bisectsearch/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 02:32:40.000000 bisectsearch-0.10/bisectsearch/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-03 02:32:41.441891 bisectsearch-0.10/bisectsearch.egg-info/
--rw-rw-rw-   0        0        0     3251 2023-07-03 02:32:41.000000 bisectsearch-0.10/bisectsearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-03 02:32:41.000000 bisectsearch-0.10/bisectsearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 02:32:41.000000 bisectsearch-0.10/bisectsearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 02:32:41.000000 bisectsearch-0.10/bisectsearch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-03 02:32:41.443885 bisectsearch-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-07-03 02:32:40.000000 bisectsearch-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 02:34:28.656752 bisectsearch-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-03 02:34:18.000000 bisectsearch-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      107 2023-07-03 02:34:16.000000 bisectsearch-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3246 2023-07-03 02:34:28.656752 bisectsearch-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2023-07-03 02:30:52.000000 bisectsearch-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 02:34:28.652762 bisectsearch-0.11/bisectsearch/
+-rw-rw-rw-   0        0        0     2616 2023-07-03 02:30:52.000000 bisectsearch-0.11/bisectsearch/README.MD
+-rw-rw-rw-   0        0        0     2734 2023-07-03 02:27:35.000000 bisectsearch-0.11/bisectsearch/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 02:34:27.000000 bisectsearch-0.11/bisectsearch/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 02:34:27.000000 bisectsearch-0.11/bisectsearch/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-03 02:34:28.656752 bisectsearch-0.11/bisectsearch.egg-info/
+-rw-rw-rw-   0        0        0     3246 2023-07-03 02:34:28.000000 bisectsearch-0.11/bisectsearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-03 02:34:28.000000 bisectsearch-0.11/bisectsearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 02:34:28.000000 bisectsearch-0.11/bisectsearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 02:34:28.000000 bisectsearch-0.11/bisectsearch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-03 02:34:28.657749 bisectsearch-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1266 2023-07-03 02:34:27.000000 bisectsearch-0.11/setup.py
```

### Comparing `bisectsearch-0.10/LICENSE.rst` & `bisectsearch-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bisectsearch-0.10/PKG-INFO` & `bisectsearch-0.11/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bisectsearch
-Version: 0.10
-Summary: Maps the elements of an iterable to categories using bisect
+Version: 0.11
+Summary: Functions for performing binary search on sorted lists
 Home-page: https://github.com/hansalemaos/bisectsearch
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: bisect,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `bisectsearch-0.10/README.md` & `bisectsearch-0.11/README.md`

 * *Files identical despite different names*

### Comparing `bisectsearch-0.10/bisectsearch/README.MD` & `bisectsearch-0.11/bisectsearch/README.MD`

 * *Files identical despite different names*

### Comparing `bisectsearch-0.10/bisectsearch/__init__.py` & `bisectsearch-0.11/bisectsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `bisectsearch-0.10/bisectsearch.egg-info/PKG-INFO` & `bisectsearch-0.11/bisectsearch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bisectsearch
-Version: 0.10
-Summary: Maps the elements of an iterable to categories using bisect
+Version: 0.11
+Summary: Functions for performing binary search on sorted lists
 Home-page: https://github.com/hansalemaos/bisectsearch
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: bisect,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `bisectsearch-0.10/setup.py` & `bisectsearch-0.11/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
-DESCRIPTION = '''Maps the elements of an iterable to categories using bisect'''
+VERSION = '''0.11'''
+DESCRIPTION = '''Functions for performing binary search on sorted lists'''
 
 # Setting up
 setup(
     name="bisectsearch",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/bisectsearch',
```


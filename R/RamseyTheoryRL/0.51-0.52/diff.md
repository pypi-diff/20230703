# Comparing `tmp/RamseyTheoryRL-0.51.tar.gz` & `tmp/RamseyTheoryRL-0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RamseyTheoryRL-0.51.tar", last modified: Mon Jul  3 03:27:00 2023, max compression
+gzip compressed data, was "RamseyTheoryRL-0.52.tar", last modified: Mon Jul  3 03:30:26 2023, max compression
```

## Comparing `RamseyTheoryRL-0.51.tar` & `RamseyTheoryRL-0.52.tar`

### file list

```diff
@@ -1,31 +1,47 @@
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.854840 RamseyTheoryRL-0.51/
--rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.51/LICENSE.txt
--rw-r--r--   0 stevevott   (501) staff       (20)     2761 2023-07-03 03:27:00.854684 RamseyTheoryRL-0.51/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     2096 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/README.md
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.850931 RamseyTheoryRL-0.51/RamseyTheoryRL/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.851487 RamseyTheoryRL-0.51/RamseyTheoryRL/src/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.852309 RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-03 03:24:44.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
--rw-r--r--   0 stevevott   (501) staff       (20)     9795 2023-07-03 03:26:34.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)     8240 2023-07-03 03:26:39.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)    11528 2023-07-03 03:26:46.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/test.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.853358 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/gfeatures.py
--rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/guseful.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.854419 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
--rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:27:00.851362 RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/
--rw-r--r--   0 stevevott   (501) staff       (20)     2761 2023-07-03 03:27:00.000000 RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)      884 2023-07-03 03:27:00.000000 RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/SOURCES.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:27:00.000000 RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/dependency_links.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 03:27:00.000000 RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/top_level.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:27:00.854892 RamseyTheoryRL-0.51/setup.cfg
--rw-r--r--   0 stevevott   (501) staff       (20)      796 2023-07-03 03:26:56.000000 RamseyTheoryRL-0.51/setup.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.949671 RamseyTheoryRL-0.52/
+-rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.52/LICENSE.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)     2761 2023-07-03 03:30:26.949546 RamseyTheoryRL-0.52/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     2096 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/README.md
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.943631 RamseyTheoryRL-0.52/RamseyTheoryRL/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.944296 RamseyTheoryRL-0.52/RamseyTheoryRL/data/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:43.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/data/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.944405 RamseyTheoryRL-0.52/RamseyTheoryRL/src/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.945595 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:39.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    12523 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/gbfs.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3539 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1070 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/igraph_train_gen.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1157 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/isofile_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3365 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/models/train_gen.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.946586 RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-03 03:24:44.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     9795 2023-07-03 03:26:34.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     8240 2023-07-03 03:26:39.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    11528 2023-07-03 03:26:46.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/test.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.947685 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/gfeatures.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/guseful.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.948427 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.949250 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:09.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1401 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/datavis.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      827 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/param_plot.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      788 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/r39_graph.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      878 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/r46_graphs.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     2123 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.52/RamseyTheoryRL/src/visuals/vis.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:26.944165 RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/
+-rw-r--r--   0 stevevott   (501) staff       (20)     2761 2023-07-03 03:30:26.000000 RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     1390 2023-07-03 03:30:26.000000 RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/SOURCES.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:30:26.000000 RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/dependency_links.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 03:30:26.000000 RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/top_level.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:30:26.949724 RamseyTheoryRL-0.52/setup.cfg
+-rw-r--r--   0 stevevott   (501) staff       (20)      796 2023-07-03 03:30:22.000000 RamseyTheoryRL-0.52/setup.py
```

### Comparing `RamseyTheoryRL-0.51/LICENSE.txt` & `RamseyTheoryRL-0.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/PKG-INFO` & `RamseyTheoryRL-0.52/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.51
+Version: 0.52
 Summary: Ramsey Number Explorer
 Home-page: https://github.com/aLehav/RamseyTheoryRL
 Author: Adam Lehavi, Steve Vott
 Author-email: svott03@gmail.com, alehavi@usc.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.51 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.52 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
 Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
 MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
```

### Comparing `RamseyTheoryRL-0.51/README.md` & `RamseyTheoryRL-0.52/README.md`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/ramsey_checker/test.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/ramsey_checker/test.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/gfeatures.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/gfeatures.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/guseful.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/guseful.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py` & `RamseyTheoryRL-0.52/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/PKG-INFO` & `RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.51
+Version: 0.52
 Summary: Ramsey Number Explorer
 Home-page: https://github.com/aLehav/RamseyTheoryRL
 Author: Adam Lehavi, Steve Vott
 Author-email: svott03@gmail.com, alehavi@usc.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.51 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.52 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
 Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
 MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
```

### Comparing `RamseyTheoryRL-0.51/RamseyTheoryRL.egg-info/SOURCES.txt` & `RamseyTheoryRL-0.52/RamseyTheoryRL.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,21 +2,34 @@
 README.md
 setup.py
 RamseyTheoryRL/__init__.py
 RamseyTheoryRL.egg-info/PKG-INFO
 RamseyTheoryRL.egg-info/SOURCES.txt
 RamseyTheoryRL.egg-info/dependency_links.txt
 RamseyTheoryRL.egg-info/top_level.txt
+RamseyTheoryRL/data/__init__.py
 RamseyTheoryRL/src/__init__.py
+RamseyTheoryRL/src/models/__init__.py
+RamseyTheoryRL/src/models/gbfs.py
+RamseyTheoryRL/src/models/heuristic.py
+RamseyTheoryRL/src/models/igraph_train_gen.py
+RamseyTheoryRL/src/models/isofile_checker.py
+RamseyTheoryRL/src/models/train_gen.py
 RamseyTheoryRL/src/ramsey_checker/__init__.py
 RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
 RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
 RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
 RamseyTheoryRL/src/ramsey_checker/test.py
 RamseyTheoryRL/src/utils/__init__.py
 RamseyTheoryRL/src/utils/gfeatures.py
 RamseyTheoryRL/src/utils/guseful.py
 RamseyTheoryRL/src/utils/heuristic/__init__.py
 RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
 RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
 RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
-RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
+RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
+RamseyTheoryRL/src/visuals/__init__.py
+RamseyTheoryRL/src/visuals/datavis.py
+RamseyTheoryRL/src/visuals/param_plot.py
+RamseyTheoryRL/src/visuals/r39_graph.py
+RamseyTheoryRL/src/visuals/r46_graphs.py
+RamseyTheoryRL/src/visuals/vis.py
```

### Comparing `RamseyTheoryRL-0.51/setup.py` & `RamseyTheoryRL-0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RamseyTheoryRL",
-    version="0.51",
+    version="0.52",
     packages=find_packages(),
     author="Adam Lehavi, Steve Vott",
     author_email="svott03@gmail.com, alehavi@usc.edu",
     description="Ramsey Number Explorer",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license="MIT",
```


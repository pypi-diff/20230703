# Comparing `tmp/RamseyTheoryRL-0.4.tar.gz` & `tmp/RamseyTheoryRL-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RamseyTheoryRL-0.4.tar", last modified: Mon Jul  3 03:13:25 2023, max compression
+gzip compressed data, was "RamseyTheoryRL-0.5.tar", last modified: Mon Jul  3 03:22:11 2023, max compression
```

## Comparing `RamseyTheoryRL-0.4.tar` & `RamseyTheoryRL-0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.136106 RamseyTheoryRL-0.4/
--rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.4/LICENSE.txt
--rw-r--r--   0 stevevott   (501) staff       (20)     2760 2023-07-03 03:13:25.135966 RamseyTheoryRL-0.4/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     2096 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/README.md
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.131536 RamseyTheoryRL-0.4/RamseyTheoryRL/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.132098 RamseyTheoryRL-0.4/RamseyTheoryRL/src/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.134398 RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
--rw-r--r--   0 stevevott   (501) staff       (20)     9794 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)     8239 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)    11476 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/test.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.134972 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/gfeatures.py
--rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/guseful.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.135715 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
--rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:13:25.131969 RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/
--rw-r--r--   0 stevevott   (501) staff       (20)     2760 2023-07-03 03:13:25.000000 RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)      884 2023-07-03 03:13:25.000000 RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/SOURCES.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:13:25.000000 RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/dependency_links.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 03:13:25.000000 RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/top_level.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:13:25.136156 RamseyTheoryRL-0.4/setup.cfg
--rw-r--r--   0 stevevott   (501) staff       (20)      795 2023-07-03 03:13:00.000000 RamseyTheoryRL-0.4/setup.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.026154 RamseyTheoryRL-0.5/
+-rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.5/LICENSE.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)     2760 2023-07-03 03:22:11.026019 RamseyTheoryRL-0.5/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     2096 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/README.md
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.022858 RamseyTheoryRL-0.5/RamseyTheoryRL/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.023453 RamseyTheoryRL-0.5/RamseyTheoryRL/src/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.024417 RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     9794 2023-07-03 03:15:06.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     8239 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    11526 2023-07-03 03:21:55.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/test.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.024999 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/gfeatures.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/guseful.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.025797 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:22:11.023300 RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/
+-rw-r--r--   0 stevevott   (501) staff       (20)     2760 2023-07-03 03:22:10.000000 RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)      884 2023-07-03 03:22:11.000000 RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/SOURCES.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:22:10.000000 RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/dependency_links.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 03:22:10.000000 RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/top_level.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:22:11.026196 RamseyTheoryRL-0.5/setup.cfg
+-rw-r--r--   0 stevevott   (501) staff       (20)      795 2023-07-03 03:22:02.000000 RamseyTheoryRL-0.5/setup.py
```

### Comparing `RamseyTheoryRL-0.4/LICENSE.txt` & `RamseyTheoryRL-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/PKG-INFO` & `RamseyTheoryRL-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.4
+Version: 0.5
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
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.4 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.5 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
 Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
 MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
```

### Comparing `RamseyTheoryRL-0.4/README.md` & `RamseyTheoryRL-0.5/README.md`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/ramsey_checker/test.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/ramsey_checker/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 S = 3
 T = 5
 
 
 class NeptuneRunner:
     def run(self):
         ramsey_checker = RamseyCheckerSingleThread()
+        ramsey_multi = RamseyCheckerMultiThread()
         if LOAD_MODEL:
             MODEL_ID = "RAM-HEUR-85"
             RUN_ID = "RAM-94"
             print(f"Loading {MODEL_ID} and {RUN_ID}.")
             run, model_version, model = load_model_by_id(project=PROJECT,
                                                         model_name=MODEL_NAME,
                                                         model_id=MODEL_ID,
```

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/gfeatures.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/gfeatures.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/guseful.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/guseful.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py` & `RamseyTheoryRL-0.5/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/PKG-INFO` & `RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.4
+Version: 0.5
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
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.4 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.5 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
 Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
 MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
```

### Comparing `RamseyTheoryRL-0.4/RamseyTheoryRL.egg-info/SOURCES.txt` & `RamseyTheoryRL-0.5/RamseyTheoryRL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.4/setup.py` & `RamseyTheoryRL-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RamseyTheoryRL",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     author="Adam Lehavi, Steve Vott",
     author_email="svott03@gmail.com, alehavi@usc.edu",
     description="Ramsey Number Explorer",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license="MIT",
```


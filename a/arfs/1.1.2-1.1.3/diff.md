# Comparing `tmp/arfs-1.1.2.tar.gz` & `tmp/arfs-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.1.2.tar", last modified: Fri Jun 16 08:23:55 2023, max compression
+gzip compressed data, was "arfs-1.1.3.tar", last modified: Mon Jul  3 13:42:56 2023, max compression
```

## Comparing `arfs-1.1.2.tar` & `arfs-1.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.778003 arfs-1.1.2/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.2/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-06-16 08:23:55.779005 arfs-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.2/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-06-16 08:23:55.787014 arfs-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.369004 arfs-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.510001 arfs-1.1.2/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-06-16 08:22:45.000000 arfs-1.1.2/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.2/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.370002 arfs-1.1.2/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.640005 arfs-1.1.2/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.2/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.2/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.745005 arfs-1.1.2/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    90379 2023-06-09 19:54:49.000000 arfs-1.1.2/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15449 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.1.2/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-1.1.2/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.2/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    30283 2023-05-31 17:10:21.000000 arfs-1.1.2/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.2/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.2/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.578002 arfs-1.1.2/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.2/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 08:23:55.000000 arfs-1.1.2/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 08:23:55.767006 arfs-1.1.2/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.2/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.2/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.875224 arfs-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0    11069 2023-07-03 13:42:56.877227 arfs-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.3/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1389 2023-07-03 13:42:56.885226 arfs-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.372239 arfs-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.551227 arfs-1.1.3/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-07-03 13:39:48.000000 arfs-1.1.3/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.3/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.3/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.374227 arfs-1.1.3/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.684226 arfs-1.1.3/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.3/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.3/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.829224 arfs-1.1.3/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.3/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    90379 2023-06-09 19:54:49.000000 arfs-1.1.3/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.3/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.3/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.3/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15454 2023-07-03 11:13:30.000000 arfs-1.1.3/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    14769 2023-07-03 11:13:51.000000 arfs-1.1.3/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-1.1.3/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.3/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    30283 2023-05-31 17:10:21.000000 arfs-1.1.3/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.3/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.3/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.616224 arfs-1.1.3/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-07-03 13:42:56.000000 arfs-1.1.3/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-07-03 13:42:56.000000 arfs-1.1.3/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:42:56.000000 arfs-1.1.3/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.3/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      365 2023-07-03 13:42:56.000000 arfs-1.1.3/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-03 13:42:56.000000 arfs-1.1.3/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:42:56.863225 arfs-1.1.3/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.3/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.3/tests/test_featselect.py
```

### Comparing `arfs-1.1.2/LICENSE.md` & `arfs-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/PKG-INFO` & `arfs-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.2
+Version: 1.1.3
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.1.2/README.md` & `arfs-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/setup.cfg` & `arfs-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/association.py` & `arfs-1.1.3/src/arfs/association.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/benchmark.py` & `arfs-1.1.3/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-1.1.3/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/dataset/data/housing.zip` & `arfs-1.1.3/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/feature_selection/__init__.py` & `arfs-1.1.3/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/feature_selection/allrelevant.py` & `arfs-1.1.3/src/arfs/feature_selection/allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/feature_selection/base.py` & `arfs-1.1.3/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/feature_selection/mrmr.py` & `arfs-1.1.3/src/arfs/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/feature_selection/summary.py` & `arfs-1.1.3/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/feature_selection/unsupervised.py` & `arfs-1.1.3/src/arfs/feature_selection/unsupervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - The ``MissingValueThreshold`` child of the ``BaseThresholdSelector``
 - The ``UniqueValuesThreshold`` child of the ``BaseThresholdSelector``
 - The ``CardinalityThreshold`` child of the ``BaseThresholdSelector``
 - The ``CollinearityThreshold`` child of the ``BaseThresholdSelector``
 """
 
 from __future__ import print_function
-from tqdm import trange
+from tqdm.auto import trange
 
 # pandas
 import pandas as pd
 
 # numpy
 import numpy as np
```

### Comparing `arfs-1.1.2/src/arfs/feature_selection/variable_importance.py` & `arfs-1.1.3/src/arfs/feature_selection/variable_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 **The module structure is the following:**
 
 - The ``VariableImportance`` main class for identifying non-important features
 
 """
 
 from __future__ import print_function
-from tqdm import trange
+from tqdm.auto import trange
 
 # pandas
 import pandas as pd
 
 # numpy
 import numpy as np
```

### Comparing `arfs-1.1.2/src/arfs/gbm.py` & `arfs-1.1.3/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/parallel.py` & `arfs-1.1.3/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/preprocessing.py` & `arfs-1.1.3/src/arfs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/sampling.py` & `arfs-1.1.3/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs/utils.py` & `arfs-1.1.3/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/src/arfs.egg-info/PKG-INFO` & `arfs-1.1.3/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.2
+Version: 1.1.3
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.1.2/src/arfs.egg-info/SOURCES.txt` & `arfs-1.1.3/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/tests/test_allrelevant.py` & `arfs-1.1.3/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.2/tests/test_featselect.py` & `arfs-1.1.3/tests/test_featselect.py`

 * *Files identical despite different names*


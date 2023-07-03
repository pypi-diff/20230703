# Comparing `tmp/pertCF-0.1.8.tar.gz` & `tmp/pertCF-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pertCF-0.1.8.tar", last modified: Mon Jul  3 14:16:35 2023, max compression
+gzip compressed data, was "pertCF-0.1.9.tar", last modified: Mon Jul  3 20:36:11 2023, max compression
```

## Comparing `pertCF-0.1.8.tar` & `pertCF-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:16:35.947276 pertCF-0.1.8/
--rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.8/LICENSE.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 14:16:35.947110 pertCF-0.1.8/PKG-INFO
--rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.8/README.md
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:16:35.946048 pertCF-0.1.8/pertCF/
--rw-r--r--   0 bbayrak    (501) staff       (20)      964 2023-07-03 14:07:23.000000 pertCF-0.1.8/pertCF/Case.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     2278 2023-07-03 14:07:23.000000 pertCF-0.1.8/pertCF/Data.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     7216 2023-07-03 14:14:09.000000 pertCF-0.1.8/pertCF/PertCF.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     3995 2023-07-03 14:07:23.000000 pertCF-0.1.8/pertCF/Similarity.py
--rw-r--r--   0 bbayrak    (501) staff       (20)      245 2023-07-03 14:16:18.000000 pertCF-0.1.8/pertCF/__init__.py
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:16:35.946889 pertCF-0.1.8/pertCF.egg-info/
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 14:16:35.000000 pertCF-0.1.8/pertCF.egg-info/PKG-INFO
--rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 14:16:35.000000 pertCF-0.1.8/pertCF.egg-info/SOURCES.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 14:16:35.000000 pertCF-0.1.8/pertCF.egg-info/dependency_links.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 14:16:35.000000 pertCF-0.1.8/pertCF.egg-info/requires.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 14:16:35.000000 pertCF-0.1.8/pertCF.egg-info/top_level.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 14:16:35.947325 pertCF-0.1.8/setup.cfg
--rw-r--r--   0 bbayrak    (501) staff       (20)      994 2023-07-03 14:16:28.000000 pertCF-0.1.8/setup.py
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 20:36:11.953923 pertCF-0.1.9/
+-rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.9/LICENSE.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 20:36:11.953759 pertCF-0.1.9/PKG-INFO
+-rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.9/README.md
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 20:36:11.952560 pertCF-0.1.9/pertCF/
+-rw-r--r--   0 bbayrak    (501) staff       (20)      964 2023-07-03 14:07:23.000000 pertCF-0.1.9/pertCF/Case.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     2278 2023-07-03 14:07:23.000000 pertCF-0.1.9/pertCF/Data.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     7252 2023-07-03 20:34:10.000000 pertCF-0.1.9/pertCF/PertCF.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     3995 2023-07-03 14:07:23.000000 pertCF-0.1.9/pertCF/Similarity.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)      225 2023-07-03 20:35:44.000000 pertCF-0.1.9/pertCF/__init__.py
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 20:36:11.953533 pertCF-0.1.9/pertCF.egg-info/
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 20:36:11.000000 pertCF-0.1.9/pertCF.egg-info/PKG-INFO
+-rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 20:36:11.000000 pertCF-0.1.9/pertCF.egg-info/SOURCES.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 20:36:11.000000 pertCF-0.1.9/pertCF.egg-info/dependency_links.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 20:36:11.000000 pertCF-0.1.9/pertCF.egg-info/requires.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 20:36:11.000000 pertCF-0.1.9/pertCF.egg-info/top_level.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 20:36:11.953974 pertCF-0.1.9/setup.cfg
+-rw-r--r--   0 bbayrak    (501) staff       (20)      920 2023-07-03 20:36:03.000000 pertCF-0.1.9/setup.py
```

### Comparing `pertCF-0.1.8/LICENSE.txt` & `pertCF-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.8/pertCF/Case.py` & `pertCF-0.1.9/pertCF/Case.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.8/pertCF/Data.py` & `pertCF-0.1.9/pertCF/Data.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.8/pertCF/PertCF.py` & `pertCF-0.1.9/pertCF/PertCF.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from scipy.special import softmax
-import Case
-import Data
-import Similarity
+from Case import Case
+from Data import Data
+from Similarity import Similarity
 import shap
 
 
 class PertCF:
     def __init__(self,
                  dataset,
                  label,
```

### Comparing `pertCF-0.1.8/pertCF/Similarity.py` & `pertCF-0.1.9/pertCF/Similarity.py`

 * *Files identical despite different names*


# Comparing `tmp/pertCF-0.1.6.tar.gz` & `tmp/pertCF-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pertCF-0.1.6.tar", last modified: Mon Jul  3 14:12:10 2023, max compression
+gzip compressed data, was "pertCF-0.1.7.tar", last modified: Mon Jul  3 14:14:35 2023, max compression
```

## Comparing `pertCF-0.1.6.tar` & `pertCF-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:12:10.601370 pertCF-0.1.6/
--rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.6/LICENSE.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 14:12:10.601203 pertCF-0.1.6/PKG-INFO
--rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.6/README.md
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:12:10.600015 pertCF-0.1.6/pertCF/
--rw-r--r--   0 bbayrak    (501) staff       (20)      964 2023-07-03 14:07:23.000000 pertCF-0.1.6/pertCF/Case.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     2278 2023-07-03 14:07:23.000000 pertCF-0.1.6/pertCF/Data.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     7252 2023-07-03 14:06:39.000000 pertCF-0.1.6/pertCF/PertCF.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     3995 2023-07-03 14:07:23.000000 pertCF-0.1.6/pertCF/Similarity.py
--rw-r--r--   0 bbayrak    (501) staff       (20)      260 2023-07-03 14:11:58.000000 pertCF-0.1.6/pertCF/__init__.py
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:12:10.600938 pertCF-0.1.6/pertCF.egg-info/
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 14:12:10.000000 pertCF-0.1.6/pertCF.egg-info/PKG-INFO
--rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 14:12:10.000000 pertCF-0.1.6/pertCF.egg-info/SOURCES.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 14:12:10.000000 pertCF-0.1.6/pertCF.egg-info/dependency_links.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 14:12:10.000000 pertCF-0.1.6/pertCF.egg-info/requires.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 14:12:10.000000 pertCF-0.1.6/pertCF.egg-info/top_level.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 14:12:10.601424 pertCF-0.1.6/setup.cfg
--rw-r--r--   0 bbayrak    (501) staff       (20)      994 2023-07-03 14:11:18.000000 pertCF-0.1.6/setup.py
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:14:35.336959 pertCF-0.1.7/
+-rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.7/LICENSE.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 14:14:35.336799 pertCF-0.1.7/PKG-INFO
+-rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.7/README.md
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:14:35.335722 pertCF-0.1.7/pertCF/
+-rw-r--r--   0 bbayrak    (501) staff       (20)      964 2023-07-03 14:07:23.000000 pertCF-0.1.7/pertCF/Case.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     2278 2023-07-03 14:07:23.000000 pertCF-0.1.7/pertCF/Data.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     7216 2023-07-03 14:14:09.000000 pertCF-0.1.7/pertCF/PertCF.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     3995 2023-07-03 14:07:23.000000 pertCF-0.1.7/pertCF/Similarity.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)      260 2023-07-03 14:11:58.000000 pertCF-0.1.7/pertCF/__init__.py
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 14:14:35.336563 pertCF-0.1.7/pertCF.egg-info/
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 14:14:35.000000 pertCF-0.1.7/pertCF.egg-info/PKG-INFO
+-rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 14:14:35.000000 pertCF-0.1.7/pertCF.egg-info/SOURCES.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 14:14:35.000000 pertCF-0.1.7/pertCF.egg-info/dependency_links.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 14:14:35.000000 pertCF-0.1.7/pertCF.egg-info/requires.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 14:14:35.000000 pertCF-0.1.7/pertCF.egg-info/top_level.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 14:14:35.337011 pertCF-0.1.7/setup.cfg
+-rw-r--r--   0 bbayrak    (501) staff       (20)      994 2023-07-03 14:14:19.000000 pertCF-0.1.7/setup.py
```

### Comparing `pertCF-0.1.6/LICENSE.txt` & `pertCF-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.6/pertCF/Case.py` & `pertCF-0.1.7/pertCF/Case.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.6/pertCF/Data.py` & `pertCF-0.1.7/pertCF/Data.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.6/pertCF/PertCF.py` & `pertCF-0.1.7/pertCF/PertCF.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from scipy.special import softmax
-from Case import Case
-from Data import Data
-from Similarity import Similarity
+import Case
+import Data
+import Similarity
 import shap
 
 
 class PertCF:
     def __init__(self,
                  dataset,
                  label,
```

### Comparing `pertCF-0.1.6/pertCF/Similarity.py` & `pertCF-0.1.7/pertCF/Similarity.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.6/setup.py` & `pertCF-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 # with open('HISTORY.md') as history_file:
 #     HISTORY = history_file.read()
 #
 setup_args = dict(
     name='pertCF',
-    version='0.1.6',
+    version='0.1.7',
     description='PertCF explainer is a counterfactual based XAI technique.',
     # long_description_content_type="text/markdown",
     # long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Betül Bayrak',
     author_email='betul.bayrak@ntnu.no',
```


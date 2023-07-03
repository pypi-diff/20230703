# Comparing `tmp/creme-nn-0.1.0.tar.gz` & `tmp/creme-nn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/creme-nn-0.1.0.tar", last modified: Mon Jul  3 03:39:01 2023, max compression
+gzip compressed data, was "dist/creme-nn-0.1.1.tar", last modified: Mon Jul  3 19:29:52 2023, max compression
```

## Comparing `creme-nn-0.1.0.tar` & `creme-nn-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 03:39:01.524285 creme-nn-0.1.0/
--rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-03 03:39:01.523876 creme-nn-0.1.0/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     1135 2023-07-03 02:58:16.000000 creme-nn-0.1.0/README.md
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 03:39:01.522148 creme-nn-0.1.0/creme/
--rwxr-xr-x   0 peter      (501) staff       (20)        0 2023-06-21 13:18:10.000000 creme-nn-0.1.0/creme/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)    18586 2023-07-03 02:09:38.000000 creme-nn-0.1.0/creme/creme.py
--rw-r--r--   0 peter      (501) staff       (20)     4406 2023-07-03 01:23:19.000000 creme-nn-0.1.0/creme/custom_model.py
--rwxr-xr-x   0 peter      (501) staff       (20)     4580 2023-06-26 02:40:44.000000 creme-nn-0.1.0/creme/shuffle.py
--rw-r--r--   0 peter      (501) staff       (20)     4340 2023-07-03 01:28:26.000000 creme-nn-0.1.0/creme/utils.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 03:39:01.523371 creme-nn-0.1.0/creme_nn.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-03 03:39:01.000000 creme-nn-0.1.0/creme_nn.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      264 2023-07-03 03:39:01.000000 creme-nn-0.1.0/creme_nn.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2023-07-03 03:39:01.000000 creme-nn-0.1.0/creme_nn.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)       89 2023-07-03 03:39:01.000000 creme-nn-0.1.0/creme_nn.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)        6 2023-07-03 03:39:01.000000 creme-nn-0.1.0/creme_nn.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2023-07-03 03:39:01.524418 creme-nn-0.1.0/setup.cfg
--rw-r--r--   0 peter      (501) staff       (20)     1454 2023-07-03 03:32:22.000000 creme-nn-0.1.0/setup.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 19:29:52.232789 creme-nn-0.1.1/
+-rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-03 19:29:52.232500 creme-nn-0.1.1/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     1135 2023-07-03 02:58:16.000000 creme-nn-0.1.1/README.md
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 19:29:52.230173 creme-nn-0.1.1/creme/
+-rwxr-xr-x   0 peter      (501) staff       (20)        0 2023-06-21 13:18:10.000000 creme-nn-0.1.1/creme/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)    18592 2023-07-03 18:04:20.000000 creme-nn-0.1.1/creme/creme.py
+-rw-r--r--   0 peter      (501) staff       (20)     4406 2023-07-03 01:23:19.000000 creme-nn-0.1.1/creme/custom_model.py
+-rwxr-xr-x   0 peter      (501) staff       (20)     4580 2023-06-26 02:40:44.000000 creme-nn-0.1.1/creme/shuffle.py
+-rw-r--r--   0 peter      (501) staff       (20)     4340 2023-07-03 01:28:26.000000 creme-nn-0.1.1/creme/utils.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-07-03 19:29:52.232030 creme-nn-0.1.1/creme_nn.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)      778 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      264 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)       89 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)        6 2023-07-03 19:29:52.000000 creme-nn-0.1.1/creme_nn.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)       38 2023-07-03 19:29:52.232904 creme-nn-0.1.1/setup.cfg
+-rw-r--r--   0 peter      (501) staff       (20)     1385 2023-07-03 19:29:37.000000 creme-nn-0.1.1/setup.py
```

### Comparing `creme-nn-0.1.0/PKG-INFO` & `creme-nn-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creme-nn
-Version: 0.1.0
+Version: 0.1.1
 Summary: An in silico perturbation framework to interpret large-scale genomic deep learning
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `creme-nn-0.1.0/README.md` & `creme-nn-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `creme-nn-0.1.0/creme/creme.py` & `creme-nn-0.1.1/creme/creme.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,23 +496,23 @@
 ########################################################################################
 # Normalization functions
 ########################################################################################
 
 
 def context_effect_on_tss(pred_wt, pred_mut, bin_index=488):
     """Normalization based on difference between the effect size of the mutation and wt divided by wt"""
-    if (pred_mut.shape) == 1:
+    if len(pred_mut.shape) == 1:
         return (pred_wt[bin_index] - pred_mut[bin_index]) / pred_wt[bin_index]
     else:
         return (pred_wt[bin_index] - pred_mut[:,bin_index])/pred_wt[bin_index]
 
 
 def fold_change_over_control(pred_wt, pred_mut, bin_index=488):
     """Normalization based on difference between the effect size of the mutation and wt divided by wt"""
-    if (pred_mut.shape) == 1:
+    if len(pred_mut.shape) == 1:
         return pred_mut[bin_index] / pred_wt[bin_index]
     else:
         return pred_mut[:,bin_index] / pred_wt[bin_index]
 
 
 def normalized_tile_effect(pred_wt, pred_mut, pred_control, bin_index=488):
     """Normalization used for sufficiency test"""
```

### Comparing `creme-nn-0.1.0/creme/custom_model.py` & `creme-nn-0.1.1/creme/custom_model.py`

 * *Files identical despite different names*

### Comparing `creme-nn-0.1.0/creme/shuffle.py` & `creme-nn-0.1.1/creme/shuffle.py`

 * *Files identical despite different names*

### Comparing `creme-nn-0.1.0/creme/utils.py` & `creme-nn-0.1.1/creme/utils.py`

 * *Files identical despite different names*

### Comparing `creme-nn-0.1.0/creme_nn.egg-info/PKG-INFO` & `creme-nn-0.1.1/creme_nn.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creme-nn
-Version: 0.1.0
+Version: 0.1.1
 Summary: An in silico perturbation framework to interpret large-scale genomic deep learning
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `creme-nn-0.1.0/setup.py` & `creme-nn-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
 setup(
     name="creme-nn",
     # TODO: Consider using https://github.com/python-versioneer/python-versioneer to
     # get version information from git.
-    version="0.1.0",
+    version="0.1.1",
     description="An in silico perturbation framework to interpret large-scale genomic deep learning",
     # author='A. Random Developer',
     # author_email='author@example.com',
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```


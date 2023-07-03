# Comparing `tmp/pycroscopy-0.62.1.tar.gz` & `tmp/pycroscopy-0.63.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycroscopy-0.62.1.tar", last modified: Thu Nov 17 13:05:11 2022, max compression
+gzip compressed data, was "pycroscopy-0.63.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
```

## Comparing `pycroscopy-0.62.1.tar` & `pycroscopy-0.63.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.564084 pycroscopy-0.62.1/pycroscopy/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.564084 pycroscopy-0.62.1/pycroscopy/corr/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/corr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.564084 pycroscopy-0.62.1/pycroscopy/fft/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/fft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4708 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/fft/image_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.564084 pycroscopy-0.62.1/pycroscopy/image/
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7364 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/image_atoms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6220 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/image_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)    19448 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/image_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    10295 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/image_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/image_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    16510 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/image/image_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.564084 pycroscopy-0.62.1/pycroscopy/learn/
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/pycroscopy/learn/dl/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/dl/datautils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14644 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/dl/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6921 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/dl/nnblocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/dl/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/pycroscopy/learn/ml/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9529 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/ml/decompose.py
--rw-r--r--   0 runner    (1001) docker     (121)     7583 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/learn/ml/matrix_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/pycroscopy/signal/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/signal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/pycroscopy/stats/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19019 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/stats/atom_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/stats/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/pycroscopy/viz/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/pycroscopy/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:11.564084 pycroscopy-0.62.1/pycroscopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-11-17 13:05:11.000000 pycroscopy-0.62.1/pycroscopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-11-17 13:05:11.000000 pycroscopy-0.62.1/pycroscopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 13:05:11.000000 pycroscopy-0.62.1/pycroscopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-17 13:05:11.000000 pycroscopy-0.62.1/pycroscopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-17 13:05:11.000000 pycroscopy-0.62.1/pycroscopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-17 13:05:11.568084 pycroscopy-0.62.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-11-17 13:02:42.000000 pycroscopy-0.62.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.671388 pycroscopy-0.63.0/pycroscopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.671388 pycroscopy-0.63.0/pycroscopy/corr/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/corr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.675387 pycroscopy-0.63.0/pycroscopy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/fft/image_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.675387 pycroscopy-0.63.0/pycroscopy/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.675387 pycroscopy-0.63.0/pycroscopy/learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.679387 pycroscopy-0.63.0/pycroscopy/learn/dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/nnblocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.679387 pycroscopy-0.63.0/pycroscopy/learn/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/ml/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/ml/matrix_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.679387 pycroscopy-0.63.0/pycroscopy/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/signal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/pycroscopy/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/atom_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/atom_stats_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/pycroscopy/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.671388 pycroscopy-0.63.0/pycroscopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/setup.py
```

### Comparing `pycroscopy-0.62.1/LICENSE.txt` & `pycroscopy-0.63.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/PKG-INFO` & `pycroscopy-0.63.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycroscopy
-Version: 0.62.1
+Version: 0.63.0
 Summary: Python library for scientific analysis of microscopy data
 Home-page: https://pycroscopy.github.io/pycroscopy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: EELS,STEM,TEM,XRD,AFM,SPM,STS,band excitation,BE,BEPS,Raman,NanoIR,electron microscopy, scanning probe, x-rays,atomic force microscopy,SIMS,energy,spectroscopy,imaging,microscopy,spectracharacterization,spectrogram,hyperspectral,multidimensional,data format,universal,clustering,decomposition,curve fitting,data analysis,PCA, SVD, NMF, DBSCAN, kMeans,machine learning,bayesian inference,fft filtering,signal processing,image cleaning,denoising,model,msa,quantification
 Platform: Linux
@@ -39,28 +39,34 @@
     :target: https://github.com/pycroscopy/pycroscopy/actions?query=workflow%3Abuild
     :alt: GitHub Actions
     
 .. image:: https://img.shields.io/pypi/v/pycroscopy.svg
     :target: https://pypi.org/project/pyCroscopy/
     :alt: PyPI
     
+.. image:: https://codecov.io/gh/pycroscopy/pycroscopy/branch/main/graph/badge.svg?token=HXGZMKzJqb
+    :target: https://codecov.io/gh/pycroscopy/pycroscopy
+    :alt: coverage
+    
 .. image:: https://img.shields.io/conda/vn/conda-forge/pycroscopy.svg
     :target: https://github.com/conda-forge/pycroscopy-feedstock
     :alt: conda-forge
 
 .. image:: https://img.shields.io/pypi/l/pycroscopy.svg
     :target: https://pypi.org/project/pyCroscopy/
     :alt: License
     
 .. image:: https://zenodo.org/badge/61456133.svg
    :target: https://zenodo.org/badge/latestdoi/61456133
    :alt: DOI
+   
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+   :target: https://colab.research.google.com/github/pycroscopy/pycroscopy/blob/main/jupyter_notebooks/Intro_to_Pycroscopy.ipynb
+   :alt: Notebook
 
-**NOTE: Pycroscopy is undergoing a major reorganization and change to the scope and nature of the package. For those interested in the older version, please visit the legacy branch. The new version is under development in the 'phoenix' branch, and this is now the default branch.**
-
-pycroscopy is a `python <http://www.python.org/>`_ package for image processing and scientific analysis of imaging modalities such as multi-frequency scanning probe microscopy, scanning tunneling spectroscopy, x-ray diffraction microscopy, and transmission electron microscopy. pycroscopy uses a data-centric model wherein the raw data collected from the microscope, results from analysis and processing routines are all written to standardized hierarchical data format (HDF5) files for traceability, reproducibility, and provenance.
+pycroscopy is a `python <http://www.python.org/>`_ package for generic (domain-agnostic) microscopy data anlaysis. More specialized or domain-specific analysis routines are contained within some of the other packages within the pycroscopy ecosystem.
 
 Please visit our `homepage <https://pycroscopy.github.io/pycroscopy/about.html>`_ for more information and installation instructions.
 
 If you use pycroscopy for research, we would appreciate if you could cite our `Arxiv paper <https://arxiv.org/abs/1903.09515>`_ titled "USID and Pycroscopy - Open frameworks for storing and analyzing spectroscopic and imaging data"
```

### Comparing `pycroscopy-0.62.1/README.rst` & `pycroscopy-0.63.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,26 +10,32 @@
     :target: https://github.com/pycroscopy/pycroscopy/actions?query=workflow%3Abuild
     :alt: GitHub Actions
     
 .. image:: https://img.shields.io/pypi/v/pycroscopy.svg
     :target: https://pypi.org/project/pyCroscopy/
     :alt: PyPI
     
+.. image:: https://codecov.io/gh/pycroscopy/pycroscopy/branch/main/graph/badge.svg?token=HXGZMKzJqb
+    :target: https://codecov.io/gh/pycroscopy/pycroscopy
+    :alt: coverage
+    
 .. image:: https://img.shields.io/conda/vn/conda-forge/pycroscopy.svg
     :target: https://github.com/conda-forge/pycroscopy-feedstock
     :alt: conda-forge
 
 .. image:: https://img.shields.io/pypi/l/pycroscopy.svg
     :target: https://pypi.org/project/pyCroscopy/
     :alt: License
     
 .. image:: https://zenodo.org/badge/61456133.svg
    :target: https://zenodo.org/badge/latestdoi/61456133
    :alt: DOI
+   
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+   :target: https://colab.research.google.com/github/pycroscopy/pycroscopy/blob/main/jupyter_notebooks/Intro_to_Pycroscopy.ipynb
+   :alt: Notebook
 
-**NOTE: Pycroscopy is undergoing a major reorganization and change to the scope and nature of the package. For those interested in the older version, please visit the legacy branch. The new version is under development in the 'phoenix' branch, and this is now the default branch.**
-
-pycroscopy is a `python <http://www.python.org/>`_ package for image processing and scientific analysis of imaging modalities such as multi-frequency scanning probe microscopy, scanning tunneling spectroscopy, x-ray diffraction microscopy, and transmission electron microscopy. pycroscopy uses a data-centric model wherein the raw data collected from the microscope, results from analysis and processing routines are all written to standardized hierarchical data format (HDF5) files for traceability, reproducibility, and provenance.
+pycroscopy is a `python <http://www.python.org/>`_ package for generic (domain-agnostic) microscopy data anlaysis. More specialized or domain-specific analysis routines are contained within some of the other packages within the pycroscopy ecosystem.
 
 Please visit our `homepage <https://pycroscopy.github.io/pycroscopy/about.html>`_ for more information and installation instructions.
 
 If you use pycroscopy for research, we would appreciate if you could cite our `Arxiv paper <https://arxiv.org/abs/1903.09515>`_ titled "USID and Pycroscopy - Open frameworks for storing and analyzing spectroscopic and imaging data"
```

### Comparing `pycroscopy-0.62.1/pycroscopy/__init__.py` & `pycroscopy-0.63.0/pycroscopy/__init__.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/fft/image_fft.py` & `pycroscopy-0.63.0/pycroscopy/fft/image_fft.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/image/__init__.py` & `pycroscopy-0.63.0/pycroscopy/image/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 Submodules
 ----------
 .. autosummary::
     :toctree: _autosummary
 
 """
-
+ 
 from .image_window import ImageWindowing
-
-from .image_utilities import crop_image
+from .image_utilities import crop_image, flatten_image
 from .image_clean import decon_lr, clean_svd
 from .image_atoms import find_atoms, atom_refine
 from .image_graph import make_structural_units, find_structural_units, get_polygons, add_graph
 from .image_registration import complete_registration, rigid_registration, demon_registration
 
 __all__ = ['ImageWindowing', 'crop_image', 'decon_lr', 'clean_svd', 'find_atoms', 'atom_refine', 
            'make_structural_units', 'find_structural_units', 'get_polygons', 'add_graph',
-           'complete_registration', 'demon_registration', 'rigid_registration']
+           'complete_registration', 'demon_registration', 'rigid_registration',
+           'flatten_image']
```

### Comparing `pycroscopy-0.62.1/pycroscopy/image/image_atoms.py` & `pycroscopy-0.63.0/pycroscopy/image/image_atoms.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/image/image_clean.py` & `pycroscopy-0.63.0/pycroscopy/image/image_clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
         raise TypeError('We need a sidpy.Dataset')
     if im.data_type.name != 'IMAGE':
         raise TypeError('We need sidpy.Dataset of sidpy.Datatype: IMAGE')
 
     patch_size = int(source_size/pixel_size)
     if patch_size < 3:
         patch_size = 3
-    patches = image.extract_patches_2d(im, (patch_size, patch_size))
+    
+    patches = image.extract_patches_2d(np.array(im), (patch_size, patch_size))
     patches = patches.reshape(patches.shape[0], patches.shape[1]*patches.shape[2])
 
     num_components = 32
 
     u, s, v = randomized_svd(patches, num_components)
     u_im_size = int(np.sqrt(u.shape[0]))
     reduced_image = u[:, 0].reshape(u_im_size, u_im_size)
```

### Comparing `pycroscopy-0.62.1/pycroscopy/image/image_graph.py` & `pycroscopy-0.63.0/pycroscopy/image/image_graph.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/image/image_registration.py` & `pycroscopy-0.63.0/pycroscopy/image/image_registration.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/image/image_window.py` & `pycroscopy-0.63.0/pycroscopy/image/image_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         ----------
         - parms_dict : dictionary
             Dictionary with parameters of the windowing process, see below.
 
             Keys:
             - 'window_size_x' (integer) (required): size of the window across the x-axis
             - 'window_size_y' (integer) (required): size of the window across the y-axis
-            - 'window_step_x' (integer) (required): step size of the window across the x-axis. Sometimes referred to as 'strides'
-            - 'window_step_y' (integer) (required): step size of the window across the y-axis. Sometimes referred to as 'strides'
+            - 'window_step_x' (integer) (required): step size of the window across the x-axis. Must divide into the image size in the x axis
+            - 'window_step_y' (integer) (required): step size of the window across the y-axis. Must divide into the image size in the y axis
             - 'mode' (string) (Optional, default is 'image'): One of 'image' or 'fft' which defines the processing to be performed for each window.
                 The choice of 'fft' will perform 2D fast Fourier transforms on each image whereas 'image' will not perform any operation on the window
             - 'fft_mode' (string) (Optional, default is 'abs'): If mode is 'fft', choose whether to look at amplitude or phase. Options are 'abs', 'phase' and 'complex'.
             - 'interpol_factor' (float) (Optional, default is 1.0): Interpolation factor for windows to increase or decrease size of the windows.
             - 'zoom_factor' (integer or list of ints) (Optional, default is 1): Zoom the window by this factor, typically done for 'fft' mode to observe higher frequencies clearly
                             If passing a list of ints, this will determine the degree of cropping per axis
             - 'filter' (string) (Optional, default is None): Filtering to use for the image window. Options are 'blackman', 'hamming'.
@@ -97,30 +97,71 @@
             else:
                 self.fft_mode = 'abs' #default to absolute value in case fft mode is not provided
                 parms_dict['fft_mode'] = 'abs'
         if self.verbose:
             print('ImageWindowing Object created with parameters {}'.format(parms_dict))
 
         self.window_parms = parms_dict
-
+        self.window_dataset = None
         return
 
     def _get_window_size(self):
         '''
         Computes window size based on zoom and interpolation factors
         '''
 
         image_test = np.random.uniform(size=(self.window_size_x, self.window_size_y))
-        #print('image test is shape {}'.format(image_test.shape))
         image_zoomed = self.zoom(image_test, self.zoom_factor)
-        #print('image zoomed is shape {}'.format(image_zoomed.shape))
+
         #interpolate it
         zoomed_interpolated = rescale(image_zoomed, self.interpol_factor)
-        #print('image zoomed interpol is shape {}'.format(zoomed_interpolated.shape))
         return zoomed_interpolated.shape[0],zoomed_interpolated.shape[1]
+    
+    def do_PCA_window_cleaning(self, num_comps = None):
+        """
+        This function performs PCA cleaning
+        Inputs: 
+            - num_comps: (int) (Default = None). Number of components to keep in reconstruction. 
+            By default, num_comps is 0.5*(window_size_x * window_size_y)
+        """
+        #Here we assume that the windowing has been done
+
+        if self.window_dataset is None:
+            raise ValueError("Windowing has not been done. Please perform windowing first before calling this function")
+
+        assert self.window_size_x == self.window_size_final_x, "Cannot use zoom and interpolation for PCA image cleaning, rerun without these"
+        assert self.window_size_y == self.window_size_final_y, "Cannot use zoom and interpolation for PCA image cleaning, rerun without these"
+        
+        windows_2d = self.window_dataset.fold(method='spaspec')
+        u, s, vh = np.linalg.svd(np.array(windows_2d), full_matrices=False )
+        
+        if num_comps is None:
+            num_comps = len(s)//2 #choose half the components as default
+        
+        s[num_comps:] = 0
+
+        recon = np.dot(u * s, vh)
+        recon_4d = recon.reshape(self.window_dataset.shape)
+
+        recon_image = np.zeros(self.image_shape)
+        window_size = [self.window_size_final_x, self.window_size_final_y]
+        m=0
+        for xind in range(recon_4d.shape[0]):
+            for yind in range(recon_4d.shape[1]):
+                cur_slice = recon_4d[xind,yind,:,:]
+                pos =self.pos_vec[m]
+                start_stop = [slice(x, x + y, 1) for x, y in zip(pos, window_size)]
+                recon_image[tuple(start_stop)] = cur_slice
+                m+=1
+
+        self.recon_image = recon_image
+        
+        #TODO: Need to return as a sidpy dataset
+
+        return recon_image
 
     def MakeWindows(self, dataset, dim_slice=None):
         '''
             Image should be a sidpy dataset object
             We will take the image to be the first two spatial dimensions,
             unless dimensions are specified
 
@@ -165,28 +206,39 @@
 
         if self.verbose:
             print('Full image shape is {}'.format(self.image_shape))
 
         window_step = [self.window_step_x, self.window_step_y]
         window_size = [self.window_size_x, self.window_size_y]
         window_size_final = [self.window_size_final_x, self.window_size_final_y]
+        #division_factor_x = self.window_size_x - self.window_step_x
+        #division_factor_y = self.window_size_y - self.window_step_y
+        if self.window_size_x == self.window_step_x: division_factor_x = self.window_size_x
+        if self.window_size_y == self.window_step_y: division_factor_y = self.window_size_y
+        
+        #assert np.mod(self.image_shape[0] - self.window_size_x, self.window_step_x) ==0, "Image shape along y is {} but window size is {}, window step is ({}) are not divisible \
+        #without remainder, change your window size or window step".format(self.image_shape[0], self.window_size_x, self.window_step_x)
+        #assert np.mod(self.image_shape[1] - self.window_size_y, self.window_step_y) ==0, "Image shape along x is {} but window size is {}, and window step is ({}) are not divisible \
+        #without remainder, change your window size or window step".format(self.image_shape[1], self.window_size_y, self.window_step_y)
 
         dim_vec = []
         for i in range(2):
             dim_vec.append(np.arange(0, self.image_shape[i] - window_size[i], window_step[i]))
+            dim_vec[i] = np.append(dim_vec[i], self.image_shape[i] - window_size[i])
 
         if self.verbose:
             print("dim vec is {}".format(dim_vec))
 
         _, pos_vec = build_ind_val_matrices(dim_vec)
         if self.verbose:
             print("Pos vec is {}".format(pos_vec))
 
         pca_mat = np.zeros(shape=(pos_vec.shape[0], np.prod(window_size_final)), dtype=np.complex64)
         pos_vec = np.int32(pos_vec)
+        self.pos_vec = pos_vec
 
         def make_windows_parallel(ind, pos):
             start_stop = [slice(x, x + y, 1) for x, y in zip(pos, window_size)]
             full_slice = image_source[tuple(start_stop)]
             full_slice = self._return_win_image_processed(full_slice)
             full_slice_flat = full_slice.flatten()
             return full_slice_flat
@@ -275,22 +327,23 @@
         data_set.set_dimension(3, sidpy.Dimension(z_dimy,
                                                   name='WindowY',
                                                   units=window_units, quantity='ky',
                                                   dimension_type='spectral'))
 
         # append metadata
         data_set.metadata = self._merge_dictionaries(dataset.metadata, self.window_parms)
-
+        self.window_dataset = data_set
         return data_set
 
     def _return_win_image_processed(self, img_window):
         #Real image slice, returns it back with image processed
 
 
         if self.mode == 'fft': # Apply FFT if needed
+            img_window = np.array(img_window)
             img_window = np.fft.fftshift(np.fft.fft2(img_window))
             if self.fft_mode == 'amp':
                 img_window = np.abs(img_window,)
             elif self.fft_mode == 'phase':
                 img_window = np.angle(img_window)
             elif self.fft_mode == 'complex':
                 img_window = np.array(img_window, dtype = np.complex64)
@@ -340,23 +393,25 @@
             imag_img = np.imag(img_window)
             real_img_scaled = rescale(real_img, interpol_factor)
             imag_img_scaled = rescale(imag_img, interpol_factor)
             complex_rescaled_image = real_img_scaled + 1j*imag_img_scaled
             
         return complex_rescaled_image
 
+    #
+    '''
     def clean_image(self, n_comps = 4):
         self.mode = 'image'
         self.interpol_factor = 1
         self.zoom_factor = 1
         self.window_size_final_x = self.window_size_x
         self.window_size_final_y = self.window_size_y
         new_windows = self.MakeWindows(self.dataset)
         
         from ..learn.ml import MatrixFactor
         svd_results = MatrixFactor(new_windows, method='svd', n_components = n_comps)
 
-        return svd_results
+        return svd_results'''
```

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/__init__.py` & `pycroscopy-0.63.0/pycroscopy/learn/__init__.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/dl/datautils.py` & `pycroscopy-0.63.0/pycroscopy/learn/dl/datautils.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/dl/models.py` & `pycroscopy-0.63.0/pycroscopy/learn/dl/models.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/dl/nnblocks.py` & `pycroscopy-0.63.0/pycroscopy/learn/dl/nnblocks.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/dl/trainer.py` & `pycroscopy-0.63.0/pycroscopy/learn/dl/trainer.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/ml/decompose.py` & `pycroscopy-0.63.0/pycroscopy/learn/ml/decompose.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy/learn/ml/matrix_factor.py` & `pycroscopy-0.63.0/pycroscopy/learn/ml/matrix_factor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Note that matrix factorization can only operate on 2D matrices. So we will automatically reshape
 # all datasets to be two dimensional (spatial v spectral)
 import sidpy
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.decomposition import NMF, PCA, FastICA, KernelPCA
 from pysptools.eea import nfindr
+import pysptools.abundance_maps as amp
 
 
 class MatrixFactor:
     def __init__(self, data, method='nmf', n_components=2, return_fit=False,
                  ) -> None:
         """
         Parameters:
@@ -62,15 +63,16 @@
         Parameters:
         (none)
 
         Returns: 
         Sidpy dataset after fit operation. Fit will calculate according to the method chosen.
 
         """
-
+        abundances, components = None, None
+        
         if self.method == 'svd':
             u, s, vh = np.linalg.svd(np.array(self.data_2d), full_matrices=False, compute_uv=True)
             abundances, components = None, None
             # abundances = u  # check...
             # components = (s * v.T).T  # check again
         elif self.method == 'nmf':
             # code goes here...
@@ -86,14 +88,22 @@
             abundances = ica.fit_transform(np.array(self.data_2d))
             components = ica.components_
         elif self.method == 'kernelpca':
             kpca = KernelPCA(n_components=self.ncomp, **kwargs)
             X_kpca = kpca.fit(np.array(self.data_2d).T)
             abundances = X_kpca.fit_transform(np.array(self.data_2d))
             components = X_kpca.eigenvectors_.T
+        elif self.method == 'nfindr':
+            nnls = amp.FCLS()
+            a1 = nfindr.NFINDR(np.array(self.data_2d), self.ncomp)  # Find endmembers
+            components = a1[0]
+            data_spec_fold = self.data.fold(method='spec')  # This will fold all the spectral dimensions into 1
+            data_amap = np.array(data_spec_fold)
+            abundances = nnls.map(data_amap, components)  # Finding abundances
+            abundances = abundances.reshape(-1, self.ncomp)
 
         if abundances is None and components is None:
 
             self.u = sidpy.Dataset.from_array(u, title='U')
 
             # We might want to write an unfolding command for s and vh
             self.s = sidpy.Dataset.from_array(s, title='singular values(s)')
@@ -105,15 +115,17 @@
                 return self.u, self.s, self.vh, self.fit_dset
             else:
                 return self.u, self.s, self.vh
         else:
             # Getting the fit dataset i.e., abundances*components and unfolding it into the original shape
             self.fit_dset = self.data_2d.like_data(np.matmul(abundances, components),
                                                    title_suffix='_factorized').unfold()
-
+            self.abundances = abundances
+            self.components = components
+            
             # Now we need to prepare an abundance dataset and a component dataset and make sure their spatial dimensions
             # are unfolded
             abundances_dset = self.data_2d.like_data(abundances, title='abundances',
                                                      check_dims=False)
             # Image stack
             # We will delete this for now and add this back manually
             del abundances_dset.metadata['fold_attr']
@@ -155,12 +167,13 @@
             # We should return a list of sidpy dataset objects
             self.abundances = abundances_dset.unfold()
             self.abundances.data_type = sidpy.DataType.IMAGE_STACK
 
             self.components = components_dset.unfold()
             self.components.data_type = sidpy.DataType.LINE_PLOT_FAMILY  # Check this again
             self.results_computed = True
+            
 
             if self.return_fit:
                 return self.abundances, self.components, self.fit_dset
             else:
                 return self.abundances, self.components
```

### Comparing `pycroscopy-0.62.1/pycroscopy/stats/atom_stats.py` & `pycroscopy-0.63.0/pycroscopy/stats/atom_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.neighbors import NearestNeighbors
 from sklearn.cluster import KMeans
 import scipy.optimize as opt
 from copy import deepcopy
 from sklearn.mixture import GaussianMixture as GM
 
-#simple helper function for intersecting lists
-def intersection(list1, list2): 
-    list_intersected = [value for value in list1 if value in list2] 
+
+# simple helper function for intersecting lists
+def intersection(list1, list2):
+    list_intersected = [value for value in list1 if value in list2]
     return list_intersected
 
+
 class LocalCrystallography:
-    def __init__(self, image_source, atom_positions, atom_descriptors = dict(), 
-                 window_size = 25, atom_types = None, border = 0.03, 
-                 image_name = '', comp = 0, **kwargs):
+    def __init__(self, image_source, atom_positions, atom_descriptors=dict(),
+                 window_size=25, atom_types=None, border=0.03,
+                 image_name='', comp=0, **kwargs):
         """
         Parameters
         ----------
         image_source
             Image from which N atoms or objects are derived
         atom_positions
             Positions of the objects/atoms as an (N,2) array
@@ -34,158 +35,154 @@
         image_name
             Name of the image, default is blank
         comp
             Composition of the sample (optional)
 
             """
 
-        
-        self.image_source = image_source #source dataset
-        self.image_name = image_name#text list of name of file
-        self.atom_positions = atom_positions #atomic positions as an Nx2 array
+        self.image_source = image_source  # source dataset
+        self.image_name = image_name  # text list of name of file
+        self.atom_positions = atom_positions  # atomic positions as an Nx2 array
         self.num_atoms = len(self.atom_positions)
-        self.atom_types = atom_types #Pass a vector of length num_atoms with index of atom type, if system has multiple types of atoms
+        # Pass a vector of length num_atoms with index of atom type, if system has
+        # multiple types of atoms
+        self.atom_types = atom_types
         if atom_types is None: self.atom_types = np.zeros(self.num_atoms)
         self.atom_descriptors = atom_descriptors
         self.neighbor_indices = None
         self.image_size_x, self.image_size_y = self.image_source.shape
-        self.window_size = window_size #size of window, roughly equal to lattice parameter in pixels
-        self.border = border #border is percentage of width to chop off
-        self.determine_border_indices(border = border)
+        self.window_size = window_size  # size of window, roughly equal to lattice parameter in pixels
+        self.border = border  # border is percentage of width to chop off
+        self.determine_border_indices(border=border)
         self.neighborhood_results = None
-        self.comp = comp #composition, usually this is the amount of atom B in the binary mixture.
-        
+        self.comp = comp  # composition, usually this is the amount of atom B in the binary mixture.
+
     def determine_border_indices(self, border=0.03):
         '''This will find the index of all the non-border and border atoms so it will not screw up
         the local crystallography analysis. Basically we find atoms nearest the edge and then move the 
         border*image_size px in, and if the atom is caught in that space, it gets marked as a border px'''
-        
+
         border_pixel_ind = []
         nonborder_pixel_ind = []
-        
-        xlims = [border*self.image_source.shape[1], self.image_source.shape[1]-border*self.image_source.shape[1]]
-        ylims = [border*self.image_source.shape[0], self.image_source.shape[1]-border*self.image_source.shape[0]]
-        
-        #print(xlims, ylims)
-        
+
+        xlims = [border * self.image_source.shape[1], self.image_source.shape[1] - border * self.image_source.shape[1]]
+        ylims = [border * self.image_source.shape[0], self.image_source.shape[1] - border * self.image_source.shape[0]]
+
+        # print(xlims, ylims)
+
         for ind in range(len(self.atom_positions)):
-            
-            x,y = self.atom_positions[ind,1], self.atom_positions[ind,0]
-            
-            if x>xlims[0] and x<xlims[1] and y>ylims[0] and y<ylims[1]:
+
+            x, y = self.atom_positions[ind, 1], self.atom_positions[ind, 0]
+
+            if x > xlims[0] and x < xlims[1] and y > ylims[0] and y < ylims[1]:
                 nonborder_pixel_ind.append(ind)
             else:
                 border_pixel_ind.append(ind)
-                
+
         self.border_pixel_inds = border_pixel_ind
         self.nonborder_pixel_inds = nonborder_pixel_ind
-        
+
         return
-        
-        
+
     def refine_atomic_positions(self):
-        #This will refine the given atomic positions
+        # This will refine the given atomic positions
         # Create fitting space
-       
-        
-        x_vec = np.linspace(-self.window_size/2, self.window_size/2, self.window_size)
-        y_vec = np.linspace(-self.window_size/2, self.window_size/2, self.window_size)
-        
+
+        x_vec = np.linspace(-self.window_size / 2, self.window_size / 2, self.window_size)
+        y_vec = np.linspace(-self.window_size / 2, self.window_size / 2, self.window_size)
+
         x_mat, y_mat = np.meshgrid(x_vec, y_vec)
-       
-        #print(x_mat.shape)
 
-        atomic_positions_corrections = np.zeros(self.atom_positions.shape, dtype = np.float32)
+        # print(x_mat.shape)
+
+        atomic_positions_corrections = np.zeros(self.atom_positions.shape, dtype=np.float32)
         num_atoms = self.atom_positions.shape[0]
-        
+
         # do a fit of each atom using a gaussian
         opt_fits = []
-        for k1 in range(0,num_atoms):
-            
-            ax = self.atom_positions[k1,0]
-            ay = self.atom_positions[k1,1]
-            t1 = int((ax>self.window_size)) 
-            t2 = int(ax<(self.image_size_x-self.window_size))
-            t3 = int((ay>self.window_size)) 
-            t4 = int(ay<(self.image_size_y-self.window_size))
+        for k1 in range(0, num_atoms):
 
-            if (t1+t2+t3+t4)==4:
-                
-                ROI =  self.image_source[int(ay-self.window_size/2):int(ay+self.window_size/2),
-                                    int(ax-self.window_size/2):int(ax+self.window_size/2)]
-                amp_guess = ROI[int(self.window_size/2),int(self.window_size/2)]
-                
+            ax = self.atom_positions[k1, 0]
+            ay = self.atom_positions[k1, 1]
+            t1 = int((ax > self.window_size))
+            t2 = int(ax < (self.image_size_x - self.window_size))
+            t3 = int((ay > self.window_size))
+            t4 = int(ay < (self.image_size_y - self.window_size))
+
+            if (t1 + t2 + t3 + t4) == 4:
+
+                ROI = self.image_source[int(ay - self.window_size / 2):int(ay + self.window_size / 2),
+                      int(ax - self.window_size / 2):int(ax + self.window_size / 2)]
+                amp_guess = ROI[int(self.window_size / 2), int(self.window_size / 2)]
 
                 initial_guess = (amp_guess, 0.1, 0.1, 2., 2., 0.001)
                 guess = self.gauss_oval_2D((x_mat, y_mat), *initial_guess)
-                    
-                guess_surface = guess.reshape(self.window_size,self.window_size)
-                
+
+                guess_surface = guess.reshape(self.window_size, self.window_size)
+
                 try:
                     popt, pcov = opt.curve_fit(self.gauss_oval_2D, (x_mat, y_mat), ROI.ravel(), p0=initial_guess)
-                        
+
                 except RuntimeError:
 
-                    popt=guess
-                    pcov=[np.nan, np.nan, np.nan, np.nan, np.nan]
+                    popt = guess
+                    pcov = [np.nan, np.nan, np.nan, np.nan, np.nan]
                     print('Failed Fit')
-                    
+
                 # need to make sure x and y are correct
                 if ~np.isnan(popt[1]) and ~np.isnan(popt[2]):
 
-                    atomic_positions_corrections[k1,0] = popt[1]
-                    atomic_positions_corrections[k1,1] = popt[2]
+                    atomic_positions_corrections[k1, 0] = popt[1]
+                    atomic_positions_corrections[k1, 1] = popt[2]
                 else:
-                    atomic_positions_corrections[k1,0] = 0.0
-                    atomic_positions_corrections[k1,1] = 0.0
-                opt_fits.append((popt,pcov))
-        
-        
+                    atomic_positions_corrections[k1, 0] = 0.0
+                    atomic_positions_corrections[k1, 1] = 0.0
+                opt_fits.append((popt, pcov))
+
         atomic_positions_corrected = self.atom_positions + atomic_positions_corrections
         self.atom_positions = atomic_positions_corrected
         self.corrections = atomic_positions_corrections
 
-        return atomic_positions_corrected , opt_fits
-    
-    @staticmethod 
+        return atomic_positions_corrected, opt_fits
+
+    @staticmethod
     def gauss_oval_2D(fitting_space, amplitude, xo, yo, sigmax, sigmay, offset):
         x = fitting_space[0]
         y = fitting_space[1]
         xo = float(xo)
-        yo = float(yo)    
-        g = amplitude*np.exp(-((x-xo)**2/(2*sigmax**2) + ((y-yo)**2 /(2*sigmay**2))));
+        yo = float(yo)
+        g = amplitude * np.exp(-((x - xo) ** 2 / (2 * sigmax ** 2) + ((y - yo) ** 2 / (2 * sigmay ** 2))));
 
         return g.ravel() + offset
-                            
 
-    def compute_neighborhood_indices (self, num_neighbors = 8):
+    def compute_neighborhood_indices(self, num_neighbors=8):
         '''
         Computes the local neighbors, returning the indices for each atom
         
         Input: - num_neighbors (int) (Default = 8): Number of neighbors
         
         Output: (None), results are stored as matrix of size (num_atoms, num_neighbors) in neighbor_indices.
         '''
-        
-        #finds indices of the neighbors
-        nbrs = NearestNeighbors(n_neighbors=num_neighbors+1, algorithm='brute').fit(self.atom_positions)
+
+        # finds indices of the neighbors
+        nbrs = NearestNeighbors(n_neighbors=num_neighbors + 1, algorithm='brute').fit(self.atom_positions)
         distance_vec, full_index = nbrs.kneighbors(self.atom_positions)
-        self.neighbor_indices = full_index #matrix of size (num_atoms, num_neighbors) with indices of neighbors
-        #Once we have the neighbor indices, we should also just write an array of the atom types by neighbor as this will be needed for local analysis down the line!
-        
+        self.neighbor_indices = full_index  # matrix of size (num_atoms, num_neighbors) with indices of neighbors
+        # Once we have the neighbor indices, we should also just write an array of the atom types by neighbor as this will be needed for local analysis down the line!
+
         neighbor_types_mat = []
         for ind in range(self.neighbor_indices.shape[0]):
-            n_indices = self.neighbor_indices[ind,:]
+            n_indices = self.neighbor_indices[ind, :]
             neighbor_types_mat.append(self.atom_types[n_indices])
-       
+
         self.neighborhood_atom_types = np.array(neighbor_types_mat)
-        
-        return 
-    
-    def compute_neighborhood (self, num_neighbors=8, atom_type = None):
+
+        return
+
+    def compute_neighborhood(self, num_neighbors=8, atom_type=None):
         '''
         Computes the distance and angle to local neighbors.
         
         Inputs: -num_neighbors (int) (default = 8): Number of neighbors
                 - atom_type: (int or str of key in atom_descriptors) (Default = None
                 ). If provided, neighborhood will be computed for the atom type given
                 If none, then atom types will be ignored.
@@ -193,245 +190,244 @@
         Output: None, but a dictionary of results is stored as neighborhood_results
         
         Note that the border pixels will be ignored in the neighborhood calculation.
         It is also reccomended to run compute_neighborhood_indices before this, but it will 
         run anyway if it has not already.
         
         '''
-     
-        if self.neighbor_indices is None: 
+
+        if self.neighbor_indices is None:
             self.compute_neighborhood_indices(num_neighbors)
         else:
-            if self.neighbor_indices.shape[-1] != num_neighbors+1:
+            if self.neighbor_indices.shape[-1] != num_neighbors + 1:
                 print('Warning - number of neighbors given to this function differs ' + \
                       'from previously computed, will recompute with {} neighbors'.format(num_neighbors))
-                
+
                 self.compute_neighborhood_indices(num_neighbors)
-        
-        
-            
-        if atom_type is not None: 
-            if type(atom_type=='str'): atom_type = self.atom_descriptors[atom_type]
-            #num_atoms = len(self.atom_types==atom_type)
+
+        if atom_type is not None:
+            if type(atom_type == 'str'): atom_type = self.atom_descriptors[atom_type]
+            # num_atoms = len(self.atom_types==atom_type)
             num_atoms = len(self.atom_types)
         else:
             atom_type = 0
-            
+
         atom_types = self.atom_types
         num_atoms = self.num_atoms
-        
-        d_vec = np.zeros((1,num_neighbors),dtype=float)
+
+        d_vec = np.zeros((1, num_neighbors), dtype=float)
         a_vec = d_vec.copy()
         xd_vec = d_vec.copy()
         yd_vec = d_vec.copy()
-        d_mat = np.zeros((num_atoms,num_neighbors),dtype=float)
+        d_mat = np.zeros((num_atoms, num_neighbors), dtype=float)
         a_mat = d_mat.copy()
         xd_mat = d_mat.copy()
         yd_mat = d_mat.copy()
-        atom_neighbor_pos = np.zeros((num_atoms,num_neighbors,2))
-        
-        #build a matrix of measurements from each atom to its nearest neighbors
-        for k1 in range(0,num_atoms):
-            
-            #compute it only if the atom is a nonborder atom
+        atom_neighbor_pos = np.zeros((num_atoms, num_neighbors, 2))
+
+        # build a matrix of measurements from each atom to its nearest neighbors
+        for k1 in range(0, num_atoms):
+
+            # compute it only if the atom is a nonborder atom
             if k1 in self.nonborder_pixel_inds:
-                
-                #Finally, compute only if the atom type matches
-                if atom_types[k1]==atom_type:
-                    
-                    x0 = self.atom_positions[k1,0]
-                    y0 = self.atom_positions[k1,1]
-
-                    if ((int(x0==0)+int(y0==0))==0):
-
-                        for k2 in range(0,num_neighbors):            
-                            x1 = self.atom_positions[self.neighbor_indices[k1,k2+1],0]
-                            y1 = self.atom_positions[self.neighbor_indices[k1,k2+1],1]
-                            d_vec[0,k2] = np.abs((x0-x1)+1j*(y0-y1)) #array of distances from each atom to its nearest neighbors
-                            a_vec[0,k2] = np.angle((x0-x1)+1j*(y0-y1)) #array of angles from each atom to its nearest neighbors
-                            xd_vec[0,k2] = (x0-x1)
-                            yd_vec[0,k2] = (y0-y1)
-                            atom_neighbor_pos[k1,k2,:] =[x1,y1] 
-
-                        # sort neighbors based on angle
-                        sort_ind = np.argsort(a_vec[0,:],axis=None)
-                        d_mat[k1,:] = d_vec[0,sort_ind]
-                        a_mat[k1,:] = a_vec[0,sort_ind]
-                        xd_mat[k1,:] = xd_vec[0,sort_ind]
-                        yd_mat[k1,:] = yd_vec[0,sort_ind]
-
-        neighborhood_results = {'distance_mat':d_mat, 'angles_mat':a_mat,
-                                        'xdistance_mat':xd_mat, 'ydistance_mat':yd_mat, 
-                                         'atom_neighbor_positions': atom_neighbor_pos,
-                                    'atom_type':atom_type}
-        
+
+                # Finally, compute only if the atom type matches
+                if atom_types[k1] == atom_type:
+
+                    x0 = self.atom_positions[k1, 0]
+                    y0 = self.atom_positions[k1, 1]
+
+                    if ((int(x0 == 0) + int(y0 == 0)) == 0):
+
+                        for k2 in range(0, num_neighbors):
+                            x1 = self.atom_positions[self.neighbor_indices[k1, k2 + 1], 0]
+                            y1 = self.atom_positions[self.neighbor_indices[k1, k2 + 1], 1]
+                            d_vec[0, k2] = np.abs((x0 - x1) + 1j * (
+                                        y0 - y1))  # array of distances from each atom to its nearest neighbors
+                            a_vec[0, k2] = np.angle(
+                                (x0 - x1) + 1j * (y0 - y1))  # array of angles from each atom to its nearest neighbors
+                            xd_vec[0, k2] = (x0 - x1)
+                            yd_vec[0, k2] = (y0 - y1)
+                            atom_neighbor_pos[k1, k2, :] = [x1, y1]
+
+                            # sort neighbors based on angle
+                        sort_ind = np.argsort(a_vec[0, :], axis=None)
+                        d_mat[k1, :] = d_vec[0, sort_ind]
+                        a_mat[k1, :] = a_vec[0, sort_ind]
+                        xd_mat[k1, :] = xd_vec[0, sort_ind]
+                        yd_mat[k1, :] = yd_vec[0, sort_ind]
+
+        neighborhood_results = {'distance_mat': d_mat, 'angles_mat': a_mat,
+                                'xdistance_mat': xd_mat, 'ydistance_mat': yd_mat,
+                                'atom_neighbor_positions': atom_neighbor_pos,
+                                'atom_type': atom_type}
+
         self.neighborhood_results = deepcopy(neighborhood_results)
-        
-        self.atom_neighbor_positions  = atom_neighbor_pos
-        
+
+        self.atom_neighbor_positions = atom_neighbor_pos
+
         return neighborhood_results
-    
+
     def compute_pca_of_neighbors(self):
         '''
         PCA of neighorhood based on results computed from compute_neighborhood
         This means that the results will depend on the settings chosen there.
         So for instance if you change number of neighbors or atom type to look for, 
         then this will be reflected once you execute this method.
         
         Inputs: - (None)
         Output: - (list) (Handles to three figures with the results).
         '''
-        
-        if self.neighborhood_results is None: 
+
+        if self.neighborhood_results is None:
             raise ValueError("Warning, neighborhood hasn't been computed yet. Run compute_neighborhood() first")
 
-        #Access the data
-        
-        #we need to pick the overlap of sets between the atom_idx of the chosen type, 
-        #and the nonborder pixel indices
+        # Access the data
+
+        # we need to pick the overlap of sets between the atom_idx of the chosen type,
+        # and the nonborder pixel indices
         atom_type = self.neighborhood_results['atom_type']
-        atom_idx = np.where(self.atom_types==atom_type)[0]        
+        atom_idx = np.where(self.atom_types == atom_type)[0]
         atoms_to_select = intersection(atom_idx, self.nonborder_pixel_inds)
-        
+
         xd_mat = self.neighborhood_results['xdistance_mat'][atoms_to_select]
         yd_mat = self.neighborhood_results['ydistance_mat'][atoms_to_select]
         d_mat = self.neighborhood_results['distance_mat'][atoms_to_select]
         a_mat = self.neighborhood_results['angles_mat'][atoms_to_select]
-        
-        
-        fig0, ax0 = plt.subplots(figsize=(8,8))
-        ax0.scatter(xd_mat,yd_mat,c='k',s=2)
+
+        fig0, ax0 = plt.subplots(figsize=(8, 8))
+        ax0.scatter(xd_mat, yd_mat, c='k', s=2)
         plt.axis('equal')
 
-        [ud,sd,vd] = np.linalg.svd(d_mat,full_matrices=0) #SVD on radial distance of nearest neighbors
-        [ua,sa,va] = np.linalg.svd(a_mat,full_matrices=0) #SVD on anglular displacement of nearest neighbors
+        [ud, sd, vd] = np.linalg.svd(d_mat, full_matrices=0)  # SVD on radial distance of nearest neighbors
+        [ua, sa, va] = np.linalg.svd(a_mat, full_matrices=0)  # SVD on anglular displacement of nearest neighbors
 
-        [us,ss,vs] = np.linalg.svd(xd_mat+1j*yd_mat,full_matrices=0) #SVD on relative position of nearest neighbors (complex valued)
+        [us, ss, vs] = np.linalg.svd(xd_mat + 1j * yd_mat,
+                                     full_matrices=0)  # SVD on relative position of nearest neighbors (complex valued)
 
-        #convert complex results of 
+        # convert complex results of
         usm = np.abs(us)
         usa = np.angle(us)
         usx = np.real(us)
         usy = np.imag(us)
 
         vsm = np.abs(vs)
         vsa = np.angle(vs)
         vsx = np.real(vs)
         vsy = np.imag(vs)
-        
+
         # plot eigenvalue radial displacements
-        fig1, axs1 = plt.subplots(2,3, figsize=(12, 8), facecolor='black', edgecolor='w')
-        fig1.subplots_adjust(hspace = .1, wspace=.1)
+        fig1, axs1 = plt.subplots(2, 3, figsize=(12, 8), facecolor='black', edgecolor='w')
+        fig1.subplots_adjust(hspace=.1, wspace=.1)
         axs1 = axs1.ravel()
-        for k1 in range(0,min(6,ud.shape[-1])):
-            up = ud[:,k1]
-            up = up-up.min()
-            up = up/up.max()
+        for k1 in range(0, min(6, ud.shape[-1])):
+            up = ud[:, k1]
+            up = up - up.min()
+            up = up / up.max()
             colors = plt.cm.bwr(up)
-            
-            axs1[k1].imshow(1-self.image_source, cmap='Greys', 
-                            interpolation='none',alpha=1)
-            
-            axs1[k1].scatter(self.atom_positions[atoms_to_select][:,0],
-                             self.atom_positions[atoms_to_select][:,1],c=colors,s=8)
+
+            axs1[k1].imshow(1 - self.image_source, cmap='Greys',
+                            interpolation='none', alpha=1)
+
+            axs1[k1].scatter(self.atom_positions[atoms_to_select][:, 0],
+                             self.atom_positions[atoms_to_select][:, 1], c=colors, s=8)
 
         # plot eigenvector maps of radial displacement eigenvectors
-        fig2, axs2 = plt.subplots(2,3, figsize=(12, 8))
-        fig2.subplots_adjust(hspace = .2, wspace=.2)
+        fig2, axs2 = plt.subplots(2, 3, figsize=(12, 8))
+        fig2.subplots_adjust(hspace=.2, wspace=.2)
         axs2 = axs2.ravel()
-        for k1 in range(0,min(6,vd.shape[0])):
-            axs2[k1].plot(0,0,'bo')
-            axs2[k1].plot(vsx[0,:],vsy[0,:],'ro')
+        for k1 in range(0, min(6, vd.shape[0])):
+            axs2[k1].plot(0, 0, 'bo')
+            axs2[k1].plot(vsx[0, :], vsy[0, :], 'ro')
             axs2[k1].axis('equal')
             c = 1.0
             axs2[k1].axis([-c, c, -c, c])
             axs2[k1].set_title(str(k1))
-            axs2[k1].quiver(vsx[0,:],vsy[0,:],vsx[0,:]*vd[k1,:],vsy[0,:]*vd[k1,:])
+            axs2[k1].quiver(vsx[0, :], vsy[0, :], vsx[0, :] * vd[k1, :], vsy[0, :] * vd[k1, :])
 
         return [fig0, fig1, fig2], ud
-    
-    def compute_kmeans_neighbors(self, num_clusters = 4):
+
+    def compute_kmeans_neighbors(self, num_clusters=4):
         '''
         K-Means of neighorhood based on results computed from compute_neighborhood
         This means that the results will depend on the settings chosen there.
         So for instance if you change number of neighbors or atom type to look for, 
         then this will be reflected once you execute this method.
         
         Inputs: - num_clusters (int) (Default = 4): number of clusters in the k-means decomposition
         Output: - (list) Results arranged as ([cluster_centers, labels, figure_handle]).
         
         '''
-    
+
         atom_type = self.neighborhood_results['atom_type']
-        atom_idx = np.where(self.atom_types==atom_type)[0]        
+        atom_idx = np.where(self.atom_types == atom_type)[0]
         atoms_to_select = intersection(atom_idx, self.nonborder_pixel_inds)
-        
+
         xd_mat2 = self.neighborhood_results['xdistance_mat'][atoms_to_select]
         yd_mat2 = self.neighborhood_results['ydistance_mat'][atoms_to_select]
-        
-        zd_mat2 = np.zeros(shape=(xd_mat2.shape[0]-1, xd_mat2.shape[1],2))
-        zd_mat2[:,:,0] = xd_mat2[:-1,:]
-        zd_mat2[:,:,1] = yd_mat2[:-1,:]
-        zd_mat2 = zd_mat2.reshape(xd_mat2.shape[0]-1, -1)
 
-        km = KMeans(n_clusters = num_clusters)
+        zd_mat2 = np.zeros(shape=(xd_mat2.shape[0] - 1, xd_mat2.shape[1], 2))
+        zd_mat2[:, :, 0] = xd_mat2[:-1, :]
+        zd_mat2[:, :, 1] = yd_mat2[:-1, :]
+        zd_mat2 = zd_mat2.reshape(xd_mat2.shape[0] - 1, -1)
+
+        km = KMeans(n_clusters=num_clusters)
         km.fit(zd_mat2)
         cluster_centroids = km.cluster_centers_
-        labels=km.labels_
-  
+        labels = km.labels_
+
         my_colors = ['r', 'b', 'c', 'k', 'g', 'y', 'gray', 'm', '#eeefff',
-                    '#eeefff', '#eeefff', '#eeefff', '#eeefff','#eeefff']
+                     '#eeefff', '#eeefff', '#eeefff', '#eeefff', '#eeefff']
 
-        fig, axes = plt.subplots(figsize =(10,10))
+        fig, axes = plt.subplots(figsize=(10, 10))
         axes.imshow(self.image_source)
-        axes.set_title('KMeans Labels', fontsize = 18)
-        
-        for i in range(min(len(self.atom_positions[atoms_to_select]),len(labels))):
-            x,y = self.atom_positions[atoms_to_select][i]
-            axes.scatter(x,y,c = my_colors[labels[i]])
-
-        if num_clusters <=4:
-            fig, axes = plt.subplots(nrows=2, ncols=2, figsize = (4,4))
-        elif num_clusters>4 and num_clusters<=6:
-            fig, axes = plt.subplots(nrows=2, ncols=3, figsize = (6,4))
-        elif num_clusters>6:
-            fig, axes = plt.subplots(nrows=3, ncols=3, figsize = (8,8))
+        axes.set_title('KMeans Labels', fontsize=18)
+
+        for i in range(min(len(self.atom_positions[atoms_to_select]), len(labels))):
+            x, y = self.atom_positions[atoms_to_select][i]
+            axes.scatter(x, y, c=my_colors[labels[i]])
+
+        if num_clusters <= 4:
+            fig, axes = plt.subplots(nrows=2, ncols=2, figsize=(4, 4))
+        elif num_clusters > 4 and num_clusters <= 6:
+            fig, axes = plt.subplots(nrows=2, ncols=3, figsize=(6, 4))
+        elif num_clusters > 6:
+            fig, axes = plt.subplots(nrows=3, ncols=3, figsize=(8, 8))
 
         for ind, ax in enumerate(axes.flat):
-            if ind< num_clusters:
-                pt = cluster_centroids[ind,:]
+            if ind < num_clusters:
+                pt = cluster_centroids[ind, :]
                 xpts = pt[::2]
                 ypts = pt[1::2]
                 my_color = my_colors[ind]
-                ax.scatter(xpts, ypts, s=50, c = my_color)
-                ax.scatter(0,0,c='b', s = 40)
-                ax.set_xlim(-100,100)
-                ax.set_ylim(-100,100)
-                ax.set_title('Cluster {}'.format(ind), fontsize = 14)
+                ax.scatter(xpts, ypts, s=50, c=my_color)
+                ax.scatter(0, 0, c='b', s=40)
+                ax.set_xlim(-100, 100)
+                ax.set_ylim(-100, 100)
+                ax.set_title('Cluster {}'.format(ind), fontsize=14)
         fig.tight_layout()
 
-        #Plot as point clouds
+        # Plot as point clouds
 
-        if num_clusters <=4:
-            fig, axes = plt.subplots(nrows=2, ncols=2, figsize = (8,8))
-        elif num_clusters>4 and num_clusters<=6:
-            fig, axes = plt.subplots(nrows=2, ncols=3, figsize = (12,8))
-        elif num_clusters>6:
-            fig, axes = plt.subplots(nrows=3, ncols=3, figsize = (12,12))
+        if num_clusters <= 4:
+            fig, axes = plt.subplots(nrows=2, ncols=2, figsize=(8, 8))
+        elif num_clusters > 4 and num_clusters <= 6:
+            fig, axes = plt.subplots(nrows=2, ncols=3, figsize=(12, 8))
+        elif num_clusters > 6:
+            fig, axes = plt.subplots(nrows=3, ncols=3, figsize=(12, 12))
 
         for ind, ax in enumerate(axes.flat):
-            if ind< num_clusters:
-                cluster_pts = zd_mat2[labels==ind,:]
+            if ind < num_clusters:
+                cluster_pts = zd_mat2[labels == ind, :]
                 my_color = my_colors[ind]
                 for atom_index in range(cluster_pts.shape[0]):
-                    xpts = cluster_pts[atom_index,::2]
+                    xpts = cluster_pts[atom_index, ::2]
                     ypts = cluster_pts[atom_index, 1::2]
-                    ax.scatter(xpts, ypts,color = my_color, s=2 )
+                    ax.scatter(xpts, ypts, color=my_color, s=2)
 
-                    ax.set_xlim(-100,100)
-                    ax.set_ylim(-100,100)
+                    ax.set_xlim(-100, 100)
+                    ax.set_ylim(-100, 100)
 
-            ax.set_title('Cluster {} Point Cloud'.format(ind), fontsize = 14)
+            ax.set_title('Cluster {} Point Cloud'.format(ind), fontsize=14)
         fig.tight_layout()
-    
+
         return [cluster_centroids, labels, fig]
-
```

### Comparing `pycroscopy-0.62.1/pycroscopy/stats/tree.py` & `pycroscopy-0.63.0/pycroscopy/stats/tree.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.62.1/pycroscopy.egg-info/PKG-INFO` & `pycroscopy-0.63.0/pycroscopy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycroscopy
-Version: 0.62.1
+Version: 0.63.0
 Summary: Python library for scientific analysis of microscopy data
 Home-page: https://pycroscopy.github.io/pycroscopy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: EELS,STEM,TEM,XRD,AFM,SPM,STS,band excitation,BE,BEPS,Raman,NanoIR,electron microscopy, scanning probe, x-rays,atomic force microscopy,SIMS,energy,spectroscopy,imaging,microscopy,spectracharacterization,spectrogram,hyperspectral,multidimensional,data format,universal,clustering,decomposition,curve fitting,data analysis,PCA, SVD, NMF, DBSCAN, kMeans,machine learning,bayesian inference,fft filtering,signal processing,image cleaning,denoising,model,msa,quantification
 Platform: Linux
@@ -39,28 +39,34 @@
     :target: https://github.com/pycroscopy/pycroscopy/actions?query=workflow%3Abuild
     :alt: GitHub Actions
     
 .. image:: https://img.shields.io/pypi/v/pycroscopy.svg
     :target: https://pypi.org/project/pyCroscopy/
     :alt: PyPI
     
+.. image:: https://codecov.io/gh/pycroscopy/pycroscopy/branch/main/graph/badge.svg?token=HXGZMKzJqb
+    :target: https://codecov.io/gh/pycroscopy/pycroscopy
+    :alt: coverage
+    
 .. image:: https://img.shields.io/conda/vn/conda-forge/pycroscopy.svg
     :target: https://github.com/conda-forge/pycroscopy-feedstock
     :alt: conda-forge
 
 .. image:: https://img.shields.io/pypi/l/pycroscopy.svg
     :target: https://pypi.org/project/pyCroscopy/
     :alt: License
     
 .. image:: https://zenodo.org/badge/61456133.svg
    :target: https://zenodo.org/badge/latestdoi/61456133
    :alt: DOI
+   
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+   :target: https://colab.research.google.com/github/pycroscopy/pycroscopy/blob/main/jupyter_notebooks/Intro_to_Pycroscopy.ipynb
+   :alt: Notebook
 
-**NOTE: Pycroscopy is undergoing a major reorganization and change to the scope and nature of the package. For those interested in the older version, please visit the legacy branch. The new version is under development in the 'phoenix' branch, and this is now the default branch.**
-
-pycroscopy is a `python <http://www.python.org/>`_ package for image processing and scientific analysis of imaging modalities such as multi-frequency scanning probe microscopy, scanning tunneling spectroscopy, x-ray diffraction microscopy, and transmission electron microscopy. pycroscopy uses a data-centric model wherein the raw data collected from the microscope, results from analysis and processing routines are all written to standardized hierarchical data format (HDF5) files for traceability, reproducibility, and provenance.
+pycroscopy is a `python <http://www.python.org/>`_ package for generic (domain-agnostic) microscopy data anlaysis. More specialized or domain-specific analysis routines are contained within some of the other packages within the pycroscopy ecosystem.
 
 Please visit our `homepage <https://pycroscopy.github.io/pycroscopy/about.html>`_ for more information and installation instructions.
 
 If you use pycroscopy for research, we would appreciate if you could cite our `Arxiv paper <https://arxiv.org/abs/1903.09515>`_ titled "USID and Pycroscopy - Open frameworks for storing and analyzing spectroscopic and imaging data"
```

### Comparing `pycroscopy-0.62.1/pycroscopy.egg-info/SOURCES.txt` & `pycroscopy-0.63.0/pycroscopy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 pycroscopy/learn/dl/trainer.py
 pycroscopy/learn/ml/__init__.py
 pycroscopy/learn/ml/decompose.py
 pycroscopy/learn/ml/matrix_factor.py
 pycroscopy/signal/__init__.py
 pycroscopy/stats/__init__.py
 pycroscopy/stats/atom_stats.py
+pycroscopy/stats/atom_stats_n.py
 pycroscopy/stats/tree.py
 pycroscopy/viz/__init__.py
```

### Comparing `pycroscopy-0.62.1/setup.py` & `pycroscopy-0.63.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
                 'torch>=1.0.0',
                 'tensorly>=0.6.0',
                 'tqdm',
                 'ipywidgets>=5.2.2',
                 'ipython',
                 'simpleitk',
                 'sidpy>=0.0.6',
-                'pysptools'
+                'pysptools',
+                'cvxopt>=1.2.7'
                 ]
 
 setup(
     name='pycroscopy',
     version=__version__,
     description='Python library for scientific analysis of microscopy data',
     long_description=long_description,
```


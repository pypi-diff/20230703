# Comparing `tmp/crtoolbox-0.1.2.tar.gz` & `tmp/crtoolbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crtoolbox-0.1.2.tar", last modified: Mon Jul  3 14:55:14 2023, max compression
+gzip compressed data, was "dist/crtoolbox-0.1.3.tar", last modified: Mon Jul  3 15:03:47 2023, max compression
```

## Comparing `crtoolbox-0.1.2.tar` & `crtoolbox-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       32 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/MANIFEST.in
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      464 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/PKG-INFO
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/README.md
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8087 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/bootstrap.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    14288 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/coverage.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    16960 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/generate.py
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox/lib/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/lib/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    32619 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/lib/boundary.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     9649 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/lib/cohens.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26132 2023-07-03 14:43:10.000000 crtoolbox-0.1.2/crtoolbox/lib/display.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    11545 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/lib/fileio.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8257 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/lib/regression.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      694 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/lib/set_theory.py
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox/tests/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/tests/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    27044 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/tests/generate_2d_data.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    11991 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/tests/generate_ni_data.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000) 13824352 2023-07-03 14:33:13.000000 crtoolbox-0.1.2/crtoolbox/tests/mask.nii
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox.egg-info/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      464 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      676 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        1 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       53 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox.egg-info/requires.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       15 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/crtoolbox.egg-info/top_level.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       38 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/setup.cfg
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      801 2023-07-03 14:54:07.000000 crtoolbox-0.1.2/setup.py
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:55:14.000000 crtoolbox-0.1.2/sims/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    12928 2023-07-03 14:33:06.000000 crtoolbox-0.1.2/sims/SpatialSims_Mmu.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:06.000000 crtoolbox-0.1.2/sims/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    17027 2023-07-03 14:33:06.000000 crtoolbox-0.1.2/sims/genCfgs_Mmu.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26300 2023-07-03 14:33:06.000000 crtoolbox-0.1.2/sims/join_and_plot_Mmu.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       32 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/MANIFEST.in
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      464 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/PKG-INFO
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/README.md
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8087 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/bootstrap.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    14288 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/coverage.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    16960 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/generate.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox/lib/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/lib/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    32619 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/lib/boundary.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     9649 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/lib/cohens.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26132 2023-07-03 14:43:10.000000 crtoolbox-0.1.3/crtoolbox/lib/display.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    11545 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/lib/fileio.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8257 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/lib/regression.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      694 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/lib/set_theory.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox/tests/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/tests/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    27044 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/tests/generate_2d_data.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    11991 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/tests/generate_ni_data.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000) 13824352 2023-07-03 14:33:13.000000 crtoolbox-0.1.3/crtoolbox/tests/mask.nii
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox.egg-info/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      464 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      644 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        1 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       15 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/crtoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       38 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/setup.cfg
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      651 2023-07-03 15:03:40.000000 crtoolbox-0.1.3/setup.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 15:03:47.000000 crtoolbox-0.1.3/sims/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    12928 2023-07-03 14:33:06.000000 crtoolbox-0.1.3/sims/SpatialSims_Mmu.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 14:33:06.000000 crtoolbox-0.1.3/sims/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    17027 2023-07-03 14:33:06.000000 crtoolbox-0.1.3/sims/genCfgs_Mmu.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26300 2023-07-03 14:33:06.000000 crtoolbox-0.1.3/sims/join_and_plot_Mmu.py
```

### Comparing `crtoolbox-0.1.2/crtoolbox/bootstrap.py` & `crtoolbox-0.1.3/crtoolbox/bootstrap.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/coverage.py` & `crtoolbox-0.1.3/crtoolbox/coverage.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/generate.py` & `crtoolbox-0.1.3/crtoolbox/generate.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/lib/boundary.py` & `crtoolbox-0.1.3/crtoolbox/lib/boundary.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/lib/cohens.py` & `crtoolbox-0.1.3/crtoolbox/lib/cohens.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/lib/display.py` & `crtoolbox-0.1.3/crtoolbox/lib/display.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/lib/fileio.py` & `crtoolbox-0.1.3/crtoolbox/lib/fileio.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/lib/regression.py` & `crtoolbox-0.1.3/crtoolbox/lib/regression.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/lib/set_theory.py` & `crtoolbox-0.1.3/crtoolbox/lib/set_theory.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/tests/generate_2d_data.py` & `crtoolbox-0.1.3/crtoolbox/tests/generate_2d_data.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/tests/generate_ni_data.py` & `crtoolbox-0.1.3/crtoolbox/tests/generate_ni_data.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox/tests/mask.nii` & `crtoolbox-0.1.3/crtoolbox/tests/mask.nii`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/crtoolbox.egg-info/SOURCES.txt` & `crtoolbox-0.1.3/crtoolbox.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 crtoolbox/__init__.py
 crtoolbox/bootstrap.py
 crtoolbox/coverage.py
 crtoolbox/generate.py
 crtoolbox.egg-info/PKG-INFO
 crtoolbox.egg-info/SOURCES.txt
 crtoolbox.egg-info/dependency_links.txt
-crtoolbox.egg-info/requires.txt
 crtoolbox.egg-info/top_level.txt
 crtoolbox/lib/__init__.py
 crtoolbox/lib/boundary.py
 crtoolbox/lib/cohens.py
 crtoolbox/lib/display.py
 crtoolbox/lib/fileio.py
 crtoolbox/lib/regression.py
```

### Comparing `crtoolbox-0.1.2/setup.py` & `crtoolbox-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 from setuptools import setup, find_packages
 
-# Read in the requirements.txt file
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="crtoolbox",
-    version="0.1.2",
+    version="0.1.3",
     author="Tom Maullin",
     author_email="TomMaullin@gmail.com",
     description="The Confidence Regions Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tommaullin/crtoolbox",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=requirements, 
     python_requires='>=3.6',
 )
```

### Comparing `crtoolbox-0.1.2/sims/SpatialSims_Mmu.py` & `crtoolbox-0.1.3/sims/SpatialSims_Mmu.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/sims/genCfgs_Mmu.py` & `crtoolbox-0.1.3/sims/genCfgs_Mmu.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.2/sims/join_and_plot_Mmu.py` & `crtoolbox-0.1.3/sims/join_and_plot_Mmu.py`

 * *Files identical despite different names*


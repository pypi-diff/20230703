# Comparing `tmp/proteusPy-0.68.tar.gz` & `tmp/proteusPy-0.681.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteusPy-0.68.tar", last modified: Sun Jul  2 20:38:32 2023, max compression
+gzip compressed data, was "proteusPy-0.681.tar", last modified: Mon Jul  3 00:45:03 2023, max compression
```

## Comparing `proteusPy-0.68.tar` & `proteusPy-0.681.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-02 20:38:32.742904 proteusPy-0.68/
--rw-r--r--   0 egs        (505) staff       (20)     3337 2023-07-02 20:38:32.742977 proteusPy-0.68/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)     2209 2023-02-07 17:54:00.000000 proteusPy-0.68/README.md
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-02 20:38:32.741192 proteusPy-0.68/proteusPy/
--rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.68/proteusPy/Disulfide.py
--rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.68/proteusPy/DisulfideClass_Constructor.py
--rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.68/proteusPy/DisulfideClasses.py
--rw-r--r--   0 egs        (505) staff       (20)     1027 2023-01-04 04:03:30.000000 proteusPy-0.68/proteusPy/DisulfideExceptions.py
--rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.68/proteusPy/DisulfideList.py
--rw-r--r--   0 egs        (505) staff       (20)    24302 2023-07-02 19:51:53.000000 proteusPy-0.68/proteusPy/DisulfideLoader.py
--rw-r--r--   0 egs        (505) staff       (20)      833 2023-07-02 19:47:15.000000 proteusPy-0.68/proteusPy/ProteusGlobals.py
--rw-r--r--   0 egs        (505) staff       (20)     1641 2023-07-02 20:38:06.000000 proteusPy-0.68/proteusPy/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.68/proteusPy/angle_annotation.py
--rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.68/proteusPy/atoms.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-02 20:38:32.742482 proteusPy-0.68/proteusPy/data/
--rw-r--r--   0 egs        (505) staff       (20)     2493 2023-07-02 19:46:00.000000 proteusPy-0.68/proteusPy/data/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.68/proteusPy/proteusPyWarning.py
--rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.68/proteusPy/residue.py
--rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.68/proteusPy/turtle3D.py
--rw-r--r--   0 egs        (505) staff       (20)    12468 2023-03-13 16:49:31.000000 proteusPy-0.68/proteusPy/utility.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-02 20:38:32.742364 proteusPy-0.68/proteusPy.egg-info/
--rw-r--r--   0 egs        (505) staff       (20)     3337 2023-07-02 20:38:32.000000 proteusPy-0.68/proteusPy.egg-info/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)      626 2023-07-02 20:38:32.000000 proteusPy-0.68/proteusPy.egg-info/SOURCES.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:38:32.000000 proteusPy-0.68/proteusPy.egg-info/dependency_links.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.68/proteusPy.egg-info/not-zip-safe
--rw-r--r--   0 egs        (505) staff       (20)       32 2023-07-02 20:38:32.000000 proteusPy-0.68/proteusPy.egg-info/requires.txt
--rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-02 20:38:32.000000 proteusPy-0.68/proteusPy.egg-info/top_level.txt
--rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-02 20:38:32.743193 proteusPy-0.68/setup.cfg
--rw-r--r--   0 egs        (505) staff       (20)     3659 2023-06-16 23:35:18.000000 proteusPy-0.68/setup.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.177892 proteusPy-0.681/
+-rw-r--r--   0 egs        (505) staff       (20)     3420 2023-07-03 00:45:03.177996 proteusPy-0.681/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)     2281 2023-07-02 23:22:12.000000 proteusPy-0.681/README.md
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.174466 proteusPy-0.681/proteusPy/
+-rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.681/proteusPy/Disulfide.py
+-rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.681/proteusPy/DisulfideClass_Constructor.py
+-rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.681/proteusPy/DisulfideClasses.py
+-rw-r--r--   0 egs        (505) staff       (20)     1027 2023-01-04 04:03:30.000000 proteusPy-0.681/proteusPy/DisulfideExceptions.py
+-rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.681/proteusPy/DisulfideList.py
+-rw-r--r--   0 egs        (505) staff       (20)    24238 2023-07-03 00:32:10.000000 proteusPy-0.681/proteusPy/DisulfideLoader.py
+-rw-r--r--   0 egs        (505) staff       (20)      833 2023-07-02 19:47:15.000000 proteusPy-0.681/proteusPy/ProteusGlobals.py
+-rw-r--r--   0 egs        (505) staff       (20)     1642 2023-07-03 00:44:38.000000 proteusPy-0.681/proteusPy/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.681/proteusPy/angle_annotation.py
+-rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.681/proteusPy/atoms.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.177469 proteusPy-0.681/proteusPy/data/
+-rw-r--r--   0 egs        (505) staff       (20)     2514 2023-07-02 22:23:54.000000 proteusPy-0.681/proteusPy/data/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.681/proteusPy/data/ss_completed.txt
+-rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.681/proteusPy/data/ss_ids.txt
+-rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.681/proteusPy/data/ss_query.json
+-rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.681/proteusPy/proteusPyWarning.py
+-rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.681/proteusPy/residue.py
+-rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.681/proteusPy/turtle3D.py
+-rw-r--r--   0 egs        (505) staff       (20)    12468 2023-03-13 16:49:31.000000 proteusPy-0.681/proteusPy/utility.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.175554 proteusPy-0.681/proteusPy.egg-info/
+-rw-r--r--   0 egs        (505) staff       (20)     3420 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)      713 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/SOURCES.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/dependency_links.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.681/proteusPy.egg-info/not-zip-safe
+-rw-r--r--   0 egs        (505) staff       (20)       36 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/requires.txt
+-rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/top_level.txt
+-rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-03 00:45:03.178375 proteusPy-0.681/setup.cfg
+-rw-r--r--   0 egs        (505) staff       (20)     3676 2023-07-02 20:46:16.000000 proteusPy-0.681/setup.py
```

### Comparing `proteusPy-0.68/PKG-INFO` & `proteusPy-0.681/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.68
+Version: 0.681
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
 Project-URL: Tracker, https://github.com/suchanek/proteusPy/issues
-Keywords: proteus suchanek
+Keywords: proteus suchanek disulfide
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,22 +32,29 @@
 1. Install Anaconda (<http://anaconda.org>)
    - Create a new environment using python 3.9
    - Activate the environment
 2. Build the environment. At this point it's probably best to clone the repo via github since it contains all
    of the notebooks and test programs. Ultimately the distribution can be used from pyPi as a normal
    package.
    - Using pyPi:
-     - python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ proteusPy
-   - From gitHub:
+     - python3 -m pip install proteusPy
+   - From the gitHub repository:
      - Install git-lfs
        - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
-       - From a shell prompt: git-lfs track "*.csv" "*.pkl" "*.mp4"
-     - git clone https://github.com/suchanek/proteusPy/proteusPy.git
+       - From a shell prompt: 
+         ```
+          $ git-lfs track "*.csv" "*.pkl" "*.mp4"
+          $ git clone https://github.com/suchanek/proteusPy/proteusPy.git
+         ```
      - cd into the repo
-     - pip install .
+     - ```
+        $ conda env create --name proteusPy --file=proteusPy.yml
+        $ pip install .
+       ```
+     - 
   
 
 #### Publications
 * https://doi.org/10.1021/bi00368a023
 * https://doi.org/10.1021/bi00368a024
 * https://doi.org/10.1016/0092-8674(92)90140-8
 * http://dx.doi.org/10.2174/092986708783330566
```

### Comparing `proteusPy-0.68/README.md` & `proteusPy-0.681/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,29 @@
 1. Install Anaconda (<http://anaconda.org>)
    - Create a new environment using python 3.9
    - Activate the environment
 2. Build the environment. At this point it's probably best to clone the repo via github since it contains all
    of the notebooks and test programs. Ultimately the distribution can be used from pyPi as a normal
    package.
    - Using pyPi:
-     - python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ proteusPy
-   - From gitHub:
+     - python3 -m pip install proteusPy
+   - From the gitHub repository:
      - Install git-lfs
        - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
-       - From a shell prompt: git-lfs track "*.csv" "*.pkl" "*.mp4"
-     - git clone https://github.com/suchanek/proteusPy/proteusPy.git
+       - From a shell prompt: 
+         ```
+          $ git-lfs track "*.csv" "*.pkl" "*.mp4"
+          $ git clone https://github.com/suchanek/proteusPy/proteusPy.git
+         ```
      - cd into the repo
-     - pip install .
+     - ```
+        $ conda env create --name proteusPy --file=proteusPy.yml
+        $ pip install .
+       ```
+     - 
   
 
 #### Publications
 * https://doi.org/10.1021/bi00368a023
 * https://doi.org/10.1021/bi00368a024
 * https://doi.org/10.1016/0092-8674(92)90140-8
 * http://dx.doi.org/10.2174/092986708783330566
```

### Comparing `proteusPy-0.68/proteusPy/Disulfide.py` & `proteusPy-0.681/proteusPy/Disulfide.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/DisulfideClass_Constructor.py` & `proteusPy-0.681/proteusPy/DisulfideClass_Constructor.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/DisulfideClasses.py` & `proteusPy-0.681/proteusPy/DisulfideClasses.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/DisulfideExceptions.py` & `proteusPy-0.681/proteusPy/DisulfideExceptions.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/DisulfideList.py` & `proteusPy-0.681/proteusPy/DisulfideList.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/DisulfideLoader.py` & `proteusPy-0.681/proteusPy/DisulfideLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,35 +555,38 @@
     '''
     # normally the .pkl files are local, EXCEPT for the first run from a newly-installed proteusPy 
     # distribution. In that case we need to download the files for all disulfides and the subset
     # from the Google Drive storage.
     
     import gdown
     url_all = "https://drive.google.com/uc?id=1igF-sppLPaNsBaUS7nkb13vtOGZZmsFp"
-    url_subset = "https://drive.google.com/uc?id=1puy9pxrClFks0KN9q5PPV_ONKvL-hg33/view?usp=drive_link"
-
+    url_subset = "https://drive.google.com/uc?id=1puy9pxrClFks0KN9q5PPV_ONKvL-hg33"
+    
+    _good1 = False # all data
+    _good2 = False # subset data
+    
+    _fname_sub = f'{loadpath}{LOADER_SUBSET_FNAME}'
+    _fname_all = f'{loadpath}{LOADER_FNAME}'
+    
     if subset:
-        _fname = f'{loadpath}{LOADER_SUBSET_FNAME}'
+        _fname = _fname_sub
     else:
-        _fname = f'{loadpath}{LOADER_FNAME}'
-
+        _fname = _fname_all
+    
     if verbose:
         print(f'-> load_PDB_SS(): Reading {_fname}... ', end='')
+
     try:
         with open(_fname, 'rb') as f:
             res = pickle.load(f)
         if verbose:
             print(f'done.')
         return res
     
     except IOError:
-        _good1 = False # all data
-        _good2 = False # subset data
-        _fname_sub = f'{loadpath}{LOADER_SUBSET_FNAME}'
-        _fname_all = f'{loadpath}{LOADER_FNAME}'
         if verbose:
             print(f'-> DisulfideLoader(): Reading disulfides from Google Drive... ')
         
         #PDB_SS_ALL_LOADER.pkl
         if verbose:
             destination = _fname_all
             print(f'-> DisulfideLoader(): Downloading the RCSB Disulfide Database from Google Drive to {destination}... ', end='')
@@ -604,34 +607,37 @@
             _good2 = True
             if verbose:
                 print(f' done.')
         else:
             print('Error downloading RCSB subset database!')
 
     if subset:
-        _fname = f'{loadpath}{LOADER_SUBSET_FNAME}'
+        _fname = _fname_sub
     else:
-        _fname = f'{loadpath}{LOADER_FNAME}'
+        _fname = _fname_all
 
     if verbose:
         print(f'-> load_PDB_SS(): Attempting to read {_fname}... ', end='')
     try:
         with open(_fname, 'rb') as f:
             res = pickle.load(f)
         if verbose:
             print(f'done.')
         return res
     except:
         # no fully built loader available. See if we can
         # build it
         print(f'\n\n!!! Unable to download database! Load_PDB_SS() is attempting to rebuild the loader.')
+        return
+        '''
         pdb = DisulfideLoader(verbose=True, subset=subset)
         if pdb is None:
             mess = f'!!! FATAL: load_PDB_SS(): cannot rebuild primary SS file!'
             raise DisulfideIOException(mess)
         else:
             pdb.save()
         print(f'-> Load_PDB_SS(): rebuild complete.')
-    
+        '''
+
     return pdb
 
 # End of file
```

### Comparing `proteusPy-0.68/proteusPy/ProteusGlobals.py` & `proteusPy-0.681/proteusPy/ProteusGlobals.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/__init__.py` & `proteusPy-0.681/proteusPy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Eric G. Suchanek, PhD., all rights reserved
 # Subject to the MIT public license.
 
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.68"
+__version__ = "0.681"
 
 import sys
 import os
 import glob
 import warnings
 import copy
```

### Comparing `proteusPy-0.68/proteusPy/angle_annotation.py` & `proteusPy-0.681/proteusPy/angle_annotation.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/atoms.py` & `proteusPy-0.681/proteusPy/atoms.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/data/__init__.py` & `proteusPy-0.681/proteusPy/data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 '''
-Global declarations for
+Global declarations for the proteusPy package
 '''
 
 # init for proteusPy data module
 # Copyright (c) 2023 Eric G. Suchanek, PhD., all rights reserved
 # Subject to the GNU public license.
 
 import os
 
 # absolute location for the disulfide .pkl files
 _abspath = os.path.dirname(os.path.abspath(__file__))
 
-
 DATA_DIR = f'{_abspath}/'
 SS_PICKLE_FILE = 'PDB_all_ss.pkl'
 SS_DICT_PICKLE_FILE = 'PDB_all_ss_dict.pkl'
 SS_DICT_PICKLE_FILE2 = 'PDB_all_ss_dict_ind.pkl'
 SS_TORSIONS_FILE = 'PDB_all_SS_torsions.csv'
 PROBLEM_ID_FILE = 'PDB_all_SS_problems.csv'
 SS_ID_FILE = 'ss_ids.txt'
```

### Comparing `proteusPy-0.68/proteusPy/residue.py` & `proteusPy-0.681/proteusPy/residue.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/turtle3D.py` & `proteusPy-0.681/proteusPy/turtle3D.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy/utility.py` & `proteusPy-0.681/proteusPy/utility.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.68/proteusPy.egg-info/PKG-INFO` & `proteusPy-0.681/proteusPy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.68
+Version: 0.681
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
 Project-URL: Tracker, https://github.com/suchanek/proteusPy/issues
-Keywords: proteus suchanek
+Keywords: proteus suchanek disulfide
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,22 +32,29 @@
 1. Install Anaconda (<http://anaconda.org>)
    - Create a new environment using python 3.9
    - Activate the environment
 2. Build the environment. At this point it's probably best to clone the repo via github since it contains all
    of the notebooks and test programs. Ultimately the distribution can be used from pyPi as a normal
    package.
    - Using pyPi:
-     - python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ proteusPy
-   - From gitHub:
+     - python3 -m pip install proteusPy
+   - From the gitHub repository:
      - Install git-lfs
        - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
-       - From a shell prompt: git-lfs track "*.csv" "*.pkl" "*.mp4"
-     - git clone https://github.com/suchanek/proteusPy/proteusPy.git
+       - From a shell prompt: 
+         ```
+          $ git-lfs track "*.csv" "*.pkl" "*.mp4"
+          $ git clone https://github.com/suchanek/proteusPy/proteusPy.git
+         ```
      - cd into the repo
-     - pip install .
+     - ```
+        $ conda env create --name proteusPy --file=proteusPy.yml
+        $ pip install .
+       ```
+     - 
   
 
 #### Publications
 * https://doi.org/10.1021/bi00368a023
 * https://doi.org/10.1021/bi00368a024
 * https://doi.org/10.1016/0092-8674(92)90140-8
 * http://dx.doi.org/10.2174/092986708783330566
```

### Comparing `proteusPy-0.68/proteusPy.egg-info/SOURCES.txt` & `proteusPy-0.681/proteusPy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 proteusPy/utility.py
 proteusPy.egg-info/PKG-INFO
 proteusPy.egg-info/SOURCES.txt
 proteusPy.egg-info/dependency_links.txt
 proteusPy.egg-info/not-zip-safe
 proteusPy.egg-info/requires.txt
 proteusPy.egg-info/top_level.txt
-proteusPy/data/__init__.py
+proteusPy/data/__init__.py
+proteusPy/data/ss_completed.txt
+proteusPy/data/ss_ids.txt
+proteusPy/data/ss_query.json
```

### Comparing `proteusPy-0.68/setup.py` & `proteusPy-0.681/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/suchanek/proteusPy/',
       author='Eric G. Suchanek, PhD',
       author_email='suchanek@mac.com',
       license='MIT',
       packages=['proteusPy'],
-      keywords='proteus suchanek',
-      install_requires=['pandas', 'numpy', 'matplotlib', 'pyvista'],
+      keywords='proteus suchanek disulfide',
+      install_requires=['pandas', 'numpy', 'matplotlib', 'pyvista', 'pip'],
       source='https://github.com/suchanek/proteusPy/',
       project_urls={
         "Documentation": "https://suchanek.github.io/proteusPy/",
         "Source": "https://github.com/suchanek/proteusPy/",
         "Tracker": "https://github.com/suchanek/proteusPy/issues",
       },
       classifiers=[
```


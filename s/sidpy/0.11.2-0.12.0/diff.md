# Comparing `tmp/sidpy-0.11.2.tar.gz` & `tmp/sidpy-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidpy-0.11.2.tar", last modified: Thu Jan 19 20:37:20 2023, max compression
+gzip compressed data, was "sidpy-0.12.0.tar", last modified: Mon Jul  3 20:48:28 2023, max compression
```

## Comparing `sidpy-0.11.2.tar` & `sidpy-0.12.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.485325 sidpy-0.11.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-19 20:31:16.000000 sidpy-0.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-19 20:31:16.000000 sidpy-0.11.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-01-19 20:37:20.485325 sidpy-0.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-19 20:31:16.000000 sidpy-0.11.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-19 20:37:20.485325 sidpy-0.11.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-01-19 20:31:17.000000 sidpy-0.11.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.477325 sidpy-0.11.2/sidpy/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.481325 sidpy-0.11.2/sidpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/base/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/base/num_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/base/string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.481325 sidpy-0.11.2/sidpy/hdf/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/hdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27179 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/hdf/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/hdf/hdf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/hdf/prov_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/hdf/reg_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.481325 sidpy-0.11.2/sidpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/io/interface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.481325 sidpy-0.11.2/sidpy/proc/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11298 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/proc/comp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22057 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/proc/fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.485325 sidpy-0.11.2/sidpy/sid/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/sid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60719 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/sid/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/sid/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/sid/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/sid/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.485325 sidpy-0.11.2/sidpy/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41686 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/dataset_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    18222 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/jupyter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.485325 sidpy-0.11.2/sidpy/viz/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/plot_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/plot_utils/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/plot_utils/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/plot_utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-01-19 20:31:17.000000 sidpy-0.11.2/sidpy/viz/plot_utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:37:20.481325 sidpy-0.11.2/sidpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-01-19 20:37:20.000000 sidpy-0.11.2/sidpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-19 20:37:20.000000 sidpy-0.11.2/sidpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 20:37:20.000000 sidpy-0.11.2/sidpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-19 20:37:20.000000 sidpy-0.11.2/sidpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-19 20:37:20.000000 sidpy-0.11.2/sidpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 20:43:43.000000 sidpy-0.12.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 20:43:43.000000 sidpy-0.12.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-03 20:48:28.791724 sidpy-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 20:43:43.000000 sidpy-0.12.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 20:48:28.795724 sidpy-0.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-03 20:43:43.000000 sidpy-0.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/num_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/hdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27179 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30933 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/hdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/prov_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/reg_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/io/interface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11298 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/proc/comp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/proc/fitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/sid/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64690 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53698 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/dataset_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/jupyter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/viz/plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/top_level.txt
```

### Comparing `sidpy-0.11.2/LICENSE` & `sidpy-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/PKG-INFO` & `sidpy-0.12.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidpy
-Version: 0.11.2
+Version: 0.12.0
 Summary: Python utilities for storing, visualizing, and processing Spectroscopic and Imaging Data (SID)
 Home-page: https://pycroscopy.github.io/sidpy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific,visualization,processing,storage,hdf5
 Platform: Linux
```

### Comparing `sidpy-0.11.2/README.rst` & `sidpy-0.12.0/README.rst`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/setup.py` & `sidpy-0.12.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
                 'h5py>=2.6.0',
                 'matplotlib>=2.0.0',
                 'distributed>=2.0.0',
                 'psutil',
                 'six',
                 'joblib>=0.11.0',
                 'ipywidgets>=5.2.2',
+                'ipykernel',
                 'ipython>=5.1.0,<6;python_version<"3.3"',  # IPython 6.0+ does not support Python < 3.5
                 'ipython>=6.0;python_version>="3.3"',  # Beginning with IPython 6.0, Python 3.3 and above is required.
                 'scikit-learn',
                 'scipy',
                 'ase'
                 ]
 
@@ -53,15 +54,15 @@
               'visualization', 'processing', 'storage', 'hdf5'],
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     url='https://pycroscopy.github.io/sidpy/about.html',
     license='MIT',
     author='Pycroscopy contributors',
     author_email='pycroscopy@gmail.com',
     install_requires=requirements,
-    setup_requires=['pytest-runner'],
+    
     tests_require=['unittest2;python_version<"3.0"', 'pytest'],
     platforms=['Linux', 'Mac OSX', 'Windows 10/8.1/8/7'],
     # package_data={'sample':['dataset_1.dat']}
     test_suite='pytest',
     # dependency='',
     # dependency_links=[''],
     include_package_data=True,
```

### Comparing `sidpy-0.11.2/sidpy/__init__.py` & `sidpy-0.12.0/sidpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/base/dict_utils.py` & `sidpy-0.12.0/sidpy/base/dict_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/base/num_utils.py` & `sidpy-0.12.0/sidpy/base/num_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,28 @@
     Returns
     -------
     float
         Slope of the line
     """
     if not isinstance(tol, float):
         raise TypeError('tol should be a float << 1')
-    step_size = np.unique(np.diff(values))
-    if len(step_size) > 1:
-        # often we end up here. In most cases,
-        step_avg = step_size.max()
-        step_size -= step_avg
-        var = np.mean(np.abs(step_size))
-        if var / step_avg < tol:
-            step_size = [step_avg]
-        else:
-            # Non-linear dimension! - see notes above
-            raise ValueError('Provided values cannot be expressed as a linear trend')
+    if len(values)==1:
+        step_size=[0]
+    else:
+        step_size = np.unique(np.diff(values))
+        if len(step_size) > 1:
+            # often we end up here. In most cases,
+            step_avg = step_size.max()
+            step_size -= step_avg
+            var = np.mean(np.abs(step_size))
+            if var / step_avg < tol:
+                step_size = [step_avg]
+            else:
+                # Non-linear dimension! - see notes above
+                raise ValueError('Provided values cannot be expressed as a linear trend')
     return step_size[0]
 
 
 def to_ranges(iterable):
     """
     Converts a sequence of iterables to range tuples
```

### Comparing `sidpy-0.11.2/sidpy/base/string_utils.py` & `sidpy-0.12.0/sidpy/base/string_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/hdf/dtype_utils.py` & `sidpy-0.12.0/sidpy/hdf/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/hdf/hdf_utils.py` & `sidpy-0.12.0/sidpy/hdf/hdf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -811,10 +811,9 @@
         raise TypeError('we need a h5py group to read from')
     if not isinstance(group_dict, dict):
         raise TypeError('group_dict needs to be a python dictionary')
    
     group_dict[group_iter.name.split('/')[-1]] = dict(group_iter.attrs)
     
     for key in group_iter.keys():
-        print(key)
         h5_group_to_dict(group_iter[key], group_dict[group_iter.name.split('/')[-1]])
     return group_dict
```

### Comparing `sidpy-0.11.2/sidpy/hdf/prov_utils.py` & `sidpy-0.12.0/sidpy/hdf/prov_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/hdf/reg_ref.py` & `sidpy-0.12.0/sidpy/hdf/reg_ref.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/io/interface_utils.py` & `sidpy-0.12.0/sidpy/io/interface_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,16 +195,15 @@
     _instance = QApplication.instance()
     if not _instance:
         # print('not_instance')
         _instance = QApplication([])
 
     return _instance
 
-
-def openfile_dialog_QT(file_types="All files (*)", multiple_files=False,
+def openfile_dialog_qt(file_types="All files (*)", multiple_files=False,
                        file_path='.', caption="Select a file..."):
     """
     Opens a File dialog which is used in open_file() function
     This function uses pyQt5.
 
     Parameters
     ----------
@@ -250,32 +249,31 @@
             if not isinstance(param, (str, unicode)):
                 raise TypeError('param must be a string')
 
     parent = None
     if multiple_files:
         func = QtWidgets.QFileDialog.getOpenFileNames
         fnames, file_filter = func(parent, caption, file_path,
-                                   filter=file_types,
-                                   options=[QtCore.Qt.WindowStaysOnTopHint])
+                                   filter=file_types)
+                                   
         if len(fnames) > 0:
             fname = fnames[0]
         else:
             return
     else:
         func = QtWidgets.QFileDialog.getOpenFileName
         fname, file_filter = func(parent, caption, file_path,
                                   filter=file_types)
 
     if multiple_files:
         return fnames
     else:
         return str(fname)
 
-
-def savefile_dialog(initial_file='*.hf5', file_path='.',
+def savefile_dialog_qt(initial_file='*.hf5', file_path='.',
                     file_types=None, caption="Save file as ..."):
     """
     Produces a window / dialog to allow users to specify the location and name
     of a file to save to.
 
     Parameters
     ----------
@@ -326,14 +324,18 @@
                                   filter=file_types)
         if len(fname) > 1:
             return fname
         else:
             return None
 
 
+# Compatibility, should be depreciated
+openfile_dialog_QT = openfile_dialog_qt
+savefile_dialog = savefile_dialog_qt
+
 try:
     from PyQt5 import QtWidgets
 
     class ProgressDialog(QtWidgets.QDialog):
         """
         Simple dialog that consists of a Progress Bar and a Button.
         Clicking on the button results in the start of a timer and
```

### Comparing `sidpy-0.11.2/sidpy/proc/comp_utils.py` & `sidpy-0.12.0/sidpy/proc/comp_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/proc/fitter.py` & `sidpy-0.12.0/sidpy/proc/fitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..sid import Dimension, Dataset
 from ..sid.dimension import DimensionType
 from ..viz.dataset_viz import SpectralImageFitVisualizer
 from ..sid.dataset import DataType
 
 try:
     from scipy.optimize import curve_fit
-except ModuleNotFoundError:
+except ImportError:
     curve_fit = None
 
 try:
     from sklearn.cluster import KMeans
 except ModuleNotFoundError:
     KMeans = None
 
@@ -94,14 +94,15 @@
         if guess_fn is None:
             if num_fit_parms is None:
                 raise ValueError("You did not supply a guess function, you must at least provide number of fit "
                                  "parameters to set the priors for scipy.optimize.curve_fit")
         self.dataset = sidpy_dataset  # Sidpy dataset
         self.fit_fn = fit_fn  # function that takes xvec, *parameters and returns yvec at each value of xvec
         self.num_fit_parms = num_fit_parms  # int: number of fitting parameters
+        self._complex_data = False  # if data is complex. Will be checked during guess/fit as needed.
 
         if ind_dims is not None:
             self.ind_dims = tuple(ind_dims)  # Tuple: containing indices of independent dimensions
         else:
             # All the dimensions that are not spectral will be considered as independent dimensions
             ind_dims = []
             for i, dim in self.dataset._axes.items():
@@ -149,15 +150,15 @@
                     raise ValueError('The number of independent dimensions provided in the xvec do not match '
                                      'with the number of dependent dimensions of the dataset')
                 else:
                     raise TypeError('Please provide a list of value-arrays corresponding to each dependent dimension')
 
         # Dealing with the meshgrid part of multidimensional fitting
         if len(self.dep_dims) > 1:
-            self.dep_vec = [ar.ravel() for ar in np.meshgrid(*dep_dims)]
+            self.dep_vec = [ar.ravel() for ar in np.meshgrid(*dep_vec, indexing='ij')]
         else:
             self.dep_vec = dep_vec
 
         self.km_guess = km_guess
         if self.km_guess:
             self.km_priors = None
             self.km_labels = None
@@ -170,20 +171,24 @@
         self.num_workers = num_workers
         self.threads = threads
         self.guess_completed = False
         self.return_std = return_std
         self.return_cov = return_cov
         self.return_fit = return_fit
         self.fitted_dset = None
+        self._numpy = True
 
         self.mean_fit_results = []
         if self.return_cov:
             self.cov_fit_results = None
         if self.return_std:
             self.std_fit_results = None
+
+        if 'complex' in self.dataset.dtype.name:
+            self._complex_data = True
         # set up dask client
         self.client = Client(threads_per_worker=self.threads, n_workers=self.num_workers)
 
     def _setup_calc(self):
         self.fold_order = [[]]  # All the independent dimensions go into the first element and will be collapsed
         self.num_computations = 1
 
@@ -200,16 +205,17 @@
 
         self.folded_dataset = self.dataset.fold(dim_order=self.fold_order)
 
         # Here is the tricky part, dataset.unfold is designed to get back the original dataset with minimal loss of
         # information. To do this, unfold utilizes the saved information while folding the original dataset.
         # Here, we are going to tweak that information and use the unfold method on the dataset with fitted parameters.
 
-        self._unfold_attr = {'dim_order_flattened': list(np.arange(len(self.fold_order[0])))+[len(self.fold_order[0])],
-                             'shape_transposed': [self.dataset.shape[i] for i in self.fold_order[0]] + [-1]}
+        self._unfold_attr = {
+            'dim_order_flattened': list(np.arange(len(self.fold_order[0]))) + [len(self.fold_order[0])],
+            'shape_transposed': [self.dataset.shape[i] for i in self.fold_order[0]] + [-1]}
         axes, j = {}, 0
         for i, dim in self.dataset._axes.items():
             if not i in self.dep_dims:
                 axes[j] = dim
                 j += 1
         self._unfold_attr['_axes'] = axes
 
@@ -221,15 +227,21 @@
         Returns:
         None
         -------
 
         """
         guess_results = []
         for ind in range(self.num_computations):
-            lazy_result = dask.delayed(self.guess_fn)(self.dep_vec, self.folded_dataset[ind, :])
+            if self._numpy:
+                self.dep_vec=np.array(self.dep_vec)
+                ydata = np.array(self.folded_dataset)
+            else:
+                ydata = self.folded_dataset
+
+            lazy_result = dask.delayed(self.guess_fn)(self.dep_vec, ydata[ind, :])
             guess_results.append(lazy_result)
 
         guess_results = dask.compute(*guess_results)
         self.prior = np.squeeze(np.array(guess_results))
         self.num_fit_parms = self.prior.shape[-1]
         self.guess_completed = True
 
@@ -249,29 +261,40 @@
                 self.do_guess()
 
             for ind in range(self.num_computations):
                 if self.prior is None:
                     p0 = np.random.normal(loc=0.5, scale=0.1, size=self.num_fit_parms)
                 else:
                     p0 = self.prior[ind, :]
-
+                ydata = self.folded_dataset[ind, :]
+                if self._complex_data:
+                    ydata = ydata.flatten_complex()
+
+                #Convert to numpy - see if this makes it faster??
+                if self._numpy:
+                    ydata = np.array(ydata)
+                    self.dep_vec = np.array(self.dep_vec)
                 lazy_result = dask.delayed(SidFitter.default_curve_fit)(self.fit_fn, self.dep_vec,
-                                                                        self.folded_dataset[ind, :],self.num_fit_parms,
+                                                                        ydata, self.num_fit_parms,
                                                                         return_cov=(self.return_cov or self.return_std),
                                                                         p0=p0, **kwargs)
                 fit_results.append(lazy_result)
 
             fit_results_comp = dask.compute(*fit_results)
             self.client.close()
 
         else:
-            self.get_km_priors()
+            self.get_km_priors(**kwargs)
             for ind in range(self.num_computations):
+                ydata = self.folded_dataset[ind, :]
+                if self._complex_data:
+                    ydata = ydata.flatten_complex()
+
                 lazy_result = dask.delayed(SidFitter.default_curve_fit)(self.fit_fn, self.dep_vec,
-                                                                        self.folded_dataset[ind, :], self.num_fit_parms,
+                                                                        ydata, self.num_fit_parms,
                                                                         return_cov=(self.return_cov or self.return_std),
                                                                         p0=self.km_priors[self.km_labels[ind]],
                                                                         **kwargs)
                 fit_results.append(lazy_result)
 
             fit_results_comp = dask.compute(*fit_results)
             self.client.close()
@@ -382,88 +405,129 @@
         else:
             return results
 
     def get_fitted_dataset(self):
         """This method returns the fitted dataset using the parameters generated by the fit function"""
         fitted_dset = self.dataset.like_data(np.zeros_like(self.dataset.compute()),
                                              title_prefix='fitted_')
-        fitted_dset_fold = fitted_dset.fold(dim_order=self.fold_order)
 
+        fitted_dset_fold = fitted_dset.fold(dim_order=self.fold_order)
+        output_shape = np.prod(fitted_dset_fold.shape[1:])
+        user_folding = False
+        ydata_fit = self.fit_fn(self.dep_vec, *self.mean_fit_results[0])
+
+        # print(r"ydata shape is {} and squeezed is {}".format(ydata_fit.shape, ydata_fit.squeeze().shape))
+        if ydata_fit.squeeze().shape[0] != output_shape:
+            print('Shapes of output of fitting function is {} and original data is {} \
+                  Reshaping output dataset. You are responsible for reshaping'.format(ydata_fit.shape[0],
+                                                                                      output_shape,
+                                                                                      ))
+
+            fitted_dset_fold = self.dataset.like_data(np.zeros((fitted_dset_fold.shape[0], ydata_fit.shape[0])),
+                                                      title_prefix='fitted_')
+            user_folding = True
         # Here we make a roundtrip to numpy as earlier versions of dask did not support the assignments
         # of the form dask_array[2] = 1
 
         np_folded_arr = fitted_dset_fold.compute()
         for i in range(np_folded_arr.shape[0]):
-            np_folded_arr[i] = self.fit_fn(self.dep_vec, *self.mean_fit_results[i])
+            # ydata_fit = self.fit_fn(self.dep_vec, *self.mean_fit_results[i])
+            # print('dep vec is {} and mean fit results are {}'.format(self.dep_vec,self.mean_fit_results[i]))
+            fit_output = self.fit_fn(self.dep_vec, *self.mean_fit_results[i])
+            # print('ydata output from fitting fn is {}'.format(fit_output))
+            if fit_output.shape != np_folded_arr[i].shape:
+                try:
+                    np_folded_arr[i] = fit_output.reshape(np_folded_arr[i].shape)
+                except:
+                    print("Cannot reshape function output to retrieve fitted dataset")
+            else:
+                np_folded_arr[i] = fit_output
 
-        fitted_sid_dset_folded = fitted_dset_fold.like_data(np_folded_arr, title=fitted_dset_fold.title)
-        fitted_sid_dset = fitted_sid_dset_folded.unfold()
-        fitted_sid_dset.original_metadata = self.dataset.original_metadata.copy()
+        if not user_folding:
+            fitted_sid_dset_folded = fitted_dset_fold.like_data(np_folded_arr, title=fitted_dset_fold.title)
+            fitted_sid_dset = fitted_sid_dset_folded.unfold()
+            fitted_sid_dset.original_metadata = self.dataset.original_metadata.copy()
+        else:
+            fitted_sid_dset = fitted_dset_fold.like_data(np_folded_arr, title=fitted_dset_fold.title)
+            fitted_sid_dset.original_metadata = self.dataset.original_metadata.copy()
         self.fitted_dset = fitted_sid_dset
         return fitted_sid_dset
 
-    def get_km_priors(self):
+    def get_km_priors(self, **kwargs):
+        kwargs['maxfev'] = 1000  # give a large number of tries for fitting the kmeans cluster centers
+
         shape = self.folded_dataset.shape  # We get the shape of the folded dataset
         # Our prior_dset will have the same shape except for the last dimension whose size will be equal to number of
         # fitting parameters
         dim_order = [[0], [i + 1 for i in range(len(shape) - 1)]]
         # We are using the fold function in case we have a multidimensional fit.
         # In that case we need all the spectral dimensions collapsed into a single dimension for kMeans
         # In case of a 1D fit the next line essentially does nothing.
         km_dset = self.folded_dataset.fold(dim_order)
 
+        if self._complex_data:
+            print('Warning: complex dataset detected. For Kmeans priors, we will treat real part only')
+            km_dset = km_dset.real
+
         if KMeans is None:
             raise ModuleNotFoundError("sklearn is not installed")
         else:
             if self.n_clus is None:
                 self.n_clus = int(self.num_computations / 100)
             km = KMeans(n_clusters=self.n_clus, random_state=0).fit(km_dset.compute())
 
-        self.km_labels, centers = km.labels_, km.cluster_centers_
+        self.km_labels, self.km_centers = km.labels_, km.cluster_centers_
+        if self._complex_data:
+            km_dset = np.array(self.folded_dataset.fold(dim_order))
+            self.km_centers = []
+            # in the case of complex data, the centers have to be recomputed based on the labels
+            for ind_l in range(self.n_clus):
+                self.km_centers.append(np.mean(km_dset[self.km_labels == ind_l, :], axis=0))
+            self.km_centers = np.array(self.km_centers)
+
         km_priors = []
-        for i, cen in enumerate(centers):
+        for i, cen in enumerate(self.km_centers):
             if self.guess_fn is not None:
                 p0 = self.guess_fn(self.dep_vec, cen)
             else:
                 p0 = np.random.normal(loc=0.5, scale=0.1, size=self.num_fit_parms)
-
+            if self._complex_data:
+                cen = np.hstack([np.real(cen), np.imag(cen)])
             km_priors.append(SidFitter.default_curve_fit(self.fit_fn, self.dep_vec, cen, self.num_fit_parms,
                                                          return_cov=False,
-                                                         p0=p0, maxfev=10000))
+                                                         p0=p0, **kwargs))
         self.km_priors = np.array(km_priors)
         self.num_fit_parms = self.km_priors.shape[-1]
 
-    def visualize_fit_results(self, figure = None, horizontal = True):
+    def visualize_fit_results(self, figure=None, horizontal=True):
         '''
         Calls the interactive visualizer for comparing raw and fit datasets.
 
         Inputs:
             - figure: (Optional, default None) - handle to existing figure
             - horiziontal: (Optional, default True) - whether spectrum should be plotted horizontally
 
         '''
-        dset_type = self.dataset.data_type 
+        dset_type = self.dataset.data_type
         supported_types = ['SPECTRAL_IMAGE']
         if self.fitted_dset == None:
             raise NotFoundErr("No fitted dataset found. Re-run with return_fit=True to use this feature")
         if dset_type == DataType.SPECTRAL_IMAGE:
             visualizer = SpectralImageFitVisualizer(self.dataset, self.fitted_dset,
-                    figure=figure, horizontal=horizontal)
+                                                    figure=figure, horizontal=horizontal)
         else:
-            raise NotImplementedError("Data type is {} but currently we only support types {}".format(dset_type, supported_types))
-        
-        return visualizer
+            raise NotImplementedError(
+                "Data type is {} but currently we only support types {}".format(dset_type, supported_types))
 
+        return visualizer
 
     @staticmethod
     def default_curve_fit(fit_fn, xvec, yvec, num_fit_parms, return_cov=True, **kwargs):
-        xvec = np.array(xvec)
-        yvec = np.array(yvec)
-        yvec = yvec.ravel()
-        xvec = xvec.ravel()
+
+        yvec = np.array(yvec).ravel()
         if curve_fit is None:
             raise ModuleNotFoundError("scipy is not installed")
         else:
             try:
                 popt, pcov = curve_fit(fit_fn, xvec, yvec, **kwargs)
             except:
                 popt = np.zeros(num_fit_parms)
```

### Comparing `sidpy-0.11.2/sidpy/sid/dataset.py` & `sidpy-0.12.0/sidpy/sid/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 import h5py
 from enum import Enum
 
 from .dimension import Dimension, DimensionType
 from ..base.num_utils import get_slope
 from ..base.dict_utils import print_nested_dict
 from ..viz.dataset_viz import CurveVisualizer, ImageVisualizer, ImageStackVisualizer
-from ..viz.dataset_viz import SpectralImageVisualizer, FourDimImageVisualizer
+from ..viz.dataset_viz import SpectralImageVisualizer, FourDimImageVisualizer, ComplexSpectralImageVisualizer
 # from ..hdf.hdf_utils import is_editable_h5
 from .dimension import DimensionType
+from copy import deepcopy
 
 
 class DataType(Enum):
     UNKNOWN = -1
     SPECTRUM = 1
     LINE_PLOT = 2
     LINE_PLOT_FAMILY = 3
@@ -387,23 +388,24 @@
             Index of the dimension
 
         Raises
         -------
         TypeError : if ind is not an integer
         IndexError : if ind is less than 0 or greater than maximum allowed
             index for Dimension
+        ValueError: if name is not 'none' and is already used.
         """
         if not isinstance(ind, int):
             raise TypeError('Dimension must be an integer')
         if (0 > ind) or (ind >= self.ndim):
             raise IndexError('Dimension must be an integer between 0 and {}'
                              ''.format(self.ndim - 1))
         for key, dim in self._axes.items():
             if key != ind:
-                if name == dim.name:
+                if name != 'none' and name == dim.name:
                     raise ValueError('name: {} already used, but must be unique'.format(name))
 
     def rename_dimension(self, ind, name):
         """
         Renames Dimension at the specified index
 
         Parameters
@@ -544,15 +546,18 @@
                 # plt.show()
             elif self.data_type == DataType.IMAGE_MAP:
                 pass
             elif self.data_type == DataType.IMAGE_STACK:
                 self.view = ImageStackVisualizer(self, figure=figure, **kwargs)
                 # plt.show()
             elif self.data_type == DataType.SPECTRAL_IMAGE:
-                self.view = SpectralImageVisualizer(self, figure=figure, **kwargs)
+                if 'complex' in self.dtype.name:
+                    self.view = ComplexSpectralImageVisualizer(self, figure=figure, **kwargs)
+                else:
+                    self.view = SpectralImageVisualizer(self, figure=figure, **kwargs)
                 # plt.show()
             else:
                 raise NotImplementedError('Datasets with data_type {} cannot be plotted, yet.'.format(self.data_type))
         elif len(self.shape) == 4:
             if verbose:
                 print('4D dataset')
             if self.data_type == DataType.IMAGE:
@@ -907,14 +912,39 @@
             fft_dset.set_dimension(axes[1],
                                    Dimension(np.fft.fftshift(np.fft.fftfreq(self.shape[axes[1]],
                                                                             d=get_slope(self._axes[axes[1]].values))),
                                              name='v', units=units_y, dimension_type=new_dimension_type,
                                              quantity='reciprocal_length'))
         return fft_dset
 
+    def flatten_complex(self):
+        '''
+        This function returns a dataset with real and imaginary components that have been flattened
+        This is necessary for scenarios such as fitting of complex functions
+        Must be a 2D or 1D dataset to begin with
+        Output:
+        - ouput_arr: sidpy.Dataset object
+        '''
+        assert self.ndim < 3, "flatten_complex() only works on 1D or 2D datasets, current dataset has {}".format(
+            self.ndim)
+        # Only the second dimension needs to be changed
+        # Because we are stacking real and imaginary, this means we just tile the existing axis values
+        if len(self._axes) == 1:
+            index_ax = 0
+        elif len(self._axes) == 2:
+            index_ax = 1
+        new_ax_values = np.tile(self._axes[index_ax].values, 2)
+        output_arr = self.like_data(dask.array.hstack([self.real, self.imag]))
+        output_arr.set_dimension(index_ax, Dimension(new_ax_values, name=output_arr._axes[index_ax].name,
+                                                     units=output_arr._axes[index_ax].units,
+                                                     dimension_type=output_arr._axes[index_ax].dimension_type,
+                                                     quantity=output_arr._axes[index_ax].quantity))
+
+        return output_arr
+
     # #####################################################
     # Original dask.array functions replaced
     # ##################################################
 
     def __eq__(self, other):  # TODO: Test __eq__
         if not isinstance(other, Dataset):
             return False
@@ -1393,15 +1423,14 @@
 
         return dataset
 
     def choose(self, choices):
         return self.like_data(super().choose(choices))
 
     def __abs__(self):
-        print(super().__abs__.__name__)
         return self.like_data(super().__abs__(), title_suffix='_absolute_value')
 
     def __add__(self, other):
         return self.like_data(super().__add__(other))
 
     def __radd__(self, other):
         return self.like_data(super().__radd__(other))
@@ -1420,14 +1449,69 @@
 
     def __gt__(self, other):
         return self.like_data(super().__gt__(other))
 
     def __ge__(self, other):
         return self.like_data(super().__ge__(other))
 
+    def __getitem__(self, idx):
+
+        # Here we need to modify the dimensions of the sliced dataset using the argument index
+        if not isinstance(idx, tuple):
+            # This comes into play when slicing is done using 'None' or just integers.
+            # For example: dset[4] or dset[None]
+            idx = tuple([idx])
+
+        # The following line creates a new sidpy dataset with generic dimensions and ..
+        # all the other attributes copied from 'self' aka parent dataset.
+        sliced = self.like_data(super().__getitem__(idx), checkdims=False)
+
+        # Delete the dimensions created by like_data
+        sliced._axes.clear()
+
+        old_dims = deepcopy(self._axes)
+        j, k = 0, 0  # j is for self (old_dims) and k is for the sliced dataset (new dimensions)
+
+        for ind in idx:
+            if ind is None:  # Add a new dimension
+                sliced.set_dimension(k, Dimension(1))
+                k += 1
+            elif isinstance(ind, (int, np.integer)):
+                j += 1
+            elif isinstance(ind, (slice, np.ndarray, list)):
+                old_dim = old_dims[j]
+                sliced.set_dimension(k, Dimension(old_dim[ind],
+                                                  name=old_dim.name, quantity=old_dim.quantity,
+                                                  units=old_dim.units,
+                                                  dimension_type=old_dim.dimension_type))
+                j += 1
+                k += 1
+            elif ind is Ellipsis:
+                start_dim = idx.index(Ellipsis)
+                ellipsis_dims = sliced.ndim - (len(idx) - 1)
+                stop_dim = start_dim + ellipsis_dims
+
+                for l in range(start_dim, stop_dim):
+                    old_dim = old_dims[j]
+                    sliced.set_dimension(k, old_dim)
+                    j += 1
+                    k += 1
+
+        # Adding the rest of the dimensions
+        for k in range(k, sliced.ndim):
+            old_dim = old_dims[j]
+            sliced.set_dimension(k, Dimension(old_dim,
+                                              name=old_dim.name, quantity=old_dim.quantity,
+                                              units=old_dim.units,
+                                              dimension_type=old_dim.dimension_type))
+            j += 1
+            k += 1
+
+        return sliced
+
     def __invert__(self):
         return self.like_data(super().__invert__())
 
     def __lshift__(self, other):
         return self.like_data(super().__lshift__(other))
 
     def __rlshift__(self, other):
```

### Comparing `sidpy-0.11.2/sidpy/sid/dimension.py` & `sidpy-0.12.0/sidpy/sid/dimension.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/sid/reader.py` & `sidpy-0.12.0/sidpy/sid/reader.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/sid/translator.py` & `sidpy-0.12.0/sidpy/sid/translator.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/viz/dataset_viz.py` & `sidpy-0.12.0/sidpy/viz/dataset_viz.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.dim = self.dset._axes[self.spectral_dims[0]]
 
         if is_complex_dtype(dset.dtype):
             # Plot real and imaginary
             self.fig, self.axes = plt.subplots(nrows=2, **fig_args)
 
-            self.axes[0].plot(self.dim.values, self.dset.squeeze().abs(), **kwargs)
+            self.axes[0].plot(self.dim.values, self.dset.squeeze().abs().compute(), **kwargs)
             if set_title:
                 self.axes[0].set_title(self.dset.title + '\n(Magnitude)', pad=15)
             self.axes[0].set_xlabel(self.dset.labels[0])
             self.axes[0].set_ylabel(self.dset.data_descriptor)
             self.axes[0].ticklabel_format(style='sci', scilimits=(-2, 3))
 
             if set_title:
@@ -89,15 +89,15 @@
             self.axes[1].ticklabel_format(style='sci', scilimits=(-2, 3))
 
             self.fig.tight_layout()
             self.fig.canvas.draw_idle()
 
         else:
             self.axis = self.fig.add_subplot(1, 1, 1, **fig_args)
-            self.axis.plot(self.dim.values, self.dset, **kwargs)
+            self.axis.plot(self.dim.values, self.dset.compute(), **kwargs)
             if set_title:
                 self.axis.set_title(self.dset.title, pad=15)
             self.axis.set_xlabel(self.dset.labels[self.spectral_dims[0]])
             self.axis.set_ylabel(self.dset.data_descriptor)
             self.axis.ticklabel_format(style='sci', scilimits=(-2, 3))
             self.fig.canvas.draw_idle()
 
@@ -586,15 +586,15 @@
                                       facecolor='red', alpha=0.2)
 
         self.axes[0].add_patch(self.rect)
         self.intensity_scale = 1.
         self.spectrum = self.get_spectrum()
         if len(self.energy_scale)!=self.spectrum.shape[0]:
             self.spectrum = self.spectrum.T
-        self.axes[1].plot(self.energy_scale, self.spectrum)
+        self.axes[1].plot(self.energy_scale, self.spectrum.compute())
         self.axes[1].set_title('spectrum {}, {}'.format(self.x, self.y))
         self.xlabel = self.dset.labels[self.spec_dim]
         self.ylabel = self.dset.data_descriptor
         self.axes[1].set_xlabel(self.dset.labels[self.spec_dim])  # + x_suffix)
         self.axes[1].set_ylabel(self.dset.data_descriptor)
         self.axes[1].ticklabel_format(style='sci', scilimits=(-2, 3))
         self.fig.tight_layout()
@@ -637,15 +637,15 @@
         if self.x > self.dset.shape[self.image_dims[0]] - self.bin_x:
             self.x = self.dset.shape[self.image_dims[0]] - self.bin_x
         if self.y > self.dset.shape[self.image_dims[1]] - self.bin_y:
             self.y = self.dset.shape[self.image_dims[1]] - self.bin_y
         selection = []
 
         for dim, axis in self.dset._axes.items():
-            print(dim, axis.dimension_type)
+            # print(dim, axis.dimension_type)
             if axis.dimension_type == DimensionType.SPATIAL:
                 if dim == self.image_dims[0]:
                     selection.append(slice(self.x, self.x + self.bin_x))
                 else:
                     selection.append(slice(self.y, self.y + self.bin_y))
 
             elif axis.dimension_type == DimensionType.SPECTRAL:
@@ -701,15 +701,15 @@
 
         xlim = self.axes[1].get_xlim()
         ylim = self.axes[1].get_ylim()
         self.axes[1].clear()
         self.get_spectrum()
         if len(self.energy_scale)!=self.spectrum.shape[0]:
             self.spectrum = self.spectrum.T
-        self.axes[1].plot(self.energy_scale, self.spectrum, label='experiment')
+        self.axes[1].plot(self.energy_scale, self.spectrum.compute(), label='experiment')
 
         if self.set_title:
             self.axes[1].set_title('spectrum {}, {}'.format(self.x, self.y))
 
         self.axes[1].set_xlim(xlim)
         #self.axes[1].set_ylim(ylim)
         self.axes[1].set_xlabel(self.xlabel)
@@ -721,14 +721,15 @@
         self.plot_legend = set_legend
 
     def get_xy(self):
         return [self.x, self.y]
 
 
 class FourDimImageVisualizer(object):
+    
     """
     ### Interactive 4D imaging plot
 
     Either you specify only two spatial dimensions or you specify
     scan_x and scan_y
     image_4d_x, image_4d_y
 
@@ -870,15 +871,15 @@
             self.axes[1].set_title('set {}, {}'.format(self.x, self.y))
         self.xlabel = self.dset.labels[self.dims_4d[0]]
         self.ylabel = self.dset.labels[self.dims_4d[1]]
         self.axes[1].set_xlabel(self.xlabel)  # + x_suffix)
         self.axes[1].set_ylabel(self.ylabel)
         self.axes[1].ticklabel_format(style='sci', scilimits=(-2, 3))
         if is_complex_dtype(dset.dtype):
-            self.axes[2].imshow(np.angle(self.image_4d))
+            self.axes[2].imshow(np.angle(np.array(self.image_4d)))
             if self.set_title:
                 self.axes[1].set_title('power {}, {}'.format(self.x, self.y))
                 self.axes[2].set_title('phase {}, {}'.format(self.x, self.y))
             self.axes[2].set_xlabel(self.xlabel)  # + x_suffix)
             self.axes[2].set_ylabel(self.ylabel)
             self.axes[2].ticklabel_format(style='sci', scilimits=(-2, 3))
             
@@ -1003,14 +1004,311 @@
         return [self.x, self.y]
 
 
 #Let's make a 
 
 #Let's make a curve fit visualizer
 
+class ComplexSpectralImageVisualizer(object):
+    """
+    ### Interactive spectrum imaging plot for Complex Data
+
+    """
+
+    def __init__(self, dset, figure=None, horizontal=True, **kwargs):
+        from ..sid.dataset import Dataset
+        from ..sid.dimension import DimensionType
+        import matplotlib.widgets
+
+        if not isinstance(dset, Dataset):
+            raise TypeError('dset should be a sidpy.Dataset object')
+        
+        scale_bar = kwargs.pop('scale_bar', False)
+        colorbar = kwargs.pop('colorbar', True)
+        self.set_title = kwargs.pop('set_title', True)
+        
+        fig_args = dict()
+        temp = kwargs.pop('figsize', None)
+        if temp is not None:
+            fig_args['figsize'] = temp
+
+        if figure is None:
+            self.fig = plt.figure(**fig_args)
+        else:
+            self.fig = figure
+
+        if len(dset.shape) !=3:
+            raise TypeError('dataset must have three dimensions')
+        if 'complex' not in dset.dtype.name:
+            raise TypeError('This visualizer is only for Complex Data, data type is {}'.format(dset.dtype))
+        
+        # We need one stack dim and two image dimes as lists in dictionary
+        selection = []
+        image_dims = []
+        spectral_dim = []
+        channel_dim = []
+        for dim, axis in dset._axes.items():
+            if axis.dimension_type in [DimensionType.SPATIAL, DimensionType.RECIPROCAL]:
+                selection.append(slice(None))
+                image_dims.append(dim)
+            elif axis.dimension_type == DimensionType.SPECTRAL:
+                selection.append(slice(0, 1))
+                spectral_dim.append(dim)
+            elif axis.dimension_type == DimensionType.CHANNEL:
+                channel_dim.append(dim)
+            else:
+                selection.append(slice(0, 1))
+        
+        if len(image_dims) != 2:
+            raise TypeError('We need two dimensions with dimension_type SPATIAL: to plot an image')
+        if len(channel_dim) >1:
+            raise ValueError("We have more than one Channel Dimension, this won't work for the visualizer")
+        if len(spectral_dim)>1:
+            raise ValueError("We have more than one Spectral Dimension, this won't work for the visualizer...")
+
+        if len(dset.shape)==4:
+            if len(channel_dim)!=1:
+                raise TypeError("We need one dimension with type CHANNEL \
+                    for a spectral image plot for a 4D dataset")
+        elif len(dset.shape)==3:
+            if len(spectral_dim) != 1:
+                raise TypeError("We need one dimension with dimension_type SPECTRAL \
+                 to plot a spectra for a 3D dataset")
+
+        self.horizontal = horizontal
+        self.x = 0
+        self.y = 0
+        self.bin_x = 1
+        self.bin_y = 1
+
+        size_x = dset.shape[image_dims[0]]
+        size_y = dset.shape[image_dims[1]]
+
+        self.dset = dset
+        self.energy_axis = spectral_dim[0]
+        if len(channel_dim)>0: self.channel_axis = channel_dim
+        self.energy_scale = dset._axes[self.energy_axis].values
+        self.extent = [0, size_x, size_y, 0]
+        self.rectangle = [0, size_x, 0, size_y]
+        self.scaleX = 1.0
+        self.scaleY = 1.0
+        self.analysis = []
+        self.plot_legend = False
+        self.ri_ap = 'Real and Imaginary' #real/imaginary of amplitude/phase plotting
+
+        self.image_dims = image_dims
+        self.spec_dim = spectral_dim[0]
+
+        if horizontal:
+            self.axes = self.fig.subplots(ncols=3)
+        else:
+            self.axes = self.fig.subplots(nrows=3, **fig_args)
+
+        if self.set_title:
+            self.fig.canvas.manager.set_window_title(self.dset.title)
+
+        if len(channel_dim)>0:
+            self.image = dset.mean(axis=(spectral_dim[0],channel_dim[0]))
+        else:
+            self.image = dset.mean(axis=(spectral_dim[0]))
+
+        if 1 in self.dset.shape:
+            self.image = dset.squeeze()
+            self.axes[0].set_aspect('auto')
+        else:
+            self.axes[0].set_aspect('equal')
+
+        self.axes[0].imshow(np.abs(self.image.T), extent=self.extent, **kwargs)
+        if horizontal:
+            self.axes[0].set_xlabel('{} [pixels]'.format(self.dset._axes[image_dims[0]].quantity))
+        else:
+            self.axes[0].set_ylabel('{} [pixels]'.format(self.dset._axes[image_dims[1]].quantity))
+
+        if 1 in self.dset.shape:
+            self.axes[0].set_aspect('auto')
+            self.axes[0].get_yaxis().set_visible(False)
+        else:
+            self.axes[0].set_aspect('equal')
+
+        self.rect = patches.Rectangle((0, 0), self.bin_x, self.bin_y, linewidth=1, edgecolor='r',
+                                      facecolor='red', alpha=0.2)
+
+        self.axes[0].add_patch(self.rect)
+        self.intensity_scale = 1.
+        self.spectrum = self.get_spectrum()
+        if len(self.energy_scale)!=self.spectrum.shape[0]:
+            self.spectrum = self.spectrum.T
+        self.axes[1].plot(self.energy_scale, np.real(self.spectrum.compute()), label = 'Real')
+        self.axes[2].plot(self.energy_scale, np.imag(self.spectrum.compute()), label = 'Imaginary')
+        for ax_ind in [1,2]:
+            self.axes[ax_ind].set_title('spectrum {}, {}'.format(self.x, self.y))
+            self.xlabel = self.dset.labels[self.spec_dim]
+            self.ylabel = self.dset.data_descriptor
+            self.axes[ax_ind].set_xlabel(self.dset.labels[self.spec_dim])  # + x_suffix)
+            self.axes[ax_ind].set_ylabel(self.dset.data_descriptor)
+            self.axes[ax_ind].ticklabel_format(style='sci', scilimits=(-2, 3))
+            leg = self.axes[ax_ind].legend(loc = 'best')
+            leg.get_frame().set_linewidth(0.0)
+        self.fig.tight_layout()
+        self.cid = self.axes[1].figure.canvas.mpl_connect('button_press_event', self._onclick)
+        import ipywidgets as iwgt
+        self.button = iwgt.widgets.Dropdown(options=['Real and Imaginary', 'Amplitude and Phase'],
+                                description='Plot',
+                                disabled=False,
+                                tooltip='How to plot complex data')
+
+        self.button.observe(self._ri_ap, 'value') #real/imag or amp/phase
+
+        widg = iwgt.HBox([self.button])
+        from IPython.display import display
+        display(widg)
+
+        self.fig.canvas.draw_idle()
+
+    def _ri_ap(self, event):
+        self.ri_ap = event.new
+        self._update()
+
+    def set_bin(self, bin_xy):
+
+        old_bin_x = self.bin_x
+        old_bin_y = self.bin_y
+        if isinstance(bin_xy, list):
+
+            self.bin_x = int(bin_xy[0])
+            self.bin_y = int(bin_xy[1])
+
+        else:
+            self.bin_x = int(bin_xy)
+            self.bin_y = int(bin_xy)
+
+        if self.bin_x > self.dset.shape[self.image_dims[0]]:
+            self.bin_x = self.dset.shape[self.image_dims[0]]
+        if self.bin_y > self.dset.shape[self.image_dims[1]]:
+            self.bin_y = self.dset.shape[self.image_dims[1]]
+
+        self.rect.set_width(self.rect.get_width() * self.bin_x / old_bin_x)
+        self.rect.set_height((self.rect.get_height() * self.bin_y / old_bin_y))
+        if self.x + self.bin_x > self.dset.shape[self.image_dims[0]]:
+            self.x = self.dset.shape[0] - self.bin_x
+        if self.y + self.bin_y > self.dset.shape[self.image_dims[1]]:
+            self.y = self.dset.shape[1] - self.bin_y
+
+        self.rect.set_xy([self.x * self.rect.get_width() / self.bin_x + self.rectangle[0],
+                          self.y * self.rect.get_height() / self.bin_y + self.rectangle[2]])
+        self._update()
+
+    def get_spectrum(self):
+        from ..sid.dimension import DimensionType
+
+        if self.x > self.dset.shape[self.image_dims[0]] - self.bin_x:
+            self.x = self.dset.shape[self.image_dims[0]] - self.bin_x
+        if self.y > self.dset.shape[self.image_dims[1]] - self.bin_y:
+            self.y = self.dset.shape[self.image_dims[1]] - self.bin_y
+        selection = []
+
+        for dim, axis in self.dset._axes.items():
+            # print(dim, axis.dimension_type)
+            if axis.dimension_type == DimensionType.SPATIAL:
+                if dim == self.image_dims[0]:
+                    selection.append(slice(self.x, self.x + self.bin_x))
+                else:
+                    selection.append(slice(self.y, self.y + self.bin_y))
+
+            elif axis.dimension_type == DimensionType.SPECTRAL:
+                selection.append(slice(None))
+            elif axis.dimension_type == DimensionType.CHANNEL:
+                selection.append(slice(None))
+            else:
+                selection.append(slice(0, 1))
+        
+        self.spectrum = self.dset[tuple(selection)].mean(axis=tuple(self.image_dims))
+        
+        # * self.intensity_scale[self.x,self.y]
+        return self.spectrum.squeeze()
+
+    def _onclick(self, event):
+        self.event = event
+        if event.inaxes in [self.axes[0]]:
+            x = int(event.xdata)
+            y = int(event.ydata)
+
+            x = int(x - self.rectangle[0])
+            y = int(y - self.rectangle[2])
+
+            if x >= 0 and y >= 0:
+                if x <= self.rectangle[1] and y <= self.rectangle[3]:
+                    self.x = int(x / (self.rect.get_width() / self.bin_x))
+                    self.y = int(y / (self.rect.get_height() / self.bin_y))
+
+                    if self.x + self.bin_x > self.dset.shape[self.image_dims[0]]:
+                        self.x = self.dset.shape[self.image_dims[0]] - self.bin_x
+                    if self.y + self.bin_y > self.dset.shape[self.image_dims[1]]:
+                        self.y = self.dset.shape[self.image_dims[1]] - self.bin_y
+
+                    self.rect.set_xy([self.x * self.rect.get_width() / self.bin_x + self.rectangle[0],
+                                      self.y * self.rect.get_height() / self.bin_y + self.rectangle[2]])
+            self._update()
+        else:
+            if event.dblclick:
+                bottom = float(self.spectrum.min())
+                if bottom < 0:
+                    bottom *= 1.02
+                else:
+                    bottom *= 0.98
+                top = float(self.spectrum.max())
+                if top > 0:
+                    top *= 1.02
+                else:
+                    top *= 0.98
+
+                self.axes[1].set_ylim(bottom=bottom, top=top)
+
+    def _update(self, ev=None):
+
+        xlim_ax1 = self.axes[1].get_xlim()
+        ylim_ax1 = self.axes[1].get_ylim()
+        xlim_ax2 = self.axes[2].get_xlim()
+        ylim_ax2 = self.axes[2].get_ylim()
+        
+        xlims = [xlim_ax1,xlim_ax2]
+        ylims = [ylim_ax1, ylim_ax2]
+
+        self.axes[1].clear()
+        self.axes[2].clear()
+        self.get_spectrum()
+        if len(self.energy_scale)!=self.spectrum.shape[0]:
+            self.spectrum = self.spectrum
+        
+        if self.ri_ap == 'Real and Imaginary':
+            self.axes[1].plot(self.energy_scale, np.real(self.spectrum.compute()), label='Real')
+            self.axes[2].plot(self.energy_scale, np.imag(self.spectrum.compute()), label='Imaginary')
+        else:
+            self.axes[1].plot(self.energy_scale, np.abs(self.spectrum.compute()), label='Amplitude')
+            self.axes[2].plot(self.energy_scale, np.angle(self.spectrum.compute()), label='Phase')
+
+        for ind,ax_ind in enumerate([1,2]):
+            if self.set_title:
+                self.axes[ax_ind].set_title('spectrum {}, {}'.format(self.x, self.y))
+            
+            self.axes[ax_ind].set_xlim(xlims[ind])
+            self.axes[ax_ind].set_xlabel(self.xlabel)
+            self.axes[ax_ind].set_ylabel(self.ylabel)
+            leg = self.axes[ax_ind].legend(loc = 'best')
+            leg.get_frame().set_linewidth(0.0)
+        self.fig.canvas.draw_idle()
+        self.fig.tight_layout()
+
+    def set_legend(self, set_legend):
+        self.plot_legend = set_legend
+
+    def get_xy(self):
+        return [self.x, self.y]
+
+
 class SpectralImageFitVisualizer(SpectralImageVisualizer):
     
     def __init__(self, original_dataset, fit_dataset, figure=None, horizontal=True):
         '''
         Visualizer for spectral image datasets, fit by the Sidpy Fitter
         This class is called by Sidpy Fitter for visualizing the raw/fit dataset interactively.
 
@@ -1047,16 +1345,16 @@
                     selection.append(slice(self.y, self.y + self.bin_y))
 
             elif axis.dimension_type == DimensionType.SPECTRAL:
                 selection.append(slice(None))
             else:
                 selection.append(slice(0, 1))
 
-        self.spectrum = self.dset[tuple(selection)].mean(axis=tuple(self.image_dims))
-        self.fit_spectrum = self.fit_dset[tuple(selection)].mean(axis=tuple(self.image_dims))
+        self.spectrum = np.array(self.dset[tuple(selection)].mean(axis=tuple(self.image_dims)))
+        self.fit_spectrum = np.array(self.fit_dset[tuple(selection)].mean(axis=tuple(self.image_dims)))
         # * self.intensity_scale[self.x,self.y]
         
         return self.fit_spectrum.squeeze(), self.spectrum.squeeze()
         
         
     def _update(self, ev=None):
```

### Comparing `sidpy-0.11.2/sidpy/viz/jupyter_utils.py` & `sidpy-0.12.0/sidpy/viz/jupyter_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     spec_dim_names = [item.name for item in spec_dims]
 
     # ################################## HELPER FUNCTIONS ##############################################################
 
     def check_data_type(data_mat):
         if data_mat.dtype.names is not None:
             return 2, list(data_mat.dtype.names), None
-        if data_mat.dtype in [np.complex64, np.complex128, np.complex]:
+        if data_mat.dtype in [np.complex64, np.complex128, complex]:
             return 1, ['Real', 'Imaginary', 'Amplitude', 'Phase'], [np.real, np.imag, np.abs, np.angle]
         else:
             return 0, None, None
 
     def get_clims(data, stdev=2):
         avg = np.mean(data)
         std = np.std(data)
```

### Comparing `sidpy-0.11.2/sidpy/viz/plot_utils/cmap.py` & `sidpy-0.12.0/sidpy/viz/plot_utils/cmap.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.11.2/sidpy/viz/plot_utils/curve.py` & `sidpy-0.12.0/sidpy/viz/plot_utils/curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,16 +345,18 @@
 
     if evenly_spaced:
         chosen_pos = np.linspace(0, num_pos - 1, nrows * ncols, dtype=int)
     else:
         chosen_pos = np.arange(nrows * ncols, dtype=int)
 
     fig, axes = plt.subplots(nrows=nrows, ncols=ncols, sharex=True, figsize=(12, 12))
-    axes_lin = axes.flatten()
-
+    if type(axes)==np.ndarray:
+        axes_lin = axes.flatten()
+    else: axes_lin = [axes]
+    
     for count, posn in enumerate(chosen_pos):
         if use_rainbow_plots:
             rainbow_plot(axes_lin[count], excit_wfms[0], datasets[0][posn], **kwargs)
         else:
             for dataset, ex_wfm, col_val in zip(datasets, excit_wfms, line_colors):
                 axes_lin[count].plot(ex_wfm, dataset[posn], color=col_val, **kwargs)
         if h5_pos is not None:
```

### Comparing `sidpy-0.11.2/sidpy/viz/plot_utils/image.py` & `sidpy-0.12.0/sidpy/viz/plot_utils/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         Keyword arguments to be passed to either matplotlib.pyplot.figure, mpl_toolkits.axes_grid1.ImageGrid, or
         pyUSID.viz.plot_utils.plot_map.  See specific function documentation for the relavent options.
 
     Returns
     ---------
     fig, axes
     """
-    plt.rcParams["mpl_toolkits.legacy_colorbar"] = False
+#    plt.rcParams["mpl_toolkits.legacy_colorbar"] = False
 
     if not isinstance(map_stack, (np.ndarray, da.core.Array)) or not map_stack.ndim == 3:
         raise TypeError('map_stack should be a 3 dimensional array arranged as [component, row, col]')
     if num_comps is None:
         num_comps = 4  # Default
     else:
         if not isinstance(num_comps, int) or num_comps < 1:
@@ -381,22 +381,25 @@
             igkwargs.update({key: kwargs.pop(key)})
 
     axes = ImageGrid(fig=fig, rect=111, nrows_ncols=(p_rows, p_cols),
                      cbar_mode=color_bar_mode,
                      axes_pad=(pad_w * fig_w, pad_h * fig_h),
                      **igkwargs)
 
-    fig.canvas.set_window_title(title)
+    try:
+        fig.canvas.set_window_title(title)
+    except:
+        fig.canvas.manager.set_window_title(title)
     # These parameters have not been easy to fix:
     if title_yoffset is None:
         title_yoffset = 0.9
     if title_size is None:
         title_size = 16 + (p_rows + p_cols)
     fig.suptitle(title, fontsize=title_size, y=title_yoffset)
-    plt.rcParams["mpl_toolkits.legacy_colorbar"] = False
+#    plt.rcParams["mpl_toolkits.legacy_colorbar"] = False
 
     for count, index, curr_subtitle in zip(range(chosen_pos.size), chosen_pos, subtitle):
         im, im_cbar = plot_map(axes[count],
                                map_stack[index],
                                stdevs=stdevs, show_cbar=False, **kwargs)
         axes[count].set_title(curr_subtitle)
```

### Comparing `sidpy-0.11.2/sidpy/viz/plot_utils/misc.py` & `sidpy-0.12.0/sidpy/viz/plot_utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 
         Parameters
         ----------
         axis : matplotlib.axes.Axes object
             axis to set font sizes
         """
         for tick in axis.xaxis.get_major_ticks():
-            tick.label.set_fontsize(font_size)
+            tick.label1.set_fontsize(font_size)
         for tick in axis.yaxis.get_major_ticks():
-            tick.label.set_fontsize(font_size)
+            tick.label1.set_fontsize(font_size)
 
     mesg = 'axes must either be a matplotlib.axes.Axes object or an iterable containing such objects'
 
     if hasattr(axes, '__iter__'):
         for axis in axes:
             assert isinstance(axis, mpl.axes.Axes), mesg
             __set_axis_tick(axis)
```

### Comparing `sidpy-0.11.2/sidpy.egg-info/PKG-INFO` & `sidpy-0.12.0/sidpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidpy
-Version: 0.11.2
+Version: 0.12.0
 Summary: Python utilities for storing, visualizing, and processing Spectroscopic and Imaging Data (SID)
 Home-page: https://pycroscopy.github.io/sidpy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific,visualization,processing,storage,hdf5
 Platform: Linux
```

### Comparing `sidpy-0.11.2/sidpy.egg-info/SOURCES.txt` & `sidpy-0.12.0/sidpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/my-favorite-things-0.2.0.tar.gz` & `tmp/my-favorite-things-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-favorite-things-0.2.0.tar", last modified: Wed May 31 17:37:40 2023, max compression
+gzip compressed data, was "my-favorite-things-0.3.0.tar", last modified: Mon Jul  3 21:12:59 2023, max compression
```

## Comparing `my-favorite-things-0.2.0.tar` & `my-favorite-things-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/
--rw-r--r--   0 person    (1000) person    (1000)       66 2023-05-30 23:22:20.000000 my-favorite-things-0.2.0/.gitattributes
--rw-r--r--   0 person    (1000) person    (1000)       55 2023-05-31 01:19:47.000000 my-favorite-things-0.2.0/.gitignore
--rw-r--r--   0 person    (1000) person    (1000)    35149 2023-05-31 00:09:30.000000 my-favorite-things-0.2.0/LICENSE
--rw-r--r--   0 person    (1000) person    (1000)    42724 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)     1509 2023-05-31 17:34:57.000000 my-favorite-things-0.2.0/README.md
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 17:37:40.268227 my-favorite-things-0.2.0/my_favorite_things/
--rw-r--r--   0 person    (1000) person    (1000)      206 2023-05-31 17:26:01.000000 my-favorite-things-0.2.0/my_favorite_things/__init__.py
--rw-r--r--   0 person    (1000) person    (1000)     1328 2023-05-31 17:22:59.000000 my-favorite-things-0.2.0/my_favorite_things/ddicts.py
--rw-r--r--   0 person    (1000) person    (1000)     5189 2023-05-31 02:11:08.000000 my-favorite-things-0.2.0/my_favorite_things/save.py
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/my_favorite_things.egg-info/
--rw-r--r--   0 person    (1000) person    (1000)    42724 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)      354 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/SOURCES.txt
--rw-r--r--   0 person    (1000) person    (1000)        1 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/dependency_links.txt
--rw-r--r--   0 person    (1000) person    (1000)       37 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/requires.txt
--rw-r--r--   0 person    (1000) person    (1000)       19 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/top_level.txt
--rw-r--r--   0 person    (1000) person    (1000)      919 2023-05-31 17:26:26.000000 my-favorite-things-0.2.0/pyproject.toml
--rw-r--r--   0 person    (1000) person    (1000)       38 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/setup.cfg
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-07-03 21:12:59.863356 my-favorite-things-0.3.0/
+-rw-r--r--   0 person    (1000) person    (1000)       66 2023-05-30 23:22:20.000000 my-favorite-things-0.3.0/.gitattributes
+-rw-r--r--   0 person    (1000) person    (1000)       76 2023-06-20 21:02:31.000000 my-favorite-things-0.3.0/.gitignore
+-rw-r--r--   0 person    (1000) person    (1000)    35149 2023-05-31 00:09:30.000000 my-favorite-things-0.3.0/LICENSE
+-rw-r--r--   0 person    (1000) person    (1000)    44192 2023-07-03 21:12:59.863356 my-favorite-things-0.3.0/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)     2977 2023-06-23 14:42:45.000000 my-favorite-things-0.3.0/README.md
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-07-03 21:12:59.860023 my-favorite-things-0.3.0/my_favorite_things/
+-rw-r--r--   0 person    (1000) person    (1000)      332 2023-06-23 14:21:43.000000 my-favorite-things-0.3.0/my_favorite_things/__init__.py
+-rw-r--r--   0 person    (1000) person    (1000)     1495 2023-07-03 21:03:29.000000 my-favorite-things-0.3.0/my_favorite_things/ddicts.py
+-rw-r--r--   0 person    (1000) person    (1000)     4867 2023-06-23 14:20:20.000000 my-favorite-things-0.3.0/my_favorite_things/plot.py
+-rw-r--r--   0 person    (1000) person    (1000)     5348 2023-06-12 17:06:54.000000 my-favorite-things-0.3.0/my_favorite_things/save.py
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-07-03 21:12:59.863356 my-favorite-things-0.3.0/my_favorite_things.egg-info/
+-rw-r--r--   0 person    (1000) person    (1000)    44192 2023-07-03 21:12:59.000000 my-favorite-things-0.3.0/my_favorite_things.egg-info/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)      381 2023-07-03 21:12:59.000000 my-favorite-things-0.3.0/my_favorite_things.egg-info/SOURCES.txt
+-rw-r--r--   0 person    (1000) person    (1000)        1 2023-07-03 21:12:59.000000 my-favorite-things-0.3.0/my_favorite_things.egg-info/dependency_links.txt
+-rw-r--r--   0 person    (1000) person    (1000)       37 2023-07-03 21:12:59.000000 my-favorite-things-0.3.0/my_favorite_things.egg-info/requires.txt
+-rw-r--r--   0 person    (1000) person    (1000)       19 2023-07-03 21:12:59.000000 my-favorite-things-0.3.0/my_favorite_things.egg-info/top_level.txt
+-rw-r--r--   0 person    (1000) person    (1000)      919 2023-07-03 21:10:37.000000 my-favorite-things-0.3.0/pyproject.toml
+-rw-r--r--   0 person    (1000) person    (1000)       38 2023-07-03 21:12:59.863356 my-favorite-things-0.3.0/setup.cfg
```

### Comparing `my-favorite-things-0.2.0/LICENSE` & `my-favorite-things-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `my-favorite-things-0.2.0/PKG-INFO` & `my-favorite-things-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-favorite-things
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convenient functions and classes I use too often.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,41 +695,63 @@
 
 ## Installation
 Install with
 ```
 pip install my-favorite-things
 ```
 
-## Current Methods
+## Current Methods (by file)
 ### save
-#### `save()`
-Import by
-```
+#### `save(name, savedir="", savepath="", stype="npz", absolute=False, parents=0, overwrite=False, append=False, dryrun=False, save_kwargs={}, **kwargs)`
+**Import by**
+```python
 from my_favorite_things import save
 ```
-This method is used for saving data to a file. You can save as an `.npz` file for numpy array(s) or as a `.pkl` file for dictionaries and other odd python objects. By default, it will not overwrite existing files but instead append a number onto the end of file name (the keywords being, by default, `overwite=False` and `append=True`). You can save relative to your current directory (`absolute=False`) or as an absolute path (`absolute=True`). Addtionally, double check that you're saving to the correct directory with `dryrun=True`. Check the doc string for more info.
+This method is used for saving data to a file. You can save as an `.npz`/`.npy` file for numpy array(s) or as a `.pkl` file for dictionaries and other odd python objects. By default, it will not overwrite existing files but instead append a number onto the end of file name (the keywords being, by default, `overwite=False` and `append=True`). You can save relative to your current directory (`absolute=False`) or as an absolute path (`absolute=True`). Addtionally, double check that you're saving to the correct directory with `dryrun=True`. Check the doc string for more info.
 
 ---
 
-### ddict
-#### `nested_ddict()`
-Import by
-```
+### ddicts
+#### `nested_ddict(depth, endtype)`
+**Import by**
+```python
 from my_favorite_things import nested_ddict
 ```
 This method allows for creating a nested defaultdictionary. This is useful if you have data that is dependent on multiple parameters that are heirarchical. For example, if we do
 ```python
 d = nested_ddict(3, list)
 ```
 then we can use it as
 ```python
 d['zero']['one']['two']['three'].append(datum)
 ```
 
-#### `format_ddict()`
-Import by
-```
+#### `format_ddict(ddict, make_nparr=True, sort_lists=False)`
+**Import by**
+```python
 from my_favorite_things import format_ddict
 ```
 This method will format your (nested) defaultdictionary into dictionaries. Additionally, it can turns lists in numpy arrays and/or sort the lists too.
 
 ---
+
+### plots
+#### `log_bins(*arrs, num_bins)`
+**Import by**
+```python
+from my_favorite_things import log_bins
+```
+This method is used for binning for histograms logarithmically. In `plt.hist`, setting the keyword `bins` to the output of this function (where `arrs` are the arrays being plotted) and `ax.set_xscale("log")` will give equally spaced bins (for multiple data sets over the logarithmic x-axis).
+
+#### `cumulative_bins(*arrs, num_bins)`
+**Import by**
+```python
+from my_favorite_things import cumulative_bins
+```
+This is similar to the previous method but for a linear scale. When plotting multiple data sets on the same plot, they may have different ranges and, thus, bin sizes. So this method will create the bin values so that the bars of the histogram will all have the same width.
+
+#### `bar_count(ax, counts, labels, label_bars, sort_type, *, bar_params, **kwargs)`
+**Import by**
+```python
+from my_favorite_things import bar_count
+```
+This method will create a bar plot for the data passed using strings as labels (either as the keys of a dictionary passed for `counts` or as a list passed from `labels`) with various conveniences like specifying the format of the label strings or the order of the plotted data.
```

### Comparing `my-favorite-things-0.2.0/my_favorite_things/ddicts.py` & `my-favorite-things-0.3.0/my_favorite_things/ddicts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 """
 This file contains methods that are related to python's defaultdict object
 from the collections package.
 """
 
 from collections import defaultdict
 from typing import Type
+
 import numpy as np
 
 
-def nested_ddict(depth: int, endtype: Type):
+def nested_ddict(depth: int, endtype: Type) -> defaultdict:
     """
     Creates defaultdict that is arbitrarily nested. For example,
     if we write `d = nested_ddict(3, list)` then we can do something
     like `d['0']['1']['2']['3'].append('stuff')`.
 
     Parameters:
     depth - How deep the defaultdict is
     endtype - What type the value of the deepest default dict is.
     """
     if depth == 0:
         return defaultdict(endtype)
     return defaultdict(lambda: nested_ddict(depth - 1, endtype))
 
 
-def format_ddict(ddict: defaultdict, make_nparr: bool = True, sort_lists: bool = False):
+def format_ddict(
+    ddict: defaultdict, make_nparr: bool = True, sort_lists: bool = False
+) -> defaultdict:
     """
     Turn nested defaultdicts into nested dicts and,optionally lists in numpy arrays.
 
     Parameters:
     ddict - Defaultdict to transform
     make_nparr - If True, will turn lists into numpy arrays
     sort_list - If True, will sort any lists it finds
     """
+    # sike, `ddict` can actually be a dict, list or other object
+    # but those cases are ONLY during recusive calls
     if isinstance(ddict, (dict, defaultdict)):
-        ddict = {k: format_ddict(v, sort_lists) for k, v in ddict.items()}
+        ddict = {k: format_ddict(v, make_nparr, sort_lists) for k, v in ddict.items()}
     elif isinstance(ddict, list):
         ddict = sorted(ddict) if sort_lists else ddict
         ddict = np.array(ddict) if make_nparr else ddict
     return ddict
```

### Comparing `my-favorite-things-0.2.0/my_favorite_things/save.py` & `my-favorite-things-0.3.0/my_favorite_things/save.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Contains method `save` with the flexibility of saving any number of object in various
+ways to a specific directory and with other functions.
+"""
 import pickle
 from pathlib import Path
 
 import numpy as np
 
 
 def save(
@@ -113,12 +117,12 @@
             np.savez(path / name, **files)
         case "npy":
             if len(files.values()) != 1:
                 raise IndexError(
                     f"Choosing stype={stype} allowing only a single array to be saved "
                     + f"but there are {len(files.values())} arrays passed as the"
                     + "`files` kwargs."
-                )
+                ) from None
             np.save(path / name, arr=list(files.values())[0], **save_kwargs)
         case "pkl":
             with open(f"{path / name}.pkl", "wb") as savefile:
                 pickle.dump(files, savefile, **save_kwargs)
```

### Comparing `my-favorite-things-0.2.0/my_favorite_things.egg-info/PKG-INFO` & `my-favorite-things-0.3.0/my_favorite_things.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-favorite-things
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convenient functions and classes I use too often.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,41 +695,63 @@
 
 ## Installation
 Install with
 ```
 pip install my-favorite-things
 ```
 
-## Current Methods
+## Current Methods (by file)
 ### save
-#### `save()`
-Import by
-```
+#### `save(name, savedir="", savepath="", stype="npz", absolute=False, parents=0, overwrite=False, append=False, dryrun=False, save_kwargs={}, **kwargs)`
+**Import by**
+```python
 from my_favorite_things import save
 ```
-This method is used for saving data to a file. You can save as an `.npz` file for numpy array(s) or as a `.pkl` file for dictionaries and other odd python objects. By default, it will not overwrite existing files but instead append a number onto the end of file name (the keywords being, by default, `overwite=False` and `append=True`). You can save relative to your current directory (`absolute=False`) or as an absolute path (`absolute=True`). Addtionally, double check that you're saving to the correct directory with `dryrun=True`. Check the doc string for more info.
+This method is used for saving data to a file. You can save as an `.npz`/`.npy` file for numpy array(s) or as a `.pkl` file for dictionaries and other odd python objects. By default, it will not overwrite existing files but instead append a number onto the end of file name (the keywords being, by default, `overwite=False` and `append=True`). You can save relative to your current directory (`absolute=False`) or as an absolute path (`absolute=True`). Addtionally, double check that you're saving to the correct directory with `dryrun=True`. Check the doc string for more info.
 
 ---
 
-### ddict
-#### `nested_ddict()`
-Import by
-```
+### ddicts
+#### `nested_ddict(depth, endtype)`
+**Import by**
+```python
 from my_favorite_things import nested_ddict
 ```
 This method allows for creating a nested defaultdictionary. This is useful if you have data that is dependent on multiple parameters that are heirarchical. For example, if we do
 ```python
 d = nested_ddict(3, list)
 ```
 then we can use it as
 ```python
 d['zero']['one']['two']['three'].append(datum)
 ```
 
-#### `format_ddict()`
-Import by
-```
+#### `format_ddict(ddict, make_nparr=True, sort_lists=False)`
+**Import by**
+```python
 from my_favorite_things import format_ddict
 ```
 This method will format your (nested) defaultdictionary into dictionaries. Additionally, it can turns lists in numpy arrays and/or sort the lists too.
 
 ---
+
+### plots
+#### `log_bins(*arrs, num_bins)`
+**Import by**
+```python
+from my_favorite_things import log_bins
+```
+This method is used for binning for histograms logarithmically. In `plt.hist`, setting the keyword `bins` to the output of this function (where `arrs` are the arrays being plotted) and `ax.set_xscale("log")` will give equally spaced bins (for multiple data sets over the logarithmic x-axis).
+
+#### `cumulative_bins(*arrs, num_bins)`
+**Import by**
+```python
+from my_favorite_things import cumulative_bins
+```
+This is similar to the previous method but for a linear scale. When plotting multiple data sets on the same plot, they may have different ranges and, thus, bin sizes. So this method will create the bin values so that the bars of the histogram will all have the same width.
+
+#### `bar_count(ax, counts, labels, label_bars, sort_type, *, bar_params, **kwargs)`
+**Import by**
+```python
+from my_favorite_things import bar_count
+```
+This method will create a bar plot for the data passed using strings as labels (either as the keys of a dictionary passed for `counts` or as a list passed from `labels`) with various conveniences like specifying the format of the label strings or the order of the plotted data.
```

### Comparing `my-favorite-things-0.2.0/pyproject.toml` & `my-favorite-things-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools.scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "my-favorite-things"
-version = "0.2.0"
+version = "0.3.0"
 description = "Convenient functions and classes I use too often."
 authors = [
     {name = "Jacob Scott", email = "jscott137@pm.me"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```


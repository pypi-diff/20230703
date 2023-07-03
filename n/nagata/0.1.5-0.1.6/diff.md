# Comparing `tmp/nagata-0.1.5.tar.gz` & `tmp/nagata-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagata-0.1.5.tar", max compression
+gzip compressed data, was "nagata-0.1.6.tar", last modified: Mon Jul  3 16:26:37 2023, max compression
```

## Comparing `nagata-0.1.5.tar` & `nagata-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     2465 2023-01-04 19:41:38.715255 nagata-0.1.5/nagata/__init__.py
--rw-r--r--   0        0        0    23561 2023-01-04 19:41:38.715255 nagata-0.1.5/nagata/core.py
--rw-r--r--   0        0        0    21524 2023-01-04 19:41:38.765904 nagata-0.1.5/nagata/formats.py
--rw-r--r--   0        0        0    10028 2023-01-04 19:41:38.766904 nagata-0.1.5/nagata/lazy.py
--rw-r--r--   0        0        0      618 2023-01-04 19:52:57.508225 nagata-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      370 2023-01-04 19:41:38.714253 nagata-0.1.5/README.md
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 nagata-0.1.5/setup.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 nagata-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0    10247 2023-07-03 15:31:39.682923 nagata-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     1966 2023-07-03 15:37:12.159207 nagata-0.1.6/docs/README.md
+-rwxr-xr-x   0        0        0     2329 2023-07-03 16:26:37.955736 nagata-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0     2465 2023-07-03 15:27:41.966755 nagata-0.1.6/src/nagata/__init__.py
+-rwxr-xr-x   0        0        0    23516 2023-07-03 15:26:58.408902 nagata-0.1.6/src/nagata/core.py
+-rwxr-xr-x   0        0        0    21524 2022-11-05 16:53:21.640837 nagata-0.1.6/src/nagata/formats.py
+-rwxr-xr-x   0        0        0    10028 2022-11-04 20:39:34.450328 nagata-0.1.6/src/nagata/lazy.py
+-rwxr-xr-x   0        0        0        0 2022-10-03 16:07:43.354000 nagata-0.1.6/tests/__init__.py
+-rwxr-xr-x   0        0        0       25 2022-11-04 15:20:39.185355 nagata-0.1.6/tests/dummy_folder/csv_test_file.csv
+-rwxr-xr-x   0        0        0      404 2022-11-01 20:18:53.279427 nagata-0.1.6/tests/dummy_folder/dummy_module.py
+-rwxr-xr-x   0        0        0     4740 2022-11-04 15:19:30.513356 nagata-0.1.6/tests/dummy_folder/excel_test_file.xlsx
+-rwxr-xr-x   0        0        0       57 2022-11-01 20:19:54.547538 nagata-0.1.6/tests/dummy_folder/poem.txt
+-rwxr-xr-x   0        0        0       57 2022-11-05 16:53:26.292122 nagata-0.1.6/tests/dummy_output_folder/poem.txt
+-rwxr-xr-x   0        0        0       57 2022-11-05 16:53:26.291970 nagata-0.1.6/tests/dummy_output_folder/poem_out.txt
+-rwxr-xr-x   0        0        0       24 2022-11-05 16:53:26.468500 nagata-0.1.6/tests/dummy_output_folder/test_csv_out.csv
+-rwxr-xr-x   0        0        0     1739 2023-07-03 15:33:06.776839 nagata-0.1.6/tests/test_nagata.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 nagata-0.1.6/PKG-INFO
```

### Comparing `nagata-0.1.5/nagata/__init__.py` & `nagata-0.1.6/src/nagata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 usable. The one exception to that general rule is unit tests, which hopefully 
 are clear enough to not require further explanation. If there is any area of the 
 documentation that could be made clearer, please don't hesitate to email me or
 any other package maintainer - I want to ensure the package is as accessible and 
 useful as possible.
      
 """
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 __package__ = 'nagata'
 
 __author__ = 'Corey Rayburn Yung'
 
 
 from .core import *
```

### Comparing `nagata-0.1.5/nagata/core.py` & `nagata-0.1.6/src/nagata/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,15 @@
     
 """
 from __future__ import annotations
 import abc
 from collections.abc import Hashable, Mapping, MutableMapping, Sequence
 import contextlib
 import dataclasses
-import importlib
-import importlib.util
 import pathlib
-import types
 from typing import Any, ClassVar, Optional, Type
 
 import camina
 import miller
 
 from . import lazy
 
@@ -193,15 +190,15 @@
         'index_column': False,
         'header': 'infer',
         'conserve_memory': False,
         'test_size': 1000,
         'threads': -1,
         'visual_tightness': 'tight', 
         'visual_format': 'png'}
-    formats: camina.Dictionary[str, FileFormat] = camina.Dictionary()
+    formats: ClassVar[camina.Dictionary[str, FileFormat]] = camina.Dictionary()
   
    
 @dataclasses.dataclass
 class FileManager(object):
     """File and folder management for nagata.
 
     Creates and stores dynamic and static file paths, properly formats files
```

### Comparing `nagata-0.1.5/nagata/formats.py` & `nagata-0.1.6/src/nagata/formats.py`

 * *Files identical despite different names*

### Comparing `nagata-0.1.5/nagata/lazy.py` & `nagata-0.1.6/src/nagata/lazy.py`

 * *Files identical despite different names*


# Comparing `tmp/naters-utils-0.2.0.tar.gz` & `tmp/naters-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naters-utils-0.2.0.tar", last modified: Mon Jul  3 15:47:20 2023, max compression
+gzip compressed data, was "naters-utils-0.2.1.tar", last modified: Mon Jul  3 16:03:19 2023, max compression
```

## Comparing `naters-utils-0.2.0.tar` & `naters-utils-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.774847 naters-utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 15:47:10.000000 naters-utils-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 15:47:20.774847 naters-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 15:47:10.000000 naters-utils-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 15:47:10.000000 naters-utils-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:47:20.774847 naters-utils-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.770847 naters-utils-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.770847 naters-utils-0.2.0/src/naters_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/_hello.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/_isntinstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.774847 naters-utils-0.2.0/src/naters_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.774847 naters-utils-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_func_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_isntinstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_match_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_none_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_thread_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:03:19.726982 naters-utils-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 16:03:09.000000 naters-utils-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 16:03:19.726982 naters-utils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 16:03:09.000000 naters-utils-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 16:03:09.000000 naters-utils-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:03:19.726982 naters-utils-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:03:19.722983 naters-utils-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:03:19.726982 naters-utils-0.2.1/src/naters_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 16:03:09.000000 naters-utils-0.2.1/src/naters_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 16:03:09.000000 naters-utils-0.2.1/src/naters_utils/_hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 16:03:09.000000 naters-utils-0.2.1/src/naters_utils/_isntinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-03 16:03:09.000000 naters-utils-0.2.1/src/naters_utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-03 16:03:09.000000 naters-utils-0.2.1/src/naters_utils/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:03:19.726982 naters-utils-0.2.1/src/naters_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 16:03:19.000000 naters-utils-0.2.1/src/naters_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 16:03:19.000000 naters-utils-0.2.1/src/naters_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:03:19.000000 naters-utils-0.2.1/src/naters_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 16:03:19.000000 naters-utils-0.2.1/src/naters_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 16:03:19.000000 naters-utils-0.2.1/src/naters_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:03:19.726982 naters-utils-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 16:03:09.000000 naters-utils-0.2.1/tests/test_func_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-03 16:03:09.000000 naters-utils-0.2.1/tests/test_isntinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-03 16:03:09.000000 naters-utils-0.2.1/tests/test_match_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 16:03:09.000000 naters-utils-0.2.1/tests/test_none_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 16:03:09.000000 naters-utils-0.2.1/tests/test_thread_wrap.py
```

### Comparing `naters-utils-0.2.0/LICENSE.txt` & `naters-utils-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/PKG-INFO` & `naters-utils-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naters-utils
-Version: 0.2.0
+Version: 0.2.1
 Author-email: Nater0214 <gamer@nater0214.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `naters-utils-0.2.0/src/naters_utils/_isntinstance.py` & `naters-utils-0.2.1/src/naters_utils/_isntinstance.py`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/src/naters_utils/functions.py` & `naters-utils-0.2.1/src/naters_utils/functions.py`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/src/naters_utils/iterables.py` & `naters-utils-0.2.1/src/naters_utils/iterables.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Iterable
 
 from . import isntinstance
 
 
 # Metadata
 __all__ = {"NoneList"}
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 # Definitions
 class NoneList(list):
     """
     ### Summary
     A list of a fixed length, but with elements set to a default of None
@@ -57,15 +57,15 @@
     def __len__(self) -> int:
         return self.length - self.count(None)
     
     
     # List method overrides
     def append(self, obj: Any) -> None:
         # Check if list is full
-        if len(self) + 1 == self.length:
+        if len(self) + 1 > self.length:
             raise IndexError("list is full")
         
         # Add item to list
         self[self.index(None)] = obj
     
     
     def extend(self, iterable: Iterable) -> None:
```

### Comparing `naters-utils-0.2.0/src/naters_utils.egg-info/PKG-INFO` & `naters-utils-0.2.1/src/naters_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naters-utils
-Version: 0.2.0
+Version: 0.2.1
 Author-email: Nater0214 <gamer@nater0214.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `naters-utils-0.2.0/src/naters_utils.egg-info/SOURCES.txt` & `naters-utils-0.2.1/src/naters_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/tests/test_func_cache.py` & `naters-utils-0.2.1/tests/test_func_cache.py`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/tests/test_match_call.py` & `naters-utils-0.2.1/tests/test_match_call.py`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/tests/test_none_list.py` & `naters-utils-0.2.1/tests/test_none_list.py`

 * *Files identical despite different names*

### Comparing `naters-utils-0.2.0/tests/test_thread_wrap.py` & `naters-utils-0.2.1/tests/test_thread_wrap.py`

 * *Files identical despite different names*


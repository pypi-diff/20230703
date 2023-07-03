# Comparing `tmp/naters-utils-0.1.2.tar.gz` & `tmp/naters-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naters-utils-0.1.2.tar", last modified: Mon Jul  3 04:15:00 2023, max compression
+gzip compressed data, was "naters-utils-0.2.0.tar", last modified: Mon Jul  3 15:47:20 2023, max compression
```

## Comparing `naters-utils-0.1.2.tar` & `naters-utils-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:15:00.984047 naters-utils-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 04:14:50.000000 naters-utils-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 04:15:00.984047 naters-utils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 04:14:50.000000 naters-utils-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 04:14:50.000000 naters-utils-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 04:15:00.984047 naters-utils-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:15:00.984047 naters-utils-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:15:00.984047 naters-utils-0.1.2/src/naters_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 04:14:50.000000 naters-utils-0.1.2/src/naters_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 04:14:50.000000 naters-utils-0.1.2/src/naters_utils/_hello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-03 04:14:50.000000 naters-utils-0.1.2/src/naters_utils/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:15:00.984047 naters-utils-0.1.2/src/naters_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 04:15:00.000000 naters-utils-0.1.2/src/naters_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 04:15:00.000000 naters-utils-0.1.2/src/naters_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:15:00.000000 naters-utils-0.1.2/src/naters_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 04:15:00.000000 naters-utils-0.1.2/src/naters_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 04:15:00.000000 naters-utils-0.1.2/src/naters_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:15:00.984047 naters-utils-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 04:14:50.000000 naters-utils-0.1.2/tests/test_func_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-03 04:14:50.000000 naters-utils-0.1.2/tests/test_match_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 04:14:50.000000 naters-utils-0.1.2/tests/test_thread_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.774847 naters-utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 15:47:10.000000 naters-utils-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 15:47:20.774847 naters-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 15:47:10.000000 naters-utils-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 15:47:10.000000 naters-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:47:20.774847 naters-utils-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.770847 naters-utils-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.770847 naters-utils-0.2.0/src/naters_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/_hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/_isntinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-03 15:47:10.000000 naters-utils-0.2.0/src/naters_utils/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.774847 naters-utils-0.2.0/src/naters_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 15:47:20.000000 naters-utils-0.2.0/src/naters_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:47:20.774847 naters-utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_func_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_isntinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_match_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_none_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 15:47:10.000000 naters-utils-0.2.0/tests/test_thread_wrap.py
```

### Comparing `naters-utils-0.1.2/LICENSE.txt` & `naters-utils-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naters-utils-0.1.2/PKG-INFO` & `naters-utils-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naters-utils
-Version: 0.1.2
+Version: 0.2.0
 Author-email: Nater0214 <gamer@nater0214.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `naters-utils-0.1.2/src/naters_utils/functions.py` & `naters-utils-0.2.0/src/naters_utils/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# src/func_cache.py
-# Caches the return values of a function
+# functions.py
+# Holds function related utils
 
 
 # Imports
 from __future__ import annotations
 
 import hashlib
 from functools import partial
 from inspect import ismethod
 from threading import Thread
 from typing import Any, Callable
 
 
 # Metadata
-__all__ = ["func_cache", "thread_wrap"]
+__all__ = ["func_cache", "MatchCall", "thread_wrap"]
 __version__ = "1.0.3"
 
 
 # Definitions
 class MatchCall:
     """
     ### Summary
@@ -87,15 +87,15 @@
             else:
                 self.map[func.__name__] = func
         
         return decorator
     
     
     def __call__(self, arg_match: Any, *args, **kwargs) -> Any:
-        self._run_function(arg_match, *args, **kwargs)
+        return self._run_function(arg_match, *args, **kwargs)
     
     
     def _run_function(self, arg_match, *args, **kwargs) -> Any:
         return self.map[arg_match](*args, **kwargs)
     
     
     def _run_method(self, method_parent_self: object, arg_match: Any, *args, **kwargs) -> Any:
```

### Comparing `naters-utils-0.1.2/src/naters_utils.egg-info/PKG-INFO` & `naters-utils-0.2.0/src/naters_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naters-utils
-Version: 0.1.2
+Version: 0.2.0
 Author-email: Nater0214 <gamer@nater0214.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `naters-utils-0.1.2/tests/test_func_cache.py` & `naters-utils-0.2.0/tests/test_func_cache.py`

 * *Files identical despite different names*

### Comparing `naters-utils-0.1.2/tests/test_match_call.py` & `naters-utils-0.2.0/tests/test_match_call.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """
     ### Summary
     Tests if match call works as intended.
     """
     
     # Imports
     from naters_utils.functions import MatchCall
-    
+
     # Define functions
     math = MatchCall()
     @math.case("add")
     def add(a, b):
         return a + b
     @math.case("subtract")
     def subtract(a, b):
@@ -38,15 +38,15 @@
     """
     ### Summary
     Tests if the match call works as intended without arg matches
     """
     
     # Imports
     from naters_utils.functions import MatchCall
-    
+
     # Define functions
     math = MatchCall()
     @math.case()
     def add(a, b):
         return a + b
     @math.case()
     def subtract(a, b):
@@ -55,29 +55,30 @@
     def multiply(a, b):
         return a * b
     @math.case()
     def divide(a, b):
         return a / b
     
     # Test functionality
-    assert math("add", 1, 2) == 3
+    result = math("add", 1, 2)
+    assert result == 3
     assert math("subtract", 1, 2) == -1
     assert math("multiply", 1, 2) == 2
     assert math("divide", 1, 2) == 0.5
 
 
 def works_with_objects_test():
     """
     ### Summary
     Tests if match call works with objects
     """
     
     # Imports
     from naters_utils.functions import MatchCall
-    
+
     # Define class
     class Math:
         __call__ = MatchCall()
         @__call__.case()
         def add(self, a, b):
             return a + b
         @__call__.case()
```

### Comparing `naters-utils-0.1.2/tests/test_thread_wrap.py` & `naters-utils-0.2.0/tests/test_thread_wrap.py`

 * *Files identical despite different names*


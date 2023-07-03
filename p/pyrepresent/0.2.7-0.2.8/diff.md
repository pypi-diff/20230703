# Comparing `tmp/pyrepresent-0.2.7.tar.gz` & `tmp/pyrepresent-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.7.tar", last modified: Mon Jul  3 14:00:37 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.8.tar", last modified: Mon Jul  3 16:05:04 2023, max compression
```

## Comparing `pyrepresent-0.2.7.tar` & `pyrepresent-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:00:37.776323 pyrepresent-0.2.7/
--rw-rw-rw-   0        0        0      115 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-03 14:00:37.775267 pyrepresent-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.7/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.7/build.py
--rw-rw-rw-   0        0        0      715 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-03 14:00:37.771300 pyrepresent-0.2.7/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 14:00:37.000000 pyrepresent-0.2.7/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 14:00:37.774297 pyrepresent-0.2.7/represent/
--rw-rw-rw-   0        0        0      116 2023-07-03 14:00:08.000000 pyrepresent-0.2.7/represent/__init__.py
--rw-rw-rw-   0        0        0     8875 2023-07-03 13:59:57.000000 pyrepresent-0.2.7/represent/colors.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.7/represent/indentation.py
--rw-rw-rw-   0        0        0    17393 2023-07-03 13:59:57.000000 pyrepresent-0.2.7/represent/object.py
--rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.7/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.7/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:00:37.776323 pyrepresent-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-03 14:00:29.000000 pyrepresent-0.2.7/setup.py
--rw-rw-rw-   0        0        0     1363 2023-07-03 13:34:56.000000 pyrepresent-0.2.7/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:05:04.342604 pyrepresent-0.2.8/
+-rw-rw-rw-   0        0        0      115 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-03 16:05:04.342604 pyrepresent-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.8/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.8/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-03 16:05:04.337603 pyrepresent-0.2.8/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 16:05:04.341574 pyrepresent-0.2.8/represent/
+-rw-rw-rw-   0        0        0      116 2023-07-03 14:00:08.000000 pyrepresent-0.2.8/represent/__init__.py
+-rw-rw-rw-   0        0        0     9089 2023-07-03 16:01:42.000000 pyrepresent-0.2.8/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.8/represent/indentation.py
+-rw-rw-rw-   0        0        0    17405 2023-07-03 16:02:23.000000 pyrepresent-0.2.8/represent/object.py
+-rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.8/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 16:05:04.342604 pyrepresent-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-03 16:02:40.000000 pyrepresent-0.2.8/setup.py
+-rw-rw-rw-   0        0        0     1363 2023-07-03 13:34:56.000000 pyrepresent-0.2.8/test.py
```

### Comparing `pyrepresent-0.2.7/PKG-INFO` & `pyrepresent-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.7
+Version: 0.2.8
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.7/README.md` & `pyrepresent-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.7/build.py` & `pyrepresent-0.2.8/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.7/pyproject.toml` & `pyrepresent-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.7'
+version = '0.2.8'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.7/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.2.8/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.7
+Version: 0.2.8
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.7/represent/colors.py` & `pyrepresent-0.2.8/represent/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # colors.py
 
 import datetime as dt
 from typing import Any, Optional
 
+import numpy as np
+
 from colorama import Fore, Style
 
 __all__ = [
     "Colors",
     "colorize",
     "decolorize",
     "SIMPLE_TYPE_COLORS"
@@ -322,14 +324,20 @@
 # end uncolor
 
 SIMPLE_TYPE_COLORS = {
     str: Colors.YELLOW,
     bytes: Colors.CYAN,
     int: Colors.MAGENTA,
     float: Colors.MAGENTA,
+    np.float64: Colors.MAGENTA,
+    np.int64: Colors.MAGENTA,
+    np.float32: Colors.MAGENTA,
+    np.int32: Colors.MAGENTA,
+    np.float16: Colors.MAGENTA,
+    np.int16: Colors.MAGENTA,
     dt.timedelta: Colors.MAGENTA,
     dt.time: Colors.MAGENTA,
     dt.datetime: Colors.MAGENTA,
     dt.date: Colors.MAGENTA,
     bool: Colors.CYAN,
     type(None): Colors.CYAN
 }
```

### Comparing `pyrepresent-0.2.7/represent/indentation.py` & `pyrepresent-0.2.8/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.7/represent/object.py` & `pyrepresent-0.2.8/represent/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,18 +190,15 @@
     return {
         name: getattr(data, name) for (name, value) in
         inspect.getmembers(
             type(data), lambda attribute: isinstance(
                 attribute, property
             )
         )
-        if (
-            properties and
-            (isinstance(properties, bool) or name in properties)
-        )
+        if (properties is True) or (name in properties)
     }
 # end extract_properties
 
 def extract_data(
         data: Any, /, properties: Optional[Iterable[str]] = None
 ) -> Dict[str, Any]:
     """
@@ -303,15 +300,14 @@
     :param hidden: The hidden values.
 
     :return: The boolean flag.
     """
 
     return (
         (hidden is not None) and
-
         (key in hidden) and
         (assignment is not None)
     )
 # end is_hidden
 
 def early_cache(
         data: Any, /, *, ids: Dict[int, Any], legalize: Optional[bool] = False
@@ -411,15 +407,17 @@
             )
         )
     )
 # end has_modifiers
 
 BASIC_TYPES = [
     bool, int, float, str, bytes, bytearray, dt.time,
-    dt.timedelta, dt.datetime, dt.timezone, dt.date
+    dt.timedelta, dt.datetime, dt.timezone, dt.date,
+    np.float64, np.int64, np.float32, np.int32,
+    np.float16, np.int16
 ]
 
 def is_basic(data: Any, /) -> bool:
     """
     Checks if the object is a basic object.
 
     :param data: The object to check.
```

### Comparing `pyrepresent-0.2.7/represent/structures.py` & `pyrepresent-0.2.8/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.7/setup.py` & `pyrepresent-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.2.7',
+        version='0.2.8',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.7/test.py` & `pyrepresent-0.2.8/test.py`

 * *Files identical despite different names*


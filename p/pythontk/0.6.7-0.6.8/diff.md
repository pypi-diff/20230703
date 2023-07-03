# Comparing `tmp/pythontk-0.6.7.tar.gz` & `tmp/pythontk-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythontk-0.6.7.tar", last modified: Wed Jun 28 02:19:30 2023, max compression
+gzip compressed data, was "pythontk-0.6.8.tar", last modified: Mon Jul  3 15:09:52 2023, max compression
```

## Comparing `pythontk-0.6.7.tar` & `pythontk-0.6.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 02:19:30.289131 pythontk-0.6.7/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.7/LICENSE
--rw-rw-rw-   0        0        0     1155 2023-06-28 02:19:30.287627 pythontk-0.6.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-28 02:19:30.256804 pythontk-0.6.7/pythontk/
--rw-rw-rw-   0        0        0     7133 2023-06-28 02:19:24.000000 pythontk-0.6.7/pythontk/__init__.py
--rw-rw-rw-   0        0        0    25637 2023-06-28 00:18:26.000000 pythontk-0.6.7/pythontk/file_utils.py
--rw-rw-rw-   0        0        0    29291 2023-06-27 22:55:30.000000 pythontk-0.6.7/pythontk/img_utils.py
--rw-rw-rw-   0        0        0    29221 2023-06-24 12:29:41.000000 pythontk-0.6.7/pythontk/img_utils.py.bak
--rw-rw-rw-   0        0        0    16161 2023-06-28 00:25:24.000000 pythontk-0.6.7/pythontk/iter_utils.py
--rw-rw-rw-   0        0        0    18070 2023-06-27 22:52:04.000000 pythontk-0.6.7/pythontk/math_utils.py
--rw-rw-rw-   0        0        0    24621 2023-06-27 23:08:47.000000 pythontk-0.6.7/pythontk/str_utils.py
--rw-rw-rw-   0        0        0    11206 2023-06-27 22:12:52.000000 pythontk-0.6.7/pythontk/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 02:19:30.287627 pythontk-0.6.7/pythontk.egg-info/
--rw-rw-rw-   0        0        0     1155 2023-06-28 02:19:30.000000 pythontk-0.6.7/pythontk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.7/pythontk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0      387 2023-06-28 02:19:30.000000 pythontk-0.6.7/pythontk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.7/pythontk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-28 02:19:30.000000 pythontk-0.6.7/pythontk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 02:19:30.000000 pythontk-0.6.7/pythontk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 02:19:30.289131 pythontk-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1416 2023-06-28 02:16:16.000000 pythontk-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:09:52.617932 pythontk-0.6.8/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0     1155 2023-07-03 15:09:52.616927 pythontk-0.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 15:09:52.592320 pythontk-0.6.8/pythontk/
+-rw-rw-rw-   0        0        0     7133 2023-07-03 15:09:47.000000 pythontk-0.6.8/pythontk/__init__.py
+-rw-rw-rw-   0        0        0    28018 2023-07-03 14:39:57.000000 pythontk-0.6.8/pythontk/file_utils.py
+-rw-rw-rw-   0        0        0    29291 2023-06-27 22:55:30.000000 pythontk-0.6.8/pythontk/img_utils.py
+-rw-rw-rw-   0        0        0    29221 2023-06-24 12:29:41.000000 pythontk-0.6.8/pythontk/img_utils.py.bak
+-rw-rw-rw-   0        0        0    16318 2023-06-30 22:19:51.000000 pythontk-0.6.8/pythontk/iter_utils.py
+-rw-rw-rw-   0        0        0    18070 2023-06-27 22:52:04.000000 pythontk-0.6.8/pythontk/math_utils.py
+-rw-rw-rw-   0        0        0    24621 2023-06-27 23:08:47.000000 pythontk-0.6.8/pythontk/str_utils.py
+-rw-rw-rw-   0        0        0    11206 2023-06-27 22:12:52.000000 pythontk-0.6.8/pythontk/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:09:52.616927 pythontk-0.6.8/pythontk.egg-info/
+-rw-rw-rw-   0        0        0     1155 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.8/pythontk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      387 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.8/pythontk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:09:52.617932 pythontk-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1383 2023-06-28 23:01:31.000000 pythontk-0.6.8/setup.py
```

### Comparing `pythontk-0.6.7/LICENSE` & `pythontk-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/PKG-INFO` & `pythontk-0.6.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythontk
-Version: 0.6.7
+Version: 0.6.8
 Summary: *pythontk is a collection of backend utilities for Python.*
 Home-page: https://github.com/m3trik/pythontk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pythontk-0.6.7/pythontk/__init__.py` & `pythontk-0.6.8/pythontk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "pythontk"
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 
 
 # Define dictionaries to map class names, method names, and class method names to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
```

### Comparing `pythontk-0.6.7/pythontk/file_utils.py` & `pythontk-0.6.8/pythontk/file_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
     @staticmethod
     def get_filepath(obj, inc_filename=False):
         """Get the filepath of a class or module.
 
         Parameters:
             obj (obj): A python module, class, or the built-in __file__ variable.
-            inc_filename (bool): Include the filename in the returned result.
+            inc_filename (bool): Include the filename (or directory if the object is a package) in the returned path.
 
         Returns:
             (str)
         """
         from types import ModuleType
         import inspect
 
@@ -361,14 +361,62 @@
             list:  the appended paths.
         """
         path = os.path.dirname(os.path.abspath(root_dir))
         return [
             sys.path.append(d) for d in cls.get_dir_contents(path, "dirs", **kwargs)
         ]
 
+    @staticmethod
+    def get_classes_from_dir(dir_path):
+        """Parses the Python source files in a directory and extracts the names of all defined classes.
+        This function uses the Abstract Syntax Tree (AST) module to parse the Python source files, and hence does not execute any code within these files. It only considers classes that are defined at the top level of each file, and not those defined within other classes or functions.
+
+        Parameters:
+            dir_path (str): The path to the directory containing the Python source files.
+
+        Raises:
+            Exception: If the provided directory path does not exist or is not a directory.
+
+        Returns:
+            dict: A dictionary where the keys are the names of the identified classes, and the values are the corresponding paths to the Python files where these classes are defined.
+
+        Examples:
+            >>> get_classes_from_dir('/path/to/directory')
+            {'MyClass1': '/path/to/directory/my_file1.py', 'MyClass2': '/path/to/directory/my_file2.py'}
+
+        Note:
+            This function will not correctly identify classes that are defined dynamically or otherwise in non-standard ways.
+        """
+        import ast
+
+        # Check if directory exists
+        if not os.path.isdir(dir_path):
+            raise Exception(f"Directory {dir_path} doesn't exist")
+
+        # Create an empty dictionary to store class names and their module file paths
+        widget_classes = {}
+
+        # Iterate over each file in the directory
+        for filename in os.listdir(dir_path):
+            # Check if the file is a Python file
+            if filename.endswith(".py"):
+                with open(os.path.join(dir_path, filename), "r") as file:
+                    module = ast.parse(file.read())
+                    classes = [
+                        node for node in module.body if isinstance(node, ast.ClassDef)
+                    ]
+
+                    for cls in classes:
+                        # Check if the class inherits from QWidget
+                        for base in cls.bases:
+                            # Add the class name and file path to the dictionary
+                            widget_classes[cls.name] = os.path.join(dir_path, filename)
+
+        return widget_classes
+
     @classmethod
     @Utils.listify(threading=True)
     def time_stamp(cls, filepath, stamp="%m-%d-%Y  %H:%M"):
         """Attach or detach a modified timestamp and date to/from a given file path.
 
         Parameters:
             filepath (str): The full path to a file. ie. 'C:/Windows/Temp/__AUTO-SAVE__untitled.0001.mb'
```

### Comparing `pythontk-0.6.7/pythontk/img_utils.py` & `pythontk-0.6.8/pythontk/img_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/pythontk/img_utils.py.bak` & `pythontk-0.6.8/pythontk/img_utils.py.bak`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/pythontk/iter_utils.py` & `pythontk-0.6.8/pythontk/iter_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # !/usr/bin/python
 # coding=utf-8
+from collections.abc import Iterable
 
 
 class IterUtils:
     """ """
 
     @staticmethod
     def make_iterable(x):
         """Convert the given obj to an iterable, unless it's a string, bytes, or bytearray.
 
         Parameters:
-            x () = The object to convert to an iterable if not already a list, set, or tuple.
+            x () = The object to convert to an iterable if not already a list, set, tuple, dict_values or range.
 
         Returns:
             (iterable)
         """
-        if isinstance(x, (list, tuple, set, dict, range)):
+        if isinstance(x, (list, tuple, set, dict, range)) or (
+            isinstance(x, Iterable) and not isinstance(x, (str, bytes, bytearray))
+        ):
             return x
         else:
             return (x,)
 
     @classmethod
     def nested_depth(cls, lst, typ=(list, set, tuple)):
         """Get the maximum nested depth of any sub-lists of the given list.
```

### Comparing `pythontk-0.6.7/pythontk/math_utils.py` & `pythontk-0.6.8/pythontk/math_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/pythontk/str_utils.py` & `pythontk-0.6.8/pythontk/str_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/pythontk/utils.py` & `pythontk-0.6.8/pythontk/utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/pythontk.egg-info/PKG-INFO` & `pythontk-0.6.8/pythontk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythontk
-Version: 0.6.7
+Version: 0.6.8
 Summary: *pythontk is a collection of backend utilities for Python.*
 Home-page: https://github.com/m3trik/pythontk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pythontk-0.6.7/pythontk.egg-info/PKG-INFO.bak` & `pythontk-0.6.8/pythontk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.7/setup.py` & `pythontk-0.6.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import setuptools
-
-from pythontk import __package__, __version__
 import pythontk as ptk
 
 
 long_description = ptk.get_file_contents("docs/README.md")
 description = ptk.get_text_between_delimiters(
     long_description,
     "<!-- short_description_start -->",
     "<!-- short_description_end -->",
     as_string=True,
 )
 
 setuptools.setup(
-    name=__package__,
-    version=__version__,
+    name=ptk.__package__,
+    version=ptk.__version__,
     author="Ryan Simpson",
     author_email="m3trik@outlook.com",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url=f"https://github.com/m3trik/{__package__}",
+    url=f"https://github.com/m3trik/{ptk.__package__}",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
     data_files=ptk.get_dir_contents(
-        __package__, "filepaths", exc_files=["*.py", "*.pyc", "*.json"]
+        ptk.__package__, "filepaths", exc_files=["*.py", "*.pyc", "*.json"]
     ),  # ie. ('uitk/ui/0', ['uitk/ui/0/init.ui']),
 )
 
 # --------------------------------------------------------------------------------------------
 
 
 # --------------------------------------------------------------------------------------------
```


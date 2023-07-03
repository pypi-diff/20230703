# Comparing `tmp/RSFlib-0.1.1.tar.gz` & `tmp/RSFlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RSFlib-0.1.1.tar", last modified: Mon Jul  3 18:08:54 2023, max compression
+gzip compressed data, was "RSFlib-0.1.2.tar", last modified: Mon Jul  3 18:55:03 2023, max compression
```

## Comparing `RSFlib-0.1.1.tar` & `RSFlib-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-03 18:08:54.956489 RSFlib-0.1.1/
--rw-r--r--   0 radimslovak   (501) staff       (20)      605 2023-07-03 18:08:54.956386 RSFlib-0.1.1/PKG-INFO
--rw-r--r--   0 radimslovak   (501) staff       (20)       82 2023-06-26 03:03:38.000000 RSFlib-0.1.1/README.md
-drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-03 18:08:54.955809 RSFlib-0.1.1/RSFlib/
--rw-r--r--   0 radimslovak   (501) staff       (20)     2192 2023-07-03 17:47:36.000000 RSFlib-0.1.1/RSFlib/CalcFunctions.py
--rw-r--r--   0 radimslovak   (501) staff       (20)      457 2023-07-03 17:48:56.000000 RSFlib-0.1.1/RSFlib/DataManagement.py
--rw-r--r--   0 radimslovak   (501) staff       (20)     1491 2023-06-27 19:20:51.000000 RSFlib-0.1.1/RSFlib/TkinkerExtension.py
--rw-r--r--   0 radimslovak   (501) staff       (20)        0 2023-03-09 22:15:22.000000 RSFlib-0.1.1/RSFlib/__init__.py
-drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-03 18:08:54.956231 RSFlib-0.1.1/RSFlib.egg-info/
--rw-r--r--   0 radimslovak   (501) staff       (20)      605 2023-07-03 18:08:54.000000 RSFlib-0.1.1/RSFlib.egg-info/PKG-INFO
--rw-r--r--   0 radimslovak   (501) staff       (20)      233 2023-07-03 18:08:54.000000 RSFlib-0.1.1/RSFlib.egg-info/SOURCES.txt
--rw-r--r--   0 radimslovak   (501) staff       (20)        1 2023-07-03 18:08:54.000000 RSFlib-0.1.1/RSFlib.egg-info/dependency_links.txt
--rw-r--r--   0 radimslovak   (501) staff       (20)        7 2023-07-03 18:08:54.000000 RSFlib-0.1.1/RSFlib.egg-info/top_level.txt
--rw-r--r--   0 radimslovak   (501) staff       (20)       38 2023-07-03 18:08:54.956526 RSFlib-0.1.1/setup.cfg
--rw-r--r--   0 radimslovak   (501) staff       (20)     1054 2023-07-03 18:08:43.000000 RSFlib-0.1.1/setup.py
+drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-03 18:55:03.567063 RSFlib-0.1.2/
+-rw-r--r--   0 radimslovak   (501) staff       (20)      619 2023-07-03 18:55:03.566948 RSFlib-0.1.2/PKG-INFO
+-rw-r--r--   0 radimslovak   (501) staff       (20)       82 2023-06-26 03:03:38.000000 RSFlib-0.1.2/README.md
+drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-03 18:55:03.566323 RSFlib-0.1.2/RSFlib/
+-rw-r--r--   0 radimslovak   (501) staff       (20)     2192 2023-07-03 17:47:36.000000 RSFlib-0.1.2/RSFlib/CalcFunctions.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)      477 2023-07-03 18:52:23.000000 RSFlib-0.1.2/RSFlib/Constants.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)      457 2023-07-03 17:48:56.000000 RSFlib-0.1.2/RSFlib/DataManagement.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)     1491 2023-06-27 19:20:51.000000 RSFlib-0.1.2/RSFlib/TkinkerExtension.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)        0 2023-03-09 22:15:22.000000 RSFlib-0.1.2/RSFlib/__init__.py
+drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-03 18:55:03.566770 RSFlib-0.1.2/RSFlib.egg-info/
+-rw-r--r--   0 radimslovak   (501) staff       (20)      619 2023-07-03 18:55:03.000000 RSFlib-0.1.2/RSFlib.egg-info/PKG-INFO
+-rw-r--r--   0 radimslovak   (501) staff       (20)      253 2023-07-03 18:55:03.000000 RSFlib-0.1.2/RSFlib.egg-info/SOURCES.txt
+-rw-r--r--   0 radimslovak   (501) staff       (20)        1 2023-07-03 18:55:03.000000 RSFlib-0.1.2/RSFlib.egg-info/dependency_links.txt
+-rw-r--r--   0 radimslovak   (501) staff       (20)        7 2023-07-03 18:55:03.000000 RSFlib-0.1.2/RSFlib.egg-info/top_level.txt
+-rw-r--r--   0 radimslovak   (501) staff       (20)       38 2023-07-03 18:55:03.567105 RSFlib-0.1.2/setup.cfg
+-rw-r--r--   0 radimslovak   (501) staff       (20)     1068 2023-07-03 18:54:18.000000 RSFlib-0.1.2/setup.py
```

### Comparing `RSFlib-0.1.1/PKG-INFO` & `RSFlib-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: RSFlib
-Version: 0.1.1
-Summary: Useful methods for Fyzing struggle
+Version: 0.1.2
+Summary: Useful methods and constants for Fyzing struggle
 Author: Radzym (Radim Slovák)
 Author-email: <slovak.radim@seznam.cz>
 Keywords: python,data analysis,physics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `RSFlib-0.1.1/RSFlib/CalcFunctions.py` & `RSFlib-0.1.2/RSFlib/CalcFunctions.py`

 * *Files identical despite different names*

### Comparing `RSFlib-0.1.1/RSFlib/TkinkerExtension.py` & `RSFlib-0.1.2/RSFlib/TkinkerExtension.py`

 * *Files identical despite different names*

### Comparing `RSFlib-0.1.1/RSFlib.egg-info/PKG-INFO` & `RSFlib-0.1.2/RSFlib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: RSFlib
-Version: 0.1.1
-Summary: Useful methods for Fyzing struggle
+Version: 0.1.2
+Summary: Useful methods and constants for Fyzing struggle
 Author: Radzym (Radim Slovák)
 Author-email: <slovak.radim@seznam.cz>
 Keywords: python,data analysis,physics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `RSFlib-0.1.1/setup.py` & `RSFlib-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
-DESCRIPTION = 'Useful methods for Fyzing struggle'
+VERSION = '0.1.2'
+DESCRIPTION = 'Useful methods and constants for Fyzing struggle'
 LONG_DESCRIPTION = 'A package that helped me at University - Radim Slovák, VUT.'
 
 # Setting up
 setup(
     name="RSFlib",
     version=VERSION,
     author="Radzym (Radim Slovák)",
```


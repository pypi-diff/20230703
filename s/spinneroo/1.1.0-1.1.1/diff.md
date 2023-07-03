# Comparing `tmp/spinneroo-1.1.0.tar.gz` & `tmp/spinneroo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinneroo-1.1.0.tar", last modified: Sat Jul  1 08:41:42 2023, max compression
+gzip compressed data, was "spinneroo-1.1.1.tar", last modified: Mon Jul  3 14:12:41 2023, max compression
```

## Comparing `spinneroo-1.1.0.tar` & `spinneroo-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 08:41:42.223305 spinneroo-1.1.0/
--rw-rw-rw-   0        0        0       98 2023-07-01 08:41:41.000000 spinneroo-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2032 2023-07-01 08:41:42.223305 spinneroo-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1240 2023-06-15 21:54:41.000000 spinneroo-1.1.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.1.0/build.py
--rw-rw-rw-   0        0        0      630 2023-07-01 08:41:41.000000 spinneroo-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 08:41:42.223305 spinneroo-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1546 2023-07-01 08:41:38.000000 spinneroo-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:41:42.212465 spinneroo-1.1.0/spinneroo/
--rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.1.0/spinneroo/__init__.py
--rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.1.0/spinneroo/elements.py
--rw-rw-rw-   0        0        0    10265 2023-07-01 08:41:05.000000 spinneroo-1.1.0/spinneroo/progress.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:41:42.222335 spinneroo-1.1.0/spinneroo.egg-info/
--rw-rw-rw-   0        0        0     2032 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 14:12:41.921661 spinneroo-1.1.1/
+-rw-rw-rw-   0        0        0       98 2023-07-03 14:12:41.000000 spinneroo-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2006 2023-07-03 14:12:41.920661 spinneroo-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1214 2023-07-01 08:57:02.000000 spinneroo-1.1.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.1.1/build.py
+-rw-rw-rw-   0        0        0      630 2023-07-03 14:12:41.000000 spinneroo-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.1.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:12:41.921661 spinneroo-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2023-07-03 14:12:31.000000 spinneroo-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:12:41.906997 spinneroo-1.1.1/spinneroo/
+-rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.1.1/spinneroo/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.1.1/spinneroo/elements.py
+-rw-rw-rw-   0        0        0    10266 2023-07-03 14:12:04.000000 spinneroo-1.1.1/spinneroo/progress.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:12:41.919694 spinneroo-1.1.1/spinneroo.egg-info/
+-rw-rw-rw-   0        0        0     2006 2023-07-03 14:12:41.000000 spinneroo-1.1.1/spinneroo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-07-03 14:12:41.000000 spinneroo-1.1.1/spinneroo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:12:41.000000 spinneroo-1.1.1/spinneroo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-03 14:12:41.000000 spinneroo-1.1.1/spinneroo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 14:12:41.000000 spinneroo-1.1.1/spinneroo.egg-info/top_level.txt
```

### Comparing `spinneroo-1.1.0/PKG-INFO` & `spinneroo-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 1.1.0
+Version: 1.1.1
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
 - all the rights are saved for: Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `spinneroo-1.1.0/README.md` & `spinneroo-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
 - all the rights are saved for: Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `spinneroo-1.1.0/build.py` & `spinneroo-1.1.1/build.py`

 * *Files identical despite different names*

### Comparing `spinneroo-1.1.0/pyproject.toml` & `spinneroo-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'spinneroo'
-version = '1.1.0'
+version = '1.1.1'
 description = 'A module for displaying progress messages and timers with spinners in the command line.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `spinneroo-1.1.0/setup.py` & `spinneroo-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='spinneroo',
-        version='1.1.0',
+        version='1.1.1',
         description=(
             "A module for displaying progress messages and "
             "timers with spinners in the command line."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `spinneroo-1.1.0/spinneroo/progress.py` & `spinneroo-1.1.1/spinneroo/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import threading
 from typing import (
     Optional, Type, Generator, Iterable,
     Union, Any, Callable, Literal
 )
 
-from represent import BaseModel, Modifiers
+from represent import represent, Modifiers
 
 __all__ = [
     "Spinner",
     "spinner",
     "format_seconds"
 ]
 
@@ -65,15 +65,16 @@
             f"or 'center', not: {side}."
         )
     # end if
 
     return message
 # end format_seconds
 
-class Spinner(BaseModel):
+@represent
+class Spinner:
     """
     A class to create a terminal spinning wheel.
 
     Using this object it is able to create a context manager for
     continuously print a progress wheel, and a message.
 
     attributes:
```

### Comparing `spinneroo-1.1.0/spinneroo.egg-info/PKG-INFO` & `spinneroo-1.1.1/spinneroo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 1.1.0
+Version: 1.1.1
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
 - all the rights are saved for: Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```


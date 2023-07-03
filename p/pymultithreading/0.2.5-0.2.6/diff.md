# Comparing `tmp/pymultithreading-0.2.5.tar.gz` & `tmp/pymultithreading-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.2.5.tar", last modified: Sat Jul  1 08:05:40 2023, max compression
+gzip compressed data, was "pymultithreading-0.2.6.tar", last modified: Mon Jul  3 16:16:38 2023, max compression
```

## Comparing `pymultithreading-0.2.5.tar` & `pymultithreading-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 08:05:40.295578 pymultithreading-0.2.5/
--rw-rw-rw-   0        0        0       98 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2045 2023-07-01 08:05:40.294673 pymultithreading-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.5/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.5/build.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:05:40.285577 pymultithreading-0.2.5/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.5/multithreading/__init__.py
--rw-rw-rw-   0        0        0    11624 2023-06-30 18:20:08.000000 pymultithreading-0.2.5/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:05:40.293575 pymultithreading-0.2.5/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-07-01 08:05:03.000000 pymultithreading-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 08:05:40.295578 pymultithreading-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-07-01 08:04:53.000000 pymultithreading-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:16:38.221646 pymultithreading-0.2.6/
+-rw-rw-rw-   0        0        0       98 2023-07-03 16:16:37.000000 pymultithreading-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2019 2023-07-03 16:16:38.220647 pymultithreading-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1217 2023-07-01 08:57:20.000000 pymultithreading-0.2.6/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.6/build.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:16:38.205097 pymultithreading-0.2.6/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.6/multithreading/__init__.py
+-rw-rw-rw-   0        0        0    11708 2023-07-03 16:16:05.000000 pymultithreading-0.2.6/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:16:38.219676 pymultithreading-0.2.6/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2019 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-03 16:16:38.000000 pymultithreading-0.2.6/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-07-03 16:16:37.000000 pymultithreading-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 16:16:38.221646 pymultithreading-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-07-03 16:16:27.000000 pymultithreading-0.2.6/setup.py
```

### Comparing `pymultithreading-0.2.5/PKG-INFO` & `pymultithreading-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
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

### Comparing `pymultithreading-0.2.5/README.md` & `pymultithreading-0.2.6/README.md`

 * *Files 6% similar despite different names*

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

### Comparing `pymultithreading-0.2.5/build.py` & `pymultithreading-0.2.6/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.5/multithreading/process.py` & `pymultithreading-0.2.6/multithreading/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from abc import ABCMeta
 from typing import (
     Any, Optional, Dict, Callable, ClassVar,
     Iterable, Union, TypeVar, Generic
 )
 
-from represent import BaseModel, Modifiers
+from represent import represent, Modifiers
 
 __all__ = [
     "Caller",
     "CallDefinition",
     "CallsResults",
     "multi_threaded_call",
     "multi_threaded_defined_call",
@@ -22,21 +22,22 @@
     "ProcessTime",
     "ProcessInfo",
     "find_caller",
     "CallResults"
 ]
 
 @dataclass(repr=False, slots=True)
-class ProcessInfo(BaseModel, metaclass=ABCMeta):
+@represent
+class ProcessInfo(metaclass=ABCMeta):
     """A class to contain the info of a call to the callers."""
 
     start: dt.datetime
     end: dt.datetime
 
-    modifiers: ClassVar[Modifiers] = Modifiers(properties=['time'])
+    __modifiers__: ClassVar[Modifiers] = Modifiers(properties=['time'])
 
     @property
     def time(self) -> dt.timedelta:
         """
         Returns the time duration of the call.
 
         :return: The call time.
@@ -49,31 +50,33 @@
 class ProcessTime(ProcessInfo):
     """A class to contain the info of a call to the callers."""
 # end ProcessTime
 
 _ReturnType = TypeVar("_ReturnType")
 
 @dataclass(repr=False, slots=True)
-class CallResults(BaseModel, Generic[_ReturnType]):
+@represent
+class CallResults(Generic[_ReturnType]):
     """A class to represent a container for the call results."""
 
     returns: Optional[_ReturnType] = None
     thread: Optional[threading.Thread] = None
     start: Optional[dt.datetime] = None
     end: Optional[dt.datetime] = None
 
-    modifiers: ClassVar[Modifiers] = Modifiers(
+    __modifiers__: ClassVar[Modifiers] = Modifiers(
         excluded=["thread"], force=True
     )
 # end CallResults
 
-class Caller(BaseModel, Generic[_ReturnType]):
+@represent
+class Caller(Generic[_ReturnType]):
     """A class to represent a function caller object."""
 
-    modifiers = Modifiers(excluded=["thread", "results"])
+    __modifiers__ = Modifiers(excluded=["thread", "results"])
 
     __slots__ = (
         "target", "identifier", "args", "kwargs",
         "thread", "results", "complete", "called"
     )
 
     def __init__(
@@ -187,15 +190,16 @@
     raise ValueError(
         f"Cannot find a caller object with the identifier: "
         f"{identifier}. valid identifiers are: "
         f"{', '.join(str(caller.identifier) for caller in callers)}"
     )
 # end find_results
 
-class CallDefinition(BaseModel):
+@represent
+class CallDefinition:
     """A class to represent the call definition."""
 
     WAIT = True
     RESET_BEFORE = True
     RESET_AFTER = False
 
     SLEEP = 0.005
@@ -238,17 +242,20 @@
         self.reset_before = reset_before
         self.reset_after = reset_after
         self.sleep = sleep
     # end __init__
 # end CallDefinition
 
 @dataclass(repr=False, slots=True)
-class CallsResults(BaseModel):
+@represent
+class CallsResults:
     """A class to contain the info of a call to the callers."""
 
+    # __modifiers__ = Modifiers(excluded=["tread"], force=True)
+
     callers: Dict[Caller, CallResults]
     total: ProcessTime
     waiting: ProcessTime
     definition: CallDefinition
 
     def caller(self, identifier: Any) -> Caller:
         """
```

### Comparing `pymultithreading-0.2.5/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-0.2.6/pymultithreading.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
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

### Comparing `pymultithreading-0.2.5/pyproject.toml` & `pymultithreading-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.2.5'
+version = '0.2.6'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.2.5/setup.py` & `pymultithreading-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.2.5',
+        version='0.2.6',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


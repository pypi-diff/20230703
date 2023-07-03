# Comparing `tmp/pyrepresent-0.2.3.tar.gz` & `tmp/pyrepresent-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.3.tar", last modified: Sun Jul  2 16:53:41 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.4.tar", last modified: Mon Jul  3 10:49:23 2023, max compression
```

## Comparing `pyrepresent-0.2.3.tar` & `pyrepresent-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:53:41.513990 pyrepresent-0.2.3/
--rw-rw-rw-   0        0        0      115 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-02 16:53:41.512977 pyrepresent-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.3/build.py
--rw-rw-rw-   0        0        0      715 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-02 16:53:41.507994 pyrepresent-0.2.3/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 16:53:41.511977 pyrepresent-0.2.3/represent/
--rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.3/represent/__init__.py
--rw-rw-rw-   0        0        0     8718 2023-07-02 15:44:34.000000 pyrepresent-0.2.3/represent/colors.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.3/represent/indentation.py
--rw-rw-rw-   0        0        0    14704 2023-07-02 16:53:32.000000 pyrepresent-0.2.3/represent/object.py
--rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.3/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 16:53:41.513990 pyrepresent-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-02 16:53:38.000000 pyrepresent-0.2.3/setup.py
--rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.3/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:49:23.223935 pyrepresent-0.2.4/
+-rw-rw-rw-   0        0        0      115 2023-07-03 10:49:21.000000 pyrepresent-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-03 10:49:23.223935 pyrepresent-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.4/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-03 10:49:21.000000 pyrepresent-0.2.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-03 10:49:23.217935 pyrepresent-0.2.4/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-03 10:49:23.000000 pyrepresent-0.2.4/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-03 10:49:23.000000 pyrepresent-0.2.4/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:49:23.000000 pyrepresent-0.2.4/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-03 10:49:23.000000 pyrepresent-0.2.4/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 10:49:23.000000 pyrepresent-0.2.4/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 10:49:23.222936 pyrepresent-0.2.4/represent/
+-rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.4/represent/__init__.py
+-rw-rw-rw-   0        0        0     8924 2023-07-03 10:48:46.000000 pyrepresent-0.2.4/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.4/represent/indentation.py
+-rw-rw-rw-   0        0        0    14819 2023-07-03 10:48:22.000000 pyrepresent-0.2.4/represent/object.py
+-rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.4/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:49:23.223935 pyrepresent-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-03 10:49:11.000000 pyrepresent-0.2.4/setup.py
+-rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.4/test.py
```

### Comparing `pyrepresent-0.2.3/PKG-INFO` & `pyrepresent-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.3
+Version: 0.2.4
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.3/README.md` & `pyrepresent-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.3/build.py` & `pyrepresent-0.2.4/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.3/pyproject.toml` & `pyrepresent-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.3'
+version = '0.2.4'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.3/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.2.4/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.3
+Version: 0.2.4
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.3/represent/colors.py` & `pyrepresent-0.2.4/represent/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,17 +178,19 @@
         if not color:
             return content
         # end if
 
         try:
             color = {
                 str: Colors.YELLOW,
+                bytes: Colors.CYAN,
                 int: Colors.MAGENTA,
                 float: Colors.MAGENTA,
                 dt.timedelta: Colors.MAGENTA,
+                dt.time: Colors.MAGENTA,
                 dt.datetime: Colors.MAGENTA,
                 dt.date: Colors.MAGENTA,
                 bool: Colors.CYAN,
                 type(None): Colors.CYAN
             }[type(value)]
 
             if type(value) == str:
@@ -210,23 +212,26 @@
                     content = content.replace(
                         char, f"{Colors.MAGENTA}{char}{Colors.END}"
                     )
                 # end for
 
                 return content
 
-            elif type(value) in (dt.datetime, dt.timedelta, dt.date):
+            elif type(value) in (dt.datetime, dt.timedelta, dt.date, dt.time):
                 content = "".join(
                     f"{color}{char}{Colors.END}"
                     if char != ":"
                     else char for char in content
                 )
                 content = content.replace(
                     ":", f"{Colors.RED}:{Colors.END}"
                 )
+                content = content.replace(
+                    "-", f"{Colors.RED}-{Colors.END}"
+                )
 
                 return content
 
             else:
                 return f"{color}{content}{Colors.END}"
             # end if
```

### Comparing `pyrepresent-0.2.3/represent/indentation.py` & `pyrepresent-0.2.4/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.3/represent/object.py` & `pyrepresent-0.2.4/represent/object.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import builtins
 import types
 import six
 from dataclasses import dataclass, field
 import datetime as dt
 from itertools import chain
 from typing import (
-    Any, Optional, Union, Iterable, Type, Dict
+    Any, Optional, Union, Iterable, Type, Dict, List
 )
 
 import pandas as pd
 import numpy as np
 
 from represent.indentation import indent
 from represent.colors import colorize
@@ -53,17 +53,35 @@
     assign: bool = True
     protected: bool = False
     force: bool = False
     legalize: bool = False
     defined: bool = True
     color: bool = True
 
-    excluded: Iterable[Any] = field(default_factory=lambda: ['modifiers'])
-    hidden: Iterable[Any] = field(default_factory=lambda: [])
-    properties: Union[bool, Iterable[str]] = field(default_factory=lambda: [])
+    excluded: Optional[Union[Iterable[Any], List[Any]]] = field(
+        default_factory=lambda: ['modifiers']
+    )
+    hidden: Optional[Union[Iterable[Any], List[Any]]] = field(
+        default_factory=list
+    )
+    properties: Optional[Union[bool, Iterable[str], List[str]]] = field(
+        default_factory=list
+    )
+
+    def __post_init__(self) -> None:
+        """Processes the attributes."""
+
+        self.excluded = list(self.excluded or [])
+        self.hidden = list(self.hidden or [])
+        self.properties = (
+            list(self.properties or [])
+            if self.properties is not True else
+            self.properties
+        )
+    # end __post_init__
 
     def __setattr__(self, key: str, value: Any) -> None:
         """
         Sets the attribute.
 
         :param key: The key to the attribute.
         :param value: The value of the attribute.
@@ -228,56 +246,34 @@
         )
     )
 # end is_excluded
 
 def is_hidden(
         key: Any,
         assignment: Optional[Any] = None,
-        hidden: Optional[Union[Dict[Any, Any], Iterable[Any]]] = None
+        hidden: Optional[Iterable[Any]] = None
 ) -> bool:
     """
     Checks if the value of the key should be hidden.
 
     :param key: The key object.
     :param assignment: The assignment value of the object.
     :param hidden: The hidden values.
 
     :return: The boolean flag.
     """
 
     return (
         (hidden is not None) and
+
         (key in hidden) and
         (assignment is not None)
     )
 # end is_hidden
 
-def hidden_value(
-        key: Any,
-        hide: Optional[bool] = None,
-        hidden: Optional[Union[Dict[Any, Any], Iterable[Any]]] = None
-) -> Any:
-    """
-    Returns the hidden value for the given value.
-
-    :param key: The key object.
-    :param hide: The value to hide the object.
-    :param hidden: The hidden values.
-
-    :return: The hidden value.
-    """
-
-    if not hide:
-        return hidden[key]
-
-    else:
-        return HiddenStructure()
-    # end if
-# end hidden_value
-
 def early_cache(
         data: Any, /, *, ids: Dict[int, Any], legalize: Optional[bool] = False
 ) -> None:
     """
     Caches the object data early in the ids.
 
     :param data: The object.
@@ -347,24 +343,47 @@
 
         data.__color__ = color
     # end if
 
     return data
 # end wrap_object
 
+def has_modifiers(data: Any, /) -> bool:
+    """
+    Checks if the object has modifiers.
+
+    :param data: The object to check.
+
+    :return: The boolean flag.
+    """
+
+    return (
+        (
+            (
+                hasattr(data, "modifiers") and
+                isinstance(data.modifiers, Modifiers)
+            ) or
+            (
+                hasattr(type(data), "modifiers") and
+                isinstance(type(data).modifiers, Modifiers)
+            )
+        )
+    )
+# end has_modifiers
+
 def unwrap(
         data: Any, /, *,
         assign: Optional[bool] = False,
         protected: Optional[bool] = False,
         legalize: Optional[bool] = False,
         force: Optional[bool] = False,
         defined: Optional[bool] = None,
         color: Optional[bool] = None,
+        hidden: Optional[Iterable[Any]] = None,
         properties: Optional[Union[bool, Iterable[str]]] = False,
-        hidden: Optional[Union[Dict[Any, Any], Iterable[Any]]] = None,
         excluded: Optional[Iterable[Union[str, Type]]] = None,
         ids: Optional[Dict[int, Any]] = None
 ) -> Any:
     """
     Unwraps the models to get the valid_values as dictionaries.
 
     :param assign: The value to assign a type name to each commands' structure.
@@ -384,26 +403,22 @@
 
     if inspect.isclass(data):
         return TypeStructure(data)
     # end if
 
     if isinstance(
         data, (
-            bool, int, float, str, dt.time,
-            dt.timedelta, dt.datetime, dt.timezone
+            bool, int, float, str, bytes, bytearray, dt.time,
+            dt.timedelta, dt.datetime, dt.timezone, dt.date
         )
     ):
         return data
     # end if
 
-    if (
-        (hasattr(data, "modifiers") or hasattr(type(data), "modifiers")) and
-        isinstance(data.modifiers, Modifiers) and
-        ids and (not force)
-    ):
+    if has_modifiers(data) and ids and (not force):
         modifiers = data.modifiers
 
         assign = modifiers.assign
         excluded = modifiers.excluded
         properties = modifiers.properties
         protected = modifiers.protected
         hidden = modifiers.hidden
@@ -432,26 +447,14 @@
 
     if isinstance(data, (HiddenStructure, StringWrapper)):
         return repr(data) if legalize else StringWrapper(repr(data))
     # end if
 
     ids = ids or {}
 
-    if (not isinstance(hidden, dict)) and (hidden is not None):
-        hide = True
-
-    elif hidden is None:
-        hide = False
-
-        hidden = ()
-
-    else:
-        hide = False
-    # end if
-
     if (data_id := id(data)) in ids:
         return ids[data_id]
 
     else:
         early_cache(data, ids=ids, legalize=legalize)
     # end if
 
@@ -473,15 +476,15 @@
                 is_protected(key=key, protected=protected, assignment=assignment) or
                 is_excluded(key=key, value=value, excluded=excluded, defined=defined)
             ):
                 continue
             # end if
 
             if is_hidden(key=key, assignment=assignment, hidden=hidden):
-                value = hidden_value(key=key, hide=hide, hidden=hidden)
+                value = HiddenStructure()
             # end if
 
             key = unwrap(
                 key, assign=assign, ids=ids, excluded=excluded,
                 properties=properties, protected=protected,
                 hidden=hidden, legalize=legalize, force=force,
                 defined=defined, color=color
```

### Comparing `pyrepresent-0.2.3/represent/structures.py` & `pyrepresent-0.2.4/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.3/setup.py` & `pyrepresent-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.2.3',
+        version='0.2.4',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.3/test.py` & `pyrepresent-0.2.4/test.py`

 * *Files identical despite different names*


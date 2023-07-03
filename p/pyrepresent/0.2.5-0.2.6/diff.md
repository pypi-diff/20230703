# Comparing `tmp/pyrepresent-0.2.5.tar.gz` & `tmp/pyrepresent-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.5.tar", last modified: Mon Jul  3 11:32:47 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.6.tar", last modified: Mon Jul  3 13:52:59 2023, max compression
```

## Comparing `pyrepresent-0.2.5.tar` & `pyrepresent-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 11:32:47.728274 pyrepresent-0.2.5/
--rw-rw-rw-   0        0        0      115 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-03 11:32:47.727273 pyrepresent-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.5/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.5/build.py
--rw-rw-rw-   0        0        0      715 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-03 11:32:47.722273 pyrepresent-0.2.5/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 11:32:47.000000 pyrepresent-0.2.5/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 11:32:47.726273 pyrepresent-0.2.5/represent/
--rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.5/represent/__init__.py
--rw-rw-rw-   0        0        0     8977 2023-07-03 11:32:13.000000 pyrepresent-0.2.5/represent/colors.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.5/represent/indentation.py
--rw-rw-rw-   0        0        0    14819 2023-07-03 10:48:22.000000 pyrepresent-0.2.5/represent/object.py
--rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.5/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 11:32:47.728274 pyrepresent-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-03 11:32:39.000000 pyrepresent-0.2.5/setup.py
--rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.5/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:52:59.621066 pyrepresent-0.2.6/
+-rw-rw-rw-   0        0        0      115 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-03 13:52:59.621066 pyrepresent-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.6/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.6/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-03 13:52:59.617066 pyrepresent-0.2.6/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 13:52:59.000000 pyrepresent-0.2.6/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:52:59.620071 pyrepresent-0.2.6/represent/
+-rw-rw-rw-   0        0        0      140 2023-07-03 13:34:37.000000 pyrepresent-0.2.6/represent/__init__.py
+-rw-rw-rw-   0        0        0     8977 2023-07-03 11:32:13.000000 pyrepresent-0.2.6/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.6/represent/indentation.py
+-rw-rw-rw-   0        0        0    16927 2023-07-03 13:49:56.000000 pyrepresent-0.2.6/represent/object.py
+-rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.6/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 13:52:59.622066 pyrepresent-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-03 13:52:57.000000 pyrepresent-0.2.6/setup.py
+-rw-rw-rw-   0        0        0     1363 2023-07-03 13:34:56.000000 pyrepresent-0.2.6/test.py
```

### Comparing `pyrepresent-0.2.5/PKG-INFO` & `pyrepresent-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.5
+Version: 0.2.6
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.5/README.md` & `pyrepresent-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.5/build.py` & `pyrepresent-0.2.6/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.5/pyproject.toml` & `pyrepresent-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.5'
+version = '0.2.6'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.5/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.2.6/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.5
+Version: 0.2.6
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.5/represent/colors.py` & `pyrepresent-0.2.6/represent/colors.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.5/represent/indentation.py` & `pyrepresent-0.2.6/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.5/represent/object.py` & `pyrepresent-0.2.6/represent/object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # object.py
 
 import inspect
 import builtins
 import types
 import six
-from dataclasses import dataclass, field
 import datetime as dt
 from itertools import chain
 from typing import (
-    Any, Optional, Union, Iterable, Type, Dict, List
+    Any, Optional, Union, Iterable,
+    Type, Dict, TypeVar
 )
 
 import pandas as pd
 import numpy as np
 
 from represent.indentation import indent
 from represent.colors import colorize
 from represent.structures import (
     structures, HiddenStructure, StringWrapper,
     CircularReferenceStructure, TypeStructure,
     FunctionStructure, hashable_structures
 )
 
 __all__ = [
-    "to_string",
-    "BaseModel",
     "Modifiers",
-    "unwrap"
+    "BaseModel",
+    "unwrap",
+    "represent",
+    "to_string"
 ]
 
 def is_bound_method(value: Any, /) -> bool:
     """
     Checks whether an object is a bound method or not.
 
     :param value: The object to check.
@@ -42,46 +43,85 @@
         return six.get_method_self(value) is not None
 
     except AttributeError:
         return False
     # end try
 # end is_bound_method
 
-@dataclass(kw_only=True, repr=False, slots=True)
 class Modifiers(dict):
     """A class to represent the modifiers of structures."""
 
-    assign: bool = True
-    protected: bool = False
-    force: bool = False
-    legalize: bool = False
-    defined: bool = True
-    color: bool = True
-
-    excluded: Optional[Union[Iterable[Any], List[Any]]] = field(
-        default_factory=lambda: ['modifiers']
-    )
-    hidden: Optional[Union[Iterable[Any], List[Any]]] = field(
-        default_factory=list
-    )
-    properties: Optional[Union[bool, Iterable[str], List[str]]] = field(
-        default_factory=list
+    __slots__ = (
+        "assign", "protected", "force", "legalize", "defined",
+        "color", "excluded", "hidden", "properties"
     )
 
-    def __post_init__(self) -> None:
-        """Processes the attributes."""
+    def __init__(
+            self, *,
+            assign: Optional[bool] = None,
+            protected: Optional[bool] = None,
+            force: Optional[bool] = None,
+            legalize: Optional[bool] = None,
+            defined: Optional[bool] = None,
+            color: Optional[bool] = None,
+            excluded: Optional[Iterable[Any]] = None,
+            hidden: Optional[Iterable[Any]] = None,
+            properties: Optional[Union[bool, Iterable[str]]] = None,
+    ) -> None:
+        """
+        Defines the class attributes.
+
+        :param assign: The value to assign a type name to each commands' structure.
+        :param excluded: The valid_values to exclude from the commands structure.
+        :param properties: The value to extract properties.
+        :param protected: The value to extract protected attributes.
+        :param legalize: The value to legalize the written valid_values to be strings.
+        :param hidden: The valid_values of hidden keywords.
+        :param color: The value to color the repr.
+        :param force: The value to force the settings of the parsing.
+        :param defined: The value to show only defined valid_values.
+        """
 
-        self.excluded = list(self.excluded or [])
-        self.hidden = list(self.hidden or [])
-        self.properties = (
-            list(self.properties or [])
-            if self.properties is not True else
-            self.properties
-        )
-    # end __post_init__
+        super().__init__()
+
+        if assign is None:
+            assign = True
+        # end if
+
+        if protected is None:
+            protected = False
+        # end if
+
+        if legalize is None:
+            legalize = False
+        # end if
+
+        if force is None:
+            force = False
+        # end if
+
+        if defined is None:
+            defined = True
+        # end if
+
+        if color is None:
+            color = True
+        # end if
+
+        self.assign = assign
+        self.protected = protected
+        self.legalize = legalize
+        self.force = force
+        self.defined = defined
+        self.color = color
+
+        self.properties = properties or []
+        self.excluded = list(excluded or ['modifiers'])
+        self.hidden = list(hidden or [])
+    # end __init__
 
     def __setattr__(self, key: str, value: Any) -> None:
         """
         Sets the attribute.
 
         :param key: The key to the attribute.
         :param value: The value of the attribute.
@@ -101,15 +141,15 @@
     def __str__(self) -> str:
         """
         Returns a string to represent the model commands and structure.
 
         :return: The string representation of the model.
         """
 
-        return to_string(self)
+        return to_string(self, modifiers=self.modifiers)
     # end __str__
 # end BaseModel
 
 def extract_attributes(data: Any, /) -> Dict[str, Any]:
     """
     Gets all attributes of an object.
 
@@ -356,34 +396,34 @@
     :return: The boolean flag.
     """
 
     return (
         (
             (
                 hasattr(data, "modifiers") and
-                isinstance(data.modifiers, Modifiers)
+                isinstance(data.__modifiers__, Modifiers)
             ) or
             (
                 hasattr(type(data), "modifiers") and
-                isinstance(type(data).modifiers, Modifiers)
+                isinstance(type(data).__modifiers__, Modifiers)
             )
         )
     )
 # end has_modifiers
 
 def unwrap(
         data: Any, /, *,
-        assign: Optional[bool] = False,
-        protected: Optional[bool] = False,
-        legalize: Optional[bool] = False,
-        force: Optional[bool] = False,
+        assign: Optional[bool] = None,
+        protected: Optional[bool] = None,
+        legalize: Optional[bool] = None,
+        force: Optional[bool] = None,
         defined: Optional[bool] = None,
         color: Optional[bool] = None,
         hidden: Optional[Iterable[Any]] = None,
-        properties: Optional[Union[bool, Iterable[str]]] = False,
+        properties: Optional[Union[bool, Iterable[str]]] = None,
         excluded: Optional[Iterable[Union[str, Type]]] = None,
         ids: Optional[Dict[int, Any]] = None
 ) -> Any:
     """
     Unwraps the models to get the valid_values as dictionaries.
 
     :param assign: The value to assign a type name to each commands' structure.
@@ -411,26 +451,33 @@
             dt.timedelta, dt.datetime, dt.timezone, dt.date
         )
     ):
         return data
     # end if
 
     if has_modifiers(data) and ids and (not force):
-        modifiers = data.modifiers
+        modifiers = data.__modifiers__
 
-        assign = modifiers.assign
-        excluded = modifiers.excluded
-        properties = modifiers.properties
-        protected = modifiers.protected
-        hidden = modifiers.hidden
-        legalize = modifiers.legalize
-        defined = modifiers.defined
-        color = modifiers.color
+    else:
+        modifiers = Modifiers(
+            assign=assign, protected=protected, legalize=legalize,
+            force=force, defined=defined, color=color, hidden=hidden,
+            properties=properties, excluded=excluded
+        )
     # end if
 
+    assign = modifiers.assign
+    excluded = modifiers.excluded
+    properties = modifiers.properties
+    protected = modifiers.protected
+    hidden = modifiers.hidden
+    legalize = modifiers.legalize
+    defined = modifiers.defined
+    color = modifiers.color
+
     if (
         inspect.isfunction(data) or
         inspect.ismethod(data)
     ):
         if is_bound_method(data) and legalize:
             return repr(data)
         # end if
@@ -522,35 +569,64 @@
     )
 
     ids[data_id] = results
 
     return results
 # end unwrap
 
-def to_string(obj: Any, /, modifiers: Optional[Modifiers] = None) -> str:
+def to_string(data: Any, /, modifiers: Optional[Modifiers] = None) -> str:
     """
     Returns a string to represent the model commands and structure.
 
+    :param data: The object to represent.
+    :param modifiers: The modifiers for the process.
+
     :return: The string representation of the model.
     """
 
     if modifiers is None:
-        if (
-            isinstance(obj, BaseModel) and
-            hasattr(obj, "modifiers") and
-            isinstance(obj.modifiers, Modifiers)
-        ):
-            modifiers = obj.modifiers
+        if has_modifiers(data):
+            modifiers = data.__modifiers__
 
         else:
             modifiers = Modifiers()
         # end if
     # end if
 
-    data = indent(str(unwrap(obj, **modifiers)))
+    result = indent(str(unwrap(data, **modifiers)))
 
     if modifiers.assign and modifiers.color:
-        data = colorize(data)
+        result = colorize(result)
     # end if
 
-    return data
-# end to_string
+    return result
+# end to_string
+
+_C = TypeVar("_C")
+
+def __str__(self) -> str:
+    """
+    Returns a string to represent the model commands and structure.
+
+    :return: The string representation of the model.
+    """
+
+    return to_string(self)
+# end __str__
+
+def represent(base: _C, /) -> _C:
+    """
+    Adds the string method and modifiers to represent the model.
+
+    :param base: The base class.
+
+    :return: The modified base class.
+    """
+
+    base.__str__ = __str__
+
+    if not has_modifiers(base):
+        base.__modifiers__ = Modifiers()
+    # end if
+
+    return base
+# end represent
```

### Comparing `pyrepresent-0.2.5/represent/structures.py` & `pyrepresent-0.2.6/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.5/setup.py` & `pyrepresent-0.2.6/setup.py`

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
-        version='0.2.5',
+        version='0.2.6',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.5/test.py` & `pyrepresent-0.2.6/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # test.py
 
 import datetime as dt
 
 import pandas as pd
 import numpy as np
 
-from represent import BaseModel, indent, unwrap, colorize, to_string
+from represent import represent, indent, unwrap, colorize, to_string
 
-class Model(BaseModel):
+@represent
+class Model:
 
     def __init__(self) -> None:
 
         self.datetime = dt.datetime.now()
         self.date = self.datetime.date()
         self.time = self.datetime.time()
 
@@ -32,15 +33,16 @@
         self.zero = 0
 
         self.data = pd.DataFrame({1: [1, 2, 3]})
         self.array = np.array([[1, 2, 3], [4, 5, 6]])
     # end __init__
 # Model
 
-class Data(BaseModel):
+@represent
+class Data:
 
     __slots__ = "x", "y"
 
     def __init__(self):
 
         self.x = 0
         self.y = 0
```


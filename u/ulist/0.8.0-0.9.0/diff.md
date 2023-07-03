# Comparing `tmp/ulist-0.8.0-cp39-none-win_amd64.whl.zip` & `tmp/ulist-0.9.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 287120 bytes, number of entries: 13
--rw-r--r--  4.6 unx       66 b- defN 22-Mar-12 11:16 ulist-0.8.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 22-Mar-12 11:16 ulist-0.8.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     5587 b- defN 22-Mar-12 11:16 ulist/constructor.py
--rw-r--r--  4.6 unx     4373 b- defN 22-Mar-12 11:16 ulist/control_flow.py
--rw-r--r--  4.6 unx    18663 b- defN 22-Mar-12 11:16 ulist/core.py
--rw-r--r--  4.6 unx      146 b- defN 22-Mar-12 11:16 ulist/mypy.ini
--rw-r--r--  4.6 unx        0 b- defN 22-Mar-12 11:16 ulist/py.typed
--rw-r--r--  4.6 unx      413 b- defN 22-Mar-12 11:16 ulist/typedef.py
--rw-r--r--  4.6 unx     8074 b- defN 22-Mar-12 11:16 ulist/ulist.pyi
--rw-r--r--  4.6 unx     8859 b- defN 22-Mar-12 11:16 ulist/utils.py
--rw-r--r--  4.6 unx      232 b- defN 22-Mar-12 11:16 ulist/__init__.py
--rwxr-xr-x  4.6 unx   737280 b- defN 22-Mar-12 11:16 ulist/ulist.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      939 b- defN 22-Mar-12 11:16 ulist-0.8.0.dist-info/RECORD
-13 files, 784728 bytes uncompressed, 285592 bytes compressed:  63.6%
+Zip file size: 359603 bytes, number of entries: 13
+-rw-r--r--  4.6 unx       66 b- defN 22-Mar-31 11:56 ulist-0.9.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 22-Mar-31 11:56 ulist-0.9.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     6824 b- defN 22-Mar-31 11:56 ulist/constructor.py
+-rw-r--r--  4.6 unx     4373 b- defN 22-Mar-31 11:56 ulist/control_flow.py
+-rw-r--r--  4.6 unx    20081 b- defN 22-Mar-31 11:56 ulist/core.py
+-rw-r--r--  4.6 unx      146 b- defN 22-Mar-31 11:56 ulist/mypy.ini
+-rw-r--r--  4.6 unx        0 b- defN 22-Mar-31 11:56 ulist/py.typed
+-rw-r--r--  4.6 unx      561 b- defN 22-Mar-31 11:56 ulist/typedef.py
+-rw-r--r--  4.6 unx    13321 b- defN 22-Mar-31 11:56 ulist/ulist.pyi
+-rw-r--r--  4.6 unx    10091 b- defN 22-Mar-31 11:56 ulist/utils.py
+-rw-r--r--  4.6 unx      232 b- defN 22-Mar-31 11:56 ulist/__init__.py
+-rwxr-xr-x  4.6 unx  1007104 b- defN 22-Mar-31 11:56 ulist/ulist.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      942 b- defN 22-Mar-31 11:56 ulist-0.9.0.dist-info/RECORD
+13 files, 1063837 bytes uncompressed, 358075 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: ulist-0.8.0.dist-info/METADATA
+Filename: ulist-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: ulist-0.8.0.dist-info/WHEEL
+Filename: ulist-0.9.0.dist-info/WHEEL
 Comment: 
 
 Filename: ulist/constructor.py
 Comment: 
 
 Filename: ulist/control_flow.py
 Comment: 
@@ -30,11 +30,11 @@
 
 Filename: ulist/__init__.py
 Comment: 
 
 Filename: ulist/ulist.cp39-win_amd64.pyd
 Comment: 
 
-Filename: ulist-0.8.0.dist-info/RECORD
+Filename: ulist-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ulist/constructor.py

```diff
@@ -1,30 +1,44 @@
 from typing import Optional, Sequence
 
 from .core import UltraFastList
-from .ulist import BooleanList, FloatList, IntegerList, StringList
-from .ulist import arange as _arange
 from .typedef import ELEM
-
-
-def arange(start: int, stop: Optional[int] = None, step: int = 1
-           ) -> UltraFastList:
+from .ulist import (
+    BooleanList,
+    FloatList32,
+    FloatList64,
+    IntegerList32,
+    IntegerList64,
+    StringList,
+    arange32,
+    arange64
+)
+
+
+def arange(
+    start: int,
+    stop: Optional[int] = None,
+    step: int = 1,
+    dtype: str = 'int',
+) -> UltraFastList:
     """Return evenly spaced values within a given interval, which is similar
     to the Python built-in range function, but returns an ulist rather than
     a list.
 
     Args:
         start (int):
             Start of interval. The interval includes this value.
             If stop is not given, then start=0 and stop=start.
         stop (Optional[int], optional):
             End of interval. The interval does not include this value.
             Defaults to None.
         step (int, optional):
             Spacing between values. Defaults to 1.
+        dtype (str, optional):
+            The type of the output ulist. 'int', 'int32', 'int64'.
 
     Returns:
         UltraFastList: A ulist object.
 
     Examples
     --------
     >>> import ulist as ul
@@ -39,31 +53,39 @@
     >>> arr3 = ul.arange(1, 6, 2)
     >>> arr3
     UltraFastList([1, 3, 5])
     """
     if stop is None:
         stop = start
         start = 0
-    return UltraFastList(_arange(start=start, stop=stop, step=step))
+    if dtype == "int" or dtype == "int64":
+        return UltraFastList(arange64(start=start, stop=stop, step=step))
+    elif dtype == "int32":
+        return UltraFastList(arange32(start=start, stop=stop, step=step))
+    else:
+        raise ValueError(
+            "Parameter dtype should be 'int', 'int32' or 'int64'!")
 
 
 def cycle(obj: Sequence, size: int, dtype: str) -> UltraFastList:
     """Repeats a sequence endlessly until the size is met.
 
     Args:
         obj (Sequence):
             Sequence object such as list, tuple and range.
         size (int):
             size (int): Size of the new ulist.
         dtype (str):
-            The type of the output ulist. 'int', 'float', 'bool' or 'string'.
+            The type of the output ulist. 'int', 'int32', 'int64',
+            'float', 'float32', 'float64', 'bool' or 'string'.
 
     Raises:
         ValueError:
-            Parameter dtype should be 'int', 'float', 'bool' or 'string'!
+            Parameter dtype should be 'int', 'int32', 'int64',
+            'float', 'float32', 'float64', 'bool' or 'string'!
 
     Returns:
         UltraFastList: A ulist object.
 
     Examples
     --------
     >>> import ulist as ul
@@ -79,40 +101,48 @@
     >>> arr3
     UltraFastList([True, True, True])
 
     >>> arr4 = ul.cycle(['foo'], 3, 'string')
     >>> arr4
     UltraFastList(['foo', 'foo', 'foo'])
     """
-    if dtype == "int":
-        result = UltraFastList(IntegerList.cycle(obj, size))
-    elif dtype == "float":
-        result = UltraFastList(FloatList.cycle(obj, size))
+    if dtype == "int" or dtype == "int64":
+        result = UltraFastList(IntegerList64.cycle(obj, size))
+    elif dtype == "int32":
+        result = UltraFastList(IntegerList32.cycle(obj, size))
+    elif dtype == "float" or dtype == "float64":
+        result = UltraFastList(FloatList64.cycle(obj, size))
+    elif dtype == "float32":
+        result = UltraFastList(FloatList32.cycle(obj, size))
     elif dtype == "bool":
         result = UltraFastList(BooleanList.cycle(obj, size))
     elif dtype == "string":
         result = UltraFastList(StringList.cycle(obj, size))
     else:
         raise ValueError(
-            "Parameter dtype should be 'int', 'float', 'bool' or 'string'!")
+            "Parameter dtype should be 'int', 'int32', 'int64', " +
+            "'float', 'float32', 'float64', 'bool' or 'string'!"
+        )
     return result
 
 
 def from_seq(obj: Sequence, dtype: str) -> UltraFastList:
     """Construct a ulist object from a sequence object.
 
     Args:
         obj (Sequence):
             Sequence object such as list, tuple and range.
         dtype (str):
-            The type of the output ulist. 'int', 'float', 'bool' or 'string'.
+            The type of the output ulist. 'int', 'int32', 'int64',
+            'float', 'float32', 'float64', 'bool' or 'string'.
 
     Raises:
         ValueError:
-            Parameter dtype should be 'int', 'float', 'bool' or 'string'!
+            Parameter dtype should be 'int', 'int32', 'int64',
+            'float', 'float32', 'float64', 'bool' or 'string'!
 
     Returns:
         UltraFastList: A ulist object.
 
     Examples
     --------
     >>> import ulist as ul
@@ -128,25 +158,31 @@
     >>> arr3
     UltraFastList([True, True, False])
 
     >>> arr4 = ul.from_seq(('foo', 'bar', 'baz'), dtype='string')
     >>> arr4
     UltraFastList(['foo', 'bar', 'baz'])
     """
-    if dtype == "int":
-        result = UltraFastList(IntegerList(obj))
-    elif dtype == "float":
-        result = UltraFastList(FloatList(obj))
+    if dtype == "int" or dtype == "int64":
+        result = UltraFastList(IntegerList64(obj))
+    elif dtype == "int32":
+        result = UltraFastList(IntegerList32(obj))
+    elif dtype == "float" or dtype == "float64":
+        result = UltraFastList(FloatList64(obj))
+    elif dtype == "float32":
+        result = UltraFastList(FloatList32(obj))
     elif dtype == "bool":
         result = UltraFastList(BooleanList(obj))
     elif dtype == "string":
         result = UltraFastList(StringList(obj))
     else:
         raise ValueError(
-            "Parameter dtype should be 'int', 'float', 'bool' or 'string'!")
+            "Parameter dtype should be 'int', 'int32', 'int64', " +
+            "'float', 'float32', 'float64', 'bool' or 'string'!"
+        )
     return result
 
 
 def repeat(elem: ELEM, size: int) -> UltraFastList:
     """Return a new ulist of given size, filled with elem.
 
     Args:
@@ -177,15 +213,15 @@
     >>> arr4 = ul.repeat('foo', 3)
     >>> arr4
     UltraFastList(['foo', 'foo', 'foo'])
     """
     if isinstance(elem, bool):
         return UltraFastList(BooleanList.repeat(elem, size))
     elif isinstance(elem, float):
-        return UltraFastList(FloatList.repeat(elem, size))
+        return UltraFastList(FloatList64.repeat(elem, size))
     elif isinstance(elem, int):
-        return UltraFastList(IntegerList.repeat(elem, size))
+        return UltraFastList(IntegerList64.repeat(elem, size))
     elif isinstance(elem, str):
         return UltraFastList(StringList.repeat(elem, size))
     else:
         raise TypeError(
             "Parameter elem should be int, float, bool or str type!")
```

## ulist/core.py

```diff
@@ -1,13 +1,21 @@
 from __future__ import annotations  # To avoid circular import.
 
 from typing import TYPE_CHECKING, Callable, Union
 
 from .typedef import COUNTER, ELEM, LIST_PY, LIST_RS, NUM
-from .ulist import BooleanList, FloatList, IndexList, IntegerList, StringList
+from .ulist import (
+    BooleanList,
+    FloatList32,
+    FloatList64,
+    IndexList,
+    IntegerList32,
+    IntegerList64,
+    StringList
+)
 
 if TYPE_CHECKING:  # To avoid circular import.
     from .control_flow import CaseObject
 
 NUM_OR_LIST = Union[NUM, "UltraFastList"]
 ELEM_OR_LIST = Union[ELEM, "UltraFastList"]
 
@@ -15,26 +23,31 @@
 class UltraFastList:
     """
     Ultra fast list data structures written in Rust with Python bindings,
     which is abbreviated as ulist.
     """
 
     def __init__(self, values: LIST_RS) -> None:
-        if type(values) is FloatList:
-            self.dtype = "float"
-        elif type(values) is IntegerList:
-            self.dtype = "int"
+        if type(values) is FloatList32:
+            self.dtype = "float32"
+        elif type(values) is FloatList64:
+            self.dtype = "float64"
+        elif type(values) is IntegerList32:
+            self.dtype = "int32"
+        elif type(values) is IntegerList64:
+            self.dtype = "int64"
         elif type(values) is BooleanList:
             self.dtype = "bool"
         elif type(values) is StringList:
             self.dtype = "string"
         else:
             raise TypeError(
-                "Parameter values should be FloatList, "
-                + "IntegerList, BooleanList or StringList type!"
+                "Parameter values should be " +
+                "FloatList32, FloatList64, IntegerList32, " +
+                "IntegerList64, BooleanList or StringList type!"
             )
         self._values = values
 
     def __len__(self) -> int:
         """Number of elements of self."""
         return self.size()
 
@@ -207,42 +220,54 @@
         return self._values.argmin()
 
     def astype(self, dtype: str) -> "UltraFastList":
         """Copy of self, cast to a specified dtype.
 
         Raises:
             ValueError:
-                Parameter dtype should be 'int', 'float', 'bool' or 'string'!
+                Parameter dtype should be 'int', 'int32', 'int64',
+                'float', 'float32', 'float64', 'bool' or 'string'!
 
         Returns:
             UltraFastList: A ulist object.
         """
-        if dtype == "int":
-            if isinstance(self._values, IntegerList):
+        if dtype == "int" or dtype == "int64":
+            if isinstance(self._values, IntegerList64):
                 result = self.copy()
             else:
-                result = UltraFastList(self._values.as_int())
-        elif dtype == "float":
-            if isinstance(self._values, FloatList):
+                result = UltraFastList(self._values.as_int64())
+        elif dtype == "int32":
+            if isinstance(self._values, IntegerList32):
                 result = self.copy()
             else:
-                result = UltraFastList(self._values.as_float())
+                result = UltraFastList(self._values.as_int32())
+        elif dtype == "float" or dtype == "float64":
+            if isinstance(self._values, FloatList64):
+                result = self.copy()
+            else:
+                result = UltraFastList(self._values.as_float64())
+        elif dtype == "float32":
+            if isinstance(self._values, FloatList32):
+                result = self.copy()
+            else:
+                result = UltraFastList(self._values.as_float32())
         elif dtype == "bool":
             if isinstance(self._values, BooleanList):
                 result = self.copy()
             else:
                 result = UltraFastList(self._values.as_bool())
         elif dtype == "string":
             if isinstance(self._values, StringList):
                 result = self.copy()
             else:
                 result = UltraFastList(self._values.as_str())
         else:
             raise ValueError(
-                "Parameter dtype should be 'int', 'float', 'bool' or 'string'!"
+                "Parameter dtype should be 'int', 'int32', 'int64', " +
+                "'float', 'float32', 'float64', 'bool' or 'string'!"
             )
         return result
 
     def case(self, default: ELEM) -> CaseObject:
         """A method similar to SQL's `case` statement.
 
         Args:
@@ -280,28 +305,33 @@
         return UltraFastList(self._values.copy())
 
     def counter(self) -> COUNTER:
         """
         Return a dictionary where the elements of self are stored as
         dictionary keys and their counts are stored as dictionary values.
         """
-        assert not isinstance(self._values, FloatList)
+        assert not isinstance(self._values, (FloatList32, FloatList64))
         return self._values.counter()
 
     def div(self, other: "UltraFastList") -> "UltraFastList":
         """Return self / other."""
         assert not isinstance(self._values, (BooleanList, StringList))
         assert not isinstance(other._values, (BooleanList, StringList))
         return UltraFastList(self._values.div(other._values))
 
     def div_scala(self, elem: float) -> "UltraFastList":
         """Return self / elem."""
         assert not isinstance(self._values, (BooleanList, StringList))
         return UltraFastList(self._values.div_scala(elem))
 
+    def ends_with(self, elem: str) -> UltraFastList:
+        """Return whether the element of self ends with `elem`."""
+        assert isinstance(self._values, StringList)
+        return UltraFastList(self._values.ends_with(elem))
+
     def equal_scala(self, elem: NUM) -> "UltraFastList":
         """Return self == elem."""
         return UltraFastList(self._values.equal_scala(elem))
 
     def filter(self, condition: "UltraFastList") -> "UltraFastList":
         """
         According to the condition, return a ulist with elements of self
@@ -407,14 +437,19 @@
                 Ascending or descending.
 
         Returns:
             UltraFastList: The sorted ulist.
         """
         return UltraFastList(self._values.sort(ascending=ascending))
 
+    def starts_with(self, elem: str) -> UltraFastList:
+        """Return whether the element of self starts with `elem`."""
+        assert isinstance(self._values, StringList)
+        return UltraFastList(self._values.starts_with(elem))
+
     def sub(self, other: "UltraFastList") -> "UltraFastList":
         """Return self - other."""
         assert not isinstance(self._values, (BooleanList, StringList))
         assert not isinstance(other._values, (BooleanList, StringList))
         return UltraFastList(self._values.sub(other._values))
 
     def sub_scala(self, elem: NUM) -> "UltraFastList":
@@ -467,17 +502,17 @@
 
         Raises:
             TypeError: Only support dtype int, float and bool.
 
         Returns:
             float: variance
         """
-        if isinstance(self._values, FloatList):
+        if isinstance(self._values, (FloatList32, FloatList64)):
             data = self
-        elif isinstance(self._values, IntegerList):
+        elif isinstance(self._values, (IntegerList32, IntegerList64)):
             data = self.astype('float')
         elif isinstance(self._values, BooleanList):
             data = self.astype('float')
         else:
             raise TypeError(f"Var method does not support dtype {self.dtype}!")
         mean = data.mean()
         numerator = data.sub_scala(mean).pow_scala(2).sum()
```

## ulist/typedef.py

```diff
@@ -1,10 +1,18 @@
-from typing import List, Union, Dict
+from typing import Dict, List, Union
 
-from .ulist import BooleanList, FloatList, IntegerList, StringList
+from .ulist import (
+    BooleanList,
+    FloatList32,
+    FloatList64,
+    IntegerList32,
+    IntegerList64,
+    StringList
+)
 
 ELEM = Union[int, float, bool, str]
 NUM = Union[int, float]
 LIST_PY = Union[List[float], List[int], List[bool], List[str]]
-LIST_RS = Union[FloatList, IntegerList, BooleanList, StringList]
-NUM_LIST_RS = Union[FloatList, IntegerList]
+LIST_RS = Union[FloatList32, FloatList64, IntegerList32,
+                IntegerList64, BooleanList, StringList]
+NUM_LIST_RS = Union[FloatList32, FloatList64, IntegerList32, IntegerList64]
 COUNTER = Union[Dict[int, int], Dict[bool, int], Dict[str, int]]
```

## ulist/ulist.pyi

```diff
@@ -7,16 +7,18 @@
     # Arrange the following methods in alphabetical order.
 
     def __init__(self, vec: Sequence[bool]) -> None: ...
     def all(self) -> bool: ...
     def and_(self, other: BooleanList) -> BooleanList: ...
     def any(self) -> bool: ...
     def append(self, elem: ELEM): ...
-    def as_float(self) -> FloatList: ...
-    def as_int(self) -> IntegerList: ...
+    def as_float32(self) -> FloatList32: ...
+    def as_float64(self) -> FloatList64: ...
+    def as_int32(self) -> IntegerList32: ...
+    def as_int64(self) -> IntegerList64: ...
     def as_str(self) -> StringList: ...
     def copy(self) -> BooleanList: ...
     def counter(self) -> Dict[bool, int]: ...
     @staticmethod
     def cycle(obj: Sequence[bool], size: int) -> BooleanList: ...
     def equal_scala(self, elem: ELEM) -> BooleanList: ...
     def filter(self, condition: BooleanList) -> BooleanList: ...
@@ -35,132 +37,237 @@
     def sum(self) -> int: ...
     def to_index(self) -> IndexList: ...
     def to_list(self) -> List[bool]: ...
     def union_all(self, other: LIST_RS) -> LIST_RS: ...
     def unique(self) -> BooleanList: ...
 
 
-class FloatList:
+class FloatList32:
     #  Arrange the following methods in alphabetical order.
 
     def __init__(self, vec: Sequence[float]) -> None: ...
-    def add(self, other: NUM_LIST_RS) -> FloatList: ...
-    def add_scala(self, elem: NUM) -> FloatList: ...
+    def add(self, other: NUM_LIST_RS) -> FloatList32: ...
+    def add_scala(self, elem: NUM) -> FloatList32: ...
     def append(self, elem: ELEM) -> None: ...
     def argmax(self) -> int: ...
     def argmin(self) -> int: ...
     def as_bool(self) -> BooleanList: ...
-    def as_int(self) -> IntegerList: ...
+    def as_float64(self) -> FloatList64: ...
+    def as_int32(self) -> IntegerList32: ...
+    def as_int64(self) -> IntegerList64: ...
     def as_str(self) -> StringList: ...
-    def copy(self) -> FloatList: ...
+    def copy(self) -> FloatList32: ...
     @staticmethod
-    def cycle(obj: Sequence[float], size: int) -> FloatList: ...
-    def div(self, other: NUM_LIST_RS) -> FloatList: ...
-    def div_scala(self, elem: float) -> FloatList: ...
+    def cycle(obj: Sequence[float], size: int) -> FloatList32: ...
+    def div(self, other: NUM_LIST_RS) -> FloatList32: ...
+    def div_scala(self, elem: float) -> FloatList32: ...
     def equal_scala(self, elem: NUM) -> BooleanList: ...
-    def filter(self, condition: BooleanList) -> FloatList: ...
+    def filter(self, condition: BooleanList) -> FloatList32: ...
     def get(self, index: int) -> float: ...
-    def get_by_indexes(self, indexes: IndexList) -> FloatList: ...
+    def get_by_indexes(self, indexes: IndexList) -> FloatList32: ...
     def greater_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
     def greater_than_scala(self, elem: NUM) -> BooleanList: ...
     def less_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
     def less_than_scala(self, elem: NUM) -> BooleanList: ...
     def max(self) -> float: ...
     def min(self) -> float: ...
-    def mul(self, other: NUM_LIST_RS) -> FloatList: ...
-    def mul_scala(self, elem: NUM) -> FloatList: ...
+    def mul(self, other: NUM_LIST_RS) -> FloatList32: ...
+    def mul_scala(self, elem: NUM) -> FloatList32: ...
     def not_equal_scala(self, elem: NUM) -> BooleanList: ...
     def pop(self) -> None: ...
-    def pow_scala(self, elem: int) -> FloatList: ...
+    def pow_scala(self, elem: int) -> FloatList32: ...
     @staticmethod
-    def repeat(elem: float, size: int) -> FloatList: ...
-    def replace(self, old: ELEM, new: ELEM) -> FloatList: ...
+    def repeat(elem: float, size: int) -> FloatList32: ...
+    def replace(self, old: ELEM, new: ELEM) -> FloatList32: ...
     def set(self, index: int, elem: ELEM) -> None: ...
     def size(self) -> int: ...
-    def sort(self, ascending: bool) -> FloatList: ...
-    def sub(self, other: NUM_LIST_RS) -> FloatList: ...
-    def sub_scala(self, elem: NUM) -> FloatList: ...
+    def sort(self, ascending: bool) -> FloatList32: ...
+    def sub(self, other: NUM_LIST_RS) -> FloatList32: ...
+    def sub_scala(self, elem: NUM) -> FloatList32: ...
     def sum(self) -> float: ...
     def to_list(self) -> List[float]: ...
     def union_all(self, other: LIST_RS) -> LIST_RS: ...
-    def unique(self) -> FloatList: ...
+    def unique(self) -> FloatList32: ...
 
 
-class IntegerList:
+class FloatList64:
+    #  Arrange the following methods in alphabetical order.
+
+    def __init__(self, vec: Sequence[float]) -> None: ...
+    def add(self, other: NUM_LIST_RS) -> FloatList64: ...
+    def add_scala(self, elem: NUM) -> FloatList64: ...
+    def append(self, elem: ELEM) -> None: ...
+    def argmax(self) -> int: ...
+    def argmin(self) -> int: ...
+    def as_bool(self) -> BooleanList: ...
+    def as_float32(self) -> FloatList32: ...
+    def as_int32(self) -> IntegerList32: ...
+    def as_int64(self) -> IntegerList64: ...
+    def as_str(self) -> StringList: ...
+    def copy(self) -> FloatList64: ...
+    @staticmethod
+    def cycle(obj: Sequence[float], size: int) -> FloatList64: ...
+    def div(self, other: NUM_LIST_RS) -> FloatList64: ...
+    def div_scala(self, elem: float) -> FloatList64: ...
+    def equal_scala(self, elem: NUM) -> BooleanList: ...
+    def filter(self, condition: BooleanList) -> FloatList64: ...
+    def get(self, index: int) -> float: ...
+    def get_by_indexes(self, indexes: IndexList) -> FloatList64: ...
+    def greater_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
+    def greater_than_scala(self, elem: NUM) -> BooleanList: ...
+    def less_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
+    def less_than_scala(self, elem: NUM) -> BooleanList: ...
+    def max(self) -> float: ...
+    def min(self) -> float: ...
+    def mul(self, other: NUM_LIST_RS) -> FloatList64: ...
+    def mul_scala(self, elem: NUM) -> FloatList64: ...
+    def not_equal_scala(self, elem: NUM) -> BooleanList: ...
+    def pop(self) -> None: ...
+    def pow_scala(self, elem: int) -> FloatList64: ...
+    @staticmethod
+    def repeat(elem: float, size: int) -> FloatList64: ...
+    def replace(self, old: ELEM, new: ELEM) -> FloatList64: ...
+    def set(self, index: int, elem: ELEM) -> None: ...
+    def size(self) -> int: ...
+    def sort(self, ascending: bool) -> FloatList64: ...
+    def sub(self, other: NUM_LIST_RS) -> FloatList64: ...
+    def sub_scala(self, elem: NUM) -> FloatList64: ...
+    def sum(self) -> float: ...
+    def to_list(self) -> List[float]: ...
+    def union_all(self, other: LIST_RS) -> LIST_RS: ...
+    def unique(self) -> FloatList64: ...
+
+
+class IntegerList32:
     #  Arrange the following methods in alphabetical order.
 
     def __init__(self, vec: Sequence[int]) -> None: ...
-    def add(self, other: NUM_LIST_RS) -> IntegerList: ...
-    def add_scala(self, elem: NUM) -> IntegerList: ...
+    def add(self, other: NUM_LIST_RS) -> IntegerList32: ...
+    def add_scala(self, elem: NUM) -> IntegerList32: ...
     def append(self, elem: ELEM) -> None: ...
     def argmax(self) -> int: ...
     def argmin(self) -> int: ...
     def as_bool(self) -> BooleanList: ...
-    def as_float(self) -> FloatList: ...
+    def as_float32(self) -> FloatList32: ...
+    def as_float64(self) -> FloatList64: ...
+    def as_int64(self) -> IntegerList64: ...
     def as_str(self) -> StringList: ...
-    def copy(self) -> IntegerList: ...
+    def copy(self) -> IntegerList32: ...
     def counter(self) -> Dict[int, int]: ...
     @staticmethod
-    def cycle(obj: Sequence[int], size: int) -> IntegerList: ...
-    def div(self, other: NUM_LIST_RS) -> FloatList: ...
-    def div_scala(self, elem: float) -> FloatList: ...
+    def cycle(obj: Sequence[int], size: int) -> IntegerList32: ...
+    def div(self, other: NUM_LIST_RS) -> FloatList32: ...
+    def div_scala(self, elem: float) -> FloatList32: ...
     def equal_scala(self, elem: NUM) -> BooleanList: ...
-    def filter(self, condition: BooleanList) -> IntegerList: ...
+    def filter(self, condition: BooleanList) -> IntegerList32: ...
     def get(self, index: int) -> int: ...
-    def get_by_indexes(self, indexes: IndexList) -> IntegerList: ...
+    def get_by_indexes(self, indexes: IndexList) -> IntegerList32: ...
     def greater_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
     def greater_than_scala(self, elem: NUM) -> BooleanList: ...
     def less_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
     def less_than_scala(self, elem: NUM) -> BooleanList: ...
     def max(self) -> int: ...
     def min(self) -> int: ...
-    def mul(self, other: NUM_LIST_RS) -> IntegerList: ...
-    def mul_scala(self, elem: NUM) -> IntegerList: ...
+    def mul(self, other: NUM_LIST_RS) -> IntegerList32: ...
+    def mul_scala(self, elem: NUM) -> IntegerList32: ...
     def not_equal_scala(self, elem: NUM) -> BooleanList: ...
     def pop(self) -> None: ...
-    def pow_scala(self, elem: int) -> IntegerList: ...
+    def pow_scala(self, elem: int) -> IntegerList32: ...
     def set(self, index: int, elem: ELEM) -> None: ...
     @staticmethod
-    def repeat(elem: int, size: int) -> IntegerList: ...
-    def replace(self, old: ELEM, new: ELEM) -> IntegerList: ...
+    def repeat(elem: int, size: int) -> IntegerList32: ...
+    def replace(self, old: ELEM, new: ELEM) -> IntegerList32: ...
     def size(self) -> int: ...
-    def sort(self, ascending: bool) -> IntegerList: ...
-    def sub(self, other: NUM_LIST_RS) -> IntegerList: ...
-    def sub_scala(self, elem: NUM) -> IntegerList: ...
+    def sort(self, ascending: bool) -> IntegerList32: ...
+    def sub(self, other: NUM_LIST_RS) -> IntegerList32: ...
+    def sub_scala(self, elem: NUM) -> IntegerList32: ...
     def sum(self) -> int: ...
     def to_list(self) -> List[int]: ...
     def union_all(self, other: LIST_RS) -> LIST_RS: ...
-    def unique(self) -> IntegerList: ...
+    def unique(self) -> IntegerList32: ...
+
+
+class IntegerList64:
+    #  Arrange the following methods in alphabetical order.
+
+    def __init__(self, vec: Sequence[int]) -> None: ...
+    def add(self, other: NUM_LIST_RS) -> IntegerList64: ...
+    def add_scala(self, elem: NUM) -> IntegerList64: ...
+    def append(self, elem: ELEM) -> None: ...
+    def argmax(self) -> int: ...
+    def argmin(self) -> int: ...
+    def as_bool(self) -> BooleanList: ...
+    def as_float32(self) -> FloatList32: ...
+    def as_float64(self) -> FloatList64: ...
+    def as_int32(self) -> IntegerList32: ...
+    def as_str(self) -> StringList: ...
+    def copy(self) -> IntegerList64: ...
+    def counter(self) -> Dict[int, int]: ...
+    @staticmethod
+    def cycle(obj: Sequence[int], size: int) -> IntegerList64: ...
+    def div(self, other: NUM_LIST_RS) -> FloatList64: ...
+    def div_scala(self, elem: float) -> FloatList64: ...
+    def equal_scala(self, elem: NUM) -> BooleanList: ...
+    def filter(self, condition: BooleanList) -> IntegerList64: ...
+    def get(self, index: int) -> int: ...
+    def get_by_indexes(self, indexes: IndexList) -> IntegerList64: ...
+    def greater_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
+    def greater_than_scala(self, elem: NUM) -> BooleanList: ...
+    def less_than_or_equal_scala(self, elem: NUM) -> BooleanList: ...
+    def less_than_scala(self, elem: NUM) -> BooleanList: ...
+    def max(self) -> int: ...
+    def min(self) -> int: ...
+    def mul(self, other: NUM_LIST_RS) -> IntegerList64: ...
+    def mul_scala(self, elem: NUM) -> IntegerList64: ...
+    def not_equal_scala(self, elem: NUM) -> BooleanList: ...
+    def pop(self) -> None: ...
+    def pow_scala(self, elem: int) -> IntegerList64: ...
+    def set(self, index: int, elem: ELEM) -> None: ...
+    @staticmethod
+    def repeat(elem: int, size: int) -> IntegerList64: ...
+    def replace(self, old: ELEM, new: ELEM) -> IntegerList64: ...
+    def size(self) -> int: ...
+    def sort(self, ascending: bool) -> IntegerList64: ...
+    def sub(self, other: NUM_LIST_RS) -> IntegerList64: ...
+    def sub_scala(self, elem: NUM) -> IntegerList64: ...
+    def sum(self) -> int: ...
+    def to_list(self) -> List[int]: ...
+    def union_all(self, other: LIST_RS) -> LIST_RS: ...
+    def unique(self) -> IntegerList64: ...
 
 
 class StringList:
     # Arrange the following methods in alphabetical order.
 
     def __init__(self, vec: Sequence[str]) -> None: ...
     def append(self, elem: ELEM): ...
     def as_bool(self) -> BooleanList: ...
-    def as_float(self) -> FloatList: ...
-    def as_int(self) -> IntegerList: ...
+    def as_float32(self) -> FloatList32: ...
+    def as_float64(self) -> FloatList64: ...
+    def as_int32(self) -> IntegerList32: ...
+    def as_int64(self) -> IntegerList64: ...
     def contains(self, elem: str) -> BooleanList: ...
     def copy(self) -> StringList: ...
     def counter(self) -> Dict[str, int]: ...
     @staticmethod
     def cycle(obj: Sequence[str], size: int) -> StringList: ...
+    def ends_with(self, elem: str) -> BooleanList: ...
     def equal_scala(self, elem: ELEM) -> BooleanList: ...
     def filter(self, condition: BooleanList) -> StringList: ...
     def get(self, index: int) -> str: ...
     def get_by_indexes(self, indexes: IndexList) -> StringList: ...
     def not_equal_scala(self, elem: ELEM) -> BooleanList: ...
     def pop(self): ...
     @staticmethod
     def repeat(elem: str, size: int) -> StringList: ...
     def replace(self, old: ELEM, new: ELEM) -> StringList: ...
     def set(self, index: int, elem: ELEM): ...
     def size(self) -> int: ...
     def sort(self, ascending: bool) -> StringList: ...
+    def starts_with(self, elem: str) -> BooleanList: ...
     def to_list(self) -> List[str]: ...
     def union_all(self, other: LIST_RS) -> LIST_RS: ...
     def unique(self) -> StringList: ...
 
 
 class IndexList:
     # Arrange the following methods in alphabetical order.
@@ -168,36 +275,39 @@
     def __init__(self, vec: Sequence[int]) -> None: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
     def back(self) -> int: ...
     def to_list(self) -> List[int]: ...
 
 
-def arange(start: int, stop: int, step: int) -> IntegerList: ...
+def arange32(start: int, stop: int, step: int) -> IntegerList32: ...
+
+
+def arange64(start: int, stop: int, step: int) -> IntegerList64: ...
 
 
 def select_bool(
     conditions: List[BooleanList],
     choices: LIST_PY,
     default: bool,
 ) -> BooleanList: ...
 
 
 def select_float(
     conditions: List[BooleanList],
     choices: LIST_PY,
     default: float,
-) -> FloatList: ...
+) -> FloatList64: ...
 
 
 def select_int(
     conditions: List[BooleanList],
     choices: LIST_PY,
     default: int,
-) -> IntegerList: ...
+) -> IntegerList64: ...
 
 
 def select_string(
     conditions: List[BooleanList],
     choices: LIST_PY,
     default: str,
-) -> IntegerList: ...
+) -> StringList: ...
```

## ulist/utils.py

```diff
@@ -7,23 +7,59 @@
 
 from .typedef import COUNTER, ELEM, LIST_PY
 
 MAX_ITEM_LEN = 16
 MAX_DTYPE_LEN = 8
 
 
+def expand_dtypes(func: Callable) -> Callable:
+    """
+    Generate test cases for `int32` and `int64` dtypes by copying the
+    test cases of `int` dtype.
+
+    Generate test cases for `float32` and `float64` dtypes by copying the
+    test cases of `float` dtype.
+    """
+    def _new_arg(s: str) -> tuple:
+        return tuple([x if x != s else s for x in arg])
+
+    result = []
+    for arg in func.pytestmark[0].args[1]:  # type: ignore
+        if 'int' in arg:
+            result.append(_new_arg('int64'))
+            result.append(_new_arg('int32'))
+        elif 'float' in arg:
+            result.append(_new_arg('float64'))
+            result.append(_new_arg('float32'))
+    for arg in result:
+        func.pytestmark[0].args[1].append(arg)  # type: ignore
+    return func
+
+
+def compare_dtypes(dtype1: str, dtype2: str) -> bool:
+    """Compare two dtypes with each other."""
+    if dtype2 == 'int' or dtype2 == 'float':
+        dtype2, dtype1 = dtype1, dtype2
+    if dtype1 == 'int':
+        return dtype2 in ('int', 'int64')
+    if dtype1 == 'float':
+        return dtype2 in ('float', 'float64')
+    return dtype1 == dtype2
+
+
 def check_test_result(
     dtype: str,
     test_method: Union[Callable, str],
     result: Union[ELEM, LIST_PY, ul.UltraFastList],
     expected_value: Union[ELEM, LIST_PY, COUNTER],
 ):
     """Test if the result is as expected. Both value and type.
     Args:
-        dtype (str): 'int', 'float' or 'bool'.
+        dtype (str): 'int', 'int32', 'int64', 'float', 'float32',
+            'float64', 'bool' or 'string'.
         test_method (Union[Callable, str]): A method name or a function.
         result (Union[ELEM, LIST_PY, ul.UltraFastList])
         expected_value (Union[ELEM, LIST_PY])
     """
     msg = (
         f"dtype - {dtype}"
         + f" test_method - {test_method}"
```

## ulist/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .constructor import arange, cycle, from_seq, repeat  # noqa:F401
 from .control_flow import select  # noqa:F401
 from .core import UltraFastList  # noqa:F401
 from .ulist import IndexList  # noqa:F401
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
```


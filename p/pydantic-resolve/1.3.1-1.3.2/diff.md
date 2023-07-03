# Comparing `tmp/pydantic_resolve-1.3.1.tar.gz` & `tmp/pydantic_resolve-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.3.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.3.2.tar", max compression
```

## Comparing `pydantic_resolve-1.3.1.tar` & `pydantic_resolve-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.3.1/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.3.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.3.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.3.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.3.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6117 2023-06-27 16:04:17.836316 pydantic_resolve-1.3.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     3931 2023-07-02 22:57:40.903487 pydantic_resolve-1.3.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-02 23:09:00.565483 pydantic_resolve-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.3.1/README.md
--rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.3.2/LICENSE
+-rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.3.2/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.3.2/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.3.2/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.3.2/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6117 2023-06-27 16:04:17.836316 pydantic_resolve-1.3.2/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     4811 2023-07-03 08:00:07.994871 pydantic_resolve-1.3.2/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-03 08:19:26.214453 pydantic_resolve-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.3.2/README.md
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.3.2/PKG-INFO
```

### Comparing `pydantic_resolve-1.3.1/LICENSE` & `pydantic_resolve-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.1/pydantic_resolve/__init__.py` & `pydantic_resolve-1.3.2/pydantic_resolve/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from .core import resolve
 from .exceptions import (
     ResolverTargetAttrNotFound,
     DataloaderDependCantBeResolved,
     LoaderFieldNotProvidedError,
     MissingAnnotationError)
 from .resolver import Resolver, LoaderDepend
-from .util import build_list, build_object, mapper
+from .util import build_list, build_object, mapper, ensure_subset
 
 __all__ = [
     'resolve',
     'Resolver',
     'LoaderDepend',
     'ResolverTargetAttrNotFound',
     'DataloaderDependCantBeResolved',
     'LoaderFieldNotProvidedError',
     'MissingAnnotationError',
     'build_list',
     'build_object',
-    'mapper'
+    'mapper',
+    'ensure_subset'
 ]
```

### Comparing `pydantic_resolve-1.3.1/pydantic_resolve/core.py` & `pydantic_resolve-1.3.2/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.1/pydantic_resolve/resolver.py` & `pydantic_resolve-1.3.2/pydantic_resolve/resolver.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.1/pydantic_resolve/util.py` & `pydantic_resolve-1.3.2/pydantic_resolve/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,8 +110,30 @@
 def apply_rule(rule: Optional[Callable], target, source: Any, is_list: bool):
     if not rule:  # no change
         return source
 
     if is_list:
         return [rule(target, s) for s in source]
     else:
-        return rule(target, source)
+        return rule(target, source)
+    
+
+def ensure_subset(base):
+    """
+    used with pydantic class to make sure a class's field is 
+    subset of target class
+    """
+    def wrap(kls):
+        assert issubclass(base, BaseModel), 'base should be pydantic class'
+        assert issubclass(kls, BaseModel), 'class should be pydantic class'
+        @functools.wraps(kls)
+        def inner():
+            for k, field in kls.__fields__.items():
+                if field.required:
+                    base_field = base.__fields__.get(k)
+                    if not base_field:
+                        raise AttributeError(f'{k} not existed in {base.__name__}.')
+                    if base_field and base_field.type_ != field.type_:
+                        raise AttributeError(f'type of {k} not consistent with {base.__name__}'  )
+            return  kls
+        return inner()
+    return wrap
```

### Comparing `pydantic_resolve-1.3.1/pyproject.toml` & `pydantic_resolve-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.3.1"
+version = "1.3.2"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.3.1/README.md` & `pydantic_resolve-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.1/PKG-INFO` & `pydantic_resolve-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.3.1
+Version: 1.3.2
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```


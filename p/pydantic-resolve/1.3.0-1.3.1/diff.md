# Comparing `tmp/pydantic_resolve-1.3.0.tar.gz` & `tmp/pydantic_resolve-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.3.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.3.1.tar", max compression
```

## Comparing `pydantic_resolve-1.3.0.tar` & `pydantic_resolve-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.3.0/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.3.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.3.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.3.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.3.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6117 2023-06-27 16:04:17.836316 pydantic_resolve-1.3.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     3916 2023-06-20 06:16:54.008785 pydantic_resolve-1.3.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-27 16:03:58.731975 pydantic_resolve-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.3.0/README.md
--rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.3.1/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.3.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.3.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.3.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.3.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6117 2023-06-27 16:04:17.836316 pydantic_resolve-1.3.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     3931 2023-07-02 22:57:40.903487 pydantic_resolve-1.3.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-02 23:09:00.565483 pydantic_resolve-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.3.1/README.md
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.3.1/PKG-INFO
```

### Comparing `pydantic_resolve-1.3.0/LICENSE` & `pydantic_resolve-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.0/pydantic_resolve/__init__.py` & `pydantic_resolve-1.3.1/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.0/pydantic_resolve/core.py` & `pydantic_resolve-1.3.1/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.0/pydantic_resolve/resolver.py` & `pydantic_resolve-1.3.1/pydantic_resolve/resolver.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.0/pydantic_resolve/util.py` & `pydantic_resolve-1.3.1/pydantic_resolve/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,17 @@
     if issubclass(target, BaseModel):
         if target.Config.orm_mode:
             if isinstance(source, dict):
                 raise AttributeError(f"{type(source)} -> {target.__name__}: pydantic from_orm can't handle dict object")
             else:
                 return lambda t, s: t.from_orm(s)
 
-        if isinstance(source, dict):
+        if isinstance(source, (dict, BaseModel)):
             return lambda t, s: t.parse_obj(s)
+
         else:
             raise AttributeError(f"{type(source)} -> {target.__name__}: pydantic can't handle non-dict data")
     
     # dataclass
     if is_dataclass(target):
         if isinstance(source, dict):
             return lambda t, s: t(**s)
```

### Comparing `pydantic_resolve-1.3.0/pyproject.toml` & `pydantic_resolve-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.3.0"
+version = "1.3.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.3.0/README.md` & `pydantic_resolve-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.0/PKG-INFO` & `pydantic_resolve-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.3.0
+Version: 1.3.1
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```


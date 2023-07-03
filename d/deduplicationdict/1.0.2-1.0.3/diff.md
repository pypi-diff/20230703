# Comparing `tmp/deduplicationdict-1.0.2.tar.gz` & `tmp/deduplicationdict-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deduplicationdict-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deduplicationdict-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deduplicationdict-1.0.2.tar` & `deduplicationdict-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.2/LICENSE
--rw-r--r--   0        0        0     4095 2023-06-16 22:18:05.371028 deduplicationdict-1.0.2/README.md
--rw-r--r--   0        0        0    11503 2023-06-16 22:05:40.683130 deduplicationdict-1.0.2/deduplicationdict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.2/deduplicationdict/py.typed
--rw-r--r--   0        0        0     4026 2023-06-16 19:06:36.445758 deduplicationdict-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4095 2023-07-03 02:39:03.107016 deduplicationdict-1.0.3/README.md
+-rw-r--r--   0        0        0    11822 2023-07-03 02:35:41.555757 deduplicationdict-1.0.3/deduplicationdict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.3/deduplicationdict/py.typed
+-rw-r--r--   0        0        0     4026 2023-07-03 02:38:13.816358 deduplicationdict-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.3/PKG-INFO
```

### Comparing `deduplicationdict-1.0.2/LICENSE` & `deduplicationdict-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.2/README.md` & `deduplicationdict-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.2/deduplicationdict/__init__.py` & `deduplicationdict-1.0.3/deduplicationdict/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,29 +47,31 @@
     This class supports nested structures by automatically converting nested dictionaries into
     DeDuplicationDict instances. It also provides various conversion methods to convert between regular
     dictionaries and DeDuplicationDict instances.
 
     Attributes:
         hash_length (int): The length of the hash value used for deduplication.
         auto_clean_up (bool): Whether to automatically clean up unused hash values when deleting items.
+        skip_update_on_setitem (bool): Whether to skip updating the value dictionary when setting an item.
+        key_dict (dict): A dictionary that maps hash values to their corresponding values.
+        value_dict (dict): A dictionary that maps values to their corresponding hash values.
     """
 
-    hash_length: int = 8
-    auto_clean_up: bool = True
-    skip_update_on_setitem: bool = True
-
     def __init__(self, *args, _value_dict: dict = None, **kwargs):
         """Initialize a DeDuplicationDict instance.
 
         Args:
             *args: Positional arguments passed to the dict constructor.
             _value_dict (dict, optional): An existing value dictionary to use for deduplication.
             **kwargs: Keyword arguments passed to the dict constructor.
         """
 
+        self.hash_length: int = 8
+        self.auto_clean_up: bool = True
+        self.skip_update_on_setitem: bool = True
         self.key_dict: Dict[str, Union[str, DeDuplicationDict]] = {}
         self.value_dict: Dict[str, Any] = {} if _value_dict is None else _value_dict
 
         for k, v in dict(*args, **kwargs).items():
             self[k] = v
 
     def _set_value_dict(self, value_dict: dict, skip_update: bool = False) -> DeDuplicationDict:
```

### Comparing `deduplicationdict-1.0.2/pyproject.toml` & `deduplicationdict-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.setuptools.packages.find]
 where = ["deduplicationdict"]
 
 [project]
 # $ pip install deduplicationdict
 name = "deduplicationdict"
-version = "1.0.2"
+version = "1.0.3"
 description = "A dictionary that de-duplicates values."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["python", "dict", "deduplication", "optimization", ]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
```

### Comparing `deduplicationdict-1.0.2/PKG-INFO` & `deduplicationdict-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deduplicationdict
-Version: 1.0.2
+Version: 1.0.3
 Summary: A dictionary that de-duplicates values.
 Keywords: python,dict,deduplication,optimization
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```


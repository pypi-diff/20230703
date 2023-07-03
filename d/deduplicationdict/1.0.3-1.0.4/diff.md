# Comparing `tmp/deduplicationdict-1.0.3.tar.gz` & `tmp/deduplicationdict-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deduplicationdict-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deduplicationdict-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deduplicationdict-1.0.3.tar` & `deduplicationdict-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.3/LICENSE
--rw-r--r--   0        0        0     4095 2023-07-03 02:39:03.107016 deduplicationdict-1.0.3/README.md
--rw-r--r--   0        0        0    11822 2023-07-03 02:35:41.555757 deduplicationdict-1.0.3/deduplicationdict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.3/deduplicationdict/py.typed
--rw-r--r--   0        0        0     4026 2023-07-03 02:38:13.816358 deduplicationdict-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4095 2023-07-03 03:22:00.711013 deduplicationdict-1.0.4/README.md
+-rw-r--r--   0        0        0    12087 2023-07-03 03:27:54.678995 deduplicationdict-1.0.4/deduplicationdict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.4/deduplicationdict/py.typed
+-rw-r--r--   0        0        0     4026 2023-07-03 03:22:00.705013 deduplicationdict-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.4/PKG-INFO
```

### Comparing `deduplicationdict-1.0.3/LICENSE` & `deduplicationdict-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.3/README.md` & `deduplicationdict-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.3/deduplicationdict/__init__.py` & `deduplicationdict-1.0.4/deduplicationdict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,20 @@
             value (VT): The value to set for the given key.
         """
 
         if key in self.key_dict:
             del self[key]
 
         if isinstance(value, dict):
-            self.key_dict[key] = DeDuplicationDict(value, _value_dict=self.value_dict)
+            new_dd_dict = DeDuplicationDict(_value_dict=self.value_dict)
+            new_dd_dict.hash_length = self.hash_length
+            new_dd_dict.auto_clean_up = self.auto_clean_up
+            new_dd_dict.skip_update_on_setitem = self.skip_update_on_setitem
+            new_dd_dict.update(value)
+            self.key_dict[key] = new_dd_dict
         elif isinstance(value, DeDuplicationDict):
             self.key_dict[key] = value
             self.value_dict.update(value.value_dict)
             value._set_value_dict(self.value_dict, skip_update=self.skip_update_on_setitem)
         else:
             hash_id = sha256(pickle.dumps(value)).hexdigest()[:self.hash_length]
             self.key_dict[key] = hash_id
```

### Comparing `deduplicationdict-1.0.3/pyproject.toml` & `deduplicationdict-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.setuptools.packages.find]
 where = ["deduplicationdict"]
 
 [project]
 # $ pip install deduplicationdict
 name = "deduplicationdict"
-version = "1.0.3"
+version = "1.0.4"
 description = "A dictionary that de-duplicates values."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["python", "dict", "deduplication", "optimization", ]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
```

### Comparing `deduplicationdict-1.0.3/PKG-INFO` & `deduplicationdict-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deduplicationdict
-Version: 1.0.3
+Version: 1.0.4
 Summary: A dictionary that de-duplicates values.
 Keywords: python,dict,deduplication,optimization
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```


# Comparing `tmp/newenvreader-0.1.0.tar.gz` & `tmp/newenvreader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newenvreader-0.1.0.tar", max compression
+gzip compressed data, was "newenvreader-0.1.1.tar", max compression
```

## Comparing `newenvreader-0.1.0.tar` & `newenvreader-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-02 07:19:49.243406 newenvreader-0.1.0/LICENSE
--rw-r--r--   0        0        0      264 2023-07-03 04:55:18.475095 newenvreader-0.1.0/README.md
--rw-r--r--   0        0        0      277 2023-07-03 04:44:56.118296 newenvreader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 07:19:49.253406 newenvreader-0.1.0/src/newenvreader/__init__.py
--rw-r--r--   0        0        0     2198 2023-07-02 07:19:49.253406 newenvreader-0.1.0/src/newenvreader/main.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 newenvreader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-02 07:19:49.243406 newenvreader-0.1.1/LICENSE
+-rw-r--r--   0        0        0      268 2023-07-03 12:51:53.593170 newenvreader-0.1.1/README.md
+-rw-r--r--   0        0        0     2790 2023-07-03 12:50:11.069549 newenvreader-0.1.1/newenvreader.py
+-rw-r--r--   0        0        0      277 2023-07-03 09:47:45.362392 newenvreader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 newenvreader-0.1.1/PKG-INFO
```

### Comparing `newenvreader-0.1.0/LICENSE` & `newenvreader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newenvreader-0.1.0/src/newenvreader/main.py` & `newenvreader-0.1.1/newenvreader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 This module provides utility functions for reading environment variables.
 """
 
 import os
+from typing import TypeVar
+
+T = TypeVar("T")
 
 
 def parse_env_file(path: str) -> dict[str, str]:
     """Parse a .env file.
 
     :param path: Path to the .env file.
     :type path: str
@@ -45,40 +48,52 @@
     if parent_dir == current_dir:
         # Reached the root directory, file not found
         raise FileNotFoundError("No .env file found")
 
     return search_env_file(parent_dir)
 
 
-class GetEnv:
-    """Class to read environment variable"""
+def load_env() -> dict[str, str]:
+    """Load environment variables from the .env file or the system environment.
+
+    :raises KeyError: If a required environment variable is not found.
+    :return: A dictionary of environment variables.
+    :rtype: dict[str, str]
+    """
+    env = {}
+    for key, value in os.environ.items():
+        env[key] = value
+
+    try:
+        found_env_path = search_env_file(os.getcwd())
+        env.update(parse_env_file(found_env_path))
+    except FileNotFoundError:
+        pass
+
+    return env
+
+
+loaded_env = load_env()
+
+
+def get_env(key: str, required: bool = True, cast: type[T] = str) -> T:
+    """Load environment variable from the .env file or the system environment.
+
+    :param key: The environment variable key.
+    :type key: str
+    :param required: Whether the environment variable is required, defaults to True
+    :type required: bool, optional
+    :param cast: The type to cast the environment variable to, defaults to str
+    :type cast: type, optional
+    :raises KeyError: If the environment variable is not found and is required.
+    :return: The environment variable value.
+    :rtype: str
+    """
+    try:
+        val = loaded_env[key]
+        return cast(val)
+    except KeyError as err:
+        if required:
+            raise KeyError(f"Environment variable {key} is not found") from err
+        val = ""
 
-    def __init__(self, key: str, required: bool = True):
-        env = parse_env_file(search_env_file(os.getcwd()))
-        try:
-            self.key = env[key]
-            return
-        except KeyError:
-            pass
-
-        try:
-            self.key = os.environ[key]
-        except KeyError as err:
-            if required:
-                raise KeyError(f"Environment variable {key} is not found") from err
-            self.key = ""
-
-    def to_int(self):
-        """Convert to int"""
-        return int(self.key)
-
-    def to_float(self):
-        """Convert to float"""
-        return float(self.key)
-
-    def to_str(self):
-        """Convert to str"""
-        return str(self.key)
-
-    def to_bool(self):
-        """Convert to bool"""
-        return bool(self.key)
+    return cast(val)
```

### Comparing `newenvreader-0.1.0/PKG-INFO` & `newenvreader-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newenvreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Ajay Karthik
 Author-email: ajaykarthik.r23@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -15,16 +15,16 @@
 # Installation
 ```bash
 pip install newenvreader
 ```
 
 # Usage
 ```python
-from newenvreader import GetEnv
+from newenvreader import get_env
 
-val = GetEnv("MY_VAR")
+val = get_env("MY_VAR")
 
 # Parse to int
-val = GetEnv("MY_VAR").to_int()
+val = get_env("MY_VAR", cast=int)
 ```
```


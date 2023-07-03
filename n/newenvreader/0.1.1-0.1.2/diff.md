# Comparing `tmp/newenvreader-0.1.1.tar.gz` & `tmp/newenvreader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newenvreader-0.1.1.tar", max compression
+gzip compressed data, was "newenvreader-0.1.2.tar", max compression
```

## Comparing `newenvreader-0.1.1.tar` & `newenvreader-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-02 07:19:49.243406 newenvreader-0.1.1/LICENSE
--rw-r--r--   0        0        0      268 2023-07-03 12:51:53.593170 newenvreader-0.1.1/README.md
--rw-r--r--   0        0        0     2790 2023-07-03 12:50:11.069549 newenvreader-0.1.1/newenvreader.py
--rw-r--r--   0        0        0      277 2023-07-03 09:47:45.362392 newenvreader-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 newenvreader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-02 07:19:49.243406 newenvreader-0.1.2/LICENSE
+-rw-r--r--   0        0        0      268 2023-07-03 13:13:58.225661 newenvreader-0.1.2/README.md
+-rw-r--r--   0        0        0     2817 2023-07-03 12:58:21.889382 newenvreader-0.1.2/newenvreader.py
+-rw-r--r--   0        0        0      278 2023-07-03 13:13:26.154632 newenvreader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 newenvreader-0.1.2/PKG-INFO
```

### Comparing `newenvreader-0.1.1/LICENSE` & `newenvreader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `newenvreader-0.1.1/newenvreader.py` & `newenvreader-0.1.2/newenvreader.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     """Parse a .env file.
 
     :param path: Path to the .env file.
     :type path: str
     :return: A dictionary of environment variables.
     :rtype: dict
     """
-    env = {}
+    env_file_val = {}
     with open(path, "r", encoding="utf-8") as file:
         for line in file:
             line = line.strip()
             if not line:
                 continue
             key, value = line.split("=", maxsplit=1)
-            env[key] = value
-    return env
+            env_file_val[key] = value
+    return env_file_val
 
 
 def search_env_file(start_path: str) -> str:
     """Search for a .env file in the current directory and its parent directories.
 
     :param start_path: Start directory to search for the .env file.
     :type start_path: str
```

### Comparing `newenvreader-0.1.1/PKG-INFO` & `newenvreader-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: newenvreader
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Ajay Karthik
 Author-email: ajaykarthik.r23@gmail.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # newenvreader
 A python library to read environment variables with typing support.
 
 # Installation
 ```bash
@@ -19,12 +20,12 @@
 
 # Usage
 ```python
 from newenvreader import get_env
 
 val = get_env("MY_VAR")
 
-# Parse to int
+# Parse as int
 val = get_env("MY_VAR", cast=int)
 ```
```


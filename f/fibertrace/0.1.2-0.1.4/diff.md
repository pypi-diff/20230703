# Comparing `tmp/fibertrace-0.1.2.tar.gz` & `tmp/fibertrace-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibertrace-0.1.2.tar", last modified: Thu Jun 29 08:42:54 2023, max compression
+gzip compressed data, was "fibertrace-0.1.4.tar", last modified: Mon Jul  3 15:05:32 2023, max compression
```

## Comparing `fibertrace-0.1.2.tar` & `fibertrace-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:42:54.430053 fibertrace-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 08:42:54.430053 fibertrace-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-29 08:42:26.000000 fibertrace-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 08:42:26.000000 fibertrace-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:42:54.430053 fibertrace-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 08:42:26.000000 fibertrace-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:42:54.426052 fibertrace-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:42:54.426052 fibertrace-0.1.2/src/fibertrace/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:42:26.000000 fibertrace-0.1.2/src/fibertrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-29 08:42:26.000000 fibertrace-0.1.2/src/fibertrace/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:42:54.430053 fibertrace-0.1.2/src/fibertrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 08:42:54.000000 fibertrace-0.1.2/src/fibertrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 08:42:54.000000 fibertrace-0.1.2/src/fibertrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:42:54.000000 fibertrace-0.1.2/src/fibertrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 08:42:54.000000 fibertrace-0.1.2/src/fibertrace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:05:32.846770 fibertrace-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-03 15:05:32.846770 fibertrace-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 15:05:08.000000 fibertrace-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-03 15:05:08.000000 fibertrace-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:05:32.846770 fibertrace-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 15:05:08.000000 fibertrace-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:05:32.842770 fibertrace-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:05:32.842770 fibertrace-0.1.4/src/fibertrace/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 15:05:08.000000 fibertrace-0.1.4/src/fibertrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-03 15:05:08.000000 fibertrace-0.1.4/src/fibertrace/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:05:32.846770 fibertrace-0.1.4/src/fibertrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-03 15:05:32.000000 fibertrace-0.1.4/src/fibertrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 15:05:32.000000 fibertrace-0.1.4/src/fibertrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:05:32.000000 fibertrace-0.1.4/src/fibertrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 15:05:32.000000 fibertrace-0.1.4/src/fibertrace.egg-info/top_level.txt
```

### Comparing `fibertrace-0.1.2/PKG-INFO` & `fibertrace-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibertrace
-Version: 0.1.2
+Version: 0.1.4
 Summary: A library for simple logging
 Home-page: https://github.com/bytesentinel-io/fibertrace.py
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fibertrace-0.1.2/README.md` & `fibertrace-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fibertrace-0.1.2/pyproject.toml` & `fibertrace-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = "fibertrace"
-version = "0.1.2"
+version = "0.1.4"
 description = "A library for simple logging"
 long_description = """
 A library for simple logging
 """
 license = "MIT"
 author = "ByteSentinel.io"
 author-email = "dev@bytesentinel.io"
```

### Comparing `fibertrace-0.1.2/setup.py` & `fibertrace-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="fibertrace",
-    version="0.1.2",
+    version="0.1.4",
     author="ByteSentinel.io",
     author_email="dev@bytesentinel.io",
     description="A library for simple logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bytesentinel-io/fibertrace.py",
     packages=find_packages(where="src"),
```

### Comparing `fibertrace-0.1.2/src/fibertrace/log.py` & `fibertrace-0.1.4/src/fibertrace/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.message = message
         self.user = user
 
 class Logger:
     def __init__(self, log_file_path, application, json_format):
         self.logger = logging.getLogger()
         self.logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s [%(levelname)s] [%(application)s] [%(module)s] [%(user)s]: %(message)s')
+        formatter = logging.Formatter('%(asctime)s %(user)s (%(application)s:%(module)s) [%(levelname)s]: %(message)s')
 
         if log_file_path:
             log_file_path = os.path.abspath(log_file_path)
             log_dir = os.path.dirname(log_file_path)
             Path(log_dir).mkdir(parents=True, exist_ok=True)
 
             self.file_handler = logging.FileHandler(log_file_path)
@@ -80,20 +80,20 @@
 
     def log_json(self, log_entry):
         log_json = json.dumps(log_entry.__dict__)
         self.write_to_file(log_json.encode())
 
     def log_text(self, log_entry):
         timestamp = log_entry.timestamp
-        log_text = f"[{timestamp}] [{log_entry.level}] [{self.application}] [{log_entry.module}] [{log_entry.user}]: {log_entry.message}"
+        log_text = f"{timestamp} {log_entry.user} ({log_entry.application}:{log_entry.module}) [{log_entry.level}]: {log_entry.message}"
         self.write_to_file(log_text.encode())
 
     def console(self, log_entry):
         timestamp = log_entry.timestamp
-        log_text = f"[{timestamp}] [{log_entry.level}] [{self.application}] [{log_entry.module}] [{log_entry.user}]: {log_entry.message}"
+        log_text = f"{timestamp} {log_entry.user} ({log_entry.application}:{log_entry.module}) [{log_entry.level}]: {log_entry.message}"
         print(log_text)
 
     def write_to_file(self, log_data):
         if hasattr(self, 'file_handler'):
             log_data = log_data.decode()  # Bytes in eine Zeichenkette umwandeln
             self.file_handler.stream.write(log_data)
             self.file_handler.stream.write('\n')  # Zeilenumbruch als Zeichenkette
```

### Comparing `fibertrace-0.1.2/src/fibertrace.egg-info/PKG-INFO` & `fibertrace-0.1.4/src/fibertrace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibertrace
-Version: 0.1.2
+Version: 0.1.4
 Summary: A library for simple logging
 Home-page: https://github.com/bytesentinel-io/fibertrace.py
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


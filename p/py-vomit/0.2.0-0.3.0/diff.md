# Comparing `tmp/py-vomit-0.2.0.tar.gz` & `tmp/py-vomit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-vomit-0.2.0.tar", last modified: Sun Jun 18 18:10:19 2023, max compression
+gzip compressed data, was "py-vomit-0.3.0.tar", last modified: Mon Jul  3 21:13:44 2023, max compression
```

## Comparing `py-vomit-0.2.0.tar` & `py-vomit-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.983970 py-vomit-0.2.0/
--rw-r--r--   0 roko      (1000) roko      (1000)     1060 2023-06-08 11:40:04.000000 py-vomit-0.2.0/LICENSE
--rw-r--r--   0 roko      (1000) roko      (1000)     1921 2023-06-18 18:10:19.983970 py-vomit-0.2.0/PKG-INFO
--rw-r--r--   0 roko      (1000) roko      (1000)     1497 2023-06-18 18:00:10.000000 py-vomit-0.2.0/README.md
--rw-r--r--   0 roko      (1000) roko      (1000)      496 2023-06-08 11:55:20.000000 py-vomit-0.2.0/pyproject.toml
--rw-r--r--   0 roko      (1000) roko      (1000)      704 2023-06-18 18:10:19.987303 py-vomit-0.2.0/setup.cfg
--rw-r--r--   0 roko      (1000) roko      (1000)       68 2023-06-08 11:32:05.000000 py-vomit-0.2.0/setup.py
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.973970 py-vomit-0.2.0/src/
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.980636 py-vomit-0.2.0/src/py_vomit.egg-info/
--rw-r--r--   0 roko      (1000) roko      (1000)     1921 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/PKG-INFO
--rw-r--r--   0 roko      (1000) roko      (1000)      376 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/SOURCES.txt
--rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/dependency_links.txt
--rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-08 15:02:31.000000 py-vomit-0.2.0/src/py_vomit.egg-info/not-zip-safe
--rw-r--r--   0 roko      (1000) roko      (1000)       80 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/requires.txt
--rw-r--r--   0 roko      (1000) roko      (1000)        6 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/top_level.txt
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.983970 py-vomit-0.2.0/src/vomit/
--rw-r--r--   0 roko      (1000) roko      (1000)     5791 2023-06-18 17:57:07.000000 py-vomit-0.2.0/src/vomit/__init__.py
--rw-r--r--   0 roko      (1000) roko      (1000)     2048 2023-06-18 18:04:49.000000 py-vomit-0.2.0/src/vomit/__main__.py
--rw-r--r--   0 roko      (1000) roko      (1000)        0 2023-06-08 11:28:38.000000 py-vomit-0.2.0/src/vomit/py.typed
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.983970 py-vomit-0.2.0/tests/
--rw-r--r--   0 roko      (1000) roko      (1000)     1506 2023-06-18 17:58:18.000000 py-vomit-0.2.0/tests/test_fuctionality.py
--rw-r--r--   0 roko      (1000) roko      (1000)      587 2023-06-18 18:03:31.000000 py-vomit-0.2.0/tests/test_walker.py
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-07-03 21:13:44.258306 py-vomit-0.3.0/
+-rw-r--r--   0 roko      (1000) roko      (1000)     1060 2023-06-08 11:40:04.000000 py-vomit-0.3.0/LICENSE
+-rw-r--r--   0 roko      (1000) roko      (1000)     2180 2023-07-03 21:13:44.258306 py-vomit-0.3.0/PKG-INFO
+-rw-r--r--   0 roko      (1000) roko      (1000)     1756 2023-07-03 21:06:18.000000 py-vomit-0.3.0/README.md
+-rw-r--r--   0 roko      (1000) roko      (1000)      496 2023-06-08 11:55:20.000000 py-vomit-0.3.0/pyproject.toml
+-rw-r--r--   0 roko      (1000) roko      (1000)      704 2023-07-03 21:13:44.258306 py-vomit-0.3.0/setup.cfg
+-rw-r--r--   0 roko      (1000) roko      (1000)       68 2023-06-08 11:32:05.000000 py-vomit-0.3.0/setup.py
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-07-03 21:13:44.254973 py-vomit-0.3.0/src/
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-07-03 21:13:44.258306 py-vomit-0.3.0/src/py_vomit.egg-info/
+-rw-r--r--   0 roko      (1000) roko      (1000)     2180 2023-07-03 21:13:44.000000 py-vomit-0.3.0/src/py_vomit.egg-info/PKG-INFO
+-rw-r--r--   0 roko      (1000) roko      (1000)      376 2023-07-03 21:13:44.000000 py-vomit-0.3.0/src/py_vomit.egg-info/SOURCES.txt
+-rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-07-03 21:13:44.000000 py-vomit-0.3.0/src/py_vomit.egg-info/dependency_links.txt
+-rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-08 15:02:31.000000 py-vomit-0.3.0/src/py_vomit.egg-info/not-zip-safe
+-rw-r--r--   0 roko      (1000) roko      (1000)       80 2023-07-03 21:13:44.000000 py-vomit-0.3.0/src/py_vomit.egg-info/requires.txt
+-rw-r--r--   0 roko      (1000) roko      (1000)        6 2023-07-03 21:13:44.000000 py-vomit-0.3.0/src/py_vomit.egg-info/top_level.txt
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-07-03 21:13:44.258306 py-vomit-0.3.0/src/vomit/
+-rw-r--r--   0 roko      (1000) roko      (1000)     6302 2023-07-03 20:48:27.000000 py-vomit-0.3.0/src/vomit/__init__.py
+-rw-r--r--   0 roko      (1000) roko      (1000)     2397 2023-07-03 21:04:19.000000 py-vomit-0.3.0/src/vomit/__main__.py
+-rw-r--r--   0 roko      (1000) roko      (1000)        0 2023-06-08 11:28:38.000000 py-vomit-0.3.0/src/vomit/py.typed
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-07-03 21:13:44.258306 py-vomit-0.3.0/tests/
+-rw-r--r--   0 roko      (1000) roko      (1000)     1506 2023-06-18 17:58:18.000000 py-vomit-0.3.0/tests/test_fuctionality.py
+-rw-r--r--   0 roko      (1000) roko      (1000)     2741 2023-07-03 20:47:14.000000 py-vomit-0.3.0/tests/test_walker.py
```

### Comparing `py-vomit-0.2.0/LICENSE` & `py-vomit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-vomit-0.2.0/PKG-INFO` & `py-vomit-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-vomit
-Version: 0.2.0
+Version: 0.3.0
 Summary: "Somewhat unintelligible"
 Home-page: https://github.com/bhmt/vomit
 Author: bhmt
 License: MIT
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,29 +35,32 @@
 
 pip install py-vomit
 
 ```
 
 ## Usage
 
-As a module run vomit with either encode or decode required option.
+As a module run vomit with a required option to either encode or decode.
 For input use a a stdin + stdout, a file, or a directory.
 
 
 ```shell
 
-usage: python -m vomit [-h] (-e | -d) [-f FILE | -s SOURCE]
+usage: python -m vomit [-h] (-e | -d) [-f FILE | -s SOURCE] [-i IGNORE] [-t EXT]
 
 options:
   -h, --help            show this help message and exit
   -e, --encode          indicate the file should be encoded
   -d, --decode          indicate the file should be decoded
   -f FILE, --file FILE  the file to encode or decode, defaults to stdin
   -s SOURCE, --source SOURCE
                         the directory to encode or decode .py files recursively
+  -i IGNORE, --ignore IGNORE
+                        comma separated values of files and directories to skip when using --source
+  -t EXT, --ext EXT     comma separated values of extensions to include along ".py" when using --source
 
 ```
 
 
 or use vomit as a library
 
 ```py
```

### Comparing `py-vomit-0.2.0/README.md` & `py-vomit-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -20,29 +20,32 @@
 
 pip install py-vomit
 
 ```
 
 ## Usage
 
-As a module run vomit with either encode or decode required option.
+As a module run vomit with a required option to either encode or decode.
 For input use a a stdin + stdout, a file, or a directory.
 
 
 ```shell
 
-usage: python -m vomit [-h] (-e | -d) [-f FILE | -s SOURCE]
+usage: python -m vomit [-h] (-e | -d) [-f FILE | -s SOURCE] [-i IGNORE] [-t EXT]
 
 options:
   -h, --help            show this help message and exit
   -e, --encode          indicate the file should be encoded
   -d, --decode          indicate the file should be decoded
   -f FILE, --file FILE  the file to encode or decode, defaults to stdin
   -s SOURCE, --source SOURCE
                         the directory to encode or decode .py files recursively
+  -i IGNORE, --ignore IGNORE
+                        comma separated values of files and directories to skip when using --source
+  -t EXT, --ext EXT     comma separated values of extensions to include along ".py" when using --source
 
 ```
 
 
 or use vomit as a library
 
 ```py
```

### Comparing `py-vomit-0.2.0/setup.cfg` & `py-vomit-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = py-vomit
 description = "Somewhat unintelligible"
 author = bhmt
-version = 0.2.0
+version = 0.3.0
 license = MIT
 license_files = LICENSE
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/bhmt/vomit
 classifiers = 
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `py-vomit-0.2.0/src/py_vomit.egg-info/PKG-INFO` & `py-vomit-0.3.0/src/py_vomit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-vomit
-Version: 0.2.0
+Version: 0.3.0
 Summary: "Somewhat unintelligible"
 Home-page: https://github.com/bhmt/vomit
 Author: bhmt
 License: MIT
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,29 +35,32 @@
 
 pip install py-vomit
 
 ```
 
 ## Usage
 
-As a module run vomit with either encode or decode required option.
+As a module run vomit with a required option to either encode or decode.
 For input use a a stdin + stdout, a file, or a directory.
 
 
 ```shell
 
-usage: python -m vomit [-h] (-e | -d) [-f FILE | -s SOURCE]
+usage: python -m vomit [-h] (-e | -d) [-f FILE | -s SOURCE] [-i IGNORE] [-t EXT]
 
 options:
   -h, --help            show this help message and exit
   -e, --encode          indicate the file should be encoded
   -d, --decode          indicate the file should be decoded
   -f FILE, --file FILE  the file to encode or decode, defaults to stdin
   -s SOURCE, --source SOURCE
                         the directory to encode or decode .py files recursively
+  -i IGNORE, --ignore IGNORE
+                        comma separated values of files and directories to skip when using --source
+  -t EXT, --ext EXT     comma separated values of extensions to include along ".py" when using --source
 
 ```
 
 
 or use vomit as a library
 
 ```py
```

### Comparing `py-vomit-0.2.0/src/vomit/__init__.py` & `py-vomit-0.3.0/src/vomit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,31 @@
 
 
 def to_unicode(code: str) -> str:
     visitor = _Visitor()
     return _action(code, visitor)
 
 
-def walker(source: str) -> Iterator[str]:
+def walker(source: str, ignore: str | None = None, extensions: str | None = None) -> Iterator[str]:
+    _extensions = {f'.{ext.strip().lstrip(".")}' for ext in extensions.split(',')} if extensions else set()
+    _extensions = _extensions | {'.py'}
+
+    _ignore = {i.strip() for i in ignore.split(',')} if ignore else set()
+
     for root, _, files in walk(source):
+        if _ignore and any(root.endswith(i) for i in _ignore):
+            continue
+
         for name in files:
-            if name.endswith('.py'):
-                yield path.join(root, name)
+            if any(name.endswith(e) for e in _extensions):
+                file = path.join(root, name)
+                if _ignore and any(file == i for i in _ignore):
+                    continue
+
+                yield file
 
 
 def _action(code: str, visitor: ast.NodeVisitor) -> str:
     tree = ast.parse(code)
     visitor.visit(tree)
     return ast.unparse(tree)
```

### Comparing `py-vomit-0.2.0/tests/test_fuctionality.py` & `py-vomit-0.3.0/tests/test_fuctionality.py`

 * *Files identical despite different names*


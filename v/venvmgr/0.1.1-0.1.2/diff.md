# Comparing `tmp/venvmgr-0.1.1.tar.gz` & `tmp/venvmgr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venvmgr-0.1.1.tar", last modified: Mon Jul  3 05:05:51 2023, max compression
+gzip compressed data, was "venvmgr-0.1.2.tar", last modified: Mon Jul  3 05:29:32 2023, max compression
```

## Comparing `venvmgr-0.1.1.tar` & `venvmgr-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:05:51.394173 venvmgr-0.1.1/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1070 2023-07-03 04:09:56.000000 venvmgr-0.1.1/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2549 2023-07-03 05:05:51.394173 venvmgr-0.1.1/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      846 2023-07-03 04:16:07.000000 venvmgr-0.1.1/README.md
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      353 2023-07-03 05:01:35.000000 venvmgr-0.1.1/pyproject.toml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      527 2023-07-03 05:05:51.394173 venvmgr-0.1.1/setup.cfg
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:05:51.390174 venvmgr-0.1.1/src/
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:05:51.390174 venvmgr-0.1.1/src/venvmgr/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3579 2023-07-03 05:05:41.000000 venvmgr-0.1.1/src/venvmgr/cli.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1049 2023-06-07 03:40:38.000000 venvmgr-0.1.1/src/venvmgr/config.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6405 2023-07-03 03:59:22.000000 venvmgr-0.1.1/src/venvmgr/venvmgr.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:05:51.394173 venvmgr-0.1.1/src/venvmgr.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2549 2023-07-03 05:05:51.000000 venvmgr-0.1.1/src/venvmgr.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      318 2023-07-03 05:05:51.000000 venvmgr-0.1.1/src/venvmgr.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-03 05:05:51.000000 venvmgr-0.1.1/src/venvmgr.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       44 2023-07-03 05:05:51.000000 venvmgr-0.1.1/src/venvmgr.egg-info/entry_points.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-07-03 05:05:51.000000 venvmgr-0.1.1/src/venvmgr.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-07-03 05:05:51.000000 venvmgr-0.1.1/src/venvmgr.egg-info/top_level.txt
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:29:32.981567 venvmgr-0.1.2/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1070 2023-07-03 04:09:56.000000 venvmgr-0.1.2/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2549 2023-07-03 05:29:32.981567 venvmgr-0.1.2/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      846 2023-07-03 04:16:07.000000 venvmgr-0.1.2/README.md
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      353 2023-07-03 05:10:44.000000 venvmgr-0.1.2/pyproject.toml
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      527 2023-07-03 05:29:32.985567 venvmgr-0.1.2/setup.cfg
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:29:32.977567 venvmgr-0.1.2/src/
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:29:32.981567 venvmgr-0.1.2/src/venvmgr/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3579 2023-07-03 05:28:08.000000 venvmgr-0.1.2/src/venvmgr/cli.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1049 2023-06-07 03:40:38.000000 venvmgr-0.1.2/src/venvmgr/config.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6436 2023-07-03 05:26:45.000000 venvmgr-0.1.2/src/venvmgr/venvmgr.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-03 05:29:32.981567 venvmgr-0.1.2/src/venvmgr.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2549 2023-07-03 05:29:32.000000 venvmgr-0.1.2/src/venvmgr.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      318 2023-07-03 05:29:32.000000 venvmgr-0.1.2/src/venvmgr.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-03 05:29:32.000000 venvmgr-0.1.2/src/venvmgr.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       44 2023-07-03 05:29:32.000000 venvmgr-0.1.2/src/venvmgr.egg-info/entry_points.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-07-03 05:29:32.000000 venvmgr-0.1.2/src/venvmgr.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-07-03 05:29:32.000000 venvmgr-0.1.2/src/venvmgr.egg-info/top_level.txt
```

### Comparing `venvmgr-0.1.1/LICENSE` & `venvmgr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `venvmgr-0.1.1/PKG-INFO` & `venvmgr-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venvmgr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manage Python virtual environments
 Home-page: https://github.com/andrewfowlie/venvmgr
 Author: Andrew Fowlie
 Author-email: Andrew Fowlie <andrew.fowlie@xjtlu.edu.cn>
 License: MIT License
         
         Copyright (c) 2023 Andrew Fowlie
```

### Comparing `venvmgr-0.1.1/README.md` & `venvmgr-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `venvmgr-0.1.1/setup.cfg` & `venvmgr-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = venvmgr
-version = 0.1.1
+version = 0.1.2
 author = Andrew Fowlie
 author_email = andrew.j.fowlie@gmail.com
 description = Manage Python virtual environments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/andrewfowlie/venvmgr
 project_urls =
```

### Comparing `venvmgr-0.1.1/src/venvmgr/cli.py` & `venvmgr-0.1.2/src/venvmgr/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import click
 
 from . import venvmgr
 from . import config
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 def get_venv_names(ctx, args, incomplete):
     return os.listdir(config.VENV_DIR)
 
 
 @click.group()
```

### Comparing `venvmgr-0.1.1/src/venvmgr/config.py` & `venvmgr-0.1.2/src/venvmgr/config.py`

 * *Files identical despite different names*

### Comparing `venvmgr-0.1.1/src/venvmgr/venvmgr.py` & `venvmgr-0.1.2/src/venvmgr/venvmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     """
     @brief Create a venv if it does not exist
     """
     if not isvenv(venv_name):
         if click.confirm(f"Create new venv '{venv_name}'?"):
             create(venv_name)
         else:
-            raise RuntimeError(f"Does not exist - {venv_name}")
+            raise click.BadParameter(f"The venv '{venv_name}' does not exist")
 
 
 def venv_must_exist(func):
     """
     @brief Raise error if venv does not exist
     """
     @functools.wraps(func)
@@ -182,28 +182,27 @@
         shutil.rmtree(d)
 
 
 def python(venv_name, file_name, *args, verbose=True, **kwargs):
     """
     @brief Run a Python file in a virtual environment
     """
-    abs_file_name = os.path.abspath(file_name)
-
     if file_name is None and venv_name is None:
-        raise RuntimeError("Require venv name or file name")
+        raise click.UsageError("Require venv name or file name")
 
     if venv_name is None:
         venv_name = config.get(
             config.ASSOCIATION).get(
-            abs_file_name,
+            os.path.abspath(file_name),
             default_venv_name(file_name))
 
     create_if_not_exist(venv_name)
 
-    config.set(config.ASSOCIATION, abs_file_name, venv_name)
+    if file_name is not None:
+        config.set(config.ASSOCIATION, os.path.abspath(file_name), venv_name)
 
     bin_python = locate(venv_name, "python")
 
     if verbose:
         click.secho(
             f"python = {click.format_filename(bin_python)}",
             fg='green',
```

### Comparing `venvmgr-0.1.1/src/venvmgr.egg-info/PKG-INFO` & `venvmgr-0.1.2/src/venvmgr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venvmgr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manage Python virtual environments
 Home-page: https://github.com/andrewfowlie/venvmgr
 Author: Andrew Fowlie
 Author-email: Andrew Fowlie <andrew.fowlie@xjtlu.edu.cn>
 License: MIT License
         
         Copyright (c) 2023 Andrew Fowlie
```


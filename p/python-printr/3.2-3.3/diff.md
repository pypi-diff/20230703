# Comparing `tmp/python-printr-3.2.tar.gz` & `tmp/python-printr-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-printr-3.2.tar", last modified: Wed Jun 14 17:48:18 2023, max compression
+gzip compressed data, was "python-printr-3.3.tar", last modified: Mon Jul  3 17:54:18 2023, max compression
```

## Comparing `python-printr-3.2.tar` & `python-printr-3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:48:18.480659 python-printr-3.2/
--rw-rw-rw-   0        0        0       64 2023-06-14 13:12:02.000000 python-printr-3.2/.gitignore
--rw-rw-rw-   0        0        0     3347 2023-06-14 17:48:18.480659 python-printr-3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3089 2023-06-11 14:12:17.000000 python-printr-3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 17:48:18.475663 python-printr-3.2/printr/
--rw-rw-rw-   0        0        0     7600 2023-06-14 13:43:47.000000 python-printr-3.2/printr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:48:18.479660 python-printr-3.2/python_printr.egg-info/
--rw-rw-rw-   0        0        0     3347 2023-06-14 17:48:18.000000 python-printr-3.2/python_printr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-14 17:48:18.000000 python-printr-3.2/python_printr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:48:18.000000 python-printr-3.2/python_printr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 17:48:18.000000 python-printr-3.2/python_printr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 17:48:18.000000 python-printr-3.2/python_printr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-14 17:48:18.480659 python-printr-3.2/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-06-14 17:48:15.000000 python-printr-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:54:18.387940 python-printr-3.3/
+-rw-rw-rw-   0        0        0       64 2023-06-14 13:12:02.000000 python-printr-3.3/.gitignore
+-rw-rw-rw-   0        0        0     3347 2023-07-03 17:54:18.387940 python-printr-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3089 2023-06-11 14:12:17.000000 python-printr-3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 17:54:18.382943 python-printr-3.3/printr/
+-rw-rw-rw-   0        0        0     7594 2023-07-03 17:54:02.000000 python-printr-3.3/printr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:54:18.386940 python-printr-3.3/python_printr.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-07-03 17:54:17.000000 python-printr-3.3/python_printr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-03 17:54:18.000000 python-printr-3.3/python_printr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:54:17.000000 python-printr-3.3/python_printr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 17:54:17.000000 python-printr-3.3/python_printr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 17:54:17.000000 python-printr-3.3/python_printr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-03 17:54:18.388939 python-printr-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-07-03 17:54:14.000000 python-printr-3.3/setup.py
```

### Comparing `python-printr-3.2/PKG-INFO` & `python-printr-3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 3.2
+Version: 3.3
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

### Comparing `python-printr-3.2/README.md` & `python-printr-3.3/README.md`

 * *Files identical despite different names*

### Comparing `python-printr-3.2/printr/__init__.py` & `python-printr-3.3/printr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys, logging, json, os, shutil, coloredlogs
 from pathlib import Path
 from datetime import datetime
 
 class logger:
-    def __init__(self, log_filepath=None, max_lines=100_000, level='info', name=None, log_to_file=False):
+    def __init__(self, log_filepath=None, max_lines=100_000, level='info', name=None, log_to_file=True):
         filename = Path(sys.argv[0]).stem
         self.filename = filename
         if not log_filepath:
             log_filepath = f'{os.getcwd()}/{filename}.txt'
         self.log_filepath = log_filepath
         self.max_lines = max_lines
         self.log_to_file = log_to_file
@@ -52,16 +52,14 @@
 
         if level == 'info':
             self.logger.info(message)
         elif level == 'error':
             self.logger.error(message)
         elif level == 'debug':
             self.logger.debug(message)
-        elif level == 'success':
-            self.logger.success(message)
         elif level == 'warning':
             self.logger.warning(message)
 
         if not message:
             if self.log_to_file:
                 log_format = logging.Formatter(fmt=self.indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S') # Reset to default log format
                 self.log_file.setFormatter(log_format)
@@ -152,14 +150,17 @@
     def __init__(self, *items, current_time=False, check_for_log=True, beautify=True):
         print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, beautify=beautify)
 
 class printr:
     def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info', beautify=True):
         print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, level=level, beautify=beautify)
 
+# from rich.pretty import pretty_repr
+# from rich.text import Text
+
 def prettify(items, beautify):
     message = ''
     for item in items:
         if message and '\n' not in message:
             message += ' ' # Add space in between variables
         if beautify and (isinstance(item, dict) or isinstance(item, list)):
             try:
```

### Comparing `python-printr-3.2/python_printr.egg-info/PKG-INFO` & `python-printr-3.3/python_printr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 3.2
+Version: 3.3
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```


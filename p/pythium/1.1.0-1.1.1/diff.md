# Comparing `tmp/pythium-1.1.0.tar.gz` & `tmp/pythium-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bo.liu/Work/pythium/dist/tmpl5q0z6ew/pythium-1.1.0.tar", last modified: Tue Jun 27 05:14:25 2023, max compression
+gzip compressed data, was "/Users/bo.liu/Work/pythium/dist/tmp2hv7lx9b/pythium-1.1.1.tar", last modified: Mon Jul  3 01:13:33 2023, max compression
```

## Comparing `pythium-1.1.0.tar` & `pythium-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-06-27 05:14:25.656953 pythium-1.1.0/
--rw-r--r--   0 bo.liu     (505) staff       (20)     4553 2023-06-27 05:14:25.656597 pythium-1.1.0/PKG-INFO
--rw-r--r--   0 bo.liu     (505) staff       (20)     3036 2022-11-16 09:06:52.000000 pythium-1.1.0/README.md
-drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-06-27 05:14:25.653686 pythium-1.1.0/pythium/
--rw-r--r--   0 bo.liu     (505) staff       (20)      359 2023-03-07 01:14:33.000000 pythium-1.1.0/pythium/__init__.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     5878 2023-03-08 06:11:02.000000 pythium-1.1.0/pythium/_impl.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     9748 2023-04-24 06:43:07.000000 pythium-1.1.0/pythium/actions.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     5793 2022-12-12 07:51:54.000000 pythium-1.1.0/pythium/assertions.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     3806 2023-03-08 09:25:12.000000 pythium-1.1.0/pythium/commands.py
--rw-r--r--   0 bo.liu     (505) staff       (20)      249 2022-01-21 07:11:16.000000 pythium-1.1.0/pythium/exceptions.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     4007 2023-06-27 02:12:03.000000 pythium-1.1.0/pythium/http_session.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     8973 2023-06-27 00:56:23.000000 pythium-1.1.0/pythium/objects.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     2599 2022-12-12 01:49:47.000000 pythium-1.1.0/pythium/utils.py
-drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-06-27 05:14:25.656059 pythium-1.1.0/pythium.egg-info/
--rw-r--r--   0 bo.liu     (505) staff       (20)     4553 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/PKG-INFO
--rw-r--r--   0 bo.liu     (505) staff       (20)      382 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/SOURCES.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)        1 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/dependency_links.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)        1 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/not-zip-safe
--rw-r--r--   0 bo.liu     (505) staff       (20)      119 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/requires.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)        8 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/top_level.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)       38 2023-06-27 05:14:25.657079 pythium-1.1.0/setup.cfg
--rw-r--r--   0 bo.liu     (505) staff       (20)     1339 2023-06-27 02:15:25.000000 pythium-1.1.0/setup.py
+drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-07-03 01:13:33.794394 pythium-1.1.1/
+-rw-r--r--   0 bo.liu     (505) staff       (20)     4553 2023-07-03 01:13:33.793573 pythium-1.1.1/PKG-INFO
+-rw-r--r--   0 bo.liu     (505) staff       (20)     3036 2022-11-16 09:06:52.000000 pythium-1.1.1/README.md
+drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-07-03 01:13:33.790417 pythium-1.1.1/pythium/
+-rw-r--r--   0 bo.liu     (505) staff       (20)      359 2023-03-07 01:14:33.000000 pythium-1.1.1/pythium/__init__.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     5878 2023-03-08 06:11:02.000000 pythium-1.1.1/pythium/_impl.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     9756 2023-07-03 01:07:25.000000 pythium-1.1.1/pythium/actions.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     5793 2022-12-12 07:51:54.000000 pythium-1.1.1/pythium/assertions.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     3806 2023-03-08 09:25:12.000000 pythium-1.1.1/pythium/commands.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)      249 2022-01-21 07:11:16.000000 pythium-1.1.1/pythium/exceptions.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     4007 2023-06-27 02:12:03.000000 pythium-1.1.1/pythium/http_session.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     8973 2023-06-27 07:52:06.000000 pythium-1.1.1/pythium/objects.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     2599 2022-12-12 01:49:47.000000 pythium-1.1.1/pythium/utils.py
+drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-07-03 01:13:33.792954 pythium-1.1.1/pythium.egg-info/
+-rw-r--r--   0 bo.liu     (505) staff       (20)     4553 2023-07-03 01:13:33.000000 pythium-1.1.1/pythium.egg-info/PKG-INFO
+-rw-r--r--   0 bo.liu     (505) staff       (20)      382 2023-07-03 01:13:33.000000 pythium-1.1.1/pythium.egg-info/SOURCES.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)        1 2023-07-03 01:13:33.000000 pythium-1.1.1/pythium.egg-info/dependency_links.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)        1 2023-07-03 01:13:33.000000 pythium-1.1.1/pythium.egg-info/not-zip-safe
+-rw-r--r--   0 bo.liu     (505) staff       (20)      119 2023-07-03 01:13:33.000000 pythium-1.1.1/pythium.egg-info/requires.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)        8 2023-07-03 01:13:33.000000 pythium-1.1.1/pythium.egg-info/top_level.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)       38 2023-07-03 01:13:33.794690 pythium-1.1.1/setup.cfg
+-rw-r--r--   0 bo.liu     (505) staff       (20)     1339 2023-07-03 01:13:26.000000 pythium-1.1.1/setup.py
```

### Comparing `pythium-1.1.0/PKG-INFO` & `pythium-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythium
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python based Page Factory.
 Home-page: https://github.com/lucas234/pythium
 Author: lucas
 Author-email: ly_liubo@163.com
 License: MIT
 Description: #### Pythium 
         ***
```

### Comparing `pythium-1.1.0/README.md` & `pythium-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium/_impl.py` & `pythium-1.1.1/pythium/_impl.py`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium/actions.py` & `pythium-1.1.1/pythium/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from selenium.common.exceptions import NoSuchElementException, TimeoutException
 from typing import NoReturn
 import inspect
 import time
 from typing import Literal
 from pythium.exceptions import IllegalArgumentException
 from pythium.utils import Utils
-from commands import IosCommands, AndroidCommands
+from pythium.commands import IosCommands, AndroidCommands
 
 
 class Actions(object):
 
     _TIMEOUT = 8
 
     def __init__(self, driver: Remote):
```

### Comparing `pythium-1.1.0/pythium/assertions.py` & `pythium-1.1.1/pythium/assertions.py`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium/commands.py` & `pythium-1.1.1/pythium/commands.py`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium/http_session.py` & `pythium-1.1.1/pythium/http_session.py`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium/objects.py` & `pythium-1.1.1/pythium/objects.py`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium/utils.py` & `pythium-1.1.1/pythium/utils.py`

 * *Files identical despite different names*

### Comparing `pythium-1.1.0/pythium.egg-info/PKG-INFO` & `pythium-1.1.1/pythium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythium
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python based Page Factory.
 Home-page: https://github.com/lucas234/pythium
 Author: lucas
 Author-email: ly_liubo@163.com
 License: MIT
 Description: #### Pythium 
         ***
```

### Comparing `pythium-1.1.0/setup.py` & `pythium-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pythium",
-    version="1.1.0",
+    version="1.1.1",
     author="lucas",
     author_email="ly_liubo@163.com",
     description="Python based Page Factory.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lucas234/pythium",
     zip_safe=False,
```


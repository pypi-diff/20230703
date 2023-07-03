# Comparing `tmp/smarthouse-0.1.4.tar.gz` & `tmp/smarthouse-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarthouse-0.1.4.tar", last modified: Mon Jun  5 15:03:54 2023, max compression
+gzip compressed data, was "smarthouse-0.1.5.tar", last modified: Mon Jul  3 10:01:41 2023, max compression
```

## Comparing `smarthouse-0.1.4.tar` & `smarthouse-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 15:03:54.728768 smarthouse-0.1.4/
--rw-r--r--   0 ivan       (501) staff       (20)     5106 2023-06-05 15:03:54.728199 smarthouse-0.1.4/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     4537 2023-06-05 14:57:33.000000 smarthouse-0.1.4/README.md
--rw-r--r--   0 ivan       (501) staff       (20)     4925 2023-06-05 15:01:13.000000 smarthouse-0.1.4/README.rst
--rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.4/pyproject.toml
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-06-05 15:03:54.729008 smarthouse-0.1.4/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1735 2023-06-05 14:55:41.000000 smarthouse-0.1.4/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 15:03:54.724013 smarthouse-0.1.4/smarthouse/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/action_decorators.py
--rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.4/smarthouse/app.py
--rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/device.py
--rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/device_generator.py
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/logger.py
--rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/storage.py
--rw-r--r--   0 ivan       (501) staff       (20)     8195 2023-06-05 12:47:44.000000 smarthouse-0.1.4/smarthouse/telegram_client.py
--rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 15:03:54.727411 smarthouse-0.1.4/smarthouse.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     5106 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      431 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      290 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       11 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-03 10:01:41.169020 smarthouse-0.1.5/
+-rw-r--r--   0 ivan       (501) staff       (20)     5106 2023-07-03 10:01:41.167986 smarthouse-0.1.5/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     4537 2023-06-05 22:03:49.000000 smarthouse-0.1.5/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)     4925 2023-06-05 22:03:49.000000 smarthouse-0.1.5/README.rst
+-rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.5/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-07-03 10:01:41.169415 smarthouse-0.1.5/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1735 2023-07-03 10:01:06.000000 smarthouse-0.1.5/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-03 10:01:41.161346 smarthouse-0.1.5/smarthouse/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/action_decorators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.5/smarthouse/app.py
+-rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/device.py
+-rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/device_generator.py
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/logger.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/storage.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8195 2023-06-05 12:47:44.000000 smarthouse-0.1.5/smarthouse/telegram_client.py
+-rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.5/smarthouse/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-03 10:01:41.166425 smarthouse-0.1.5/smarthouse.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     5106 2023-07-03 10:01:41.000000 smarthouse-0.1.5/smarthouse.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      431 2023-07-03 10:01:41.000000 smarthouse-0.1.5/smarthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-07-03 10:01:41.000000 smarthouse-0.1.5/smarthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      290 2023-07-03 10:01:41.000000 smarthouse-0.1.5/smarthouse.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       11 2023-07-03 10:01:41.000000 smarthouse-0.1.5/smarthouse.egg-info/top_level.txt
```

### Comparing `smarthouse-0.1.4/PKG-INFO` & `smarthouse-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.4
+Version: 0.1.5
 Summary: Smart House Scenarios
 Home-page: https://smarthouselib.readthedocs.io/
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `smarthouse-0.1.4/README.md` & `smarthouse-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/README.rst` & `smarthouse-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/pyproject.toml` & `smarthouse-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/setup.py` & `smarthouse-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "python-dotenv",
     ]
 }
 
 
 setup(
     name="smarthouse",
-    version="0.1.4",
+    version="0.1.5",
     description="Smart House Scenarios",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://smarthouselib.readthedocs.io/",
     author="Ivan Kriuchkov",
     author_email="vivenchik@gmail.com",
     license="MIT",
```

### Comparing `smarthouse-0.1.4/smarthouse/action_decorators.py` & `smarthouse-0.1.5/smarthouse/action_decorators.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/smarthouse/app.py` & `smarthouse-0.1.5/smarthouse/app.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/smarthouse/device.py` & `smarthouse-0.1.5/smarthouse/device.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/smarthouse/storage.py` & `smarthouse-0.1.5/smarthouse/storage.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/smarthouse/telegram_client.py` & `smarthouse-0.1.5/smarthouse/telegram_client.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/smarthouse/utils.py` & `smarthouse-0.1.5/smarthouse/utils.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.4/smarthouse.egg-info/PKG-INFO` & `smarthouse-0.1.5/smarthouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.4
+Version: 0.1.5
 Summary: Smart House Scenarios
 Home-page: https://smarthouselib.readthedocs.io/
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


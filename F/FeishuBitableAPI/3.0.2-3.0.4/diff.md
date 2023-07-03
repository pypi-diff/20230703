# Comparing `tmp/FeishuBitableAPI-3.0.2.tar.gz` & `tmp/FeishuBitableAPI-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeishuBitableAPI-3.0.2.tar", last modified: Mon Jul  3 03:26:57 2023, max compression
+gzip compressed data, was "FeishuBitableAPI-3.0.4.tar", last modified: Mon Jul  3 03:34:30 2023, max compression
```

## Comparing `FeishuBitableAPI-3.0.2.tar` & `FeishuBitableAPI-3.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:26:57.901890 FeishuBitableAPI-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:26:57.901890 FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 03:26:57.000000 FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 03:26:57.000000 FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:26:57.000000 FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 03:26:57.000000 FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:26:57.000000 FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 03:26:46.000000 FeishuBitableAPI-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 03:26:57.901890 FeishuBitableAPI-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 03:26:46.000000 FeishuBitableAPI-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:26:57.901890 FeishuBitableAPI-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 03:26:46.000000 FeishuBitableAPI-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:26:57.901890 FeishuBitableAPI-3.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 03:26:46.000000 FeishuBitableAPI-3.0.2/test/test#GET_INFO_FROM_URL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:34:30.103075 FeishuBitableAPI-3.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:34:30.103075 FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 03:34:30.000000 FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-03 03:34:30.000000 FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:34:30.000000 FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 03:34:30.000000 FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:34:30.000000 FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 03:34:15.000000 FeishuBitableAPI-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 03:34:30.103075 FeishuBitableAPI-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 03:34:15.000000 FeishuBitableAPI-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:34:30.103075 FeishuBitableAPI-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 03:34:15.000000 FeishuBitableAPI-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:34:30.103075 FeishuBitableAPI-3.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 03:34:15.000000 FeishuBitableAPI-3.0.4/test/test#GET_INFO_FROM_URL-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 03:34:15.000000 FeishuBitableAPI-3.0.4/test/test#GET_INFO_FROM_URL.py
```

### Comparing `FeishuBitableAPI-3.0.2/FeishuBitableAPI.egg-info/PKG-INFO` & `FeishuBitableAPI-3.0.4/FeishuBitableAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.0.2
+Version: 3.0.4
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.0.2/LICENSE` & `FeishuBitableAPI-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.0.2/PKG-INFO` & `FeishuBitableAPI-3.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.0.2
+Version: 3.0.4
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.0.2/README.md` & `FeishuBitableAPI-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.0.2/setup.py` & `FeishuBitableAPI-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.0.2',
+    version='3.0.4',
     packages=find_packages(),
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

### Comparing `FeishuBitableAPI-3.0.2/test/test#GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.0.4/test/test#GET_INFO_FROM_URL.py`

 * *Files identical despite different names*


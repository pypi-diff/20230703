# Comparing `tmp/baysalt_christmas-0.1.7.9.tar.gz` & `tmp/baysalt_christmas-0.1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.9.tar", last modified: Wed Jun 28 02:51:27 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.8.0.tar", last modified: Mon Jul  3 02:25:51 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.9.tar` & `baysalt_christmas-0.1.8.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-28 02:51:27.965598 baysalt_christmas-0.1.7.9/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.7.9/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.9/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-28 02:51:27.965463 baysalt_christmas-0.1.7.9/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.9/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-28 02:51:27.962493 baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-28 02:51:27.000000 baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-28 02:51:27.000000 baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-28 02:51:27.000000 baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-28 02:51:27.000000 baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-28 02:51:27.000000 baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-28 02:51:27.963601 baysalt_christmas-0.1.7.9/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.7.9/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.9/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.9/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.9/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.9/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-28 02:51:27.964279 baysalt_christmas-0.1.7.9/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-28 02:51:27.965112 baysalt_christmas-0.1.7.9/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.9/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9042 2023-06-28 02:50:13.000000 baysalt_christmas-0.1.7.9/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.7.9/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.9/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.9/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-28 02:51:27.965649 baysalt_christmas-0.1.7.9/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-28 02:50:29.000000 baysalt_christmas-0.1.7.9/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 02:25:51.303280 baysalt_christmas-0.1.8.0/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.0/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.0/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-03 02:25:51.303148 baysalt_christmas-0.1.8.0/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.0/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 02:25:51.298489 baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-03 02:25:51.000000 baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-03 02:25:51.000000 baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-03 02:25:51.000000 baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-03 02:25:51.000000 baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-03 02:25:51.000000 baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 02:25:51.300396 baysalt_christmas-0.1.8.0/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.0/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 02:25:51.300965 baysalt_christmas-0.1.8.0/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5977 2023-07-03 02:06:47.000000 baysalt_christmas-0.1.8.0/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.0/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.0/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.0/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.0/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.0/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 02:25:51.301925 baysalt_christmas-0.1.8.0/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 02:25:51.302790 baysalt_christmas-0.1.8.0/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.0/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9042 2023-06-28 02:50:13.000000 baysalt_christmas-0.1.8.0/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.0/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.0/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.0/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-03 02:25:51.303335 baysalt_christmas-0.1.8.0/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-03 02:25:48.000000 baysalt_christmas-0.1.8.0/setup.py
```

### Comparing `baysalt_christmas-0.1.7.9/.DS_Store` & `baysalt_christmas-0.1.8.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/PKG-INFO` & `baysalt_christmas-0.1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.9
+Version: 0.1.8.0
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.9/README.md` & `baysalt_christmas-0.1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.9
+Version: 0.1.8.0
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.9/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.8.0/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 christmas/S_DateTime.py
 christmas/__init__.py
 christmas/commonCode.py
 christmas/cprintf.py
 christmas/processBar.py
 christmas/read_conf.py
 christmas/server_info.py
+christmas/Pyshell/RS_File.py
+christmas/Pyshell/__init__.py
 christmas/mncPy/.gitignore
 christmas/mncPy/LICENSE
 christmas/mncPy/__init__.py
 christmas/mncPy/common.py
 christmas/mncPy/compress.py
 christmas/mncPy/__pycache__/__init__.cpython-39.pyc
 christmas/mncPy/__pycache__/common.cpython-39.pyc
```

### Comparing `baysalt_christmas-0.1.7.9/christmas/Blogging.py` & `baysalt_christmas-0.1.8.0/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/S_DateTime.py` & `baysalt_christmas-0.1.8.0/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/commonCode.py` & `baysalt_christmas-0.1.8.0/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/cprintf.py` & `baysalt_christmas-0.1.8.0/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.8.0/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.8.0/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.8.0/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.8.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/mncPy/common.py` & `baysalt_christmas-0.1.8.0/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.8.0/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/processBar.py` & `baysalt_christmas-0.1.8.0/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/read_conf.py` & `baysalt_christmas-0.1.8.0/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/christmas/server_info.py` & `baysalt_christmas-0.1.8.0/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.9/setup.py` & `baysalt_christmas-0.1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.9",
+    version="0.1.8.0",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```


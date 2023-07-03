# Comparing `tmp/pput-0.1.1.tar.gz` & `tmp/pput-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pput-0.1.1.tar", last modified: Mon Jul  3 07:40:15 2023, max compression
+gzip compressed data, was "pput-0.1.2.tar", last modified: Mon Jul  3 07:45:21 2023, max compression
```

## Comparing `pput-0.1.1.tar` & `pput-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 07:40:15.022939 pput-0.1.1/
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 pput-0.1.1/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)      793 2023-07-03 07:40:15.022794 pput-0.1.1/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)       72 2023-07-01 04:28:36.000000 pput-0.1.1/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 07:40:15.021809 pput-0.1.1/pput/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-01 04:24:25.000000 pput-0.1.1/pput/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      269 2023-07-01 12:42:01.000000 pput-0.1.1/pput/main.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 07:40:15.022584 pput-0.1.1/pput.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)      793 2023-07-03 07:40:14.000000 pput-0.1.1/pput.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-03 07:40:15.000000 pput-0.1.1/pput.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-03 07:40:14.000000 pput-0.1.1/pput.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       40 2023-07-03 07:40:14.000000 pput-0.1.1/pput.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       31 2023-07-03 07:40:14.000000 pput-0.1.1/pput.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        5 2023-07-03 07:40:14.000000 pput-0.1.1/pput.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-03 07:40:15.022979 pput-0.1.1/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     1215 2023-07-03 07:39:33.000000 pput-0.1.1/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 07:45:21.267902 pput-0.1.2/
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 pput-0.1.2/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)      793 2023-07-03 07:45:21.267782 pput-0.1.2/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)       72 2023-07-01 04:28:36.000000 pput-0.1.2/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 07:45:21.266867 pput-0.1.2/pput/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-01 04:24:25.000000 pput-0.1.2/pput/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      269 2023-07-01 12:42:01.000000 pput-0.1.2/pput/main.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 07:45:21.267613 pput-0.1.2/pput.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)      793 2023-07-03 07:45:21.000000 pput-0.1.2/pput.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-03 07:45:21.000000 pput-0.1.2/pput.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-03 07:45:21.000000 pput-0.1.2/pput.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       40 2023-07-03 07:45:21.000000 pput-0.1.2/pput.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       31 2023-07-03 07:45:21.000000 pput-0.1.2/pput.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        5 2023-07-03 07:45:21.000000 pput-0.1.2/pput.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-03 07:45:21.267941 pput-0.1.2/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     1283 2023-07-03 07:45:09.000000 pput-0.1.2/setup.py
```

### Comparing `pput-0.1.1/LICENSE` & `pput-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pput-0.1.1/PKG-INFO` & `pput-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pput
-Version: 0.1.1
+Version: 0.1.2
 Summary: Test how to use setup.py.
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: pput
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pput-0.1.1/pput.egg-info/PKG-INFO` & `pput-0.1.2/pput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pput
-Version: 0.1.1
+Version: 0.1.2
 Summary: Test how to use setup.py.
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: pput
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pput-0.1.1/setup.py` & `pput-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
-with open('requirements.txt', 'r') as f:
-    requirements = f.readlines()
+# with open('requirements.txt', 'r') as f:
+#     requirements = f.readlines()
+requirements = [
+    'tyro~=0.5.3',
+    'setuptools~=68.0.0'
+]
+
 
 setup(
     name='pput',
-    version='0.1.1',
+    version='0.1.2',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     description='Test how to use setup.py.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='pput',
```


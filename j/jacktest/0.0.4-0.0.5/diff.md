# Comparing `tmp/jacktest-0.0.4.tar.gz` & `tmp/jacktest-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacktest-0.0.4.tar", last modified: Mon Jul  3 03:22:29 2023, max compression
+gzip compressed data, was "jacktest-0.0.5.tar", last modified: Mon Jul  3 03:36:55 2023, max compression
```

## Comparing `jacktest-0.0.4.tar` & `jacktest-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:22:29.308615 jacktest-0.0.4/
--rw-r--r--   0 bytedance   (501) staff       (20)     1074 2023-06-29 12:19:57.000000 jacktest-0.0.4/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:22:29.308202 jacktest-0.0.4/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      172 2023-06-29 12:19:40.000000 jacktest-0.0.4/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:22:29.305380 jacktest-0.0.4/jacktest/
--rw-r--r--   0 bytedance   (501) staff       (20)       78 2023-07-03 03:21:37.000000 jacktest-0.0.4/jacktest/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      155 2023-07-03 02:26:11.000000 jacktest-0.0.4/jacktest/print_hi.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:22:29.307565 jacktest-0.0.4/jacktest.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      196 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        9 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-03 03:22:29.308739 jacktest-0.0.4/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1748 2023-07-03 03:21:55.000000 jacktest-0.0.4/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:36:55.104024 jacktest-0.0.5/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1074 2023-06-29 12:19:57.000000 jacktest-0.0.5/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:36:55.103694 jacktest-0.0.5/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      172 2023-06-29 12:19:40.000000 jacktest-0.0.5/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:36:55.101127 jacktest-0.0.5/jacktest/
+-rw-r--r--   0 bytedance   (501) staff       (20)       73 2023-07-03 03:36:27.000000 jacktest-0.0.5/jacktest/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      155 2023-07-03 03:36:00.000000 jacktest-0.0.5/jacktest/print_hi.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:36:55.103142 jacktest-0.0.5/jacktest.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      196 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        9 2023-07-03 03:36:55.000000 jacktest-0.0.5/jacktest.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-03 03:36:55.104139 jacktest-0.0.5/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)     1748 2023-07-03 03:36:50.000000 jacktest-0.0.5/setup.py
```

### Comparing `jacktest-0.0.4/LICENSE` & `jacktest-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jacktest-0.0.4/PKG-INFO` & `jacktest-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktest
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jack
 Author-email: jack@example.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `jacktest-0.0.4/jacktest.egg-info/PKG-INFO` & `jacktest-0.0.5/jacktest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktest
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jack
 Author-email: jack@example.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `jacktest-0.0.4/setup.py` & `jacktest-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(name='jacktest',  # 包名
-      version='0.0.4',  # 版本号
+      version='0.0.5',  # 版本号
       description='A small example package',
       long_description=long_description,
       author='jack',
       author_email='jack@example.com',
       url='https://github.com/pypa/sampleproject',
       install_requires=[],
       license='BSD License',
```


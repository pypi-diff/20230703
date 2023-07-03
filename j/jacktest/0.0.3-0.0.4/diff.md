# Comparing `tmp/jacktest-0.0.3.tar.gz` & `tmp/jacktest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacktest-0.0.3.tar", last modified: Mon Jul  3 03:15:38 2023, max compression
+gzip compressed data, was "jacktest-0.0.4.tar", last modified: Mon Jul  3 03:22:29 2023, max compression
```

## Comparing `jacktest-0.0.3.tar` & `jacktest-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:15:38.889033 jacktest-0.0.3/
--rw-r--r--   0 bytedance   (501) staff       (20)     1074 2023-06-29 12:19:57.000000 jacktest-0.0.3/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:15:38.888665 jacktest-0.0.3/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      172 2023-06-29 12:19:40.000000 jacktest-0.0.3/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:15:38.886337 jacktest-0.0.3/core/
--rw-r--r--   0 bytedance   (501) staff       (20)       87 2023-07-03 03:15:34.000000 jacktest-0.0.3/core/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      155 2023-07-03 02:26:11.000000 jacktest-0.0.3/core/print_hi.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:15:38.888174 jacktest-0.0.3/jacktest.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:15:38.000000 jacktest-0.0.3/jacktest.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      188 2023-07-03 03:15:38.000000 jacktest-0.0.3/jacktest.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-03 03:15:38.000000 jacktest-0.0.3/jacktest.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        5 2023-07-03 03:15:38.000000 jacktest-0.0.3/jacktest.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-03 03:15:38.889153 jacktest-0.0.3/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1748 2023-07-03 03:15:34.000000 jacktest-0.0.3/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:22:29.308615 jacktest-0.0.4/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1074 2023-06-29 12:19:57.000000 jacktest-0.0.4/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:22:29.308202 jacktest-0.0.4/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      172 2023-06-29 12:19:40.000000 jacktest-0.0.4/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:22:29.305380 jacktest-0.0.4/jacktest/
+-rw-r--r--   0 bytedance   (501) staff       (20)       78 2023-07-03 03:21:37.000000 jacktest-0.0.4/jacktest/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      155 2023-07-03 02:26:11.000000 jacktest-0.0.4/jacktest/print_hi.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-03 03:22:29.307565 jacktest-0.0.4/jacktest.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)      997 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      196 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        9 2023-07-03 03:22:29.000000 jacktest-0.0.4/jacktest.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-03 03:22:29.308739 jacktest-0.0.4/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)     1748 2023-07-03 03:21:55.000000 jacktest-0.0.4/setup.py
```

### Comparing `jacktest-0.0.3/LICENSE` & `jacktest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jacktest-0.0.3/PKG-INFO` & `jacktest-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktest
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jack
 Author-email: jack@example.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `jacktest-0.0.3/jacktest.egg-info/PKG-INFO` & `jacktest-0.0.4/jacktest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktest
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jack
 Author-email: jack@example.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `jacktest-0.0.3/setup.py` & `jacktest-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(name='jacktest',  # 包名
-      version='0.0.3',  # 版本号
+      version='0.0.4',  # 版本号
       description='A small example package',
       long_description=long_description,
       author='jack',
       author_email='jack@example.com',
       url='https://github.com/pypa/sampleproject',
       install_requires=[],
       license='BSD License',
```


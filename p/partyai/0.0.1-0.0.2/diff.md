# Comparing `tmp/partyai-0.0.1.tar.gz` & `tmp/partyai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partyai-0.0.1.tar", last modified: Tue Jun 27 10:48:08 2023, max compression
+gzip compressed data, was "partyai-0.0.2.tar", last modified: Mon Jul  3 09:52:10 2023, max compression
```

## Comparing `partyai-0.0.1.tar` & `partyai-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 imad       (501) staff       (20)        0 2023-06-27 10:48:08.641792 partyai-0.0.1/
--rw-r--r--   0 imad       (501) staff       (20)      411 2023-06-27 10:48:08.641620 partyai-0.0.1/PKG-INFO
--rw-r--r--   0 imad       (501) staff       (20)        7 2023-06-27 10:48:00.000000 partyai-0.0.1/README.md
-drwxr-xr-x   0 imad       (501) staff       (20)        0 2023-06-27 10:48:08.640565 partyai-0.0.1/partyai/
--rw-r--r--   0 imad       (501) staff       (20)       29 2023-06-27 10:45:17.000000 partyai-0.0.1/partyai/__init__.py
--rw-r--r--   0 imad       (501) staff       (20)     1537 2023-06-27 10:38:13.000000 partyai-0.0.1/partyai/partyai.py
-drwxr-xr-x   0 imad       (501) staff       (20)        0 2023-06-27 10:48:08.641413 partyai-0.0.1/partyai.egg-info/
--rw-r--r--   0 imad       (501) staff       (20)      411 2023-06-27 10:48:08.000000 partyai-0.0.1/partyai.egg-info/PKG-INFO
--rw-r--r--   0 imad       (501) staff       (20)      211 2023-06-27 10:48:08.000000 partyai-0.0.1/partyai.egg-info/SOURCES.txt
--rw-r--r--   0 imad       (501) staff       (20)        1 2023-06-27 10:48:08.000000 partyai-0.0.1/partyai.egg-info/dependency_links.txt
--rw-r--r--   0 imad       (501) staff       (20)        9 2023-06-27 10:48:08.000000 partyai-0.0.1/partyai.egg-info/requires.txt
--rw-r--r--   0 imad       (501) staff       (20)        8 2023-06-27 10:48:08.000000 partyai-0.0.1/partyai.egg-info/top_level.txt
--rw-r--r--   0 imad       (501) staff       (20)       38 2023-06-27 10:48:08.641840 partyai-0.0.1/setup.cfg
--rw-r--r--   0 imad       (501) staff       (20)      665 2023-06-27 10:47:09.000000 partyai-0.0.1/setup.py
+drwxr-xr-x   0 imad       (501) staff       (20)        0 2023-07-03 09:52:10.100767 partyai-0.0.2/
+-rw-r--r--   0 imad       (501) staff       (20)      439 2023-07-03 09:52:10.100628 partyai-0.0.2/PKG-INFO
+-rw-r--r--   0 imad       (501) staff       (20)       45 2023-07-03 09:47:35.000000 partyai-0.0.2/README.md
+drwxr-xr-x   0 imad       (501) staff       (20)        0 2023-07-03 09:52:10.099348 partyai-0.0.2/partyai/
+-rw-r--r--   0 imad       (501) staff       (20)       29 2023-06-27 10:45:17.000000 partyai-0.0.2/partyai/__init__.py
+-rw-r--r--   0 imad       (501) staff       (20)     1537 2023-06-27 19:08:39.000000 partyai-0.0.2/partyai/partyai.py
+drwxr-xr-x   0 imad       (501) staff       (20)        0 2023-07-03 09:52:10.100390 partyai-0.0.2/partyai.egg-info/
+-rw-r--r--   0 imad       (501) staff       (20)      439 2023-07-03 09:52:10.000000 partyai-0.0.2/partyai.egg-info/PKG-INFO
+-rw-r--r--   0 imad       (501) staff       (20)      211 2023-07-03 09:52:10.000000 partyai-0.0.2/partyai.egg-info/SOURCES.txt
+-rw-r--r--   0 imad       (501) staff       (20)        1 2023-07-03 09:52:10.000000 partyai-0.0.2/partyai.egg-info/dependency_links.txt
+-rw-r--r--   0 imad       (501) staff       (20)        9 2023-07-03 09:52:10.000000 partyai-0.0.2/partyai.egg-info/requires.txt
+-rw-r--r--   0 imad       (501) staff       (20)        8 2023-07-03 09:52:10.000000 partyai-0.0.2/partyai.egg-info/top_level.txt
+-rw-r--r--   0 imad       (501) staff       (20)       38 2023-07-03 09:52:10.100821 partyai-0.0.2/setup.cfg
+-rw-r--r--   0 imad       (501) staff       (20)      655 2023-07-03 09:48:06.000000 partyai-0.0.2/setup.py
```

### Comparing `partyai-0.0.1/partyai/partyai.py` & `partyai-0.0.2/partyai/partyai.py`

 * *Files identical despite different names*

### Comparing `partyai-0.0.1/setup.py` & `partyai-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 setup(
     name="partyai",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
-    description="Community functions for ChatGPT",
+    description="Functions for ChatGPT",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/partyai/partyai",
     author="Imad Bouziani",
     author_email="imad.a.bouziani@gmail.com",
     license="MIT",
     classifiers=[
```


# Comparing `tmp/dsna_complete-0.0.1.tar.gz` & `tmp/dsna_complete-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.1.tar", last modified: Mon Jul  3 12:18:44 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.2.tar", last modified: Mon Jul  3 12:43:18 2023, max compression
```

## Comparing `dsna_complete-0.0.1.tar` & `dsna_complete-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:18:44.463807 dsna_complete-0.0.1/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-03 12:18:44.463851 dsna_complete-0.0.1/PKG-INFO
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:18:44.462659 dsna_complete-0.0.1/automl/
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)        0 2023-06-08 03:05:14.000000 dsna_complete-0.0.1/automl/__init__.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     1726 2023-06-08 03:05:14.000000 dsna_complete-0.0.1/automl/generate.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     9436 2023-07-03 12:15:55.000000 dsna_complete-0.0.1/automl/process.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     2739 2023-06-08 03:05:14.000000 dsna_complete-0.0.1/automl/test.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)    19852 2023-07-03 12:06:17.000000 dsna_complete-0.0.1/automl/train.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:18:44.461291 dsna_complete-0.0.1/base/
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:18:44.463033 dsna_complete-0.0.1/base/utils/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)     3339 2023-07-03 11:35:14.000000 dsna_complete-0.0.1/base/utils/servant.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:18:44.463712 dsna_complete-0.0.1/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-03 12:18:44.000000 dsna_complete-0.0.1/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      326 2023-07-03 12:18:44.000000 dsna_complete-0.0.1/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-03 12:18:44.000000 dsna_complete-0.0.1/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-03 12:18:44.000000 dsna_complete-0.0.1/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       17 2023-07-03 12:18:44.000000 dsna_complete-0.0.1/dsna_complete.egg-info/top_level.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.1/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      386 2023-07-03 12:18:44.464081 dsna_complete-0.0.1/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.1/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.812575 dsna_complete-0.0.2/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-03 12:43:18.812630 dsna_complete-0.0.2/PKG-INFO
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.811417 dsna_complete-0.0.2/automl/
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)        0 2023-06-08 03:05:14.000000 dsna_complete-0.0.2/automl/__init__.py
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)     1726 2023-06-08 03:05:14.000000 dsna_complete-0.0.2/automl/generate.py
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)     9436 2023-07-03 12:40:48.000000 dsna_complete-0.0.2/automl/process.py
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)     2739 2023-07-03 12:37:42.000000 dsna_complete-0.0.2/automl/test.py
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)    19852 2023-07-03 12:06:17.000000 dsna_complete-0.0.2/automl/train.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.809969 dsna_complete-0.0.2/base/
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.811776 dsna_complete-0.0.2/base/utils/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)     3339 2023-07-03 11:35:14.000000 dsna_complete-0.0.2/base/utils/servant.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.812476 dsna_complete-0.0.2/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      326 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       17 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/top_level.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.2/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      386 2023-07-03 12:43:18.812866 dsna_complete-0.0.2/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.2/setup.py
```

### Comparing `dsna_complete-0.0.1/automl/generate.py` & `dsna_complete-0.0.2/automl/generate.py`

 * *Files identical despite different names*

### Comparing `dsna_complete-0.0.1/automl/process.py` & `dsna_complete-0.0.2/automl/process.py`

 * *Files identical despite different names*

### Comparing `dsna_complete-0.0.1/automl/test.py` & `dsna_complete-0.0.2/automl/test.py`

 * *Files identical despite different names*

### Comparing `dsna_complete-0.0.1/automl/train.py` & `dsna_complete-0.0.2/automl/train.py`

 * *Files identical despite different names*

### Comparing `dsna_complete-0.0.1/base/utils/servant.py` & `dsna_complete-0.0.2/base/utils/servant.py`

 * *Files identical despite different names*


# Comparing `tmp/locdataMAC-0.0.7.tar.gz` & `tmp/locdataMAC-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locdataMAC-0.0.7.tar", last modified: Sat Feb 18 12:34:48 2023, max compression
+gzip compressed data, was "locdataMAC-0.0.8.tar", last modified: Mon Jul  3 16:30:23 2023, max compression
```

## Comparing `locdataMAC-0.0.7.tar` & `locdataMAC-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 12:34:48.710162 locdataMAC-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-18 12:34:48.710162 locdataMAC-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-18 12:34:48.710162 locdataMAC-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 12:34:48.706162 locdataMAC-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 12:34:48.706162 locdataMAC-0.0.7/src/locdataMAC/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/cutom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-02-18 12:34:37.000000 locdataMAC-0.0.7/src/locdataMAC/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 12:34:48.710162 locdataMAC-0.0.7/src/locdataMAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-18 12:34:48.000000 locdataMAC-0.0.7/src/locdataMAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-18 12:34:48.000000 locdataMAC-0.0.7/src/locdataMAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 12:34:48.000000 locdataMAC-0.0.7/src/locdataMAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-18 12:34:48.000000 locdataMAC-0.0.7/src/locdataMAC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-18 12:34:48.000000 locdataMAC-0.0.7/src/locdataMAC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.769907 locdataMAC-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.769907 locdataMAC-0.0.8/src/locdataMAC/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/cutom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/src/locdataMAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/top_level.txt
```

### Comparing `locdataMAC-0.0.7/LICENSE` & `locdataMAC-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.7/setup.py` & `locdataMAC-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 REPO_NAME = "locdataMAC"
 AUTHOR_USER_NAME = "SachinMishra-ux"
 SRC_REPO = "locdataMAC"
 AUTHOR_EMAIL = "sachin19566@gmail.com"
 
 setuptools.setup(
```

### Comparing `locdataMAC-0.0.7/src/locdataMAC/activity.py` & `locdataMAC-0.0.8/src/locdataMAC/activity.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.7/src/locdataMAC/analytics.py` & `locdataMAC-0.0.8/src/locdataMAC/analytics.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.7/src/locdataMAC/charts.py` & `locdataMAC-0.0.8/src/locdataMAC/charts.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.7/src/locdataMAC/timer.py` & `locdataMAC-0.0.8/src/locdataMAC/timer.py`

 * *Files identical despite different names*


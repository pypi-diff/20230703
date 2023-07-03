# Comparing `tmp/pipsqlite3kitV2-1.0.0.tar.gz` & `tmp/pipsqlite3kitV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlite3kitV2-1.0.0.tar", last modified: Mon Jul  3 02:34:05 2023, max compression
+gzip compressed data, was "pipsqlite3kitV2-1.1.0.tar", last modified: Mon Jul  3 02:36:18 2023, max compression
```

## Comparing `pipsqlite3kitV2-1.0.0.tar` & `pipsqlite3kitV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:34:05.716705 pipsqlite3kitV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-03 02:34:05.716705 pipsqlite3kitV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:34:05.716705 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 02:34:05.000000 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:34:05.716705 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-03 02:34:05.000000 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-03 02:34:05.000000 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:34:05.000000 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-03 02:34:05.000000 pipsqlite3kitV2-1.0.0/pipsqlite3kitV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:34:05.716705 pipsqlite3kitV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-07-03 02:34:05.000000 pipsqlite3kitV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:36:18.348361 pipsqlite3kitV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-03 02:36:18.348361 pipsqlite3kitV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:36:18.344361 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-03 02:36:17.000000 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:36:18.348361 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-03 02:36:18.000000 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-03 02:36:18.000000 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:36:18.000000 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-03 02:36:18.000000 pipsqlite3kitV2-1.1.0/pipsqlite3kitV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:36:18.348361 pipsqlite3kitV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-07-03 02:36:17.000000 pipsqlite3kitV2-1.1.0/setup.py
```

### Comparing `pipsqlite3kitV2-1.0.0/setup.py` & `pipsqlite3kitV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlite3kitV2",
     version=VERSION,
```


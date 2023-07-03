# Comparing `tmp/stc-geck-1.1.3.tar.gz` & `tmp/stc-geck-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.1.3.tar", last modified: Fri Jun 23 09:02:47 2023, max compression
+gzip compressed data, was "stc-geck-1.2.0.tar", last modified: Mon Jul  3 16:34:05 2023, max compression
```

## Comparing `stc-geck-1.1.3.tar` & `stc-geck-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-23 09:02:47.557919 stc-geck-1.1.3/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-23 09:02:47.557384 stc-geck-1.1.3/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.3/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-23 09:01:59.000000 stc-geck-1.1.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-23 09:01:52.000000 stc-geck-1.1.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-23 09:02:47.558183 stc-geck-1.1.3/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-23 09:02:47.552314 stc-geck-1.1.3/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6152 2023-06-18 14:44:03.000000 stc-geck-1.1.3/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     6236 2023-06-18 18:47:15.000000 stc-geck-1.1.3/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.1.3/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-23 09:02:47.556494 stc-geck-1.1.3/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 16:34:05.631859 stc-geck-1.2.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 16:34:05.631604 stc-geck-1.2.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.2.0/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-03 16:33:46.000000 stc-geck-1.2.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-03 15:18:02.000000 stc-geck-1.2.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-03 16:34:05.631993 stc-geck-1.2.0/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 16:34:05.629471 stc-geck-1.2.0/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6152 2023-06-18 14:44:03.000000 stc-geck-1.2.0/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6236 2023-06-18 18:47:15.000000 stc-geck-1.2.0/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.0/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 16:34:05.631202 stc-geck-1.2.0/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.1.3/pyproject.toml` & `stc-geck-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.1.3"
+version = "1.2.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.1.3/stc_geck/cli.py` & `stc-geck-1.2.0/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.1.3/stc_geck/client.py` & `stc-geck-1.2.0/stc_geck/client.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.1.3/stc_geck/utils.py` & `stc-geck-1.2.0/stc_geck/utils.py`

 * *Files identical despite different names*


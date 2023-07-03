# Comparing `tmp/data_merge-0.1.tar.gz` & `tmp/data_merge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_merge-0.1.tar", last modified: Sun Jul  2 05:43:13 2023, max compression
+gzip compressed data, was "data_merge-0.1.1.tar", last modified: Mon Jul  3 10:05:48 2023, max compression
```

## Comparing `data_merge-0.1.tar` & `data_merge-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ojo        (501) staff       (20)        0 2023-07-02 05:43:13.420092 data_merge-0.1/
--rw-r--r--   0 ojo        (501) staff       (20)     1068 2023-07-02 05:27:57.000000 data_merge-0.1/LICENSE
--rw-r--r--   0 ojo        (501) staff       (20)      253 2023-07-02 05:43:13.419972 data_merge-0.1/PKG-INFO
-drwxr-xr-x   0 ojo        (501) staff       (20)        0 2023-07-02 05:43:13.419006 data_merge-0.1/data_fusion/
--rw-r--r--   0 ojo        (501) staff       (20)        0 2023-07-01 18:49:36.000000 data_merge-0.1/data_fusion/__init__.py
--rw-r--r--   0 ojo        (501) staff       (20)     1324 2023-07-01 18:54:23.000000 data_merge-0.1/data_fusion/file_merger.py
-drwxr-xr-x   0 ojo        (501) staff       (20)        0 2023-07-02 05:43:13.419820 data_merge-0.1/data_merge.egg-info/
--rw-r--r--   0 ojo        (501) staff       (20)      253 2023-07-02 05:43:13.000000 data_merge-0.1/data_merge.egg-info/PKG-INFO
--rw-r--r--   0 ojo        (501) staff       (20)      236 2023-07-02 05:43:13.000000 data_merge-0.1/data_merge.egg-info/SOURCES.txt
--rw-r--r--   0 ojo        (501) staff       (20)        1 2023-07-02 05:43:13.000000 data_merge-0.1/data_merge.egg-info/dependency_links.txt
--rw-r--r--   0 ojo        (501) staff       (20)       14 2023-07-02 05:43:13.000000 data_merge-0.1/data_merge.egg-info/requires.txt
--rw-r--r--   0 ojo        (501) staff       (20)       12 2023-07-02 05:43:13.000000 data_merge-0.1/data_merge.egg-info/top_level.txt
--rw-r--r--   0 ojo        (501) staff       (20)       38 2023-07-02 05:43:13.420132 data_merge-0.1/setup.cfg
--rw-r--r--   0 ojo        (501) staff       (20)      328 2023-07-02 05:40:52.000000 data_merge-0.1/setup.py
+drwxr-xr-x   0 ojo        (501) staff       (20)        0 2023-07-03 10:05:48.437695 data_merge-0.1.1/
+-rw-r--r--   0 ojo        (501) staff       (20)     1068 2023-07-02 05:27:57.000000 data_merge-0.1.1/LICENSE
+-rw-r--r--   0 ojo        (501) staff       (20)      255 2023-07-03 10:05:48.437572 data_merge-0.1.1/PKG-INFO
+drwxr-xr-x   0 ojo        (501) staff       (20)        0 2023-07-03 10:05:48.436600 data_merge-0.1.1/data_merge/
+-rw-r--r--   0 ojo        (501) staff       (20)        0 2023-07-01 18:49:36.000000 data_merge-0.1.1/data_merge/__init__.py
+-rw-r--r--   0 ojo        (501) staff       (20)     1324 2023-07-01 18:54:23.000000 data_merge-0.1.1/data_merge/file_merger.py
+drwxr-xr-x   0 ojo        (501) staff       (20)        0 2023-07-03 10:05:48.437414 data_merge-0.1.1/data_merge.egg-info/
+-rw-r--r--   0 ojo        (501) staff       (20)      255 2023-07-03 10:05:48.000000 data_merge-0.1.1/data_merge.egg-info/PKG-INFO
+-rw-r--r--   0 ojo        (501) staff       (20)      234 2023-07-03 10:05:48.000000 data_merge-0.1.1/data_merge.egg-info/SOURCES.txt
+-rw-r--r--   0 ojo        (501) staff       (20)        1 2023-07-03 10:05:48.000000 data_merge-0.1.1/data_merge.egg-info/dependency_links.txt
+-rw-r--r--   0 ojo        (501) staff       (20)       14 2023-07-03 10:05:48.000000 data_merge-0.1.1/data_merge.egg-info/requires.txt
+-rw-r--r--   0 ojo        (501) staff       (20)       11 2023-07-03 10:05:48.000000 data_merge-0.1.1/data_merge.egg-info/top_level.txt
+-rw-r--r--   0 ojo        (501) staff       (20)       38 2023-07-03 10:05:48.437741 data_merge-0.1.1/setup.cfg
+-rw-r--r--   0 ojo        (501) staff       (20)      330 2023-07-03 09:48:22.000000 data_merge-0.1.1/setup.py
```

### Comparing `data_merge-0.1/LICENSE` & `data_merge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `data_merge-0.1/data_fusion/file_merger.py` & `data_merge-0.1.1/data_merge/file_merger.py`

 * *Files identical despite different names*


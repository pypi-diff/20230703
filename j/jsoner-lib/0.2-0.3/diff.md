# Comparing `tmp/jsoner-lib-0.2.tar.gz` & `tmp/jsoner-lib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoner-lib-0.2.tar", last modified: Mon Jul  3 00:57:32 2023, max compression
+gzip compressed data, was "jsoner-lib-0.3.tar", last modified: Mon Jul  3 01:01:23 2023, max compression
```

## Comparing `jsoner-lib-0.2.tar` & `jsoner-lib-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:57:32.725702 jsoner-lib-0.2/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-03 00:29:20.000000 jsoner-lib-0.2/LICENSE
--rw-r--r--   0 bigmag_    (502) staff       (20)      202 2023-07-03 00:57:32.725214 jsoner-lib-0.2/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)     1673 2023-07-03 00:57:05.000000 jsoner-lib-0.2/README.md
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:57:32.717416 jsoner-lib-0.2/jsoner/
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:57:32.724195 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/
--rw-r--r--   0 bigmag_    (502) staff       (20)      202 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)      230 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/SOURCES.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/dependency_links.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        9 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/requires.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/top_level.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-03 00:57:32.726374 jsoner-lib-0.2/setup.cfg
--rw-r--r--   0 bigmag_    (502) staff       (20)      374 2023-07-03 00:57:09.000000 jsoner-lib-0.2/setup.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:01:23.318425 jsoner-lib-0.3/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-03 00:29:20.000000 jsoner-lib-0.3/LICENSE
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1916 2023-07-03 01:01:23.316820 jsoner-lib-0.3/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1673 2023-07-03 00:57:05.000000 jsoner-lib-0.3/README.md
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:01:23.308707 jsoner-lib-0.3/jsoner/
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:01:23.315076 jsoner-lib-0.3/jsoner/jsoner_lib.egg-info/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1916 2023-07-03 01:01:23.000000 jsoner-lib-0.3/jsoner/jsoner_lib.egg-info/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)      230 2023-07-03 01:01:23.000000 jsoner-lib-0.3/jsoner/jsoner_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 01:01:23.000000 jsoner-lib-0.3/jsoner/jsoner_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        9 2023-07-03 01:01:23.000000 jsoner-lib-0.3/jsoner/jsoner_lib.egg-info/requires.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 01:01:23.000000 jsoner-lib-0.3/jsoner/jsoner_lib.egg-info/top_level.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-03 01:01:23.318853 jsoner-lib-0.3/setup.cfg
+-rw-r--r--   0 bigmag_    (502) staff       (20)      592 2023-07-03 01:01:17.000000 jsoner-lib-0.3/setup.py
```

### Comparing `jsoner-lib-0.2/LICENSE` & `jsoner-lib-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoner-lib-0.2/README.md` & `jsoner-lib-0.3/README.md`

 * *Files identical despite different names*


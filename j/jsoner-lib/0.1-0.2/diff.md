# Comparing `tmp/jsoner-lib-0.1.tar.gz` & `tmp/jsoner-lib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoner-lib-0.1.tar", last modified: Mon Jul  3 00:35:20 2023, max compression
+gzip compressed data, was "jsoner-lib-0.2.tar", last modified: Mon Jul  3 00:57:32 2023, max compression
```

## Comparing `jsoner-lib-0.1.tar` & `jsoner-lib-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:35:20.336238 jsoner-lib-0.1/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-03 00:29:20.000000 jsoner-lib-0.1/LICENSE
--rw-r--r--   0 bigmag_    (502) staff       (20)      202 2023-07-03 00:35:20.335263 jsoner-lib-0.1/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)       95 2023-07-03 00:29:20.000000 jsoner-lib-0.1/README.md
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:35:20.311101 jsoner-lib-0.1/jsoner/
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:35:20.334444 jsoner-lib-0.1/jsoner/jsoner_lib.egg-info/
--rw-r--r--   0 bigmag_    (502) staff       (20)      202 2023-07-03 00:35:20.000000 jsoner-lib-0.1/jsoner/jsoner_lib.egg-info/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)      230 2023-07-03 00:35:20.000000 jsoner-lib-0.1/jsoner/jsoner_lib.egg-info/SOURCES.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 00:35:20.000000 jsoner-lib-0.1/jsoner/jsoner_lib.egg-info/dependency_links.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        9 2023-07-03 00:35:20.000000 jsoner-lib-0.1/jsoner/jsoner_lib.egg-info/requires.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 00:35:20.000000 jsoner-lib-0.1/jsoner/jsoner_lib.egg-info/top_level.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-03 00:35:20.336420 jsoner-lib-0.1/setup.cfg
--rw-r--r--   0 bigmag_    (502) staff       (20)      374 2023-07-03 00:34:52.000000 jsoner-lib-0.1/setup.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:57:32.725702 jsoner-lib-0.2/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-03 00:29:20.000000 jsoner-lib-0.2/LICENSE
+-rw-r--r--   0 bigmag_    (502) staff       (20)      202 2023-07-03 00:57:32.725214 jsoner-lib-0.2/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1673 2023-07-03 00:57:05.000000 jsoner-lib-0.2/README.md
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:57:32.717416 jsoner-lib-0.2/jsoner/
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 00:57:32.724195 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/
+-rw-r--r--   0 bigmag_    (502) staff       (20)      202 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)      230 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        9 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/requires.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 00:57:32.000000 jsoner-lib-0.2/jsoner/jsoner_lib.egg-info/top_level.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-03 00:57:32.726374 jsoner-lib-0.2/setup.cfg
+-rw-r--r--   0 bigmag_    (502) staff       (20)      374 2023-07-03 00:57:09.000000 jsoner-lib-0.2/setup.py
```

### Comparing `jsoner-lib-0.1/LICENSE` & `jsoner-lib-0.2/LICENSE`

 * *Files identical despite different names*


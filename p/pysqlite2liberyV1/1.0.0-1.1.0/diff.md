# Comparing `tmp/pysqlite2liberyV1-1.0.0.tar.gz` & `tmp/pysqlite2liberyV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlite2liberyV1-1.0.0.tar", last modified: Mon Jul  3 02:37:30 2023, max compression
+gzip compressed data, was "pysqlite2liberyV1-1.1.0.tar", last modified: Mon Jul  3 02:39:36 2023, max compression
```

## Comparing `pysqlite2liberyV1-1.0.0.tar` & `pysqlite2liberyV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:37:30.808172 pysqlite2liberyV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-03 02:37:30.804172 pysqlite2liberyV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:37:30.804172 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 02:37:30.000000 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:37:30.804172 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-03 02:37:30.000000 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-03 02:37:30.000000 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:37:30.000000 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 02:37:30.000000 pysqlite2liberyV1-1.0.0/pysqlite2liberyV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:37:30.808172 pysqlite2liberyV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-03 02:37:30.000000 pysqlite2liberyV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:39:36.035845 pysqlite2liberyV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-03 02:39:36.035845 pysqlite2liberyV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:39:36.031844 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-03 02:39:35.000000 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:39:36.035845 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-03 02:39:35.000000 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-03 02:39:35.000000 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:39:35.000000 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 02:39:35.000000 pysqlite2liberyV1-1.1.0/pysqlite2liberyV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:39:36.035845 pysqlite2liberyV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-03 02:39:35.000000 pysqlite2liberyV1-1.1.0/setup.py
```


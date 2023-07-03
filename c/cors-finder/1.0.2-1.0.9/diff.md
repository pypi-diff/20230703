# Comparing `tmp/cors-finder-1.0.2.tar.gz` & `tmp/cors-finder-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cors-finder-1.0.2.tar", last modified: Sun Jul  2 17:23:20 2023, max compression
+gzip compressed data, was "cors-finder-1.0.9.tar", last modified: Mon Jul  3 20:36:27 2023, max compression
```

## Comparing `cors-finder-1.0.2.tar` & `cors-finder-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-02 17:23:20.632897 cors-finder-1.0.2/
--rw-rw-r--   0 hari      (1000) hari      (1000)      295 2023-07-02 17:23:20.632897 cors-finder-1.0.2/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.2/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-02 17:23:20.632897 cors-finder-1.0.2/cors_finder.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)      295 2023-07-02 17:23:20.000000 cors-finder-1.0.2/cors_finder.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      220 2023-07-02 17:23:20.000000 cors-finder-1.0.2/cors_finder.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-02 17:23:20.000000 cors-finder-1.0.2/cors_finder.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-02 17:23:20.000000 cors-finder-1.0.2/cors_finder.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-02 17:23:20.000000 cors-finder-1.0.2/cors_finder.egg-info/top_level.txt
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-02 17:23:20.632897 cors-finder-1.0.2/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.2/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     1763 2023-07-02 17:07:00.000000 cors-finder-1.0.2/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       38 2023-07-02 17:23:20.632897 cors-finder-1.0.2/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      419 2023-07-02 17:22:49.000000 cors-finder-1.0.2/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:36:27.112696 cors-finder-1.0.9/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:36:27.112696 cors-finder-1.0.9/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     2770 2023-07-01 12:08:51.000000 cors-finder-1.0.9/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:36:27.112696 cors-finder-1.0.9/cors_finder.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3098 2023-07-03 20:36:27.000000 cors-finder-1.0.9/cors_finder.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      268 2023-07-03 20:36:27.000000 cors-finder-1.0.9/cors_finder.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-03 20:36:27.000000 cors-finder-1.0.9/cors_finder.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       47 2023-07-03 20:36:27.000000 cors-finder-1.0.9/cors_finder.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       26 2023-07-03 20:36:27.000000 cors-finder-1.0.9/cors_finder.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-03 20:36:27.000000 cors-finder-1.0.9/cors_finder.egg-info/top_level.txt
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-03 20:36:27.112696 cors-finder-1.0.9/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 cors-finder-1.0.9/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-03 20:04:38.000000 cors-finder-1.0.9/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-03 20:36:27.112696 cors-finder-1.0.9/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      708 2023-07-03 20:35:58.000000 cors-finder-1.0.9/setup.py
```

### Comparing `cors-finder-1.0.2/README.md` & `cors-finder-1.0.9/README.md`

 * *Files identical despite different names*


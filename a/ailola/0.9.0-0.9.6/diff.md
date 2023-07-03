# Comparing `tmp/ailola-0.9.0.tar.gz` & `tmp/ailola-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailola-0.9.0.tar", last modified: Mon Jul  3 11:08:22 2023, max compression
+gzip compressed data, was "ailola-0.9.6.tar", last modified: Mon Jul  3 11:48:18 2023, max compression
```

## Comparing `ailola-0.9.0.tar` & `ailola-0.9.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 11:08:22.683516 ailola-0.9.0/
--rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 11:08:22.683608 ailola-0.9.0/PKG-INFO
--rw-r--r--   0 elhayefrat   (501) staff       (20)     2948 2023-07-03 11:06:32.000000 ailola-0.9.0/README.md
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 11:08:22.674376 ailola-0.9.0/ailola/
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 11:08:22.683183 ailola-0.9.0/ailola/ailola.egg-info/
--rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/PKG-INFO
--rw-r--r--   0 elhayefrat   (501) staff       (20)      269 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/SOURCES.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)        1 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/dependency_links.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       38 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/entry_points.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       31 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/requires.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)        7 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/top_level.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)     3417 2023-07-03 10:45:15.000000 ailola-0.9.0/ailola/ailola.py
--rw-r--r--   0 elhayefrat   (501) staff       (20)      107 2023-07-03 11:08:22.685179 ailola-0.9.0/setup.cfg
--rw-r--r--   0 elhayefrat   (501) staff       (20)      427 2023-07-03 10:45:50.000000 ailola-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:48:18.629430 ailola-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 11:48:18.629430 ailola-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-03 11:48:09.000000 ailola-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:48:18.629430 ailola-0.9.6/ailola/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:48:18.629430 ailola-0.9.6/ailola/ailola.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 11:48:18.000000 ailola-0.9.6/ailola/ailola.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:48:18.000000 ailola-0.9.6/ailola/ailola.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:48:18.000000 ailola-0.9.6/ailola/ailola.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:48:18.000000 ailola-0.9.6/ailola/ailola.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 11:48:18.000000 ailola-0.9.6/ailola/ailola.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:48:18.000000 ailola-0.9.6/ailola/ailola.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-03 11:48:09.000000 ailola-0.9.6/ailola/ailola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 11:48:18.629430 ailola-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 11:48:09.000000 ailola-0.9.6/setup.py
```

### Comparing `ailola-0.9.0/README.md` & `ailola-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ailola-0.9.0/ailola/ailola.py` & `ailola-0.9.6/ailola/ailola.py`

 * *Files identical despite different names*


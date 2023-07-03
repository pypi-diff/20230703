# Comparing `tmp/summo-0.0.2.tar.gz` & `tmp/summo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summo-0.0.2.tar", last modified: Fri Jun 30 23:28:18 2023, max compression
+gzip compressed data, was "summo-0.0.3.tar", last modified: Mon Jul  3 17:54:40 2023, max compression
```

## Comparing `summo-0.0.2.tar` & `summo-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1071 2023-06-29 18:44:42.000000 summo-0.0.2/LICENSE
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      417 2023-06-30 23:28:18.217963 summo-0.0.2/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      202 2023-06-29 21:36:53.000000 summo-0.0.2/README.md
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      605 2023-06-30 23:28:10.000000 summo-0.0.2/pyproject.toml
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-30 23:28:18.217963 summo-0.0.2/setup.cfg
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/src/
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/src/summo/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       34 2023-06-30 17:04:57.000000 summo-0.0.2/src/summo/__init__.py
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      611 2023-06-30 18:08:00.000000 summo-0.0.2/src/summo/summary.py
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/src/summo.egg-info/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      417 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      261 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/SOURCES.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/dependency_links.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       34 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/requires.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        6 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/top_level.txt
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/tests/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1233 2023-06-30 18:09:22.000000 summo-0.0.2/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 17:54:31.000000 summo-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 17:54:40.330558 summo-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 17:54:31.000000 summo-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-03 17:54:31.000000 summo-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:54:40.330558 summo-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.326558 summo-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/src/summo/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 17:54:31.000000 summo-0.0.3/src/summo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 17:54:31.000000 summo-0.0.3/src/summo/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/src/summo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-03 17:54:31.000000 summo-0.0.3/tests/test_summary.py
```

### Comparing `summo-0.0.2/LICENSE` & `summo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `summo-0.0.2/tests/test_summary.py` & `summo-0.0.3/tests/test_summary.py`

 * *Files identical despite different names*


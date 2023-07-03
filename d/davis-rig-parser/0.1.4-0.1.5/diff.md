# Comparing `tmp/davis_rig_parser-0.1.4.tar.gz` & `tmp/davis_rig_parser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/davis_rig_parser-0.1.4.tar", last modified: Sat Jul  1 20:57:00 2023, max compression
+gzip compressed data, was "dist/davis_rig_parser-0.1.5.tar", last modified: Mon Jul  3 16:07:48 2023, max compression
```

## Comparing `davis_rig_parser-0.1.4.tar` & `davis_rig_parser-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5451 2023-06-28 21:25:04.000000 davis_rig_parser-0.1.4/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.4/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18214 2023-06-28 21:45:24.000000 davis_rig_parser-0.1.4/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-01 20:55:25.000000 davis_rig_parser-0.1.4/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-01 20:57:00.000000 davis_rig_parser-0.1.4/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      303 2023-06-30 21:50:47.000000 davis_rig_parser-0.1.4/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5451 2023-07-03 16:07:20.000000 davis_rig_parser-0.1.5/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.5/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18214 2023-06-28 21:45:24.000000 davis_rig_parser-0.1.5/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-03 16:07:05.000000 davis_rig_parser-0.1.5/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      302 2023-07-01 22:08:21.000000 davis_rig_parser-0.1.5/tests/test.py
```

### Comparing `davis_rig_parser-0.1.4/README.md` & `davis_rig_parser-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `davis_rig_parser-0.1.4/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.1.5/davis_rig_parser/davis_rig_parser.py`

 * *Files identical despite different names*


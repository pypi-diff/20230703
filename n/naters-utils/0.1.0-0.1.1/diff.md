# Comparing `tmp/naters-utils-0.1.0.tar.gz` & `tmp/naters-utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naters-utils-0.1.0.tar", last modified: Sun Jul  2 21:42:09 2023, max compression
+gzip compressed data, was "naters-utils-0.1.1.tar", last modified: Mon Jul  3 02:13:26 2023, max compression
```

## Comparing `naters-utils-0.1.0.tar` & `naters-utils-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:42:09.392170 naters-utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-02 21:41:58.000000 naters-utils-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    40757 2023-07-02 21:42:09.392170 naters-utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-02 21:41:58.000000 naters-utils-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-02 21:41:58.000000 naters-utils-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 21:42:09.392170 naters-utils-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:42:09.388170 naters-utils-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:42:09.388170 naters-utils-0.1.0/src/naters-utils/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-02 21:41:58.000000 naters-utils-0.1.0/src/naters-utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 21:41:58.000000 naters-utils-0.1.0/src/naters-utils/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:42:09.392170 naters-utils-0.1.0/src/naters_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40757 2023-07-02 21:42:09.000000 naters-utils-0.1.0/src/naters_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-02 21:42:09.000000 naters-utils-0.1.0/src/naters_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:42:09.000000 naters-utils-0.1.0/src/naters_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 21:42:09.000000 naters-utils-0.1.0/src/naters_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 21:42:09.000000 naters-utils-0.1.0/src/naters_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:13:26.380592 naters-utils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 02:13:16.000000 naters-utils-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 02:13:26.380592 naters-utils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 02:13:16.000000 naters-utils-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 02:13:16.000000 naters-utils-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:13:26.380592 naters-utils-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:13:26.376592 naters-utils-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:13:26.376592 naters-utils-0.1.1/src/naters_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 02:13:16.000000 naters-utils-0.1.1/src/naters_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 02:13:16.000000 naters-utils-0.1.1/src/naters_utils/_hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-03 02:13:16.000000 naters-utils-0.1.1/src/naters_utils/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:13:26.376592 naters-utils-0.1.1/src/naters_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40928 2023-07-03 02:13:26.000000 naters-utils-0.1.1/src/naters_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-03 02:13:26.000000 naters-utils-0.1.1/src/naters_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:13:26.000000 naters-utils-0.1.1/src/naters_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 02:13:26.000000 naters-utils-0.1.1/src/naters_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 02:13:26.000000 naters-utils-0.1.1/src/naters_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:13:26.380592 naters-utils-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 02:13:16.000000 naters-utils-0.1.1/tests/test_func_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-03 02:13:16.000000 naters-utils-0.1.1/tests/test_thread_wrap.py
```

### Comparing `naters-utils-0.1.0/LICENSE.txt` & `naters-utils-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naters-utils-0.1.0/PKG-INFO` & `naters-utils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naters-utils
-Version: 0.1.0
+Version: 0.1.1
 Author-email: Nater0214 <gamer@nater0214.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -677,8 +677,11 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# 
+# Nater's Utils
+Various things I have made that I find useful and want to share
+
+Not much else to say honestly. Your code editor should tell you everything you need to know.
```

### Comparing `naters-utils-0.1.0/src/naters_utils.egg-info/PKG-INFO` & `naters-utils-0.1.1/src/naters_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naters-utils
-Version: 0.1.0
+Version: 0.1.1
 Author-email: Nater0214 <gamer@nater0214.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -677,8 +677,11 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# 
+# Nater's Utils
+Various things I have made that I find useful and want to share
+
+Not much else to say honestly. Your code editor should tell you everything you need to know.
```


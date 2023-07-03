# Comparing `tmp/Exam2excel_converter-0.0.1.tar.gz` & `tmp/Exam2excel_converter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Exam2excel_converter-0.0.1.tar", last modified: Fri Jun 30 02:59:03 2023, max compression
+gzip compressed data, was "Exam2excel_converter-0.0.2.tar", last modified: Mon Jul  3 06:56:55 2023, max compression
```

## Comparing `Exam2excel_converter-0.0.1.tar` & `Exam2excel_converter-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:59:03.792825 Exam2excel_converter-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-30 02:58:51.000000 Exam2excel_converter-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-30 02:59:03.792825 Exam2excel_converter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-30 02:58:51.000000 Exam2excel_converter-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-30 02:58:51.000000 Exam2excel_converter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 02:59:03.792825 Exam2excel_converter-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:59:03.792825 Exam2excel_converter-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:59:03.792825 Exam2excel_converter-0.0.1/src/Exam2excel_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-30 02:59:03.000000 Exam2excel_converter-0.0.1/src/Exam2excel_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-30 02:59:03.000000 Exam2excel_converter-0.0.1/src/Exam2excel_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 02:59:03.000000 Exam2excel_converter-0.0.1/src/Exam2excel_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 02:59:03.000000 Exam2excel_converter-0.0.1/src/Exam2excel_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 02:58:51.000000 Exam2excel_converter-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-30 02:58:51.000000 Exam2excel_converter-0.0.1/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-30 02:58:51.000000 Exam2excel_converter-0.0.1/src/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:56:55.929810 Exam2excel_converter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 06:56:43.000000 Exam2excel_converter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 06:56:55.929810 Exam2excel_converter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 06:56:43.000000 Exam2excel_converter-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 06:56:43.000000 Exam2excel_converter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 06:56:55.929810 Exam2excel_converter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:56:55.925810 Exam2excel_converter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:56:55.929810 Exam2excel_converter-0.0.2/src/Exam2excel_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 06:56:55.000000 Exam2excel_converter-0.0.2/src/Exam2excel_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-03 06:56:55.000000 Exam2excel_converter-0.0.2/src/Exam2excel_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:56:55.000000 Exam2excel_converter-0.0.2/src/Exam2excel_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 06:56:55.000000 Exam2excel_converter-0.0.2/src/Exam2excel_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:56:43.000000 Exam2excel_converter-0.0.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-03 06:56:43.000000 Exam2excel_converter-0.0.2/src/exam2excel_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 06:56:43.000000 Exam2excel_converter-0.0.2/src/test.py
```

### Comparing `Exam2excel_converter-0.0.1/LICENSE` & `Exam2excel_converter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Exam2excel_converter-0.0.1/PKG-INFO` & `Exam2excel_converter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exam2excel_converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool convert question of exam to excel
 Author-email: akakshuki <le.dinhhoang.1207@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `Exam2excel_converter-0.0.1/src/Exam2excel_converter.egg-info/PKG-INFO` & `Exam2excel_converter-0.0.2/src/Exam2excel_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exam2excel-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool convert question of exam to excel
 Author-email: akakshuki <le.dinhhoang.1207@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `Exam2excel_converter-0.0.1/src/main.py` & `Exam2excel_converter-0.0.2/src/exam2excel_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse
+
 import re
 import sys
 import pandas as pd
 from openpyxl import Workbook
 
 # Class object question
 class Question:
```

### Comparing `Exam2excel_converter-0.0.1/src/test.py` & `Exam2excel_converter-0.0.2/src/test.py`

 * *Files identical despite different names*


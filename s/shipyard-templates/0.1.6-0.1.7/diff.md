# Comparing `tmp/shipyard_templates-0.1.6.tar.gz` & `tmp/shipyard_templates-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.1.6.tar", max compression
+gzip compressed data, was "shipyard_templates-0.1.7.tar", max compression
```

## Comparing `shipyard_templates-0.1.6.tar` & `shipyard_templates-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.1.6/README.md
--rw-r--r--   0        0        0      342 2023-06-21 19:54:52.519126 shipyard_templates-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      420 2023-06-21 19:54:18.753024 shipyard_templates-0.1.6/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      552 2023-05-12 18:48:21.819618 shipyard_templates-0.1.6/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0     1965 2023-05-12 18:48:21.819681 shipyard_templates-0.1.6/shipyard_templates/database.py
--rw-r--r--   0        0        0      267 2023-05-12 18:48:21.819750 shipyard_templates-0.1.6/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     1103 2023-06-21 19:54:18.753455 shipyard_templates-0.1.6/shipyard_templates/etl.py
--rw-r--r--   0        0        0      179 2023-06-21 19:54:18.753791 shipyard_templates-0.1.6/shipyard_templates/exit_code_exception.py
--rw-r--r--   0        0        0      245 2023-06-13 18:40:24.030409 shipyard_templates-0.1.6/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      235 2023-05-12 18:48:21.819939 shipyard_templates-0.1.6/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      993 2023-06-06 18:57:29.881235 shipyard_templates-0.1.6/shipyard_templates/projectmanagement.py
--rw-r--r--   0        0        0      543 2023-05-23 01:46:27.306492 shipyard_templates-0.1.6/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      280 2023-05-12 18:48:21.820063 shipyard_templates-0.1.6/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.1.7/README.md
+-rw-r--r--   0        0        0      342 2023-07-03 14:05:58.552677 shipyard_templates-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-06-21 19:54:18.753024 shipyard_templates-0.1.7/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      552 2023-06-22 02:02:44.823645 shipyard_templates-0.1.7/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0     1965 2023-06-22 02:02:44.823946 shipyard_templates-0.1.7/shipyard_templates/database.py
+-rw-r--r--   0        0        0      267 2023-05-12 18:48:21.819750 shipyard_templates-0.1.7/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     1150 2023-07-03 14:05:58.553249 shipyard_templates-0.1.7/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      179 2023-06-22 02:02:44.825164 shipyard_templates-0.1.7/shipyard_templates/exit_code_exception.py
+-rw-r--r--   0        0        0      245 2023-06-13 18:40:24.030409 shipyard_templates-0.1.7/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      235 2023-05-12 18:48:21.819939 shipyard_templates-0.1.7/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      993 2023-06-06 18:57:29.881235 shipyard_templates-0.1.7/shipyard_templates/projectmanagement.py
+-rw-r--r--   0        0        0      543 2023-06-22 02:02:44.825706 shipyard_templates-0.1.7/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      280 2023-06-22 02:02:44.825962 shipyard_templates-0.1.7/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.7/PKG-INFO
```

### Comparing `shipyard_templates-0.1.6/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.1.7/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.6/shipyard_templates/database.py` & `shipyard_templates-0.1.7/shipyard_templates/database.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.6/shipyard_templates/etl.py` & `shipyard_templates-0.1.7/shipyard_templates/etl.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     EXIT_CODE_FINAL_STATUS_COMPLETED = 0
     EXIT_CODE_INVALID_CREDENTIALS = 200
     EXIT_CODE_BAD_REQUEST = 201
     # trigger sync exit codes
     EXIT_CODE_SYNC_REFRESH_ERROR = 202
     EXIT_CODE_SYNC_ALREADY_RUNNING = 203
     EXIT_CODE_SYNC_INVALID_SOURCE_ID = 204
+    EXIT_CODE_SYNC_INVALID_POKE_INTERVAL = 205
     EXIT_CODE_SYNC_CHECK_ERROR = 220
     # verify status exit codes
     EXIT_CODE_FINAL_STATUS_INCOMPLETE = 210
     EXIT_CODE_FINAL_STATUS_ERRORED = 211
     EXIT_CODE_FINAL_STATUS_INVALID = 212
     EXIT_CODE_FINAL_STATUS_CANCELLED = 213
     EXIT_CODE_FINAL_STATUS_PENDING = 214
```

### Comparing `shipyard_templates-0.1.6/shipyard_templates/projectmanagement.py` & `shipyard_templates-0.1.7/shipyard_templates/projectmanagement.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.6/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.1.7/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.6/PKG-INFO` & `shipyard_templates-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-templates
-Version: 0.1.6
+Version: 0.1.7
 Summary: Super classes for blueprint development
 License: Apache-2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/FeishuBitableAPI-3.0.5.tar.gz` & `tmp/FeishuBitableAPI-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeishuBitableAPI-3.0.5.tar", last modified: Mon Jul  3 03:41:11 2023, max compression
+gzip compressed data, was "FeishuBitableAPI-3.1.0.tar", last modified: Mon Jul  3 04:45:49 2023, max compression
```

## Comparing `FeishuBitableAPI-3.0.5.tar` & `FeishuBitableAPI-3.1.0.tar`

### file list

```diff
@@ -1,15 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:41:11.875377 FeishuBitableAPI-3.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:41:11.875377 FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 03:41:11.000000 FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-03 03:41:11.000000 FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:41:11.000000 FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 03:41:11.000000 FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:41:11.000000 FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 03:40:55.000000 FeishuBitableAPI-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 03:41:11.875377 FeishuBitableAPI-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 03:40:55.000000 FeishuBitableAPI-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:41:11.875377 FeishuBitableAPI-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 03:40:55.000000 FeishuBitableAPI-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:41:11.875377 FeishuBitableAPI-3.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 03:40:55.000000 FeishuBitableAPI-3.0.5/test/test#GET_INFO_FROM_URL-2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 03:40:55.000000 FeishuBitableAPI-3.0.5/test/test#GET_INFO_FROM_URL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:45:49.225695 FeishuBitableAPI-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/ADD_RECORDS_FROM_CSV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/BUILD_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/CHECK_FIELD_EXIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/CREATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/CREATE_TABLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/CREATE_TABLE_QUICK.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/DELETE_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/DELETE_FIELDS_DEFAULT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/DELETE_RECORD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:45:49.221695 FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 04:45:49.000000 FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 04:45:49.000000 FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:45:49.000000 FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 04:45:49.000000 FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 04:45:49.000000 FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/FeishuBitableAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/GET_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/LIST_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/LIST_RECORDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/LIST_TABLES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/LIST_VIEWS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 04:45:49.225695 FeishuBitableAPI-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/REFRESH_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/UPDATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/UPDATE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/WRITE_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 04:45:49.225695 FeishuBitableAPI-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:45:49.225695 FeishuBitableAPI-3.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/test/test#GET_INFO_FROM_URL-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 04:45:35.000000 FeishuBitableAPI-3.1.0/test/test#GET_INFO_FROM_URL.py
```

### Comparing `FeishuBitableAPI-3.0.5/FeishuBitableAPI.egg-info/PKG-INFO` & `FeishuBitableAPI-3.1.0/FeishuBitableAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.0.5
+Version: 3.1.0
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.0.5/LICENSE` & `FeishuBitableAPI-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.0.5/PKG-INFO` & `FeishuBitableAPI-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.0.5
+Version: 3.1.0
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.0.5/README.md` & `FeishuBitableAPI-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.0.5/test/test#GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.1.0/test/test#GET_INFO_FROM_URL.py`

 * *Files identical despite different names*


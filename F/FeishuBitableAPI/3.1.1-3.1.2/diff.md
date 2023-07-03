# Comparing `tmp/FeishuBitableAPI-3.1.1.tar.gz` & `tmp/FeishuBitableAPI-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeishuBitableAPI-3.1.1.tar", last modified: Mon Jul  3 05:01:28 2023, max compression
+gzip compressed data, was "FeishuBitableAPI-3.1.2.tar", last modified: Mon Jul  3 05:15:53 2023, max compression
```

## Comparing `FeishuBitableAPI-3.1.1.tar` & `FeishuBitableAPI-3.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:01:28.258392 FeishuBitableAPI-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:01:28.258392 FeishuBitableAPI-3.1.1/FeishuBitableAPI/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/BUILD_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/CHECK_FIELD_EXIST.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/CREATE_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/CREATE_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/CREATE_TABLE_QUICK.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/DELETE_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/DELETE_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/FeishuBitableAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_FIELD_INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_INFO_FROM_URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_LOGIN_CODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_RECORD_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_TABLE_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_VIEW_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_RECORDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_TABLES.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_VIEWS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/UPDATE_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/UPDATE_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_FIELD_INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_INFO_FROM_URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_LOGIN_CODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_RECORD_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_TABLE_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_VIEW_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 05:01:21.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:01:28.258392 FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 05:01:28.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-03 05:01:28.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 05:01:28.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 05:01:28.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 05:01:28.000000 FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 05:01:14.000000 FeishuBitableAPI-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 05:01:28.258392 FeishuBitableAPI-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 05:01:14.000000 FeishuBitableAPI-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 05:01:28.258392 FeishuBitableAPI-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 05:01:14.000000 FeishuBitableAPI-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:01:28.258392 FeishuBitableAPI-3.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 05:01:14.000000 FeishuBitableAPI-3.1.1/test/test#GET_INFO_FROM_URL-2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 05:01:14.000000 FeishuBitableAPI-3.1.1/test/test#GET_INFO_FROM_URL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:15:53.221138 FeishuBitableAPI-3.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:15:53.221138 FeishuBitableAPI-3.1.2/FeishuBitableAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/BUILD_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/CHECK_FIELD_EXIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/CREATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/CREATE_TABLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/CREATE_TABLE_QUICK.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/DELETE_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/DELETE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/FeishuBitableAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_RECORDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_TABLES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_VIEWS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/UPDATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/UPDATE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 05:15:45.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:15:53.221138 FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 05:15:53.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-03 05:15:53.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 05:15:53.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 05:15:53.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 05:15:53.000000 FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 05:15:38.000000 FeishuBitableAPI-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 05:15:53.221138 FeishuBitableAPI-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 05:15:38.000000 FeishuBitableAPI-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 05:15:53.221138 FeishuBitableAPI-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 05:15:38.000000 FeishuBitableAPI-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:15:53.221138 FeishuBitableAPI-3.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 05:15:38.000000 FeishuBitableAPI-3.1.2/test/test#GET_INFO_FROM_URL-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 05:15:38.000000 FeishuBitableAPI-3.1.2/test/test#GET_INFO_FROM_URL.py
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import configparser
 import json
-from BUILD_FIELD import BUILD_FIELD
-from CHECK_FIELD_EXIST import CHECK_FIELD_EXIST
+from .BUILD_FIELD import BUILD_FIELD
+from .CHECK_FIELD_EXIST import CHECK_FIELD_EXIST
 
 def ADD_RECORDS_FROM_CSV(app_token=None, table_id=None, view_id=None, page_token=None, page_size=None, csv_file=None, config_file=None, field_file=None):
     if config_file is None:
         config_file = 'feishu-config.ini'
     if field_file is None:
         field_file = 'feishu-field.ini'
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/BUILD_FIELD.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/BUILD_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/CHECK_FIELD_EXIST.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/CHECK_FIELD_EXIST.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import configparser
 import pandas as pd
 import argparse
-from LIST_FIELDS import LIST_FIELDS
-from CREATE_FIELD import CREATE_FIELD
+from .LIST_FIELDS import LIST_FIELDS
+from .CREATE_FIELD import CREATE_FIELD
 
 def CHECK_FIELD_EXIST(app_token=None, table_id=None, view_id=None, page_token=None, page_size=None, csv_file=None, config_file=None):
     if config_file is None:
         config_file = 'feishu-config.ini'
 
     config = configparser.ConfigParser()
     config.read(config_file, encoding='utf-8')
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/CREATE_FIELD.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/CREATE_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/CREATE_TABLE.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/CREATE_TABLE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/CREATE_TABLE_QUICK.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/CREATE_TABLE_QUICK.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/DELETE_FIELDS.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/DELETE_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import argparse
-from DELETE_FIELDS import DELETE_FIELD
-from DELETE_RECORD import DELETE_RECORD
+from .DELETE_FIELDS import DELETE_FIELD
+from .DELETE_RECORD import DELETE_RECORD
 from GET_FIELD_INFO import GET_FIELD_ID
-from LIST_RECORDS import LIST_RECORDS
+from .LIST_RECORDS import LIST_RECORDS
 
 # 默认要删除的字段列表
 DEFAULT_FIELDS_TO_DELETE = ["单选", "多选", "群组", "日期", "附件", "人员"]
 
 def DELETE_EMPTY_RECORDS(app_token, table_id):
     page_token = None
     while True:
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/DELETE_RECORD.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/DELETE_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/FeishuBitableAPI.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/FeishuBitableAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from GET_APP_ACCESS_TOKEN import GET_APP_ACCESS_TOKEN
-from GET_FIELD_INFO import GET_FIELD_INFO, GET_FIELD_ID, GET_FIELD_NAME
-from GET_INFO_FROM_URL import GET_INFO_FROM_URL,GET_INFO_FROM_URL_JSON,GET_APPTOKEN_FROM_URL,GET_TABLEID_FROM_URL,GET_VIEWID_FROM_URL
-from GET_LOGIN_CODE import GET_LOGIN_CODE
-from GET_RECORD_ID import GET_RECORD_ID
-from GET_RECORD import GET_RECORD
-from GET_TABLE_ID import GET_TABLE_ID
-from GET_USER_ACCESS_TOKEN import GET_USER_ACCESS_TOKEN
-from GET_VIEW_ID import GET_VIEW_ID
-
-from LIST_FIELDS import LIST_FIELDS
-from LIST_RECORDS import LIST_RECORDS
-from LIST_TABLES import LIST_TABLES
-from LIST_VIEWS import LIST_VIEWS
-
-from REFRESH_USER_ACCESS_TOKEN import REFRESH_USER_ACCESS_TOKEN
-
-from WRITE_APP_ACCESS_TOKEN import WRITE_APP_ACCESS_TOKEN
-from WRITE_FIELD_INFO import WRITE_FIELD_INFO
-from WRITE_INFO_FROM_URL import WRITE_INFO_FROM_URL
-from WRITE_LOGIN_CODE import WRITE_LOGIN_CODE
-from WRITE_RECORD_ID import WRITE_RECORD_ID
-from WRITE_TABLE_ID import WRITE_TABLE_ID
-from WRITE_VIEW_ID import WRITE_VIEW_ID
-
-from CREATE_FIELD import CREATE_FIELD
-from CREATE_TABLE import CREATE_TABLE
-
-from CHECK_FIELD_EXIST import CHECK_FIELD_EXIST
-
-from DELETE_FIELDS import DELETE_FIELD
-from DELETE_RECORD import DELETE_RECORD
+from .GET_APP_ACCESS_TOKEN import GET_APP_ACCESS_TOKEN
+from .GET_FIELD_INFO import GET_FIELD_INFO, GET_FIELD_ID, GET_FIELD_NAME
+from .GET_INFO_FROM_URL import GET_INFO_FROM_URL, GET_INFO_FROM_URL_JSON, GET_APPTOKEN_FROM_URL, GET_TABLEID_FROM_URL, GET_VIEWID_FROM_URL
+from .GET_LOGIN_CODE import GET_LOGIN_CODE
+from .GET_RECORD_ID import GET_RECORD_ID
+from .GET_RECORD import GET_RECORD
+from .GET_TABLE_ID import GET_TABLE_ID
+from .GET_USER_ACCESS_TOKEN import GET_USER_ACCESS_TOKEN
+from .GET_VIEW_ID import GET_VIEW_ID
+
+from .LIST_FIELDS import LIST_FIELDS
+from .LIST_RECORDS import LIST_RECORDS
+from .LIST_TABLES import LIST_TABLES
+from .LIST_VIEWS import LIST_VIEWS
+
+from .REFRESH_USER_ACCESS_TOKEN import REFRESH_USER_ACCESS_TOKEN
+
+from .WRITE_APP_ACCESS_TOKEN import WRITE_APP_ACCESS_TOKEN
+from .WRITE_FIELD_INFO import WRITE_FIELD_INFO
+from .WRITE_INFO_FROM_URL import WRITE_INFO_FROM_URL
+from .WRITE_LOGIN_CODE import WRITE_LOGIN_CODE
+from .WRITE_RECORD_ID import WRITE_RECORD_ID
+from .WRITE_TABLE_ID import WRITE_TABLE_ID
+from .WRITE_VIEW_ID import WRITE_VIEW_ID
+
+from .CREATE_FIELD import CREATE_FIELD
+from .CREATE_TABLE import CREATE_TABLE
+
+from .CHECK_FIELD_EXIST import CHECK_FIELD_EXIST
+
+from .DELETE_FIELDS import DELETE_FIELD
+from .DELETE_RECORD import DELETE_RECORD
 
-from BUILD_FIELD import BUILD_FIELD
+from .BUILD_FIELD import BUILD_FIELD
 
-from UPDATE_FIELD import UPDATE_FIELD
-from UPDATE_RECORD import UPDATE_RECORD
+from .UPDATE_FIELD import UPDATE_FIELD
+from .UPDATE_RECORD import UPDATE_RECORD
 
-from ADD_RECORDS_FROM_CSV import ADD_RECORDS_FROM_CSV
+from .ADD_RECORDS_FROM_CSV import ADD_RECORDS_FROM_CSV
 
 
 class FeishuBitableAPI:
     def __init__(self):
         pass
 
     # 调用 ping 函数进行验证
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_FIELD_INFO.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_FIELD_INFO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import configparser
 import json
-from LIST_FIELDS import LIST_FIELDS
+from .LIST_FIELDS import LIST_FIELDS
 
 # 使用字段名称获取字段ID
 def GET_FIELD_ID(field_name, app_token=None, table_id=None, view_id=None, page_token=None, page_size=None, config_file=None):
     if config_file is None:
         config_file = "feishu-config.ini"
 
     config = configparser.ConfigParser()
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_INFO_FROM_URL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_LOGIN_CODE.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_LOGIN_CODE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_RECORD.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_RECORD_ID.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_RECORD_ID.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import configparser
-from LIST_RECORDS import LIST_RECORDS
+from .LIST_RECORDS import LIST_RECORDS
 
 # 从给定的响应中获取具有特定字段值的记录的ID
 def GET_RECORD_ID(field_value, field_name=None, config_file=None):
     if config_file is None:
         config_file = 'feishu-config.ini'
 
     config = configparser.ConfigParser()
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_TABLE_ID.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_TABLE_ID.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import configparser
 import argparse
-from LIST_TABLES import LIST_TABLES
+from .LIST_TABLES import LIST_TABLES
 
 # 检索字段
 # 此函数用于通过给定的名称获取表的ID
 def GET_TABLE_ID(name="数据表", app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
     if config_file is None:
         config_file = 'feishu-config.ini'
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/GET_VIEW_ID.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/GET_VIEW_ID.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import configparser
-from LIST_VIEWS import LIST_VIEWS
+from .LIST_VIEWS import LIST_VIEWS
 
 # 检索视图
 # 此函数用于通过给定的名称获取视图的ID
 def GET_VIEW_ID(view_name="默认视图", app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
     if config_file is None or not config_file.strip():  # 如果未提供配置文件路径，则使用默认的配置文件 'feishu-config.ini'
         config_file = 'feishu-config.ini'
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_FIELDS.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_RECORDS.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_RECORDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_TABLES.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_TABLES.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/LIST_VIEWS.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/LIST_VIEWS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/UPDATE_FIELD.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/UPDATE_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/UPDATE_RECORD.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/UPDATE_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import configparser
-from GET_APP_ACCESS_TOKEN import GET_APP_ACCESS_TOKEN
+from .GET_APP_ACCESS_TOKEN import GET_APP_ACCESS_TOKEN
 import argparse
 
 def WRITE_APP_ACCESS_TOKEN(app_id=None, app_secret=None, config_file=None):
     config = configparser.ConfigParser()  # 创建一个ConfigParser对象
     if config_file:
         config.read(config_file, encoding='utf-8')  # 读取指定的配置文件
     else:
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_FIELD_INFO.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_FIELD_INFO.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_INFO_FROM_URL.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_INFO_FROM_URL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_LOGIN_CODE.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_LOGIN_CODE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_RECORD_ID.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_RECORD_ID.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import configparser
 import argparse
-from GET_RECORD_ID import GET_RECORD_ID
+from .GET_RECORD_ID import GET_RECORD_ID
 
 # 此函数用于将从GET_RECORD_ID获取的record_id写入到配置文件
 def WRITE_RECORD_ID(value, field_name=None, config_file=None):
     if config_file is None:
         config_file = 'feishu-config.ini'
 
     config = configparser.ConfigParser()  # 创建一个ConfigParser对象
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_TABLE_ID.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_TABLE_ID.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import configparser
-from GET_TABLE_ID import GET_TABLE_ID
+from .GET_TABLE_ID import GET_TABLE_ID
 
 # 检索字段并写入配置文件
 # 这个函数用于将从 GET_TABLE_ID 获取的 table_id 写入到配置文件
 def WRITE_TABLE_ID(name, app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
     config = configparser.ConfigParser()  # 创建一个 ConfigParser 对象
     config.read(config_file, encoding='utf-8')  # 读取配置文件
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/WRITE_VIEW_ID.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/WRITE_VIEW_ID.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import configparser
-from GET_VIEW_ID import GET_VIEW_ID
+from .GET_VIEW_ID import GET_VIEW_ID
 
 # 检索视图并写入配置文件
 # 这个函数用于将从GET_VIEW_ID获取的view_id写入到配置文件
 def WRITE_VIEW_ID(view_name, app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
     if config_file is None or not config_file.strip():  # 如果未提供配置文件路径，则使用默认的配置文件 'feishu-config.ini'
         config_file = 'feishu-config.ini'
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI/setup.py` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.1.1',
+    version='3.1.2',
     packages=find_packages(),
     #py_modules=[],
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/PKG-INFO` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.1.1
+Version: 3.1.2
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.1.1/FeishuBitableAPI.egg-info/SOURCES.txt` & `FeishuBitableAPI-3.1.2/FeishuBitableAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/LICENSE` & `FeishuBitableAPI-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/PKG-INFO` & `FeishuBitableAPI-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.1.1
+Version: 3.1.2
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.1.1/README.md` & `FeishuBitableAPI-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.1/setup.py` & `FeishuBitableAPI-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.1.1',
+    version='3.1.2',
     packages=find_packages(),
     #py_modules=[],
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

### Comparing `FeishuBitableAPI-3.1.1/test/test#GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.1.2/test/test#GET_INFO_FROM_URL.py`

 * *Files identical despite different names*


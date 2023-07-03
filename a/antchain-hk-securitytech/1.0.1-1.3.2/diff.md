# Comparing `tmp/antchain_hk_securitytech-1.0.1.tar.gz` & `tmp/antchain_hk_securitytech-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_hk_securitytech-1.0.1.tar", last modified: Fri May 26 06:43:41 2023, max compression
+gzip compressed data, was "dist/antchain_hk_securitytech-1.3.2.tar", last modified: Mon Jul  3 09:22:54 2023, max compression
```

## Comparing `antchain_hk_securitytech-1.0.1.tar` & `antchain_hk_securitytech-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:43:41.000000 antchain_hk_securitytech-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2234 2023-05-26 06:43:41.000000 antchain_hk_securitytech-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      840 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:43:41.000000 antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2234 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-26 06:43:41.000000 antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:43:41.000000 antchain_hk_securitytech-1.0.1/antchain_sdk_hk_securitytech/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_sdk_hk_securitytech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15196 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_sdk_hk_securitytech/client.py
--rw-r--r--   0 root         (0) root         (0)    12130 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/antchain_sdk_hk_securitytech/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 06:43:41.000000 antchain_hk_securitytech-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2550 2023-05-26 06:43:40.000000 antchain_hk_securitytech-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26858 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/client.py
+-rw-r--r--   0 root         (0) root         (0)    42759 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/setup.py
```

### Comparing `antchain_hk_securitytech-1.0.1/LICENSE` & `antchain_hk_securitytech-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.0.1/PKG-INFO` & `antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_hk_securitytech
-Version: 1.0.1
+Name: antchain-hk-securitytech
+Version: 1.3.2
 Summary: Ant Chain HK_SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_hk_securitytech-1.0.1/README-CN.md` & `antchain_hk_securitytech-1.3.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.0.1/README.md` & `antchain_hk_securitytech-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.0.1/antchain_hk_securitytech.egg-info/PKG-INFO` & `antchain_hk_securitytech-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-hk-securitytech
-Version: 1.0.1
+Name: antchain_hk_securitytech
+Version: 1.3.2
 Summary: Ant Chain HK_SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_hk_securitytech-1.0.1/setup.py` & `antchain_hk_securitytech-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_hk_securitytech.
 
-Created on 26/05/2023
+Created on 03/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_hk_securitytech"
 NAME = "antchain_hk_securitytech" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain HK_SECURITYTECH SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```


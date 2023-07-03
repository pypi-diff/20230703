# Comparing `tmp/cloudboss_cloudlib-1.0.1.tar.gz` & `tmp/cloudboss_cloudlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudboss_cloudlib-1.0.1.tar", max compression
+gzip compressed data, was "cloudboss_cloudlib-1.0.2.tar", max compression
```

## Comparing `cloudboss_cloudlib-1.0.1.tar` & `cloudboss_cloudlib-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       13 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/__init__.py
--rw-r--r--   0        0        0     2534 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/account_utils.py
--rw-r--r--   0        0        0       41 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/constants.py
--rw-r--r--   0        0        0      185 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/datetime_helpers.py
--rw-r--r--   0        0        0       98 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/exceptions.py
--rw-r--r--   0        0        0      633 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/logging.py
--rw-r--r--   0        0        0      322 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/metadata.py
--rw-r--r--   0        0        0      341 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/package_management.py
--rw-r--r--   0        0        0      435 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/roles.py
--rw-r--r--   0        0        0      896 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/cloudlib/secrets.py
--rw-r--r--   0        0        0      472 2023-05-16 16:08:54.709381 cloudboss_cloudlib-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 cloudboss_cloudlib-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/__init__.py
+-rw-r--r--   0        0        0     2569 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/account_utils.py
+-rw-r--r--   0        0        0       41 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/constants.py
+-rw-r--r--   0        0        0      185 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/datetime_helpers.py
+-rw-r--r--   0        0        0       98 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/exceptions.py
+-rw-r--r--   0        0        0      633 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/logging.py
+-rw-r--r--   0        0        0      322 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/metadata.py
+-rw-r--r--   0        0        0      341 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/package_management.py
+-rw-r--r--   0        0        0      435 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/roles.py
+-rw-r--r--   0        0        0      896 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/cloudlib/secrets.py
+-rw-r--r--   0        0        0      472 2023-07-03 16:13:59.837620 cloudboss_cloudlib-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 cloudboss_cloudlib-1.0.2/PKG-INFO
```

### Comparing `cloudboss_cloudlib-1.0.1/cloudlib/account_utils.py` & `cloudboss_cloudlib-1.0.2/cloudlib/account_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import logging
 
 import boto3
+from botocore.config import Config
 from botocore.exceptions import ClientError
 
 from cloudlib.constants import LIST_ACCOUNT_ROLE
 from cloudlib.exceptions import MissingResourceException
 from cloudlib.roles import assume_role
 
 logger = logging.getLogger(__name__)
```

### Comparing `cloudboss_cloudlib-1.0.1/cloudlib/logging.py` & `cloudboss_cloudlib-1.0.2/cloudlib/logging.py`

 * *Files identical despite different names*

### Comparing `cloudboss_cloudlib-1.0.1/cloudlib/secrets.py` & `cloudboss_cloudlib-1.0.2/cloudlib/secrets.py`

 * *Files identical despite different names*


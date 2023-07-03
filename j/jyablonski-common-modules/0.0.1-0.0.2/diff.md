# Comparing `tmp/jyablonski_common_modules-0.0.1.tar.gz` & `tmp/jyablonski_common_modules-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jyablonski_common_modules-0.0.1.tar", max compression
+gzip compressed data, was "jyablonski_common_modules-0.0.2.tar", max compression
```

## Comparing `jyablonski_common_modules-0.0.1.tar` & `jyablonski_common_modules-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,16 @@
--rw-r--r--   0        0        0        0 2023-07-01 23:31:10.116284 jyablonski_common_modules-0.0.1/jyablonski_common_modules/__init__.py
--rw-r--r--   0        0        0      276 2023-07-02 19:08:12.382326 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/__init__.py
--rw-r--r--   0        0        0      500 2023-07-02 21:38:07.293036 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      358 2023-07-02 21:38:07.293036 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0        0        0     1061 2023-07-02 21:46:00.195869 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/__pycache__/s3.cpython-39.pyc
--rw-r--r--   0        0        0      820 2023-07-02 21:56:30.828935 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/__pycache__/secrets_manager.cpython-39.pyc
--rw-r--r--   0        0        0     1032 2023-07-02 22:01:24.053704 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/__pycache__/ssm.cpython-39.pyc
--rw-r--r--   0        0        0       49 2023-07-02 19:08:12.382326 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/exceptions.py
--rw-r--r--   0        0        0      887 2023-07-02 21:45:56.879906 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/s3.py
--rw-r--r--   0        0        0      560 2023-07-02 21:56:29.192953 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/secrets_manager.py
--rw-r--r--   0        0        0      784 2023-07-02 21:57:44.296126 jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/ssm.py
--rw-r--r--   0        0        0      218 2023-07-02 22:07:42.289533 jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/__init__.py
--rw-r--r--   0        0        0      383 2023-07-02 22:02:06.013241 jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      703 2023-07-02 19:06:54.443204 jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/__pycache__/core.cpython-39.pyc
--rw-r--r--   0        0        0      873 2023-07-02 22:04:36.047587 jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/__pycache__/feature_flags.cpython-39.pyc
--rw-r--r--   0        0        0      465 2023-07-02 18:49:11.431174 jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/core.py
--rw-r--r--   0        0        0      542 2023-07-02 22:07:42.297533 jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/feature_flags.py
--rw-r--r--   0        0        0       22 2023-07-02 19:08:12.382326 jyablonski_common_modules-0.0.1/jyablonski_common_modules/logging/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-02 19:08:12.398326 jyablonski_common_modules-0.0.1/jyablonski_common_modules/logging/logger.py
--rw-r--r--   0        0        0      146 2023-07-02 19:08:12.382326 jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/__init__.py
--rw-r--r--   0        0        0      226 2023-07-02 21:07:33.659946 jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1237 2023-07-02 21:18:47.185059 jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/__pycache__/connection.cpython-39.pyc
--rw-r--r--   0        0        0     4598 2023-07-02 21:34:08.743617 jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/__pycache__/writers.cpython-39.pyc
--rw-r--r--   0        0        0     1152 2023-07-02 21:18:01.185485 jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/connection.py
--rw-r--r--   0        0        0     5352 2023-07-02 21:34:07.339632 jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/writers.py
--rw-r--r--   0        0        0      775 2023-07-02 21:37:43.717292 jyablonski_common_modules-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 jyablonski_common_modules-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/exceptions.py
+-rw-r--r--   0        0        0      887 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/s3.py
+-rw-r--r--   0        0        0      560 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/secrets_manager.py
+-rw-r--r--   0        0        0      784 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/ssm.py
+-rw-r--r--   0        0        0      218 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/__init__.py
+-rw-r--r--   0        0        0      465 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/core.py
+-rw-r--r--   0        0        0      542 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/feature_flags.py
+-rw-r--r--   0        0        0       22 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/logging/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/logging/logger.py
+-rw-r--r--   0        0        0      146 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/__init__.py
+-rw-r--r--   0        0        0     1152 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/connection.py
+-rw-r--r--   0        0        0     5352 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/writers.py
+-rw-r--r--   0        0        0      775 2023-07-03 00:54:19.399967 jyablonski_common_modules-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 jyablonski_common_modules-0.0.2/PKG-INFO
```

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/s3.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/s3.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/secrets_manager.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/aws/ssm.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/general/feature_flags.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/general/feature_flags.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/logging/logger.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/logging/logger.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/connection.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/connection.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/jyablonski_common_modules/sql/writers.py` & `jyablonski_common_modules-0.0.2/jyablonski_common_modules/sql/writers.py`

 * *Files identical despite different names*

### Comparing `jyablonski_common_modules-0.0.1/pyproject.toml` & `jyablonski_common_modules-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jyablonski_common_modules"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["jyablonski9 <jyablonski9@gmail.com>"]
 maintainers = ["jyablonski9 <jyablonski9@gmail.com>"]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `jyablonski_common_modules-0.0.1/PKG-INFO` & `jyablonski_common_modules-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyablonski-common-modules
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: jyablonski9
 Author-email: jyablonski9@gmail.com
 Maintainer: jyablonski9
 Maintainer-email: jyablonski9@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```


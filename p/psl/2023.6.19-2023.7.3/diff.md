# Comparing `tmp/psl-2023.6.19.tar.gz` & `tmp/psl-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.6.19.tar", last modified: Mon Jun 19 13:06:30 2023, max compression
+gzip compressed data, was "psl-2023.7.3.tar", last modified: Mon Jul  3 13:09:44 2023, max compression
```

## Comparing `psl-2023.6.19.tar` & `psl-2023.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:06:30.439833 psl-2023.6.19/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-19 13:05:57.000000 psl-2023.6.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 13:05:57.000000 psl-2023.6.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 13:06:30.439833 psl-2023.6.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-19 13:05:57.000000 psl-2023.6.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:06:30.439833 psl-2023.6.19/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-19 13:06:05.000000 psl-2023.6.19/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   109723 2023-06-19 13:06:05.000000 psl-2023.6.19/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:05:57.000000 psl-2023.6.19/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:06:30.439833 psl-2023.6.19/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:06:18.000000 psl-2023.6.19/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 13:06:30.000000 psl-2023.6.19/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:06:30.439833 psl-2023.6.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-19 13:05:57.000000 psl-2023.6.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:44.307404 psl-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-03 13:09:02.000000 psl-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 13:09:02.000000 psl-2023.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 13:09:44.307404 psl-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-03 13:09:02.000000 psl-2023.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:44.303404 psl-2023.7.3/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-03 13:09:14.000000 psl-2023.7.3/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   111024 2023-07-03 13:09:14.000000 psl-2023.7.3/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:02.000000 psl-2023.7.3/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:44.307404 psl-2023.7.3/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:09:30.000000 psl-2023.7.3/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:09:44.307404 psl-2023.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 13:09:02.000000 psl-2023.7.3/setup.py
```

### Comparing `psl-2023.6.19/LICENSE` & `psl-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.6.19/PKG-INFO` & `psl-2023.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.6.19
+Version: 2023.7.3
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.6.19/README.md` & `psl-2023.7.3/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.6.19/psl/__init__.py` & `psl-2023.7.3/psl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.6.19"
-__checksum__ = "e59b87a5d8e71edb2dee3d57fc35c9a6a5fb3806"
+__version__ = "2023.7.3"
+__checksum__ = "c6a23cf216230ba3c1b9863f7a89d9529ea6f702"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.6.19/psl/psl.txt` & `psl-2023.7.3/psl/psl.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6997,54 +6997,80 @@
 s3-website-us-west-1.amazonaws.com
 s3-website-us-west-2.amazonaws.com
 s3.dualstack.sa-east-1.amazonaws.com
 s3.dualstack.us-east-1.amazonaws.com
 s3.dualstack.us-east-2.amazonaws.com
 s3.us-east-2.amazonaws.com
 s3-website.us-east-2.amazonaws.com
+analytics-gateway.ap-northeast-1.amazonaws.com
+analytics-gateway.eu-west-1.amazonaws.com
+analytics-gateway.us-east-1.amazonaws.com
+analytics-gateway.us-east-2.amazonaws.com
+analytics-gateway.us-west-2.amazonaws.com
+webview-assets.aws-cloud9.af-south-1.amazonaws.com
 vfs.cloud9.af-south-1.amazonaws.com
 webview-assets.cloud9.af-south-1.amazonaws.com
+webview-assets.aws-cloud9.ap-east-1.amazonaws.com
 vfs.cloud9.ap-east-1.amazonaws.com
 webview-assets.cloud9.ap-east-1.amazonaws.com
+webview-assets.aws-cloud9.ap-northeast-1.amazonaws.com
 vfs.cloud9.ap-northeast-1.amazonaws.com
 webview-assets.cloud9.ap-northeast-1.amazonaws.com
+webview-assets.aws-cloud9.ap-northeast-2.amazonaws.com
 vfs.cloud9.ap-northeast-2.amazonaws.com
 webview-assets.cloud9.ap-northeast-2.amazonaws.com
+webview-assets.aws-cloud9.ap-northeast-3.amazonaws.com
 vfs.cloud9.ap-northeast-3.amazonaws.com
 webview-assets.cloud9.ap-northeast-3.amazonaws.com
+webview-assets.aws-cloud9.ap-south-1.amazonaws.com
 vfs.cloud9.ap-south-1.amazonaws.com
 webview-assets.cloud9.ap-south-1.amazonaws.com
+webview-assets.aws-cloud9.ap-southeast-1.amazonaws.com
 vfs.cloud9.ap-southeast-1.amazonaws.com
 webview-assets.cloud9.ap-southeast-1.amazonaws.com
+webview-assets.aws-cloud9.ap-southeast-2.amazonaws.com
 vfs.cloud9.ap-southeast-2.amazonaws.com
 webview-assets.cloud9.ap-southeast-2.amazonaws.com
+webview-assets.aws-cloud9.ca-central-1.amazonaws.com
 vfs.cloud9.ca-central-1.amazonaws.com
 webview-assets.cloud9.ca-central-1.amazonaws.com
+webview-assets.aws-cloud9.eu-central-1.amazonaws.com
 vfs.cloud9.eu-central-1.amazonaws.com
 webview-assets.cloud9.eu-central-1.amazonaws.com
+webview-assets.aws-cloud9.eu-north-1.amazonaws.com
 vfs.cloud9.eu-north-1.amazonaws.com
 webview-assets.cloud9.eu-north-1.amazonaws.com
+webview-assets.aws-cloud9.eu-south-1.amazonaws.com
 vfs.cloud9.eu-south-1.amazonaws.com
 webview-assets.cloud9.eu-south-1.amazonaws.com
+webview-assets.aws-cloud9.eu-west-1.amazonaws.com
 vfs.cloud9.eu-west-1.amazonaws.com
 webview-assets.cloud9.eu-west-1.amazonaws.com
+webview-assets.aws-cloud9.eu-west-2.amazonaws.com
 vfs.cloud9.eu-west-2.amazonaws.com
 webview-assets.cloud9.eu-west-2.amazonaws.com
+webview-assets.aws-cloud9.eu-west-3.amazonaws.com
 vfs.cloud9.eu-west-3.amazonaws.com
 webview-assets.cloud9.eu-west-3.amazonaws.com
+webview-assets.aws-cloud9.me-south-1.amazonaws.com
 vfs.cloud9.me-south-1.amazonaws.com
 webview-assets.cloud9.me-south-1.amazonaws.com
+webview-assets.aws-cloud9.sa-east-1.amazonaws.com
 vfs.cloud9.sa-east-1.amazonaws.com
 webview-assets.cloud9.sa-east-1.amazonaws.com
+webview-assets.aws-cloud9.us-east-1.amazonaws.com
 vfs.cloud9.us-east-1.amazonaws.com
 webview-assets.cloud9.us-east-1.amazonaws.com
+webview-assets.aws-cloud9.us-east-2.amazonaws.com
 vfs.cloud9.us-east-2.amazonaws.com
 webview-assets.cloud9.us-east-2.amazonaws.com
+webview-assets.aws-cloud9.us-west-1.amazonaws.com
 vfs.cloud9.us-west-1.amazonaws.com
 webview-assets.cloud9.us-west-1.amazonaws.com
+webview-assets.aws-cloud9.us-west-2.amazonaws.com
 vfs.cloud9.us-west-2.amazonaws.com
 webview-assets.cloud9.us-west-2.amazonaws.com
 cn-north-1.eb.amazonaws.com.cn
 cn-northwest-1.eb.amazonaws.com.cn
 elasticbeanstalk.com
 ap-northeast-1.elasticbeanstalk.com
 ap-northeast-2.elasticbeanstalk.com
```

### Comparing `psl-2023.6.19/psl.egg-info/PKG-INFO` & `psl-2023.7.3/psl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.6.19
+Version: 2023.7.3
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.6.19/setup.py` & `psl-2023.7.3/setup.py`

 * *Files identical despite different names*


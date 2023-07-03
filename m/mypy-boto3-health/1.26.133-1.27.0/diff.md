# Comparing `tmp/mypy-boto3-health-1.26.133.tar.gz` & `tmp/mypy-boto3-health-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-health-1.26.133.tar", last modified: Thu May 11 19:32:34 2023, max compression
+gzip compressed data, was "mypy-boto3-health-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-health-1.26.133.tar` & `mypy-boto3-health-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/mypy_boto3_health/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-05-11 19:32:12.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.303355 mypy-boto3-health-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-03 19:50:50.295355 mypy-boto3-health-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.295355 mypy-boto3-health-1.27.0/mypy_boto3_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-07-03 19:38:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-07-03 19:38:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.295355 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.303355 mypy-boto3-health-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/setup.py
```

### Comparing `mypy-boto3-health-1.26.133/LICENSE` & `mypy-boto3-health-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/PKG-INFO` & `mypy-boto3-health-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.26.133
-Summary: Type annotations for boto3.Health 1.26.133 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Health 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-health-1.26.133/README.md` & `mypy-boto3-health-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.py` & `mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.pyi` & `mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/__main__.py` & `mypy-boto3-health-1.27.0/mypy_boto3_health/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Health 1.26.133\nVersion:         1.26.133\nBuilder version:"
+        "Type annotations for boto3.Health 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.133")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/client.py` & `mypy-boto3-health-1.27.0/mypy_boto3_health/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/client.pyi` & `mypy-boto3-health-1.27.0/mypy_boto3_health/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/literals.py` & `mypy-boto3-health-1.27.0/mypy_boto3_health/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -115,14 +116,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -264,14 +266,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -293,14 +296,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -384,14 +389,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/literals.pyi` & `mypy-boto3-health-1.27.0/mypy_boto3_health/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -113,14 +114,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -262,14 +264,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -291,14 +294,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -382,14 +387,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.py` & `mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.pyi` & `mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.py` & `mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.pyi` & `mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/PKG-INFO` & `mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.26.133
-Summary: Type annotations for boto3.Health 1.26.133 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Health 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/SOURCES.txt` & `mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.133/setup.py` & `mypy-boto3-health-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-health",
-    version="1.26.133",
+    version="1.27.0",
     packages=["mypy_boto3_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Health 1.26.133 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Health 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


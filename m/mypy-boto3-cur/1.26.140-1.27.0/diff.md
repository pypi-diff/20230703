# Comparing `tmp/mypy-boto3-cur-1.26.140.tar.gz` & `tmp/mypy-boto3-cur-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cur-1.26.140.tar", last modified: Wed May 24 20:47:52 2023, max compression
+gzip compressed data, was "mypy-boto3-cur-1.27.0.tar", last modified: Mon Jul  3 19:50:36 2023, max compression
```

## Comparing `mypy-boto3-cur-1.26.140.tar` & `mypy-boto3-cur-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/mypy_boto3_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.683073 mypy-boto3-cur-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-03 19:50:36.683073 mypy-boto3-cur-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.683073 mypy-boto3-cur-1.27.0/mypy_boto3_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.683073 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-03 19:50:36.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:36.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:36.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:36.000000 mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:36.683073 mypy-boto3-cur-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-03 19:35:09.000000 mypy-boto3-cur-1.27.0/setup.py
```

### Comparing `mypy-boto3-cur-1.26.140/LICENSE` & `mypy-boto3-cur-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/PKG-INFO` & `mypy-boto3-cur-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.26.140
-Summary: Type annotations for boto3.CostandUsageReportService 1.26.140 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CostandUsageReportService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.26.140](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cur-1.26.140/README.md` & `mypy-boto3-cur-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.26.140](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.py` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.pyi` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/__main__.py` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostandUsageReportService 1.26.140\nVersion:        "
-        " 1.26.140\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CostandUsageReportService 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.140")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.py` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.pyi` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.py` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -31,15 +30,14 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
@@ -85,14 +83,15 @@
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
@@ -132,14 +131,15 @@
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
@@ -311,14 +311,16 @@
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
@@ -402,14 +404,15 @@
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

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.pyi` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -30,14 +31,15 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
@@ -83,14 +85,15 @@
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
@@ -130,14 +133,15 @@
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
@@ -309,14 +313,16 @@
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
@@ -400,14 +406,15 @@
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

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.py` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.pyi` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.py` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.pyi` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/PKG-INFO` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.26.140
-Summary: Type annotations for boto3.CostandUsageReportService 1.26.140 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CostandUsageReportService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.26.140](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/SOURCES.txt` & `mypy-boto3-cur-1.27.0/mypy_boto3_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.140/setup.py` & `mypy-boto3-cur-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cur",
-    version="1.26.140",
+    version="1.27.0",
     packages=["mypy_boto3_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostandUsageReportService 1.26.140 service generated with"
+        "Type annotations for boto3.CostandUsageReportService 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


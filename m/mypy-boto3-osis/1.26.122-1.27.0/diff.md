# Comparing `tmp/mypy-boto3-osis-1.26.122.tar.gz` & `tmp/mypy-boto3-osis-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.26.122.tar", last modified: Thu Apr 27 19:33:42 2023, max compression
+gzip compressed data, was "mypy-boto3-osis-1.27.0.tar", last modified: Mon Jul  3 19:51:13 2023, max compression
```

## Comparing `mypy-boto3-osis-1.26.122.tar` & `mypy-boto3-osis-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/mypy_boto3_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-27 19:33:00.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-27 19:33:00.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.095768 mypy-boto3-osis-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-03 19:51:13.091768 mypy-boto3-osis-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.083768 mypy-boto3-osis-1.27.0/mypy_boto3_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-07-03 19:43:14.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-03 19:43:14.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.091768 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-03 19:51:12.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-03 19:51:12.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:12.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:12.000000 mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:13.095768 mypy-boto3-osis-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-03 19:43:13.000000 mypy-boto3-osis-1.27.0/setup.py
```

### Comparing `mypy-boto3-osis-1.26.122/LICENSE` & `mypy-boto3-osis-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.122/PKG-INFO` & `mypy-boto3-osis-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.26.122
-Summary: Type annotations for boto3.OpenSearchIngestion 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.OpenSearchIngestion 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -302,34 +302,34 @@
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
-    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PipelineStatusReasonTypeDef,
+    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
     ChangeProgressStatusTypeDef,
     LogPublishingOptionsTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     VpcEndpointTypeDef,
-    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
```

### Comparing `mypy-boto3-osis-1.26.122/README.md` & `mypy-boto3-osis-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -270,34 +270,34 @@
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
-    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PipelineStatusReasonTypeDef,
+    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
     ChangeProgressStatusTypeDef,
     LogPublishingOptionsTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     VpcEndpointTypeDef,
-    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
```

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/__main__.py` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchIngestion 1.26.122\nVersion:        "
-        " 1.26.122\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpenSearchIngestion 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.122")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.py` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.pyi` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.py` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
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
@@ -103,14 +104,15 @@
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
@@ -252,14 +254,15 @@
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
@@ -281,14 +284,16 @@
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
@@ -372,14 +377,15 @@
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

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.pyi` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -101,14 +102,15 @@
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
@@ -250,14 +252,15 @@
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
@@ -279,14 +282,16 @@
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
@@ -370,14 +375,15 @@
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

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.py` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -22,40 +22,39 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
-    "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PipelineStatusReasonTypeDef",
+    "ResponseMetadataTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
     "ChangeProgressStatusTypeDef",
     "LogPublishingOptionsTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "VpcEndpointTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
@@ -104,30 +103,17 @@
     "_OptionalVpcOptionsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -189,14 +175,25 @@
     "PipelineStatusReasonTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 StartPipelineRequestRequestTypeDef = TypedDict(
     "StartPipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -246,14 +243,22 @@
     {
         "IsLoggingEnabled": bool,
         "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -264,35 +269,27 @@
         "VpcEndpointId": str,
         "VpcId": str,
         "VpcOptions": VpcOptionsTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPipelineBlueprintsResponseTypeDef = TypedDict(
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
@@ -308,23 +305,23 @@
 )
 
 ValidatePipelineResponseTypeDef = TypedDict(
     "ValidatePipelineResponseTypeDef",
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
@@ -339,21 +336,19 @@
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcOptions": VpcOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -363,21 +358,19 @@
         "MaxUnits": int,
         "PipelineConfigurationBody": str,
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
-
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
@@ -394,50 +387,50 @@
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "NextToken": str,
         "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineResponseTypeDef = TypedDict(
     "GetPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartPipelineResponseTypeDef = TypedDict(
     "StartPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopPipelineResponseTypeDef = TypedDict(
     "StopPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.pyi` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,39 +22,40 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
-    "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PipelineStatusReasonTypeDef",
+    "ResponseMetadataTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
     "ChangeProgressStatusTypeDef",
     "LogPublishingOptionsTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "VpcEndpointTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
@@ -103,27 +104,18 @@
     "_OptionalVpcOptionsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
 
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
@@ -186,14 +178,25 @@
     "PipelineStatusReasonTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 StartPipelineRequestRequestTypeDef = TypedDict(
     "StartPipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -243,14 +246,22 @@
     {
         "IsLoggingEnabled": bool,
         "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -261,35 +272,27 @@
         "VpcEndpointId": str,
         "VpcId": str,
         "VpcOptions": VpcOptionsTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPipelineBlueprintsResponseTypeDef = TypedDict(
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
@@ -305,23 +308,23 @@
 )
 
 ValidatePipelineResponseTypeDef = TypedDict(
     "ValidatePipelineResponseTypeDef",
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
@@ -336,19 +339,21 @@
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcOptions": VpcOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -358,19 +363,21 @@
         "MaxUnits": int,
         "PipelineConfigurationBody": str,
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
@@ -387,50 +394,50 @@
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "NextToken": str,
         "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineResponseTypeDef = TypedDict(
     "GetPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartPipelineResponseTypeDef = TypedDict(
     "StartPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopPipelineResponseTypeDef = TypedDict(
     "StopPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/PKG-INFO` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.26.122
-Summary: Type annotations for boto3.OpenSearchIngestion 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.OpenSearchIngestion 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -302,34 +302,34 @@
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
-    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PipelineStatusReasonTypeDef,
+    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
     ChangeProgressStatusTypeDef,
     LogPublishingOptionsTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     VpcEndpointTypeDef,
-    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
```

### Comparing `mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/SOURCES.txt` & `mypy-boto3-osis-1.27.0/mypy_boto3_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.122/setup.py` & `mypy-boto3-osis-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-osis",
-    version="1.26.122",
+    version="1.27.0",
     packages=["mypy_boto3_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchIngestion 1.26.122 service generated with"
+        "Type annotations for boto3.OpenSearchIngestion 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


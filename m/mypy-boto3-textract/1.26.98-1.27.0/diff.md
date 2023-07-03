# Comparing `tmp/mypy-boto3-textract-1.26.98.tar.gz` & `tmp/mypy-boto3-textract-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-textract-1.26.98.tar", last modified: Thu Mar 23 19:33:06 2023, max compression
+gzip compressed data, was "mypy-boto3-textract-1.27.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
```

## Comparing `mypy-boto3-textract-1.26.98.tar` & `mypy-boto3-textract-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.879667 mypy-boto3-textract-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-03-23 19:33:06.879667 mypy-boto3-textract-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.859667 mypy-boto3-textract-1.26.98/mypy_boto3_textract/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22918 2023-03-23 19:32:53.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.859667 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-03-23 19:33:06.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-23 19:33:06.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:06.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-23 19:33:06.000000 mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:06.879667 mypy-boto3-textract-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-23 19:32:52.000000 mypy-boto3-textract-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.448097 mypy-boto3-textract-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-03 19:51:33.448097 mypy-boto3-textract-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.448097 mypy-boto3-textract-1.27.0/mypy_boto3_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-03 19:49:04.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-07-03 19:49:04.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-07-03 19:49:04.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.448097 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-03 19:51:33.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:51:33.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:33.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:33.000000 mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:33.448097 mypy-boto3-textract-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:49:03.000000 mypy-boto3-textract-1.27.0/setup.py
```

### Comparing `mypy-boto3-textract-1.26.98/LICENSE` & `mypy-boto3-textract-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.26.98/PKG-INFO` & `mypy-boto3-textract-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-textract
-Version: 1.26.98
-Summary: Type annotations for boto3.Textract 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Textract 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-textract"></a>
 
 # mypy-boto3-textract
 
 [![PyPI - mypy-boto3-textract](https://img.shields.io/pypi/v/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-textract?color=blue)](https://pypistats.org/packages/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,15 +306,14 @@
 `mypy_boto3_textract.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
-    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
     QueryTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
@@ -329,14 +328,15 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
+    ResponseMetadataTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
     QueriesConfigTypeDef,
     DocumentGroupTypeDef,
```

### Comparing `mypy-boto3-textract-1.26.98/README.md` & `mypy-boto3-textract-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-textract"></a>
 
 # mypy-boto3-textract
 
 [![PyPI - mypy-boto3-textract](https://img.shields.io/pypi/v/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-textract?color=blue)](https://pypistats.org/packages/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,15 +274,14 @@
 `mypy_boto3_textract.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
-    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
     QueryTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
@@ -297,14 +296,15 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
+    ResponseMetadataTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
     QueriesConfigTypeDef,
     DocumentGroupTypeDef,
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/__main__.py` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Textract 1.26.98\nVersion:         1.26.98\nBuilder version:"
-        " 7.14.2\nDocs:           "
+        "Type annotations for boto3.Textract 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.98")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/client.py` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/client.pyi` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/literals.py` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -139,14 +140,15 @@
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
@@ -288,14 +290,15 @@
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
@@ -314,16 +317,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
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
@@ -407,15 +413,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/literals.pyi` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -286,14 +288,15 @@
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
@@ -312,16 +315,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
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
@@ -405,15 +411,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/type_defs.py` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
     "QueryTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
@@ -59,14 +58,15 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
     "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
@@ -123,25 +123,14 @@
         "HumanLoopArn": str,
         "HumanLoopActivationReasons": List[str],
         "HumanLoopActivationConditionsEvaluationResults": str,
     },
     total=False,
 )
 
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
 NormalizedValueTypeDef = TypedDict(
     "NormalizedValueTypeDef",
     {
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
@@ -406,43 +395,54 @@
     {
         "Value": str,
         "Confidence": float,
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
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartDocumentTextDetectionResponseTypeDef = TypedDict(
     "StartDocumentTextDetectionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartExpenseAnalysisResponseTypeDef = TypedDict(
     "StartExpenseAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartLendingAnalysisResponseTypeDef = TypedDict(
     "StartLendingAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAnalyzeIDDetectionsTypeDef = TypedDict(
     "_RequiredAnalyzeIDDetectionsTypeDef",
     {
         "Text": str,
@@ -761,64 +761,64 @@
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnalyzeDocumentResponseTypeDef = TypedDict(
     "AnalyzeDocumentResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectDocumentTextResponseTypeDef = TypedDict(
     "DetectDocumentTextResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentAnalysisResponseTypeDef = TypedDict(
     "GetDocumentAnalysisResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentTextDetectionResponseTypeDef = TypedDict(
     "GetDocumentTextDetectionResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdentityDocumentTypeDef = TypedDict(
     "IdentityDocumentTypeDef",
     {
         "DocumentIndex": int,
@@ -853,15 +853,15 @@
 
 AnalyzeIDResponseTypeDef = TypedDict(
     "AnalyzeIDResponseTypeDef",
     {
         "IdentityDocuments": List[IdentityDocumentTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "AnalyzeIDModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LineItemFieldsTypeDef = TypedDict(
     "LineItemFieldsTypeDef",
     {
         "LineItemExpenseFields": List[ExpenseFieldTypeDef],
@@ -899,15 +899,15 @@
 )
 
 AnalyzeExpenseResponseTypeDef = TypedDict(
     "AnalyzeExpenseResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExtractionTypeDef = TypedDict(
     "ExtractionTypeDef",
     {
         "LendingDocument": LendingDocumentTypeDef,
@@ -923,15 +923,15 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeExpenseModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LendingResultTypeDef = TypedDict(
     "LendingResultTypeDef",
     {
         "Page": int,
@@ -947,10 +947,10 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Results": List[LendingResultTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract/type_defs.pyi` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
     "QueryTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
@@ -58,14 +57,15 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
     "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
@@ -122,25 +122,14 @@
         "HumanLoopArn": str,
         "HumanLoopActivationReasons": List[str],
         "HumanLoopActivationConditionsEvaluationResults": str,
     },
     total=False,
 )
 
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
 NormalizedValueTypeDef = TypedDict(
     "NormalizedValueTypeDef",
     {
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
@@ -393,43 +382,54 @@
     {
         "Value": str,
         "Confidence": float,
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
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartDocumentTextDetectionResponseTypeDef = TypedDict(
     "StartDocumentTextDetectionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartExpenseAnalysisResponseTypeDef = TypedDict(
     "StartExpenseAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartLendingAnalysisResponseTypeDef = TypedDict(
     "StartLendingAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAnalyzeIDDetectionsTypeDef = TypedDict(
     "_RequiredAnalyzeIDDetectionsTypeDef",
     {
         "Text": str,
@@ -734,64 +734,64 @@
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnalyzeDocumentResponseTypeDef = TypedDict(
     "AnalyzeDocumentResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectDocumentTextResponseTypeDef = TypedDict(
     "DetectDocumentTextResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentAnalysisResponseTypeDef = TypedDict(
     "GetDocumentAnalysisResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentTextDetectionResponseTypeDef = TypedDict(
     "GetDocumentTextDetectionResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdentityDocumentTypeDef = TypedDict(
     "IdentityDocumentTypeDef",
     {
         "DocumentIndex": int,
@@ -826,15 +826,15 @@
 
 AnalyzeIDResponseTypeDef = TypedDict(
     "AnalyzeIDResponseTypeDef",
     {
         "IdentityDocuments": List[IdentityDocumentTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "AnalyzeIDModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LineItemFieldsTypeDef = TypedDict(
     "LineItemFieldsTypeDef",
     {
         "LineItemExpenseFields": List[ExpenseFieldTypeDef],
@@ -872,15 +872,15 @@
 )
 
 AnalyzeExpenseResponseTypeDef = TypedDict(
     "AnalyzeExpenseResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExtractionTypeDef = TypedDict(
     "ExtractionTypeDef",
     {
         "LendingDocument": LendingDocumentTypeDef,
@@ -896,15 +896,15 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeExpenseModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LendingResultTypeDef = TypedDict(
     "LendingResultTypeDef",
     {
         "Page": int,
@@ -920,10 +920,10 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Results": List[LendingResultTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/PKG-INFO` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-textract
-Version: 1.26.98
-Summary: Type annotations for boto3.Textract 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Textract 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-textract"></a>
 
 # mypy-boto3-textract
 
 [![PyPI - mypy-boto3-textract](https://img.shields.io/pypi/v/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-textract?color=blue)](https://pypistats.org/packages/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,15 +306,14 @@
 `mypy_boto3_textract.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
-    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
     QueryTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
@@ -329,14 +328,15 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
+    ResponseMetadataTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
     QueriesConfigTypeDef,
     DocumentGroupTypeDef,
```

### Comparing `mypy-boto3-textract-1.26.98/mypy_boto3_textract.egg-info/SOURCES.txt` & `mypy-boto3-textract-1.27.0/mypy_boto3_textract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.26.98/setup.py` & `mypy-boto3-textract-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-textract",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_textract"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Textract 1.26.98 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.Textract 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


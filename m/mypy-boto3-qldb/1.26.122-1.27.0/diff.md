# Comparing `tmp/mypy-boto3-qldb-1.26.122.tar.gz` & `tmp/mypy-boto3-qldb-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-1.26.122.tar", last modified: Thu Apr 27 19:33:42 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-1.27.0.tar", last modified: Mon Jul  3 19:51:17 2023, max compression
```

## Comparing `mypy-boto3-qldb-1.26.122.tar` & `mypy-boto3-qldb-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-04-27 19:33:02.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.203836 mypy-boto3-qldb-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-07-03 19:51:17.203836 mypy-boto3-qldb-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.199836 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-03 19:43:54.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-03 19:43:54.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-07-03 19:43:54.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-03 19:43:54.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17762 2023-07-03 19:43:54.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.203836 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-07-03 19:51:17.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-03 19:51:17.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:17.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:17.000000 mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:17.203836 mypy-boto3-qldb-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 19:43:53.000000 mypy-boto3-qldb-1.27.0/setup.py
```

### Comparing `mypy-boto3-qldb-1.26.122/LICENSE` & `mypy-boto3-qldb-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.122/PKG-INFO` & `mypy-boto3-qldb-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.26.122
-Summary: Type annotations for boto3.QLDB 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.QLDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -304,42 +304,42 @@
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerRequestRequestTypeDef,
+    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3EncryptionConfigurationTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
-    CreateLedgerResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
+    UpdateLedgerRequestRequestTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
```

### Comparing `mypy-boto3-qldb-1.26.122/README.md` & `mypy-boto3-qldb-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -272,42 +272,42 @@
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerRequestRequestTypeDef,
+    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3EncryptionConfigurationTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
-    CreateLedgerResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
+    UpdateLedgerRequestRequestTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
```

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__main__.py` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDB 1.26.122\nVersion:         1.26.122\nBuilder version:"
+        "Type annotations for boto3.QLDB 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.py` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.pyi` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.py` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -102,14 +103,15 @@
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
@@ -251,14 +253,15 @@
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
@@ -280,14 +283,16 @@
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
@@ -371,14 +376,15 @@
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

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.pyi` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
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
@@ -100,14 +101,15 @@
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
@@ -249,14 +251,15 @@
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
@@ -278,14 +281,16 @@
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
@@ -369,14 +374,15 @@
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

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.py` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,45 +27,44 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJournalKinesisStreamResponseTypeDef",
     "CreateLedgerRequestRequestTypeDef",
+    "CreateLedgerResponseTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportJournalToS3ResponseTypeDef",
     "ValueHolderTypeDef",
     "GetDigestRequestRequestTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3EncryptionConfigurationTypeDef",
+    "StreamJournalToKinesisResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
-    "UpdateLedgerRequestRequestTypeDef",
-    "CancelJournalKinesisStreamResponseTypeDef",
-    "CreateLedgerResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportJournalToS3ResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StreamJournalToKinesisResponseTypeDef",
     "UpdateLedgerPermissionsModeResponseTypeDef",
+    "UpdateLedgerRequestRequestTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
     "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
@@ -86,22 +85,19 @@
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     {
         "LedgerName": str,
         "StreamId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJournalKinesisStreamResponseTypeDef = TypedDict(
+    "CancelJournalKinesisStreamResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "StreamId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLedgerRequestRequestTypeDef",
     {
         "Name": str,
@@ -114,20 +110,32 @@
         "Tags": Mapping[str, str],
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
-
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
+CreateLedgerResponseTypeDef = TypedDict(
+    "CreateLedgerResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "State": LedgerStateType,
+        "CreationDateTime": datetime,
+        "PermissionsMode": PermissionsModeType,
+        "DeletionProtection": bool,
+        "KmsKeyArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -166,20 +174,33 @@
     "_OptionalLedgerEncryptionDescriptionTypeDef",
     {
         "InaccessibleKmsKeyDateTime": datetime,
     },
     total=False,
 )
 
-
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ExportJournalToS3ResponseTypeDef = TypedDict(
+    "ExportJournalToS3ResponseTypeDef",
+    {
+        "ExportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
@@ -202,21 +223,19 @@
     "_OptionalKinesisConfigurationTypeDef",
     {
         "AggregationEnabled": bool,
     },
     total=False,
 )
 
-
 class KinesisConfigurationTypeDef(
     _RequiredKinesisConfigurationTypeDef, _OptionalKinesisConfigurationTypeDef
 ):
     pass
 
-
 LedgerSummaryTypeDef = TypedDict(
     "LedgerSummaryTypeDef",
     {
         "Name": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
     },
@@ -234,22 +253,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJournalKinesisStreamsForLedgerRequestRequestTypeDef(
     _RequiredListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     _OptionalListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
@@ -257,22 +274,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJournalS3ExportsForLedgerRequestRequestTypeDef(
     _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef,
     _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef,
 ):
     pass
 
-
 ListJournalS3ExportsRequestRequestTypeDef = TypedDict(
     "ListJournalS3ExportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -290,34 +305,59 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
     "_OptionalS3EncryptionConfigurationTypeDef",
     {
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
+StreamJournalToKinesisResponseTypeDef = TypedDict(
+    "StreamJournalToKinesisResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
@@ -335,14 +375,24 @@
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionsMode": PermissionsModeType,
     },
 )
 
+UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
+    "UpdateLedgerPermissionsModeResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "PermissionsMode": PermissionsModeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateLedgerRequestRequestTypeDef = TypedDict(
@@ -350,108 +400,43 @@
     {
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
-
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
-
-CancelJournalKinesisStreamResponseTypeDef = TypedDict(
-    "CancelJournalKinesisStreamResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLedgerResponseTypeDef = TypedDict(
-    "CreateLedgerResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "State": LedgerStateType,
-        "CreationDateTime": datetime,
-        "PermissionsMode": PermissionsModeType,
-        "DeletionProtection": bool,
-        "KmsKeyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportJournalToS3ResponseTypeDef = TypedDict(
-    "ExportJournalToS3ResponseTypeDef",
-    {
-        "ExportId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StreamJournalToKinesisResponseTypeDef = TypedDict(
-    "StreamJournalToKinesisResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
-    "UpdateLedgerPermissionsModeResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "PermissionsMode": PermissionsModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeLedgerResponseTypeDef = TypedDict(
     "DescribeLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "PermissionsMode": PermissionsModeType,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLedgerResponseTypeDef = TypedDict(
     "UpdateLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlockRequestRequestTypeDef",
     {
         "Name": str,
@@ -462,36 +447,34 @@
     "_OptionalGetBlockRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
-
 class GetBlockRequestRequestTypeDef(
     _RequiredGetBlockRequestRequestTypeDef, _OptionalGetBlockRequestRequestTypeDef
 ):
     pass
 
-
 GetBlockResponseTypeDef = TypedDict(
     "GetBlockResponseTypeDef",
     {
         "Block": ValueHolderTypeDef,
         "Proof": ValueHolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDigestResponseTypeDef = TypedDict(
     "GetDigestResponseTypeDef",
     {
         "Digest": bytes,
         "DigestTipAddress": ValueHolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
@@ -503,27 +486,25 @@
     "_OptionalGetRevisionRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
-
 class GetRevisionRequestRequestTypeDef(
     _RequiredGetRevisionRequestRequestTypeDef, _OptionalGetRevisionRequestRequestTypeDef
 ):
     pass
 
-
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
         "Proof": ValueHolderTypeDef,
         "Revision": ValueHolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
@@ -542,21 +523,19 @@
         "ExclusiveEndTime": datetime,
         "Arn": str,
         "ErrorCause": ErrorCauseType,
     },
     total=False,
 )
 
-
 class JournalKinesisStreamDescriptionTypeDef(
     _RequiredJournalKinesisStreamDescriptionTypeDef, _OptionalJournalKinesisStreamDescriptionTypeDef
 ):
     pass
 
-
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "InclusiveStartTime": Union[datetime, str],
         "KinesisConfiguration": KinesisConfigurationTypeDef,
@@ -568,28 +547,26 @@
     {
         "Tags": Mapping[str, str],
         "ExclusiveEndTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
     _OptionalStreamJournalToKinesisRequestRequestTypeDef,
 ):
     pass
 
-
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
@@ -598,24 +575,24 @@
     },
 )
 
 DescribeJournalKinesisStreamResponseTypeDef = TypedDict(
     "DescribeJournalKinesisStreamResponseTypeDef",
     {
         "Stream": JournalKinesisStreamDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJournalKinesisStreamsForLedgerResponseTypeDef = TypedDict(
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
         "Name": str,
@@ -629,21 +606,19 @@
     "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-
 class ExportJournalToS3RequestRequestTypeDef(
     _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
 ):
     pass
 
-
 _RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
     "_RequiredJournalS3ExportDescriptionTypeDef",
     {
         "LedgerName": str,
         "ExportId": str,
         "ExportCreationTime": datetime,
         "Status": ExportStatusType,
@@ -657,39 +632,37 @@
     "_OptionalJournalS3ExportDescriptionTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-
 class JournalS3ExportDescriptionTypeDef(
     _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
 ):
     pass
 
-
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJournalS3ExportsForLedgerResponseTypeDef = TypedDict(
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJournalS3ExportsResponseTypeDef = TypedDict(
     "ListJournalS3ExportsResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.pyi` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,44 +27,45 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJournalKinesisStreamResponseTypeDef",
     "CreateLedgerRequestRequestTypeDef",
+    "CreateLedgerResponseTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportJournalToS3ResponseTypeDef",
     "ValueHolderTypeDef",
     "GetDigestRequestRequestTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3EncryptionConfigurationTypeDef",
+    "StreamJournalToKinesisResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
-    "UpdateLedgerRequestRequestTypeDef",
-    "CancelJournalKinesisStreamResponseTypeDef",
-    "CreateLedgerResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportJournalToS3ResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StreamJournalToKinesisResponseTypeDef",
     "UpdateLedgerPermissionsModeResponseTypeDef",
+    "UpdateLedgerRequestRequestTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
     "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
@@ -85,22 +86,19 @@
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     {
         "LedgerName": str,
         "StreamId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJournalKinesisStreamResponseTypeDef = TypedDict(
+    "CancelJournalKinesisStreamResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "StreamId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLedgerRequestRequestTypeDef",
     {
         "Name": str,
@@ -113,19 +111,35 @@
         "Tags": Mapping[str, str],
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
+
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
+
+CreateLedgerResponseTypeDef = TypedDict(
+    "CreateLedgerResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "State": LedgerStateType,
+        "CreationDateTime": datetime,
+        "PermissionsMode": PermissionsModeType,
+        "DeletionProtection": bool,
+        "KmsKeyArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -163,19 +177,36 @@
     "_OptionalLedgerEncryptionDescriptionTypeDef",
     {
         "InaccessibleKmsKeyDateTime": datetime,
     },
     total=False,
 )
 
+
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ExportJournalToS3ResponseTypeDef = TypedDict(
+    "ExportJournalToS3ResponseTypeDef",
+    {
+        "ExportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
@@ -197,19 +228,21 @@
     "_OptionalKinesisConfigurationTypeDef",
     {
         "AggregationEnabled": bool,
     },
     total=False,
 )
 
+
 class KinesisConfigurationTypeDef(
     _RequiredKinesisConfigurationTypeDef, _OptionalKinesisConfigurationTypeDef
 ):
     pass
 
+
 LedgerSummaryTypeDef = TypedDict(
     "LedgerSummaryTypeDef",
     {
         "Name": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
     },
@@ -227,20 +260,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJournalKinesisStreamsForLedgerRequestRequestTypeDef(
     _RequiredListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     _OptionalListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
@@ -248,20 +283,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJournalS3ExportsForLedgerRequestRequestTypeDef(
     _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef,
     _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef,
 ):
     pass
 
+
 ListJournalS3ExportsRequestRequestTypeDef = TypedDict(
     "ListJournalS3ExportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -279,33 +316,62 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
     "_OptionalS3EncryptionConfigurationTypeDef",
     {
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
+
+StreamJournalToKinesisResponseTypeDef = TypedDict(
+    "StreamJournalToKinesisResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -322,14 +388,24 @@
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionsMode": PermissionsModeType,
     },
 )
 
+UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
+    "UpdateLedgerPermissionsModeResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "PermissionsMode": PermissionsModeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateLedgerRequestRequestTypeDef = TypedDict(
@@ -337,106 +413,45 @@
     {
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
+
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
-CancelJournalKinesisStreamResponseTypeDef = TypedDict(
-    "CancelJournalKinesisStreamResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLedgerResponseTypeDef = TypedDict(
-    "CreateLedgerResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "State": LedgerStateType,
-        "CreationDateTime": datetime,
-        "PermissionsMode": PermissionsModeType,
-        "DeletionProtection": bool,
-        "KmsKeyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportJournalToS3ResponseTypeDef = TypedDict(
-    "ExportJournalToS3ResponseTypeDef",
-    {
-        "ExportId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StreamJournalToKinesisResponseTypeDef = TypedDict(
-    "StreamJournalToKinesisResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
-    "UpdateLedgerPermissionsModeResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "PermissionsMode": PermissionsModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 DescribeLedgerResponseTypeDef = TypedDict(
     "DescribeLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "PermissionsMode": PermissionsModeType,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLedgerResponseTypeDef = TypedDict(
     "UpdateLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlockRequestRequestTypeDef",
     {
         "Name": str,
@@ -447,34 +462,36 @@
     "_OptionalGetBlockRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
+
 class GetBlockRequestRequestTypeDef(
     _RequiredGetBlockRequestRequestTypeDef, _OptionalGetBlockRequestRequestTypeDef
 ):
     pass
 
+
 GetBlockResponseTypeDef = TypedDict(
     "GetBlockResponseTypeDef",
     {
         "Block": ValueHolderTypeDef,
         "Proof": ValueHolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDigestResponseTypeDef = TypedDict(
     "GetDigestResponseTypeDef",
     {
         "Digest": bytes,
         "DigestTipAddress": ValueHolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
@@ -486,25 +503,27 @@
     "_OptionalGetRevisionRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
+
 class GetRevisionRequestRequestTypeDef(
     _RequiredGetRevisionRequestRequestTypeDef, _OptionalGetRevisionRequestRequestTypeDef
 ):
     pass
 
+
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
         "Proof": ValueHolderTypeDef,
         "Revision": ValueHolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
@@ -523,19 +542,21 @@
         "ExclusiveEndTime": datetime,
         "Arn": str,
         "ErrorCause": ErrorCauseType,
     },
     total=False,
 )
 
+
 class JournalKinesisStreamDescriptionTypeDef(
     _RequiredJournalKinesisStreamDescriptionTypeDef, _OptionalJournalKinesisStreamDescriptionTypeDef
 ):
     pass
 
+
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "InclusiveStartTime": Union[datetime, str],
         "KinesisConfiguration": KinesisConfigurationTypeDef,
@@ -547,26 +568,28 @@
     {
         "Tags": Mapping[str, str],
         "ExclusiveEndTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
     _OptionalStreamJournalToKinesisRequestRequestTypeDef,
 ):
     pass
 
+
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
@@ -575,24 +598,24 @@
     },
 )
 
 DescribeJournalKinesisStreamResponseTypeDef = TypedDict(
     "DescribeJournalKinesisStreamResponseTypeDef",
     {
         "Stream": JournalKinesisStreamDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJournalKinesisStreamsForLedgerResponseTypeDef = TypedDict(
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
         "Name": str,
@@ -606,19 +629,21 @@
     "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
+
 class ExportJournalToS3RequestRequestTypeDef(
     _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
 ):
     pass
 
+
 _RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
     "_RequiredJournalS3ExportDescriptionTypeDef",
     {
         "LedgerName": str,
         "ExportId": str,
         "ExportCreationTime": datetime,
         "Status": ExportStatusType,
@@ -632,37 +657,39 @@
     "_OptionalJournalS3ExportDescriptionTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
+
 class JournalS3ExportDescriptionTypeDef(
     _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
 ):
     pass
 
+
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJournalS3ExportsForLedgerResponseTypeDef = TypedDict(
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJournalS3ExportsResponseTypeDef = TypedDict(
     "ListJournalS3ExportsResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/PKG-INFO` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.26.122
-Summary: Type annotations for boto3.QLDB 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.QLDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -304,42 +304,42 @@
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerRequestRequestTypeDef,
+    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3EncryptionConfigurationTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
-    CreateLedgerResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
+    UpdateLedgerRequestRequestTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
```

### Comparing `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/SOURCES.txt` & `mypy-boto3-qldb-1.27.0/mypy_boto3_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.122/setup.py` & `mypy-boto3-qldb-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb",
-    version="1.26.122",
+    version="1.27.0",
     packages=["mypy_boto3_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDB 1.26.122 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.QLDB 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


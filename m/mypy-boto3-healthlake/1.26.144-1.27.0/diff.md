# Comparing `tmp/mypy-boto3-healthlake-1.26.144.tar.gz` & `tmp/mypy-boto3-healthlake-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-healthlake-1.26.144.tar", last modified: Wed May 31 19:48:12 2023, max compression
+gzip compressed data, was "mypy-boto3-healthlake-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-healthlake-1.26.144.tar` & `mypy-boto3-healthlake-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:48:12.432929 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-05-31 19:47:31.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-05-31 19:47:31.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.471360 mypy-boto3-healthlake-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-03 19:50:50.471360 mypy-boto3-healthlake-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.463360 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-03 19:38:51.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-07-03 19:38:51.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.471360 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-03 19:50:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 19:50:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:50.000000 mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.471360 mypy-boto3-healthlake-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:38:50.000000 mypy-boto3-healthlake-1.27.0/setup.py
```

### Comparing `mypy-boto3-healthlake-1.26.144/LICENSE` & `mypy-boto3-healthlake-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.26.144/PKG-INFO` & `mypy-boto3-healthlake-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.26.144
-Summary: Type annotations for boto3.HealthLake 1.26.144 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.HealthLake 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.26.144](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -304,33 +304,33 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.26.144/README.md` & `mypy-boto3-healthlake-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.26.144](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -272,33 +272,33 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__main__.py` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthLake 1.26.144\nVersion:         1.26.144\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.HealthLake 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.144")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.py` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.pyi` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.py` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
@@ -61,14 +59,15 @@
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
@@ -108,14 +107,15 @@
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
@@ -287,14 +287,16 @@
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
@@ -378,14 +380,15 @@
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

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.pyi` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
@@ -59,14 +61,15 @@
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
@@ -106,14 +109,15 @@
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
@@ -285,14 +289,16 @@
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
@@ -376,14 +382,15 @@
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

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.py` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,33 +27,33 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateFHIRDatastoreResponseTypeDef",
     "DatastoreFilterTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
+    "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "KmsEncryptionConfigTypeDef",
     "ListFHIRExportJobsRequestRequestTypeDef",
     "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateFHIRDatastoreResponseTypeDef",
-    "DeleteFHIRDatastoreResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartFHIRExportJobResponseTypeDef",
     "StartFHIRImportJobResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListFHIRDatastoresRequestRequestTypeDef",
     "SseConfigurationTypeDef",
     "OutputDataConfigTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
@@ -101,22 +101,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateFHIRDatastoreResponseTypeDef = TypedDict(
+    "CreateFHIRDatastoreResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatastoreFilterTypeDef = TypedDict(
     "DatastoreFilterTypeDef",
     {
         "DatastoreName": str,
@@ -130,14 +130,25 @@
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
+DeleteFHIRDatastoreResponseTypeDef = TypedDict(
+    "DeleteFHIRDatastoreResponseTypeDef",
+    {
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -251,77 +262,66 @@
     "S3ConfigurationTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartFHIRExportJobResponseTypeDef = TypedDict(
+    "StartFHIRExportJobResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "DatastoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFHIRDatastoreResponseTypeDef = TypedDict(
-    "CreateFHIRDatastoreResponseTypeDef",
+StartFHIRImportJobResponseTypeDef = TypedDict(
+    "StartFHIRImportJobResponseTypeDef",
     {
+        "JobId": str,
+        "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteFHIRDatastoreResponseTypeDef = TypedDict(
-    "DeleteFHIRDatastoreResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartFHIRExportJobResponseTypeDef = TypedDict(
-    "StartFHIRExportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "DatastoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFHIRImportJobResponseTypeDef = TypedDict(
-    "StartFHIRImportJobResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "DatastoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
     "ListFHIRDatastoresRequestRequestTypeDef",
     {
         "Filter": DatastoreFilterTypeDef,
@@ -510,53 +510,53 @@
     pass
 
 
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFHIRDatastoresResponseTypeDef = TypedDict(
     "ListFHIRDatastoresResponseTypeDef",
     {
         "DatastorePropertiesList": List[DatastorePropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFHIRExportJobResponseTypeDef = TypedDict(
     "DescribeFHIRExportJobResponseTypeDef",
     {
         "ExportJobProperties": ExportJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFHIRExportJobsResponseTypeDef = TypedDict(
     "ListFHIRExportJobsResponseTypeDef",
     {
         "ExportJobPropertiesList": List[ExportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFHIRImportJobResponseTypeDef = TypedDict(
     "DescribeFHIRImportJobResponseTypeDef",
     {
         "ImportJobProperties": ImportJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFHIRImportJobsResponseTypeDef = TypedDict(
     "ListFHIRImportJobsResponseTypeDef",
     {
         "ImportJobPropertiesList": List[ImportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.pyi` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -26,33 +26,33 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateFHIRDatastoreResponseTypeDef",
     "DatastoreFilterTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
+    "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "KmsEncryptionConfigTypeDef",
     "ListFHIRExportJobsRequestRequestTypeDef",
     "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateFHIRDatastoreResponseTypeDef",
-    "DeleteFHIRDatastoreResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartFHIRExportJobResponseTypeDef",
     "StartFHIRImportJobResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListFHIRDatastoresRequestRequestTypeDef",
     "SseConfigurationTypeDef",
     "OutputDataConfigTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
@@ -98,22 +98,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateFHIRDatastoreResponseTypeDef = TypedDict(
+    "CreateFHIRDatastoreResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatastoreFilterTypeDef = TypedDict(
     "DatastoreFilterTypeDef",
     {
         "DatastoreName": str,
@@ -127,14 +127,25 @@
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
+DeleteFHIRDatastoreResponseTypeDef = TypedDict(
+    "DeleteFHIRDatastoreResponseTypeDef",
+    {
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -242,77 +253,66 @@
     "S3ConfigurationTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartFHIRExportJobResponseTypeDef = TypedDict(
+    "StartFHIRExportJobResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "DatastoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFHIRDatastoreResponseTypeDef = TypedDict(
-    "CreateFHIRDatastoreResponseTypeDef",
+StartFHIRImportJobResponseTypeDef = TypedDict(
+    "StartFHIRImportJobResponseTypeDef",
     {
+        "JobId": str,
+        "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteFHIRDatastoreResponseTypeDef = TypedDict(
-    "DeleteFHIRDatastoreResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartFHIRExportJobResponseTypeDef = TypedDict(
-    "StartFHIRExportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "DatastoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFHIRImportJobResponseTypeDef = TypedDict(
-    "StartFHIRImportJobResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "DatastoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
     "ListFHIRDatastoresRequestRequestTypeDef",
     {
         "Filter": DatastoreFilterTypeDef,
@@ -489,53 +489,53 @@
 ):
     pass
 
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFHIRDatastoresResponseTypeDef = TypedDict(
     "ListFHIRDatastoresResponseTypeDef",
     {
         "DatastorePropertiesList": List[DatastorePropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFHIRExportJobResponseTypeDef = TypedDict(
     "DescribeFHIRExportJobResponseTypeDef",
     {
         "ExportJobProperties": ExportJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFHIRExportJobsResponseTypeDef = TypedDict(
     "ListFHIRExportJobsResponseTypeDef",
     {
         "ExportJobPropertiesList": List[ExportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFHIRImportJobResponseTypeDef = TypedDict(
     "DescribeFHIRImportJobResponseTypeDef",
     {
         "ImportJobProperties": ImportJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFHIRImportJobsResponseTypeDef = TypedDict(
     "ListFHIRImportJobsResponseTypeDef",
     {
         "ImportJobPropertiesList": List[ImportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/PKG-INFO` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.26.144
-Summary: Type annotations for boto3.HealthLake 1.26.144 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.HealthLake 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.26.144](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -304,33 +304,33 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/SOURCES.txt` & `mypy-boto3-healthlake-1.27.0/mypy_boto3_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.26.144/setup.py` & `mypy-boto3-healthlake-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-healthlake",
-    version="1.26.144",
+    version="1.27.0",
     packages=["mypy_boto3_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthLake 1.26.144 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.HealthLake 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


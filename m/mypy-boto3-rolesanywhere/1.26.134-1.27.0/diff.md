# Comparing `tmp/mypy-boto3-rolesanywhere-1.26.134.tar.gz` & `tmp/mypy-boto3-rolesanywhere-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.26.134.tar", last modified: Mon May 15 20:22:58 2023, max compression
+gzip compressed data, was "mypy-boto3-rolesanywhere-1.27.0.tar", last modified: Mon Jul  3 19:51:21 2023, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.26.134.tar` & `mypy-boto3-rolesanywhere-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-15 20:22:42.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-05-15 20:22:41.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 20:22:58.000000 mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:22:58.859293 mypy-boto3-rolesanywhere-1.26.134/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-15 20:22:40.000000 mypy-boto3-rolesanywhere-1.26.134/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.039896 mypy-boto3-rolesanywhere-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-07-03 19:51:21.035896 mypy-boto3-rolesanywhere-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.027896 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-03 19:46:26.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-07-03 19:46:26.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-03 19:46:26.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-07-03 19:46:26.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.035896 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-07-03 19:51:20.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:51:20.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:20.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:20.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:20.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:20.000000 mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:21.043896 mypy-boto3-rolesanywhere-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-03 19:46:25.000000 mypy-boto3-rolesanywhere-1.27.0/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/LICENSE` & `mypy-boto3-rolesanywhere-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.134/PKG-INFO` & `mypy-boto3-rolesanywhere-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.26.134
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.26.134 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.26.134](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -338,45 +338,45 @@
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
-    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    PaginatorConfigTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/README.md` & `mypy-boto3-rolesanywhere-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.26.134](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -306,45 +306,45 @@
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
-    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    PaginatorConfigTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.py` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/__main__.py` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.26.134\nVersion:         1.26.134\nBuilder"
+        "Type annotations for boto3.IAMRolesAnywhere 1.27.0\nVersion:         1.27.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.134")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.py` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/client.pyi` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.py` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/literals.py`

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

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/literals.pyi` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -99,14 +100,15 @@
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
@@ -248,14 +250,15 @@
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
@@ -277,14 +280,16 @@
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
@@ -368,14 +373,15 @@
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

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.py` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,58 +58,58 @@
 class ListCrlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCrlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
         """
 
 
 class ListProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
         """
 
 
 class ListSubjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
         """
 
 
 class ListTrustAnchorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrustAnchorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,55 +55,55 @@
 class ListCrlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCrlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
         """
 
 class ListProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
         """
 
 class ListSubjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
         """
 
 class ListTrustAnchorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrustAnchorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.py` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,45 +30,45 @@
 
 
 __all__ = (
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListRequestListCrlsPaginateTypeDef",
+    "ListRequestListProfilesPaginateTypeDef",
+    "ListRequestListSubjectsPaginateTypeDef",
+    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
-    "ListRequestListCrlsPaginateTypeDef",
-    "ListRequestListProfilesPaginateTypeDef",
-    "ListRequestListSubjectsPaginateTypeDef",
-    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
@@ -133,25 +133,14 @@
         "name": str,
         "trustAnchorArn": str,
         "updatedAt": datetime,
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
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": bool,
         "properties": Dict[str, str],
         "seenAt": datetime,
     },
@@ -173,20 +162,46 @@
         "roleArns": List[str],
         "sessionPolicy": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRequestListCrlsPaginateTypeDef = TypedDict(
+    "ListRequestListCrlsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListRequestListProfilesPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListRequestListSubjectsPaginateTypeDef = TypedDict(
+    "ListRequestListSubjectsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
+    "ListRequestListTrustAnchorsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRequestRequestTypeDef = TypedDict(
     "ListRequestRequestTypeDef",
     {
@@ -258,14 +273,35 @@
 
 class NotificationSettingKeyTypeDef(
     _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
 ):
     pass
 
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
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
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -401,14 +437,22 @@
 
 class ImportCrlRequestRequestTypeDef(
     _RequiredImportCrlRequestRequestTypeDef, _OptionalImportCrlRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -421,32 +465,24 @@
     },
 )
 
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCrlsResponseTypeDef = TypedDict(
     "ListCrlsResponseTypeDef",
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
@@ -463,68 +499,32 @@
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "nextToken": str,
         "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProfileDetailResponseTypeDef = TypedDict(
     "ProfileDetailResponseTypeDef",
     {
         "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRequestListCrlsPaginateTypeDef = TypedDict(
-    "ListRequestListCrlsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListRequestListProfilesPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListRequestListSubjectsPaginateTypeDef = TypedDict(
-    "ListRequestListSubjectsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
-    "ListRequestListTrustAnchorsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListSubjectsResponseTypeDef = TypedDict(
     "ListSubjectsResponseTypeDef",
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
@@ -541,15 +541,15 @@
     total=False,
 )
 
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
@@ -611,34 +611,34 @@
 
 
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutNotificationSettingsResponseTypeDef = TypedDict(
     "PutNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetNotificationSettingsResponseTypeDef = TypedDict(
     "ResetNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,45 +29,45 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListRequestListCrlsPaginateTypeDef",
+    "ListRequestListProfilesPaginateTypeDef",
+    "ListRequestListSubjectsPaginateTypeDef",
+    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
-    "ListRequestListCrlsPaginateTypeDef",
-    "ListRequestListProfilesPaginateTypeDef",
-    "ListRequestListSubjectsPaginateTypeDef",
-    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
@@ -130,25 +130,14 @@
         "name": str,
         "trustAnchorArn": str,
         "updatedAt": datetime,
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
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": bool,
         "properties": Dict[str, str],
         "seenAt": datetime,
     },
@@ -170,20 +159,46 @@
         "roleArns": List[str],
         "sessionPolicy": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRequestListCrlsPaginateTypeDef = TypedDict(
+    "ListRequestListCrlsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListRequestListProfilesPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListRequestListSubjectsPaginateTypeDef = TypedDict(
+    "ListRequestListSubjectsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
+    "ListRequestListTrustAnchorsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRequestRequestTypeDef = TypedDict(
     "ListRequestRequestTypeDef",
     {
@@ -251,14 +266,35 @@
 )
 
 class NotificationSettingKeyTypeDef(
     _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
 ):
     pass
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
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
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -386,14 +422,22 @@
 )
 
 class ImportCrlRequestRequestTypeDef(
     _RequiredImportCrlRequestRequestTypeDef, _OptionalImportCrlRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -406,32 +450,24 @@
     },
 )
 
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCrlsResponseTypeDef = TypedDict(
     "ListCrlsResponseTypeDef",
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
@@ -448,68 +484,32 @@
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "nextToken": str,
         "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProfileDetailResponseTypeDef = TypedDict(
     "ProfileDetailResponseTypeDef",
     {
         "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRequestListCrlsPaginateTypeDef = TypedDict(
-    "ListRequestListCrlsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListRequestListProfilesPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListRequestListSubjectsPaginateTypeDef = TypedDict(
-    "ListRequestListSubjectsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
-    "ListRequestListTrustAnchorsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListSubjectsResponseTypeDef = TypedDict(
     "ListSubjectsResponseTypeDef",
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
@@ -526,15 +526,15 @@
     total=False,
 )
 
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
@@ -592,34 +592,34 @@
     pass
 
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutNotificationSettingsResponseTypeDef = TypedDict(
     "PutNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetNotificationSettingsResponseTypeDef = TypedDict(
     "ResetNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.26.134
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.26.134 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.26.134](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -338,45 +338,45 @@
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
-    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    PaginatorConfigTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
```

### Comparing `mypy-boto3-rolesanywhere-1.26.134/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy-boto3-rolesanywhere-1.27.0/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.26.134/setup.py` & `mypy-boto3-rolesanywhere-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.26.134",
+    version="1.27.0",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAMRolesAnywhere 1.26.134 service generated with"
+        "Type annotations for boto3.IAMRolesAnywhere 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


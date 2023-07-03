# Comparing `tmp/mypy-boto3-appfabric-1.26.162.tar.gz` & `tmp/mypy-boto3-appfabric-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appfabric-1.26.162.tar", last modified: Tue Jun 27 21:23:10 2023, max compression
+gzip compressed data, was "mypy-boto3-appfabric-1.27.0.tar", last modified: Mon Jul  3 19:50:20 2023, max compression
```

## Comparing `mypy-boto3-appfabric-1.26.162.tar` & `mypy-boto3-appfabric-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:10.514103 mypy-boto3-appfabric-1.26.162/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-27 21:23:10.506103 mypy-boto3-appfabric-1.26.162/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:10.498103 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25020 2023-06-27 21:22:02.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:10.506103 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-27 21:23:10.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-27 21:23:10.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:10.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:10.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 21:23:10.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 21:23:10.000000 mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:23:10.514103 mypy-boto3-appfabric-1.26.162/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-27 21:22:01.000000 mypy-boto3-appfabric-1.26.162/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.302781 mypy-boto3-appfabric-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-03 19:50:20.294781 mypy-boto3-appfabric-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.294781 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25097 2023-07-03 19:32:26.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.294781 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-03 19:50:20.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:20.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:20.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:20.000000 mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:20.302781 mypy-boto3-appfabric-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:32:25.000000 mypy-boto3-appfabric-1.27.0/setup.py
```

### Comparing `mypy-boto3-appfabric-1.26.162/LICENSE` & `mypy-boto3-appfabric-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/PKG-INFO` & `mypy-boto3-appfabric-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appfabric
-Version: 1.26.162
-Summary: Type annotations for boto3.AppFabric 1.26.162 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.AppFabric 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appfabric?color=blue)](https://pypistats.org/packages/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -348,15 +348,14 @@
     ApiKeyCredentialTypeDef,
     TenantTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
@@ -364,46 +363,47 @@
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
     IngestionSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
     ListAppAuthorizationsRequestRequestTypeDef,
+    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
+    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
+    ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
-    ProcessingConfigurationTypeDef,
-    ConnectAppAuthorizationRequestRequestTypeDef,
+    ListAppBundlesResponseTypeDef,
     CreateAppBundleResponseTypeDef,
     GetAppBundleResponseTypeDef,
-    ListAppBundlesResponseTypeDef,
+    ProcessingConfigurationTypeDef,
+    ConnectAppAuthorizationRequestRequestTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
-    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
-    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    ListIngestionsRequestListIngestionsPaginateTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
```

### Comparing `mypy-boto3-appfabric-1.26.162/README.md` & `mypy-boto3-appfabric-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appfabric?color=blue)](https://pypistats.org/packages/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -316,15 +316,14 @@
     ApiKeyCredentialTypeDef,
     TenantTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
@@ -332,46 +331,47 @@
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
     IngestionSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
     ListAppAuthorizationsRequestRequestTypeDef,
+    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
+    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
+    ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
-    ProcessingConfigurationTypeDef,
-    ConnectAppAuthorizationRequestRequestTypeDef,
+    ListAppBundlesResponseTypeDef,
     CreateAppBundleResponseTypeDef,
     GetAppBundleResponseTypeDef,
-    ListAppBundlesResponseTypeDef,
+    ProcessingConfigurationTypeDef,
+    ConnectAppAuthorizationRequestRequestTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
-    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
-    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    ListIngestionsRequestListIngestionsPaginateTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/__init__.py` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/__init__.pyi` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/__main__.py` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppFabric 1.26.162\nVersion:         1.26.162\nBuilder version:"
+        "Type annotations for boto3.AppFabric 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.162")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/client.py` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/client.pyi` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/literals.py` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/literals.pyi` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/paginator.py` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 class ListAppAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
         """
 
 
 class ListAppBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppBundlesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
         """
 
 
@@ -92,28 +92,28 @@
     """
 
     def paginate(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIngestionDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestiondestinationspaginator)
         """
 
 
 class ListIngestionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIngestionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
         """
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/paginator.pyi` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,29 +55,29 @@
 class ListAppAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
         """
 
 class ListAppBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppBundlesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
         """
 
 class ListIngestionDestinationsPaginator(Paginator):
@@ -87,27 +87,27 @@
     """
 
     def paginate(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIngestionDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestiondestinationspaginator)
         """
 
 class ListIngestionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIngestionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
         """
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/type_defs.py` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     "ApiKeyCredentialTypeDef",
     "TenantTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
     "BatchGetUserAccessTasksRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "IngestionTypeDef",
     "Oauth2CredentialTypeDef",
     "DeleteAppAuthorizationRequestRequestTypeDef",
     "DeleteAppBundleRequestRequestTypeDef",
     "DeleteIngestionDestinationRequestRequestTypeDef",
     "DeleteIngestionRequestRequestTypeDef",
@@ -56,46 +55,47 @@
     "S3BucketTypeDef",
     "GetAppAuthorizationRequestRequestTypeDef",
     "GetAppBundleRequestRequestTypeDef",
     "GetIngestionDestinationRequestRequestTypeDef",
     "GetIngestionRequestRequestTypeDef",
     "IngestionDestinationSummaryTypeDef",
     "IngestionSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
     "ListAppAuthorizationsRequestRequestTypeDef",
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
     "ListAppBundlesRequestRequestTypeDef",
+    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     "ListIngestionDestinationsRequestRequestTypeDef",
+    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartIngestionRequestRequestTypeDef",
     "StartUserAccessTasksRequestRequestTypeDef",
     "StopIngestionRequestRequestTypeDef",
     "TaskErrorTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppAuthorizationSummaryTypeDef",
     "AppAuthorizationTypeDef",
-    "ProcessingConfigurationTypeDef",
-    "ConnectAppAuthorizationRequestRequestTypeDef",
+    "ListAppBundlesResponseTypeDef",
     "CreateAppBundleResponseTypeDef",
     "GetAppBundleResponseTypeDef",
-    "ListAppBundlesResponseTypeDef",
+    "ProcessingConfigurationTypeDef",
+    "ConnectAppAuthorizationRequestRequestTypeDef",
     "CreateAppBundleRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIngestionResponseTypeDef",
     "GetIngestionResponseTypeDef",
     "CredentialTypeDef",
     "DestinationTypeDef",
     "ListIngestionDestinationsResponseTypeDef",
     "ListIngestionsResponseTypeDef",
-    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
-    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "UserAccessResultItemTypeDef",
     "UserAccessTaskItemTypeDef",
     "ConnectAppAuthorizationResponseTypeDef",
     "ListAppAuthorizationsResponseTypeDef",
     "CreateAppAuthorizationResponseTypeDef",
     "GetAppAuthorizationResponseTypeDef",
     "UpdateAppAuthorizationResponseTypeDef",
@@ -174,25 +174,14 @@
     "BatchGetUserAccessTasksRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "taskIdList": Sequence[str],
     },
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -322,24 +311,36 @@
         "arn": str,
         "app": str,
         "tenantId": str,
         "state": IngestionStateType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
+    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAppAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppAuthorizationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListAppAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -355,23 +356,54 @@
 class ListAppAuthorizationsRequestRequestTypeDef(
     _RequiredListAppAuthorizationsRequestRequestTypeDef,
     _OptionalListAppAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
 
+ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAppBundlesRequestRequestTypeDef = TypedDict(
     "ListAppBundlesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+    },
+)
+_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
+    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListIngestionDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionDestinationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
@@ -388,14 +420,36 @@
 class ListIngestionDestinationsRequestRequestTypeDef(
     _RequiredListIngestionDestinationsRequestRequestTypeDef,
     _OptionalListIngestionDestinationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListIngestionsRequestListIngestionsPaginateTypeDef(
+    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
+    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListIngestionsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListIngestionsRequestRequestTypeDef = TypedDict(
@@ -417,14 +471,35 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
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
 StartIngestionRequestRequestTypeDef = TypedDict(
     "StartIngestionRequestRequestTypeDef",
     {
         "ingestionIdentifier": str,
         "appBundleIdentifier": str,
     },
 )
@@ -497,14 +572,39 @@
 )
 
 
 class AppAuthorizationTypeDef(_RequiredAppAuthorizationTypeDef, _OptionalAppAuthorizationTypeDef):
     pass
 
 
+ListAppBundlesResponseTypeDef = TypedDict(
+    "ListAppBundlesResponseTypeDef",
+    {
+        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAppBundleResponseTypeDef = TypedDict(
+    "CreateAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAppBundleResponseTypeDef = TypedDict(
+    "GetAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "auditLog": AuditLogProcessingConfigurationTypeDef,
     },
     total=False,
 )
@@ -528,39 +628,14 @@
 class ConnectAppAuthorizationRequestRequestTypeDef(
     _RequiredConnectAppAuthorizationRequestRequestTypeDef,
     _OptionalConnectAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAppBundleResponseTypeDef = TypedDict(
-    "CreateAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppBundleResponseTypeDef = TypedDict(
-    "GetAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppBundlesResponseTypeDef = TypedDict(
-    "ListAppBundlesResponseTypeDef",
-    {
-        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateAppBundleRequestRequestTypeDef = TypedDict(
     "CreateAppBundleRequestRequestTypeDef",
     {
         "clientToken": str,
         "customerManagedKeyIdentifier": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -592,15 +667,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -608,23 +683,23 @@
     },
 )
 
 CreateIngestionResponseTypeDef = TypedDict(
     "CreateIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIngestionResponseTypeDef = TypedDict(
     "GetIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CredentialTypeDef = TypedDict(
     "CredentialTypeDef",
     {
         "oauth2Credential": Oauth2CredentialTypeDef,
@@ -643,102 +718,27 @@
 )
 
 ListIngestionDestinationsResponseTypeDef = TypedDict(
     "ListIngestionDestinationsResponseTypeDef",
     {
         "ingestionDestinations": List[IngestionDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIngestionsResponseTypeDef = TypedDict(
     "ListIngestionsResponseTypeDef",
     {
         "ingestions": List[IngestionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-
-class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
-    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-):
-    pass
-
-
-ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-    },
-)
-_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
-
-class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
-    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListIngestionsRequestListIngestionsPaginateTypeDef(
-    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
-    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
-):
-    pass
-
-
 UserAccessResultItemTypeDef = TypedDict(
     "UserAccessResultItemTypeDef",
     {
         "app": str,
         "tenantId": str,
         "tenantDisplayName": str,
         "taskId": str,
@@ -777,48 +777,48 @@
     pass
 
 
 ConnectAppAuthorizationResponseTypeDef = TypedDict(
     "ConnectAppAuthorizationResponseTypeDef",
     {
         "appAuthorizationSummary": AppAuthorizationSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppAuthorizationsResponseTypeDef = TypedDict(
     "ListAppAuthorizationsResponseTypeDef",
     {
         "appAuthorizationSummaryList": List[AppAuthorizationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppAuthorizationResponseTypeDef = TypedDict(
     "CreateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppAuthorizationResponseTypeDef = TypedDict(
     "GetAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppAuthorizationResponseTypeDef = TypedDict(
     "UpdateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAppAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppAuthorizationRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
@@ -876,23 +876,23 @@
     },
 )
 
 BatchGetUserAccessTasksResponseTypeDef = TypedDict(
     "BatchGetUserAccessTasksResponseTypeDef",
     {
         "userAccessResultsList": List[UserAccessResultItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartUserAccessTasksResponseTypeDef = TypedDict(
     "StartUserAccessTasksResponseTypeDef",
     {
         "userAccessTasksList": List[UserAccessTaskItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "auditLog": AuditLogDestinationConfigurationTypeDef,
@@ -963,26 +963,26 @@
     },
 )
 
 CreateIngestionDestinationResponseTypeDef = TypedDict(
     "CreateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIngestionDestinationResponseTypeDef = TypedDict(
     "GetIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIngestionDestinationResponseTypeDef = TypedDict(
     "UpdateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric/type_defs.pyi` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     "ApiKeyCredentialTypeDef",
     "TenantTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
     "BatchGetUserAccessTasksRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "IngestionTypeDef",
     "Oauth2CredentialTypeDef",
     "DeleteAppAuthorizationRequestRequestTypeDef",
     "DeleteAppBundleRequestRequestTypeDef",
     "DeleteIngestionDestinationRequestRequestTypeDef",
     "DeleteIngestionRequestRequestTypeDef",
@@ -55,46 +54,47 @@
     "S3BucketTypeDef",
     "GetAppAuthorizationRequestRequestTypeDef",
     "GetAppBundleRequestRequestTypeDef",
     "GetIngestionDestinationRequestRequestTypeDef",
     "GetIngestionRequestRequestTypeDef",
     "IngestionDestinationSummaryTypeDef",
     "IngestionSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
     "ListAppAuthorizationsRequestRequestTypeDef",
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
     "ListAppBundlesRequestRequestTypeDef",
+    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     "ListIngestionDestinationsRequestRequestTypeDef",
+    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartIngestionRequestRequestTypeDef",
     "StartUserAccessTasksRequestRequestTypeDef",
     "StopIngestionRequestRequestTypeDef",
     "TaskErrorTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppAuthorizationSummaryTypeDef",
     "AppAuthorizationTypeDef",
-    "ProcessingConfigurationTypeDef",
-    "ConnectAppAuthorizationRequestRequestTypeDef",
+    "ListAppBundlesResponseTypeDef",
     "CreateAppBundleResponseTypeDef",
     "GetAppBundleResponseTypeDef",
-    "ListAppBundlesResponseTypeDef",
+    "ProcessingConfigurationTypeDef",
+    "ConnectAppAuthorizationRequestRequestTypeDef",
     "CreateAppBundleRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIngestionResponseTypeDef",
     "GetIngestionResponseTypeDef",
     "CredentialTypeDef",
     "DestinationTypeDef",
     "ListIngestionDestinationsResponseTypeDef",
     "ListIngestionsResponseTypeDef",
-    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
-    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "UserAccessResultItemTypeDef",
     "UserAccessTaskItemTypeDef",
     "ConnectAppAuthorizationResponseTypeDef",
     "ListAppAuthorizationsResponseTypeDef",
     "CreateAppAuthorizationResponseTypeDef",
     "GetAppAuthorizationResponseTypeDef",
     "UpdateAppAuthorizationResponseTypeDef",
@@ -171,25 +171,14 @@
     "BatchGetUserAccessTasksRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "taskIdList": Sequence[str],
     },
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -317,24 +306,34 @@
         "arn": str,
         "app": str,
         "tenantId": str,
         "state": IngestionStateType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
+    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAppAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppAuthorizationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListAppAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -348,23 +347,52 @@
 
 class ListAppAuthorizationsRequestRequestTypeDef(
     _RequiredListAppAuthorizationsRequestRequestTypeDef,
     _OptionalListAppAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
+ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAppBundlesRequestRequestTypeDef = TypedDict(
     "ListAppBundlesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+    },
+)
+_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
+    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListIngestionDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionDestinationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
@@ -379,14 +407,34 @@
 
 class ListIngestionDestinationsRequestRequestTypeDef(
     _RequiredListIngestionDestinationsRequestRequestTypeDef,
     _OptionalListIngestionDestinationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListIngestionsRequestListIngestionsPaginateTypeDef(
+    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
+    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListIngestionsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListIngestionsRequestRequestTypeDef = TypedDict(
@@ -406,14 +454,35 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
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
 StartIngestionRequestRequestTypeDef = TypedDict(
     "StartIngestionRequestRequestTypeDef",
     {
         "ingestionIdentifier": str,
         "appBundleIdentifier": str,
     },
 )
@@ -484,14 +553,39 @@
     },
     total=False,
 )
 
 class AppAuthorizationTypeDef(_RequiredAppAuthorizationTypeDef, _OptionalAppAuthorizationTypeDef):
     pass
 
+ListAppBundlesResponseTypeDef = TypedDict(
+    "ListAppBundlesResponseTypeDef",
+    {
+        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAppBundleResponseTypeDef = TypedDict(
+    "CreateAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAppBundleResponseTypeDef = TypedDict(
+    "GetAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "auditLog": AuditLogProcessingConfigurationTypeDef,
     },
     total=False,
 )
@@ -513,39 +607,14 @@
 
 class ConnectAppAuthorizationRequestRequestTypeDef(
     _RequiredConnectAppAuthorizationRequestRequestTypeDef,
     _OptionalConnectAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
-CreateAppBundleResponseTypeDef = TypedDict(
-    "CreateAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppBundleResponseTypeDef = TypedDict(
-    "GetAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppBundlesResponseTypeDef = TypedDict(
-    "ListAppBundlesResponseTypeDef",
-    {
-        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateAppBundleRequestRequestTypeDef = TypedDict(
     "CreateAppBundleRequestRequestTypeDef",
     {
         "clientToken": str,
         "customerManagedKeyIdentifier": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -575,15 +644,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -591,23 +660,23 @@
     },
 )
 
 CreateIngestionResponseTypeDef = TypedDict(
     "CreateIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIngestionResponseTypeDef = TypedDict(
     "GetIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CredentialTypeDef = TypedDict(
     "CredentialTypeDef",
     {
         "oauth2Credential": Oauth2CredentialTypeDef,
@@ -626,96 +695,27 @@
 )
 
 ListIngestionDestinationsResponseTypeDef = TypedDict(
     "ListIngestionDestinationsResponseTypeDef",
     {
         "ingestionDestinations": List[IngestionDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIngestionsResponseTypeDef = TypedDict(
     "ListIngestionsResponseTypeDef",
     {
         "ingestions": List[IngestionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
-    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-):
-    pass
-
-ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-    },
-)
-_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
-    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-):
-    pass
-
-_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListIngestionsRequestListIngestionsPaginateTypeDef(
-    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
-    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
-):
-    pass
-
 UserAccessResultItemTypeDef = TypedDict(
     "UserAccessResultItemTypeDef",
     {
         "app": str,
         "tenantId": str,
         "tenantDisplayName": str,
         "taskId": str,
@@ -752,48 +752,48 @@
 ):
     pass
 
 ConnectAppAuthorizationResponseTypeDef = TypedDict(
     "ConnectAppAuthorizationResponseTypeDef",
     {
         "appAuthorizationSummary": AppAuthorizationSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppAuthorizationsResponseTypeDef = TypedDict(
     "ListAppAuthorizationsResponseTypeDef",
     {
         "appAuthorizationSummaryList": List[AppAuthorizationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppAuthorizationResponseTypeDef = TypedDict(
     "CreateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppAuthorizationResponseTypeDef = TypedDict(
     "GetAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppAuthorizationResponseTypeDef = TypedDict(
     "UpdateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAppAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppAuthorizationRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
@@ -847,23 +847,23 @@
     },
 )
 
 BatchGetUserAccessTasksResponseTypeDef = TypedDict(
     "BatchGetUserAccessTasksResponseTypeDef",
     {
         "userAccessResultsList": List[UserAccessResultItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartUserAccessTasksResponseTypeDef = TypedDict(
     "StartUserAccessTasksResponseTypeDef",
     {
         "userAccessTasksList": List[UserAccessTaskItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "auditLog": AuditLogDestinationConfigurationTypeDef,
@@ -930,26 +930,26 @@
     },
 )
 
 CreateIngestionDestinationResponseTypeDef = TypedDict(
     "CreateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIngestionDestinationResponseTypeDef = TypedDict(
     "GetIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIngestionDestinationResponseTypeDef = TypedDict(
     "UpdateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/PKG-INFO` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appfabric
-Version: 1.26.162
-Summary: Type annotations for boto3.AppFabric 1.26.162 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.AppFabric 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appfabric?color=blue)](https://pypistats.org/packages/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -348,15 +348,14 @@
     ApiKeyCredentialTypeDef,
     TenantTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
@@ -364,46 +363,47 @@
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
     IngestionSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
     ListAppAuthorizationsRequestRequestTypeDef,
+    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
+    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
+    ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
-    ProcessingConfigurationTypeDef,
-    ConnectAppAuthorizationRequestRequestTypeDef,
+    ListAppBundlesResponseTypeDef,
     CreateAppBundleResponseTypeDef,
     GetAppBundleResponseTypeDef,
-    ListAppBundlesResponseTypeDef,
+    ProcessingConfigurationTypeDef,
+    ConnectAppAuthorizationRequestRequestTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
-    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
-    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    ListIngestionsRequestListIngestionsPaginateTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
```

### Comparing `mypy-boto3-appfabric-1.26.162/mypy_boto3_appfabric.egg-info/SOURCES.txt` & `mypy-boto3-appfabric-1.27.0/mypy_boto3_appfabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.26.162/setup.py` & `mypy-boto3-appfabric-1.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appfabric",
-    version="1.26.162",
+    version="1.27.0",
     packages=["mypy_boto3_appfabric"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppFabric 1.26.162 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.AppFabric 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


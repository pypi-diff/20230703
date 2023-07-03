# Comparing `tmp/mypy-boto3-sms-1.26.104.tar.gz` & `tmp/mypy-boto3-sms-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sms-1.26.104.tar", last modified: Fri Mar 31 19:33:13 2023, max compression
+gzip compressed data, was "mypy-boto3-sms-1.27.0.tar", last modified: Mon Jul  3 19:51:28 2023, max compression
```

## Comparing `mypy-boto3-sms-1.26.104.tar` & `mypy-boto3-sms-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:13.120558 mypy-boto3-sms-1.26.104/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-03-31 19:33:13.116558 mypy-boto3-sms-1.26.104/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:13.112558 mypy-boto3-sms-1.26.104/mypy_boto3_sms/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25822 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11175 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-03-31 19:33:02.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28445 2023-03-31 19:33:02.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:13.116558 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-03-31 19:33:12.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-31 19:33:12.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:33:12.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:33:12.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-31 19:33:12.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 19:33:12.000000 mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:33:13.120558 mypy-boto3-sms-1.26.104/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-31 19:33:01.000000 mypy-boto3-sms-1.26.104/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.776021 mypy-boto3-sms-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-07-03 19:51:28.776021 mypy-boto3-sms-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.768020 mypy-boto3-sms-1.27.0/mypy_boto3_sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25822 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-03 19:48:16.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28504 2023-07-03 19:48:16.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-07-03 19:48:16.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.776021 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-07-03 19:51:28.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:28.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:28.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:28.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:28.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:28.000000 mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:28.776021 mypy-boto3-sms-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:48:15.000000 mypy-boto3-sms-1.27.0/setup.py
```

### Comparing `mypy-boto3-sms-1.26.104/LICENSE` & `mypy-boto3-sms-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.26.104/PKG-INFO` & `mypy-boto3-sms-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.26.104
-Summary: Type annotations for boto3.SMS 1.26.104 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.SMS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms?color=blue)](https://pypistats.org/packages/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.26.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -357,60 +357,60 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
+    CreateReplicationJobResponseTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
     S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetConnectorsRequestRequestTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
+    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
+    ResponseMetadataTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
-    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
```

### Comparing `mypy-boto3-sms-1.26.104/README.md` & `mypy-boto3-sms-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms?color=blue)](https://pypistats.org/packages/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.26.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -325,60 +325,60 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
+    CreateReplicationJobResponseTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
     S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetConnectorsRequestRequestTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
+    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
+    ResponseMetadataTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
-    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/__init__.py` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/__init__.pyi` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/__main__.py` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SMS 1.26.104\nVersion:         1.26.104\nBuilder version:"
+        "Type annotations for boto3.SMS 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.104")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/client.py` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/client.pyi` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/literals.py` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AppLaunchConfigurationStatusType",
     "AppLaunchStatusType",
     "AppReplicationConfigurationStatusType",
     "AppReplicationStatusType",
     "AppStatusType",
     "AppValidationStrategyType",
@@ -47,15 +46,14 @@
     "SMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AppLaunchConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 AppLaunchStatusType = Literal[
     "CONFIGURATION_INVALID",
     "CONFIGURATION_IN_PROGRESS",
     "DELTA_LAUNCH_FAILED",
     "DELTA_LAUNCH_IN_PROGRESS",
     "LAUNCHED",
@@ -136,14 +134,15 @@
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
@@ -183,14 +182,15 @@
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
@@ -332,14 +332,15 @@
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
@@ -358,16 +359,19 @@
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
@@ -451,14 +455,15 @@
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

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/literals.pyi` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AppLaunchConfigurationStatusType",
     "AppLaunchStatusType",
     "AppReplicationConfigurationStatusType",
     "AppReplicationStatusType",
     "AppStatusType",
     "AppValidationStrategyType",
@@ -46,14 +47,15 @@
     "SMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AppLaunchConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 AppLaunchStatusType = Literal[
     "CONFIGURATION_INVALID",
     "CONFIGURATION_IN_PROGRESS",
     "DELTA_LAUNCH_FAILED",
     "DELTA_LAUNCH_IN_PROGRESS",
     "LAUNCHED",
@@ -134,14 +136,15 @@
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
@@ -181,14 +184,15 @@
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
@@ -330,14 +334,15 @@
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
@@ -356,16 +361,19 @@
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
@@ -449,14 +457,15 @@
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

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/paginator.py` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,94 +45,87 @@
     "GetConnectorsPaginator",
     "GetReplicationJobsPaginator",
     "GetReplicationRunsPaginator",
     "GetServersPaginator",
     "ListAppsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
         """
 
-
 class GetReplicationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, replicationJobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReplicationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
         """
 
-
 class GetReplicationRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, replicationJobId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReplicationRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
         """
 
-
 class GetServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
         """
 
-
 class ListAppsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
     """
 
     def paginate(
-        self, *, appIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, appIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
         """
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/paginator.pyi` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,87 +45,94 @@
     "GetConnectorsPaginator",
     "GetReplicationJobsPaginator",
     "GetReplicationRunsPaginator",
     "GetServersPaginator",
     "ListAppsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
         """
 
+
 class GetReplicationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, replicationJobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReplicationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
         """
 
+
 class GetReplicationRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, replicationJobId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReplicationRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
         """
 
+
 class GetServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
         """
 
+
 class ListAppsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
     """
 
     def paginate(
-        self, *, appIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, appIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
         """
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/type_defs.py` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,60 +44,60 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
+    "CreateReplicationJobResponseTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
     "S3LocationTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     "GetConnectorsRequestRequestTypeDef",
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationJobsRequestRequestTypeDef",
+    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
+    "ListAppsRequestListAppsPaginateTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
+    "PaginatorConfigTypeDef",
     "ReplicationRunStageDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
+    "StartOnDemandReplicationRunResponseTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
     "AppSummaryTypeDef",
-    "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
-    "StartOnDemandReplicationRunResponseTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
@@ -164,25 +164,14 @@
     {
         "key": str,
         "value": str,
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
 _RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationJobRequestRequestTypeDef",
     {
         "serverId": str,
         "seedReplicationTime": Union[datetime, str],
     },
 )
@@ -205,14 +194,22 @@
 class CreateReplicationJobRequestRequestTypeDef(
     _RequiredCreateReplicationJobRequestRequestTypeDef,
     _OptionalCreateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
 
+CreateReplicationJobResponseTypeDef = TypedDict(
+    "CreateReplicationJobResponseTypeDef",
+    {
+        "replicationJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -317,43 +314,72 @@
 GetAppValidationOutputRequestRequestTypeDef = TypedDict(
     "GetAppValidationOutputRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetConnectorsRequestRequestTypeDef = TypedDict(
     "GetConnectorsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetReplicationJobsRequestRequestTypeDef = TypedDict(
     "GetReplicationJobsRequestRequestTypeDef",
     {
         "replicationJobId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
+    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetReplicationRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetReplicationRunsRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalGetReplicationRunsRequestRequestTypeDef = TypedDict(
@@ -394,14 +420,23 @@
     "LaunchAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
+ListAppsRequestListAppsPaginateTypeDef = TypedDict(
+    "ListAppsRequestListAppsPaginateTypeDef",
+    {
+        "appIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -414,23 +449,44 @@
         "validationId": str,
         "status": ValidationStatusType,
         "statusMessage": str,
     },
     total=False,
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
 ReplicationRunStageDetailsTypeDef = TypedDict(
     "ReplicationRunStageDetailsTypeDef",
     {
         "stage": str,
         "stageProgress": str,
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
 ServerReplicationParametersTypeDef = TypedDict(
     "ServerReplicationParametersTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
@@ -489,14 +545,22 @@
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
 
+StartOnDemandReplicationRunResponseTypeDef = TypedDict(
+    "StartOnDemandReplicationRunResponseTypeDef",
+    {
+        "replicationRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -560,52 +624,36 @@
         "roleName": str,
         "totalServerGroups": int,
         "totalServers": int,
     },
     total=False,
 )
 
-CreateReplicationJobResponseTypeDef = TypedDict(
-    "CreateReplicationJobResponseTypeDef",
-    {
-        "replicationJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetConnectorsResponseTypeDef = TypedDict(
     "GetConnectorsResponseTypeDef",
     {
         "connectorList": List[ConnectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartOnDemandReplicationRunResponseTypeDef = TypedDict(
-    "StartOnDemandReplicationRunResponseTypeDef",
-    {
-        "replicationRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
         "s3Location": S3LocationTypeDef,
@@ -625,67 +673,19 @@
     "UserDataTypeDef",
     {
         "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
-    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-):
-    pass
-
-
-ListAppsRequestListAppsPaginateTypeDef = TypedDict(
-    "ListAppsRequestListAppsPaginateTypeDef",
-    {
-        "appIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetServersRequestGetServersPaginateTypeDef = TypedDict(
     "GetServersRequestGetServersPaginateTypeDef",
     {
         "vmServerAddressList": Sequence[VmServerAddressTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetServersRequestRequestTypeDef = TypedDict(
     "GetServersRequestRequestTypeDef",
     {
@@ -749,15 +749,15 @@
 )
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AppValidationOutputTypeDef = TypedDict(
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
@@ -838,15 +838,15 @@
 GetServersResponseTypeDef = TypedDict(
     "GetServersResponseTypeDef",
     {
         "lastModifiedOn": datetime,
         "serverCatalogStatus": ServerCatalogStatusType,
         "serverList": List[ServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
@@ -905,25 +905,25 @@
 )
 
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReplicationRunsResponseTypeDef = TypedDict(
     "GetReplicationRunsResponseTypeDef",
     {
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppRequestRequestTypeDef = TypedDict(
     "CreateAppRequestRequestTypeDef",
     {
         "name": str,
@@ -938,25 +938,25 @@
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppResponseTypeDef = TypedDict(
     "GetAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppRequestRequestTypeDef = TypedDict(
     "UpdateAppRequestRequestTypeDef",
     {
         "appId": str,
@@ -971,15 +971,15 @@
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
@@ -1024,15 +1024,15 @@
 GetAppLaunchConfigurationResponseTypeDef = TypedDict(
     "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
         "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
@@ -1043,15 +1043,15 @@
     total=False,
 )
 
 GetAppReplicationConfigurationResponseTypeDef = TypedDict(
     "GetAppReplicationConfigurationResponseTypeDef",
     {
         "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
@@ -1063,15 +1063,15 @@
 )
 
 GetAppValidationConfigurationResponseTypeDef = TypedDict(
     "GetAppValidationConfigurationResponseTypeDef",
     {
         "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
         "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
@@ -1094,10 +1094,10 @@
     pass
 
 
 GetAppValidationOutputResponseTypeDef = TypedDict(
     "GetAppValidationOutputResponseTypeDef",
     {
         "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms/type_defs.pyi` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,60 +43,60 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
+    "CreateReplicationJobResponseTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
     "S3LocationTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     "GetConnectorsRequestRequestTypeDef",
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationJobsRequestRequestTypeDef",
+    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
+    "ListAppsRequestListAppsPaginateTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
+    "PaginatorConfigTypeDef",
     "ReplicationRunStageDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
+    "StartOnDemandReplicationRunResponseTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
     "AppSummaryTypeDef",
-    "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
-    "StartOnDemandReplicationRunResponseTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
@@ -163,25 +163,14 @@
     {
         "key": str,
         "value": str,
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
 _RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationJobRequestRequestTypeDef",
     {
         "serverId": str,
         "seedReplicationTime": Union[datetime, str],
     },
 )
@@ -202,14 +191,22 @@
 
 class CreateReplicationJobRequestRequestTypeDef(
     _RequiredCreateReplicationJobRequestRequestTypeDef,
     _OptionalCreateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
+CreateReplicationJobResponseTypeDef = TypedDict(
+    "CreateReplicationJobResponseTypeDef",
+    {
+        "replicationJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -314,43 +311,70 @@
 GetAppValidationOutputRequestRequestTypeDef = TypedDict(
     "GetAppValidationOutputRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetConnectorsRequestRequestTypeDef = TypedDict(
     "GetConnectorsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetReplicationJobsRequestRequestTypeDef = TypedDict(
     "GetReplicationJobsRequestRequestTypeDef",
     {
         "replicationJobId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
+    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetReplicationRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetReplicationRunsRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalGetReplicationRunsRequestRequestTypeDef = TypedDict(
@@ -389,14 +413,23 @@
     "LaunchAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
+ListAppsRequestListAppsPaginateTypeDef = TypedDict(
+    "ListAppsRequestListAppsPaginateTypeDef",
+    {
+        "appIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -409,23 +442,44 @@
         "validationId": str,
         "status": ValidationStatusType,
         "statusMessage": str,
     },
     total=False,
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
 ReplicationRunStageDetailsTypeDef = TypedDict(
     "ReplicationRunStageDetailsTypeDef",
     {
         "stage": str,
         "stageProgress": str,
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
 ServerReplicationParametersTypeDef = TypedDict(
     "ServerReplicationParametersTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
@@ -480,14 +534,22 @@
 
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
+StartOnDemandReplicationRunResponseTypeDef = TypedDict(
+    "StartOnDemandReplicationRunResponseTypeDef",
+    {
+        "replicationRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -549,52 +611,36 @@
         "roleName": str,
         "totalServerGroups": int,
         "totalServers": int,
     },
     total=False,
 )
 
-CreateReplicationJobResponseTypeDef = TypedDict(
-    "CreateReplicationJobResponseTypeDef",
-    {
-        "replicationJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetConnectorsResponseTypeDef = TypedDict(
     "GetConnectorsResponseTypeDef",
     {
         "connectorList": List[ConnectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartOnDemandReplicationRunResponseTypeDef = TypedDict(
-    "StartOnDemandReplicationRunResponseTypeDef",
-    {
-        "replicationRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
         "s3Location": S3LocationTypeDef,
@@ -614,65 +660,19 @@
     "UserDataTypeDef",
     {
         "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
-    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-):
-    pass
-
-ListAppsRequestListAppsPaginateTypeDef = TypedDict(
-    "ListAppsRequestListAppsPaginateTypeDef",
-    {
-        "appIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetServersRequestGetServersPaginateTypeDef = TypedDict(
     "GetServersRequestGetServersPaginateTypeDef",
     {
         "vmServerAddressList": Sequence[VmServerAddressTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetServersRequestRequestTypeDef = TypedDict(
     "GetServersRequestRequestTypeDef",
     {
@@ -734,15 +734,15 @@
 )
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AppValidationOutputTypeDef = TypedDict(
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
@@ -823,15 +823,15 @@
 GetServersResponseTypeDef = TypedDict(
     "GetServersResponseTypeDef",
     {
         "lastModifiedOn": datetime,
         "serverCatalogStatus": ServerCatalogStatusType,
         "serverList": List[ServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
@@ -890,25 +890,25 @@
 )
 
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReplicationRunsResponseTypeDef = TypedDict(
     "GetReplicationRunsResponseTypeDef",
     {
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppRequestRequestTypeDef = TypedDict(
     "CreateAppRequestRequestTypeDef",
     {
         "name": str,
@@ -923,25 +923,25 @@
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppResponseTypeDef = TypedDict(
     "GetAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppRequestRequestTypeDef = TypedDict(
     "UpdateAppRequestRequestTypeDef",
     {
         "appId": str,
@@ -956,15 +956,15 @@
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
@@ -1009,15 +1009,15 @@
 GetAppLaunchConfigurationResponseTypeDef = TypedDict(
     "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
         "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
@@ -1028,15 +1028,15 @@
     total=False,
 )
 
 GetAppReplicationConfigurationResponseTypeDef = TypedDict(
     "GetAppReplicationConfigurationResponseTypeDef",
     {
         "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
@@ -1048,15 +1048,15 @@
 )
 
 GetAppValidationConfigurationResponseTypeDef = TypedDict(
     "GetAppValidationConfigurationResponseTypeDef",
     {
         "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
         "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
@@ -1077,10 +1077,10 @@
 ):
     pass
 
 GetAppValidationOutputResponseTypeDef = TypedDict(
     "GetAppValidationOutputResponseTypeDef",
     {
         "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/PKG-INFO` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.26.104
-Summary: Type annotations for boto3.SMS 1.26.104 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.SMS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms?color=blue)](https://pypistats.org/packages/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.26.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -357,60 +357,60 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
+    CreateReplicationJobResponseTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
     S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetConnectorsRequestRequestTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
+    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
+    ResponseMetadataTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
-    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
```

### Comparing `mypy-boto3-sms-1.26.104/mypy_boto3_sms.egg-info/SOURCES.txt` & `mypy-boto3-sms-1.27.0/mypy_boto3_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.26.104/setup.py` & `mypy-boto3-sms-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sms",
-    version="1.26.104",
+    version="1.27.0",
     packages=["mypy_boto3_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SMS 1.26.104 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SMS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


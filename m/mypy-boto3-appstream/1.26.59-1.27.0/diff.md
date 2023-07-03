# Comparing `tmp/mypy-boto3-appstream-1.26.59.tar.gz` & `tmp/mypy-boto3-appstream-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appstream-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-appstream-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-appstream-1.26.59.tar` & `mypy-boto3-appstream-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51155 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51071 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60863 2023-01-27 20:32:02.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60776 2023-01-27 20:32:02.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.722826 mypy-boto3-appstream-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-07-03 19:50:22.722826 mypy-boto3-appstream-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.722826 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69713 2023-07-03 19:32:44.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69616 2023-07-03 19:32:44.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 19:32:42.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.722826 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-07-03 19:50:22.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 19:50:22.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:22.000000 mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.722826 mypy-boto3-appstream-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:32:41.000000 mypy-boto3-appstream-1.27.0/setup.py
```

### Comparing `mypy-boto3-appstream-1.26.59/LICENSE` & `mypy-boto3-appstream-1.27.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-appstream-1.26.59/PKG-INFO` & `mypy-boto3-appstream-1.27.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.26.59
-Summary: Type annotations for boto3.AppStream 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppStream 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,14 +349,19 @@
 `mypy_boto3_appstream.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_appstream.literals import (
     AccessEndpointTypeType,
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderPlatformTypeType,
+    AppBlockBuilderStateChangeReasonCodeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     AppVisibilityType,
     ApplicationAttributeType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     DescribeDirectoryConfigsPaginatorName,
     DescribeFleetsPaginatorName,
     DescribeImageBuildersPaginatorName,
@@ -374,14 +379,15 @@
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     ListAssociatedFleetsPaginatorName,
     ListAssociatedStacksPaginatorName,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -410,103 +416,130 @@
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
+    AppBlockBuilderAppBlockAssociationTypeDef,
+    AppBlockBuilderStateChangeReasonTypeDef,
+    ResourceErrorTypeDef,
+    VpcConfigTypeDef,
+    ErrorDetailsTypeDef,
     S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
+    CopyImageResponseTypeDef,
+    CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
-    VpcConfigTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
+    CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
+    CreateStreamingURLResultTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
+    CreateUsageReportSubscriptionResultTypeDef,
     CreateUserRequestRequestTypeDef,
+    DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteImageBuilderRequestRequestTypeDef,
     DeleteImagePermissionsRequestRequestTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
+    DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
+    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeFleetsRequestRequestTypeDef,
+    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImageBuildersRequestRequestTypeDef,
     DescribeImagePermissionsRequestRequestTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
+    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
+    DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
+    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
     DisableUserRequestRequestTypeDef,
+    DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
-    ResourceErrorTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
+    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
+    ListAssociatedFleetsResultTypeDef,
+    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
+    ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StackErrorTypeDef,
+    StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
+    StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    AppBlockBuilderTypeDef,
+    CreateAppBlockBuilderRequestRequestTypeDef,
+    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     AssociateApplicationFleetResultTypeDef,
-    CopyImageResponseTypeDef,
-    CreateImageBuilderStreamingURLResultTypeDef,
-    CreateStreamingURLResultTypeDef,
-    CreateUsageReportSubscriptionResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
-    ListAssociatedFleetsResultTypeDef,
-    ListAssociatedStacksResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
     UserStackAssociationErrorTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
     DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
@@ -514,35 +547,30 @@
     EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
-    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
-    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
-    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    DescribeStacksRequestDescribeStacksPaginateTypeDef,
-    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
-    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
     DescribeUsersResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     FleetTypeDef,
-    SessionTypeDef,
     ImageBuilderTypeDef,
+    SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
+    StartAppBlockBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
     ImageTypeDef,
     UpdateApplicationResultTypeDef,
     AppBlockTypeDef,
     CreateAppBlockRequestRequestTypeDef,
     BatchAssociateUserStackResultTypeDef,
@@ -552,20 +580,20 @@
     UpdateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     UpdateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     DescribeFleetsResultTypeDef,
     UpdateFleetResultTypeDef,
-    DescribeSessionsResultTypeDef,
     CreateImageBuilderResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DescribeImageBuildersResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
+    DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
@@ -582,42 +610,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-appstream-1.26.59/README.md` & `mypy-boto3-appstream-1.27.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,14 +317,19 @@
 `mypy_boto3_appstream.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_appstream.literals import (
     AccessEndpointTypeType,
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderPlatformTypeType,
+    AppBlockBuilderStateChangeReasonCodeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     AppVisibilityType,
     ApplicationAttributeType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     DescribeDirectoryConfigsPaginatorName,
     DescribeFleetsPaginatorName,
     DescribeImageBuildersPaginatorName,
@@ -342,14 +347,15 @@
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     ListAssociatedFleetsPaginatorName,
     ListAssociatedStacksPaginatorName,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -378,103 +384,130 @@
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
+    AppBlockBuilderAppBlockAssociationTypeDef,
+    AppBlockBuilderStateChangeReasonTypeDef,
+    ResourceErrorTypeDef,
+    VpcConfigTypeDef,
+    ErrorDetailsTypeDef,
     S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
+    CopyImageResponseTypeDef,
+    CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
-    VpcConfigTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
+    CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
+    CreateStreamingURLResultTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
+    CreateUsageReportSubscriptionResultTypeDef,
     CreateUserRequestRequestTypeDef,
+    DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteImageBuilderRequestRequestTypeDef,
     DeleteImagePermissionsRequestRequestTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
+    DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
+    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeFleetsRequestRequestTypeDef,
+    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImageBuildersRequestRequestTypeDef,
     DescribeImagePermissionsRequestRequestTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
+    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
+    DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
+    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
     DisableUserRequestRequestTypeDef,
+    DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
-    ResourceErrorTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
+    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
+    ListAssociatedFleetsResultTypeDef,
+    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
+    ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StackErrorTypeDef,
+    StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
+    StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    AppBlockBuilderTypeDef,
+    CreateAppBlockBuilderRequestRequestTypeDef,
+    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     AssociateApplicationFleetResultTypeDef,
-    CopyImageResponseTypeDef,
-    CreateImageBuilderStreamingURLResultTypeDef,
-    CreateStreamingURLResultTypeDef,
-    CreateUsageReportSubscriptionResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
-    ListAssociatedFleetsResultTypeDef,
-    ListAssociatedStacksResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
     UserStackAssociationErrorTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
     DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
@@ -482,35 +515,30 @@
     EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
-    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
-    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
-    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    DescribeStacksRequestDescribeStacksPaginateTypeDef,
-    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
-    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
     DescribeUsersResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     FleetTypeDef,
-    SessionTypeDef,
     ImageBuilderTypeDef,
+    SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
+    StartAppBlockBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
     ImageTypeDef,
     UpdateApplicationResultTypeDef,
     AppBlockTypeDef,
     CreateAppBlockRequestRequestTypeDef,
     BatchAssociateUserStackResultTypeDef,
@@ -520,20 +548,20 @@
     UpdateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     UpdateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     DescribeFleetsResultTypeDef,
     UpdateFleetResultTypeDef,
-    DescribeSessionsResultTypeDef,
     CreateImageBuilderResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DescribeImageBuildersResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
+    DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
@@ -550,42 +578,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.pyi` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__main__.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppStream 1.26.59\nVersion:         1.26.59\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.AppStream 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     FleetAttributeType,
     FleetTypeType,
     MessageActionType,
+    PackagingTypeType,
     PlatformTypeType,
     StackAttributeType,
     StreamViewType,
     VisibilityTypeType,
 )
 from .paginator import (
     DescribeDirectoryConfigsPaginator,
@@ -41,33 +43,38 @@
     DescribeUserStackAssociationsPaginator,
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .type_defs import (
     AccessEndpointTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     BatchAssociateUserStackResultTypeDef,
     BatchDisassociateUserStackResultTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityTypeDef,
     CopyImageResponseTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateAppBlockResultTypeDef,
     CreateApplicationResultTypeDef,
     CreateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     CreateImageBuilderResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStackResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DeleteImageResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
     DescribeAppBlocksResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     DescribeApplicationsResultTypeDef,
     DescribeDirectoryConfigsResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     DescribeFleetsResultTypeDef,
     DescribeImageBuildersResultTypeDef,
@@ -84,18 +91,21 @@
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
+    StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
@@ -151,14 +161,24 @@
         """
         AppStreamClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#exceptions)
         """
 
+    def associate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> AssociateAppBlockBuilderAppBlockResultTypeDef:
+        """
+        Associates the specified app block builder with the specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_app_block_builder_app_block)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#associate_app_block_builder_app_block)
+        """
+
     def associate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> AssociateApplicationFleetResultTypeDef:
         """
         Associates the specified application with the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_application_fleet)
@@ -236,26 +256,59 @@
         """
 
     def create_app_block(
         self,
         *,
         Name: str,
         SourceS3Location: S3LocationTypeDef,
-        SetupScriptDetails: ScriptDetailsTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
-        Tags: Mapping[str, str] = ...
+        SetupScriptDetails: ScriptDetailsTypeDef = ...,
+        Tags: Mapping[str, str] = ...,
+        PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
+        PackagingType: PackagingTypeType = ...
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block)
         """
 
+    def create_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Platform: Literal["WINDOWS_SERVER_2019"],
+        InstanceType: str,
+        VpcConfig: VpcConfigTypeDef,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Tags: Mapping[str, str] = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+    ) -> CreateAppBlockBuilderResultTypeDef:
+        """
+        Creates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder)
+        """
+
+    def create_app_block_builder_streaming_url(
+        self, *, AppBlockBuilderName: str, Validity: int = ...
+    ) -> CreateAppBlockBuilderStreamingURLResultTypeDef:
+        """
+        Creates a URL to start a create app block builder streaming session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder_streaming_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder_streaming_url)
+        """
+
     def create_application(
         self,
         *,
         Name: str,
         IconS3Location: S3LocationTypeDef,
         LaunchPath: str,
         Platforms: Sequence[PlatformTypeType],
@@ -458,14 +511,22 @@
         """
         Deletes an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block)
         """
 
+    def delete_app_block_builder(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block_builder)
+        """
+
     def delete_application(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_application)
         """
@@ -540,14 +601,39 @@
         """
         Deletes a user from the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_user)
         """
 
+    def describe_app_block_builder_app_block_associations(
+        self,
+        *,
+        AppBlockArn: str = ...,
+        AppBlockBuilderName: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builder associations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builder_app_block_associations)
+        """
+
+    def describe_app_block_builders(
+        self, *, Names: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> DescribeAppBlockBuildersResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builders.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builders)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builders)
+        """
+
     def describe_app_blocks(
         self, *, Arns: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeAppBlocksResultTypeDef:
         """
         Retrieves a list that describes one or more app blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_blocks)
@@ -730,14 +816,24 @@
         """
         Disables the specified user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disable_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disable_user)
         """
 
+    def disassociate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> Dict[str, Any]:
+        """
+        Disassociates a specified app block builder from a specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_app_block_builder_app_block)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disassociate_app_block_builder_app_block)
+        """
+
     def disassociate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> Dict[str, Any]:
         """
         Disassociates the specified application from the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_application_fleet)
@@ -828,14 +924,22 @@
         """
         Retrieves a list of all tags for the specified AppStream 2.0 resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#list_tags_for_resource)
         """
 
+    def start_app_block_builder(self, *, Name: str) -> StartAppBlockBuilderResultTypeDef:
+        """
+        Starts an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_app_block_builder)
+        """
+
     def start_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_fleet)
         """
@@ -846,14 +950,22 @@
         """
         Starts the specified image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_image_builder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_image_builder)
         """
 
+    def stop_app_block_builder(self, *, Name: str) -> StopAppBlockBuilderResultTypeDef:
+        """
+        Stops an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_app_block_builder)
+        """
+
     def stop_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_fleet)
         """
@@ -879,14 +991,35 @@
         Disassociates one or more specified tags from the specified AppStream 2.0
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#untag_resource)
         """
 
+    def update_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Platform: PlatformTypeType = ...,
+        InstanceType: str = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
+        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
+    ) -> UpdateAppBlockBuilderResultTypeDef:
+        """
+        Updates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#update_app_block_builder)
+        """
+
     def update_application(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.pyi` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     FleetAttributeType,
     FleetTypeType,
     MessageActionType,
+    PackagingTypeType,
     PlatformTypeType,
     StackAttributeType,
     StreamViewType,
     VisibilityTypeType,
 )
 from .paginator import (
     DescribeDirectoryConfigsPaginator,
@@ -41,33 +43,38 @@
     DescribeUserStackAssociationsPaginator,
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .type_defs import (
     AccessEndpointTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     BatchAssociateUserStackResultTypeDef,
     BatchDisassociateUserStackResultTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityTypeDef,
     CopyImageResponseTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateAppBlockResultTypeDef,
     CreateApplicationResultTypeDef,
     CreateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     CreateImageBuilderResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStackResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DeleteImageResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
     DescribeAppBlocksResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     DescribeApplicationsResultTypeDef,
     DescribeDirectoryConfigsResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     DescribeFleetsResultTypeDef,
     DescribeImageBuildersResultTypeDef,
@@ -84,18 +91,21 @@
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
+    StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
@@ -146,14 +156,23 @@
     def exceptions(self) -> Exceptions:
         """
         AppStreamClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#exceptions)
         """
+    def associate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> AssociateAppBlockBuilderAppBlockResultTypeDef:
+        """
+        Associates the specified app block builder with the specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_app_block_builder_app_block)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#associate_app_block_builder_app_block)
+        """
     def associate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> AssociateApplicationFleetResultTypeDef:
         """
         Associates the specified application with the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_application_fleet)
@@ -223,25 +242,56 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#copy_image)
         """
     def create_app_block(
         self,
         *,
         Name: str,
         SourceS3Location: S3LocationTypeDef,
-        SetupScriptDetails: ScriptDetailsTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
-        Tags: Mapping[str, str] = ...
+        SetupScriptDetails: ScriptDetailsTypeDef = ...,
+        Tags: Mapping[str, str] = ...,
+        PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
+        PackagingType: PackagingTypeType = ...
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block)
         """
+    def create_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Platform: Literal["WINDOWS_SERVER_2019"],
+        InstanceType: str,
+        VpcConfig: VpcConfigTypeDef,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Tags: Mapping[str, str] = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+    ) -> CreateAppBlockBuilderResultTypeDef:
+        """
+        Creates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder)
+        """
+    def create_app_block_builder_streaming_url(
+        self, *, AppBlockBuilderName: str, Validity: int = ...
+    ) -> CreateAppBlockBuilderStreamingURLResultTypeDef:
+        """
+        Creates a URL to start a create app block builder streaming session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder_streaming_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder_streaming_url)
+        """
     def create_application(
         self,
         *,
         Name: str,
         IconS3Location: S3LocationTypeDef,
         LaunchPath: str,
         Platforms: Sequence[PlatformTypeType],
@@ -432,14 +482,21 @@
     def delete_app_block(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block)
         """
+    def delete_app_block_builder(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block_builder)
+        """
     def delete_application(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_application)
         """
@@ -504,14 +561,37 @@
     ) -> Dict[str, Any]:
         """
         Deletes a user from the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_user)
         """
+    def describe_app_block_builder_app_block_associations(
+        self,
+        *,
+        AppBlockArn: str = ...,
+        AppBlockBuilderName: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builder associations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builder_app_block_associations)
+        """
+    def describe_app_block_builders(
+        self, *, Names: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> DescribeAppBlockBuildersResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builders.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builders)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builders)
+        """
     def describe_app_blocks(
         self, *, Arns: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeAppBlocksResultTypeDef:
         """
         Retrieves a list that describes one or more app blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_blocks)
@@ -679,14 +759,23 @@
     ) -> Dict[str, Any]:
         """
         Disables the specified user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disable_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disable_user)
         """
+    def disassociate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> Dict[str, Any]:
+        """
+        Disassociates a specified app block builder from a specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_app_block_builder_app_block)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disassociate_app_block_builder_app_block)
+        """
     def disassociate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> Dict[str, Any]:
         """
         Disassociates the specified application from the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_application_fleet)
@@ -767,14 +856,21 @@
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves a list of all tags for the specified AppStream 2.0 resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#list_tags_for_resource)
         """
+    def start_app_block_builder(self, *, Name: str) -> StartAppBlockBuilderResultTypeDef:
+        """
+        Starts an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_app_block_builder)
+        """
     def start_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_fleet)
         """
@@ -783,14 +879,21 @@
     ) -> StartImageBuilderResultTypeDef:
         """
         Starts the specified image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_image_builder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_image_builder)
         """
+    def stop_app_block_builder(self, *, Name: str) -> StopAppBlockBuilderResultTypeDef:
+        """
+        Stops an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_app_block_builder)
+        """
     def stop_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_fleet)
         """
@@ -812,14 +915,34 @@
         """
         Disassociates one or more specified tags from the specified AppStream 2.0
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#untag_resource)
         """
+    def update_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Platform: PlatformTypeType = ...,
+        InstanceType: str = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
+        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
+    ) -> UpdateAppBlockBuilderResultTypeDef:
+        """
+        Updates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#update_app_block_builder)
+        """
     def update_application(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccessEndpointTypeType",
     "ActionType",
+    "AppBlockBuilderAttributeType",
+    "AppBlockBuilderPlatformTypeType",
+    "AppBlockBuilderStateChangeReasonCodeType",
+    "AppBlockBuilderStateType",
+    "AppBlockStateType",
     "AppVisibilityType",
     "ApplicationAttributeType",
     "AuthenticationTypeType",
     "CertificateBasedAuthStatusType",
     "DescribeDirectoryConfigsPaginatorName",
     "DescribeFleetsPaginatorName",
     "DescribeImageBuildersPaginatorName",
@@ -43,14 +48,15 @@
     "ImageBuilderStateChangeReasonCodeType",
     "ImageBuilderStateType",
     "ImageStateChangeReasonCodeType",
     "ImageStateType",
     "ListAssociatedFleetsPaginatorName",
     "ListAssociatedStacksPaginatorName",
     "MessageActionType",
+    "PackagingTypeType",
     "PermissionType",
     "PlatformTypeType",
     "PreferredProtocolType",
     "SessionConnectionStateType",
     "SessionStateType",
     "StackAttributeType",
     "StackErrorCodeType",
@@ -75,14 +81,21 @@
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
     "FILE_UPLOAD",
     "PRINTING_TO_LOCAL_DEVICE",
 ]
+AppBlockBuilderAttributeType = Literal[
+    "ACCESS_ENDPOINTS", "IAM_ROLE_ARN", "VPC_CONFIGURATION_SECURITY_GROUP_IDS"
+]
+AppBlockBuilderPlatformTypeType = Literal["WINDOWS_SERVER_2019"]
+AppBlockBuilderStateChangeReasonCodeType = Literal["INTERNAL_ERROR"]
+AppBlockBuilderStateType = Literal["RUNNING", "STARTING", "STOPPED", "STOPPING"]
+AppBlockStateType = Literal["ACTIVE", "INACTIVE"]
 AppVisibilityType = Literal["ALL", "ASSOCIATED"]
 ApplicationAttributeType = Literal["LAUNCH_PARAMETERS", "WORKING_DIRECTORY"]
 AuthenticationTypeType = Literal["API", "AWS_AD", "SAML", "USERPOOL"]
 CertificateBasedAuthStatusType = Literal[
     "DISABLED", "ENABLED", "ENABLED_NO_DIRECTORY_LOGIN_FALLBACK"
 ]
 DescribeDirectoryConfigsPaginatorName = Literal["describe_directory_configs"]
@@ -156,14 +169,15 @@
 ]
 ImageStateType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETING", "FAILED", "IMPORTING", "PENDING"
 ]
 ListAssociatedFleetsPaginatorName = Literal["list_associated_fleets"]
 ListAssociatedStacksPaginatorName = Literal["list_associated_stacks"]
 MessageActionType = Literal["RESEND", "SUPPRESS"]
+PackagingTypeType = Literal["APPSTREAM2", "CUSTOM"]
 PermissionType = Literal["DISABLED", "ENABLED"]
 PlatformTypeType = Literal["AMAZON_LINUX2", "WINDOWS", "WINDOWS_SERVER_2016", "WINDOWS_SERVER_2019"]
 PreferredProtocolType = Literal["TCP", "UDP"]
 SessionConnectionStateType = Literal["CONNECTED", "NOT_CONNECTED"]
 SessionStateType = Literal["ACTIVE", "EXPIRED", "PENDING"]
 StackAttributeType = Literal[
     "ACCESS_ENDPOINTS",
@@ -202,14 +216,15 @@
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
@@ -241,21 +256,23 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
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
@@ -334,14 +351,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -352,14 +370,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -395,14 +414,15 @@
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
@@ -421,16 +441,19 @@
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
@@ -510,18 +533,21 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
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

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.pyi` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccessEndpointTypeType",
     "ActionType",
+    "AppBlockBuilderAttributeType",
+    "AppBlockBuilderPlatformTypeType",
+    "AppBlockBuilderStateChangeReasonCodeType",
+    "AppBlockBuilderStateType",
+    "AppBlockStateType",
     "AppVisibilityType",
     "ApplicationAttributeType",
     "AuthenticationTypeType",
     "CertificateBasedAuthStatusType",
     "DescribeDirectoryConfigsPaginatorName",
     "DescribeFleetsPaginatorName",
     "DescribeImageBuildersPaginatorName",
@@ -42,14 +47,15 @@
     "ImageBuilderStateChangeReasonCodeType",
     "ImageBuilderStateType",
     "ImageStateChangeReasonCodeType",
     "ImageStateType",
     "ListAssociatedFleetsPaginatorName",
     "ListAssociatedStacksPaginatorName",
     "MessageActionType",
+    "PackagingTypeType",
     "PermissionType",
     "PlatformTypeType",
     "PreferredProtocolType",
     "SessionConnectionStateType",
     "SessionStateType",
     "StackAttributeType",
     "StackErrorCodeType",
@@ -73,14 +79,21 @@
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
     "FILE_UPLOAD",
     "PRINTING_TO_LOCAL_DEVICE",
 ]
+AppBlockBuilderAttributeType = Literal[
+    "ACCESS_ENDPOINTS", "IAM_ROLE_ARN", "VPC_CONFIGURATION_SECURITY_GROUP_IDS"
+]
+AppBlockBuilderPlatformTypeType = Literal["WINDOWS_SERVER_2019"]
+AppBlockBuilderStateChangeReasonCodeType = Literal["INTERNAL_ERROR"]
+AppBlockBuilderStateType = Literal["RUNNING", "STARTING", "STOPPED", "STOPPING"]
+AppBlockStateType = Literal["ACTIVE", "INACTIVE"]
 AppVisibilityType = Literal["ALL", "ASSOCIATED"]
 ApplicationAttributeType = Literal["LAUNCH_PARAMETERS", "WORKING_DIRECTORY"]
 AuthenticationTypeType = Literal["API", "AWS_AD", "SAML", "USERPOOL"]
 CertificateBasedAuthStatusType = Literal[
     "DISABLED", "ENABLED", "ENABLED_NO_DIRECTORY_LOGIN_FALLBACK"
 ]
 DescribeDirectoryConfigsPaginatorName = Literal["describe_directory_configs"]
@@ -154,14 +167,15 @@
 ]
 ImageStateType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETING", "FAILED", "IMPORTING", "PENDING"
 ]
 ListAssociatedFleetsPaginatorName = Literal["list_associated_fleets"]
 ListAssociatedStacksPaginatorName = Literal["list_associated_stacks"]
 MessageActionType = Literal["RESEND", "SUPPRESS"]
+PackagingTypeType = Literal["APPSTREAM2", "CUSTOM"]
 PermissionType = Literal["DISABLED", "ENABLED"]
 PlatformTypeType = Literal["AMAZON_LINUX2", "WINDOWS", "WINDOWS_SERVER_2016", "WINDOWS_SERVER_2019"]
 PreferredProtocolType = Literal["TCP", "UDP"]
 SessionConnectionStateType = Literal["CONNECTED", "NOT_CONNECTED"]
 SessionStateType = Literal["ACTIVE", "EXPIRED", "PENDING"]
 StackAttributeType = Literal[
     "ACCESS_ENDPOINTS",
@@ -200,14 +214,15 @@
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
@@ -239,21 +254,23 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
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
@@ -332,14 +349,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -350,14 +368,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -393,14 +412,15 @@
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
@@ -419,16 +439,19 @@
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
@@ -508,18 +531,21 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
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

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,45 +83,48 @@
 class DescribeDirectoryConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
     """
 
     def paginate(
-        self, *, DirectoryNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        DirectoryNames: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectoryConfigsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
         """
 
 
 class DescribeFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
         """
 
 
 class DescribeImageBuildersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImageBuildersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
         """
 
 
@@ -133,15 +136,15 @@
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagespaginator)
         """
 
 
@@ -154,30 +157,30 @@
     def paginate(
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describesessionspaginator)
         """
 
 
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
         """
 
 
@@ -189,15 +192,15 @@
 
     def paginate(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUserStackAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserstackassociationspaginator)
         """
 
 
@@ -207,43 +210,43 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
         """
 
 
 class ListAssociatedFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
         """
 
 
 class ListAssociatedStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
     """
 
     def paginate(
-        self, *, FleetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FleetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
         """
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.pyi` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -80,43 +80,46 @@
 class DescribeDirectoryConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
     """
 
     def paginate(
-        self, *, DirectoryNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        DirectoryNames: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectoryConfigsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
         """
 
 class DescribeFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
         """
 
 class DescribeImageBuildersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImageBuildersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
         """
 
 class DescribeImagesPaginator(Paginator):
@@ -127,15 +130,15 @@
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagespaginator)
         """
 
 class DescribeSessionsPaginator(Paginator):
@@ -147,29 +150,29 @@
     def paginate(
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describesessionspaginator)
         """
 
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
         """
 
 class DescribeUserStackAssociationsPaginator(Paginator):
@@ -180,15 +183,15 @@
 
     def paginate(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUserStackAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserstackassociationspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -197,41 +200,41 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
         """
 
 class ListAssociatedFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
         """
 
 class ListAssociatedStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
     """
 
     def paginate(
-        self, *, FleetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FleetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
         """
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     FleetAttributeType,
     FleetErrorCodeType,
     FleetStateType,
     FleetTypeType,
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -49,106 +53,132 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessEndpointTypeDef",
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    "ResourceErrorTypeDef",
+    "VpcConfigTypeDef",
+    "ErrorDetailsTypeDef",
     "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
+    "CopyImageResponseTypeDef",
+    "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
-    "VpcConfigTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
+    "CreateImageBuilderStreamingURLResultTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
+    "CreateStreamingURLResultTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
+    "CreateUsageReportSubscriptionResultTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteImageBuilderRequestRequestTypeDef",
     "DeleteImagePermissionsRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFleetsRequestRequestTypeDef",
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     "DescribeImageBuildersRequestRequestTypeDef",
     "DescribeImagePermissionsRequestRequestTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
+    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
     "DisableUserRequestRequestTypeDef",
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
-    "ResourceErrorTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
+    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
+    "ListAssociatedFleetsResultTypeDef",
+    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
+    "ListAssociatedStacksResultTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StackErrorTypeDef",
+    "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
+    "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    "AppBlockBuilderTypeDef",
+    "CreateAppBlockBuilderRequestRequestTypeDef",
+    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "AssociateApplicationFleetResultTypeDef",
-    "CopyImageResponseTypeDef",
-    "CreateImageBuilderStreamingURLResultTypeDef",
-    "CreateStreamingURLResultTypeDef",
-    "CreateUsageReportSubscriptionResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
-    "ListAssociatedFleetsResultTypeDef",
-    "ListAssociatedStacksResultTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
     "UserStackAssociationErrorTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
     "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
@@ -156,35 +186,30 @@
     "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
     "DescribeUsersResultTypeDef",
     "ListEntitledApplicationsResultTypeDef",
     "FleetTypeDef",
-    "SessionTypeDef",
     "ImageBuilderTypeDef",
+    "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
+    "CreateAppBlockBuilderResultTypeDef",
+    "DescribeAppBlockBuildersResultTypeDef",
+    "StartAppBlockBuilderResultTypeDef",
+    "StopAppBlockBuilderResultTypeDef",
+    "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
     "ImageTypeDef",
     "UpdateApplicationResultTypeDef",
     "AppBlockTypeDef",
     "CreateAppBlockRequestRequestTypeDef",
     "BatchAssociateUserStackResultTypeDef",
@@ -194,20 +219,20 @@
     "UpdateDirectoryConfigResultTypeDef",
     "CreateEntitlementResultTypeDef",
     "DescribeEntitlementsResultTypeDef",
     "UpdateEntitlementResultTypeDef",
     "CreateFleetResultTypeDef",
     "DescribeFleetsResultTypeDef",
     "UpdateFleetResultTypeDef",
-    "DescribeSessionsResultTypeDef",
     "CreateImageBuilderResultTypeDef",
     "DeleteImageBuilderResultTypeDef",
     "DescribeImageBuildersResultTypeDef",
     "StartImageBuilderResultTypeDef",
     "StopImageBuilderResultTypeDef",
+    "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
@@ -226,27 +251,79 @@
     "_OptionalAccessEndpointTypeDef",
     {
         "VpceId": str,
     },
     total=False,
 )
 
-
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
+AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+AppBlockBuilderStateChangeReasonTypeDef = TypedDict(
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    {
+        "Code": Literal["INTERNAL_ERROR"],
+        "Message": str,
+    },
+    total=False,
+)
+
+ResourceErrorTypeDef = TypedDict(
+    "ResourceErrorTypeDef",
+    {
+        "ErrorCode": FleetErrorCodeType,
+        "ErrorMessage": str,
+        "ErrorTimestamp": datetime,
+    },
+    total=False,
+)
+
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
+ErrorDetailsTypeDef = TypedDict(
+    "ErrorDetailsTypeDef",
+    {
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
     {
         "S3Bucket": str,
+    },
+)
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
+    {
         "S3Key": str,
     },
+    total=False,
 )
 
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+    pass
+
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -271,40 +348,35 @@
     "_OptionalApplicationSettingsTypeDef",
     {
         "SettingsGroup": str,
     },
     total=False,
 )
 
-
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
+AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
 
 AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "AssociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
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
 AssociateApplicationToEntitlementRequestRequestTypeDef = TypedDict(
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
         "ApplicationIdentifier": str,
     },
@@ -330,21 +402,19 @@
     "_OptionalUserStackAssociationTypeDef",
     {
         "SendEmailNotification": bool,
     },
     total=False,
 )
 
-
 class UserStackAssociationTypeDef(
     _RequiredUserStackAssociationTypeDef, _OptionalUserStackAssociationTypeDef
 ):
     pass
 
-
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusType,
         "CertificateAuthorityArn": str,
     },
     total=False,
@@ -362,21 +432,19 @@
         "Running": int,
         "InUse": int,
         "Available": int,
     },
     total=False,
 )
 
-
 class ComputeCapacityStatusTypeDef(
     _RequiredComputeCapacityStatusTypeDef, _OptionalComputeCapacityStatusTypeDef
 ):
     pass
 
-
 ComputeCapacityTypeDef = TypedDict(
     "ComputeCapacityTypeDef",
     {
         "DesiredInstances": int,
     },
 )
 
@@ -392,20 +460,55 @@
     "_OptionalCopyImageRequestRequestTypeDef",
     {
         "DestinationImageDescription": str,
     },
     total=False,
 )
 
-
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
+CopyImageResponseTypeDef = TypedDict(
+    "CopyImageResponseTypeDef",
+    {
+        "DestinationImageName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "AppBlockBuilderName": str,
+    },
+)
+_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "Validity": int,
+    },
+    total=False,
+)
+
+class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+):
+    pass
+
+CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
@@ -424,44 +527,42 @@
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedName": str,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Validity": int,
     },
     total=False,
 )
 
-
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
+CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateImageBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredStorageConnectorTypeDef = TypedDict(
     "_RequiredStorageConnectorTypeDef",
     {
         "ConnectorType": StorageConnectorTypeType,
     },
 )
@@ -470,19 +571,17 @@
     {
         "ResourceIdentifier": str,
         "Domains": Sequence[str],
     },
     total=False,
 )
 
-
 class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
     pass
 
-
 StreamingExperienceSettingsTypeDef = TypedDict(
     "StreamingExperienceSettingsTypeDef",
     {
         "PreferredProtocol": PreferredProtocolType,
     },
     total=False,
 )
@@ -509,21 +608,28 @@
         "ApplicationId": str,
         "Validity": int,
         "SessionContext": str,
     },
     total=False,
 )
 
-
 class CreateStreamingURLRequestRequestTypeDef(
     _RequiredCreateStreamingURLRequestRequestTypeDef,
     _OptionalCreateStreamingURLRequestRequestTypeDef,
 ):
     pass
 
+CreateStreamingURLResultTypeDef = TypedDict(
+    "CreateStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateUpdatedImageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUpdatedImageRequestRequestTypeDef",
     {
         "existingImageName": str,
         "newImageName": str,
     },
@@ -535,21 +641,28 @@
         "newImageDisplayName": str,
         "newImageTags": Mapping[str, str],
         "dryRun": bool,
     },
     total=False,
 )
 
-
 class CreateUpdatedImageRequestRequestTypeDef(
     _RequiredCreateUpdatedImageRequestRequestTypeDef,
     _OptionalCreateUpdatedImageRequestRequestTypeDef,
 ):
     pass
 
+CreateUsageReportSubscriptionResultTypeDef = TypedDict(
+    "CreateUsageReportSubscriptionResultTypeDef",
+    {
+        "S3BucketName": str,
+        "Schedule": Literal["DAILY"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
@@ -560,20 +673,25 @@
         "MessageAction": MessageActionType,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
 
 DeleteAppBlockRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -640,14 +758,35 @@
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+DescribeAppBlockBuildersRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeAppBlocksRequestRequestTypeDef = TypedDict(
     "DescribeAppBlocksRequestRequestTypeDef",
     {
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -671,20 +810,19 @@
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DirectoryNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDirectoryConfigsRequestRequestTypeDef = TypedDict(
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     {
@@ -707,21 +845,28 @@
         "Name": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeEntitlementsRequestRequestTypeDef(
     _RequiredDescribeEntitlementsRequestRequestTypeDef,
     _OptionalDescribeEntitlementsRequestRequestTypeDef,
 ):
     pass
 
+DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
@@ -733,14 +878,23 @@
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeImageBuildersRequestRequestTypeDef = TypedDict(
     "DescribeImageBuildersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -759,34 +913,66 @@
         "MaxResults": int,
         "SharedAwsAccountIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeImagePermissionsRequestRequestTypeDef(
     _RequiredDescribeImagePermissionsRequestRequestTypeDef,
     _OptionalDescribeImagePermissionsRequestRequestTypeDef,
 ):
     pass
 
+DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "Arns": Sequence[str],
+        "Type": VisibilityTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeImagesRequestRequestTypeDef = TypedDict(
     "DescribeImagesRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "Arns": Sequence[str],
         "Type": VisibilityTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    {
+        "StackName": str,
+        "FleetName": str,
+    },
+)
+_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    {
+        "UserId": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
+    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "StackName": str,
         "FleetName": str,
     },
 )
@@ -797,20 +983,27 @@
         "NextToken": str,
         "Limit": int,
         "AuthenticationType": AuthenticationTypeType,
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
+DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeStacksRequestRequestTypeDef = TypedDict(
     "DescribeStacksRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
@@ -822,26 +1015,57 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
+    {
+        "StackName": str,
+        "UserName": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUserStackAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     {
         "StackName": str,
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationType": AuthenticationTypeType,
+    },
+)
+_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeUsersRequestDescribeUsersPaginateTypeDef(
+    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
+    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeUsersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalDescribeUsersRequestRequestTypeDef = TypedDict(
@@ -849,21 +1073,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeUsersRequestRequestTypeDef(
     _RequiredDescribeUsersRequestRequestTypeDef, _OptionalDescribeUsersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalUserTypeDef = TypedDict(
@@ -876,27 +1098,33 @@
         "FirstName": str,
         "LastName": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-
 DisableUserRequestRequestTypeDef = TypedDict(
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
 DisassociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "DisassociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -963,24 +1191,14 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
-ResourceErrorTypeDef = TypedDict(
-    "ResourceErrorTypeDef",
-    {
-        "ErrorCode": FleetErrorCodeType,
-        "ErrorMessage": str,
-        "ErrorTimestamp": datetime,
-    },
-    total=False,
-)
-
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1000,35 +1218,82 @@
     {
         "ErrorCode": UsageReportExecutionErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
+    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedFleetsRequestRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_OptionalListAssociatedFleetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociatedFleetsRequestRequestTypeDef(
     _RequiredListAssociatedFleetsRequestRequestTypeDef,
     _OptionalListAssociatedFleetsRequestRequestTypeDef,
 ):
     pass
 
+ListAssociatedFleetsResultTypeDef = TypedDict(
+    "ListAssociatedFleetsResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
+    {
+        "FleetName": str,
+    },
+)
+_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
+    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+):
+    pass
 
 _RequiredListAssociatedStacksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedStacksRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
@@ -1036,21 +1301,28 @@
     "_OptionalListAssociatedStacksRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociatedStacksRequestRequestTypeDef(
     _RequiredListAssociatedStacksRequestRequestTypeDef,
     _OptionalListAssociatedStacksRequestRequestTypeDef,
 ):
     pass
 
+ListAssociatedStacksResultTypeDef = TypedDict(
+    "ListAssociatedStacksResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredListEntitledApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitledApplicationsRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
     },
@@ -1060,38 +1332,72 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEntitledApplicationsRequestRequestTypeDef(
     _RequiredListEntitledApplicationsRequestRequestTypeDef,
     _OptionalListEntitledApplicationsRequestRequestTypeDef,
 ):
     pass
 
-
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
 StackErrorTypeDef = TypedDict(
     "StackErrorTypeDef",
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StartAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StartFleetRequestRequestTypeDef = TypedDict(
     "StartFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1105,20 +1411,25 @@
     "_OptionalStartImageBuilderRequestRequestTypeDef",
     {
         "AppstreamAgentVersion": str,
     },
     total=False,
 )
 
-
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
+StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StopAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
 
 StopFleetRequestRequestTypeDef = TypedDict(
     "StopFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -1142,14 +1453,116 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredAppBlockBuilderTypeDef = TypedDict(
+    "_RequiredAppBlockBuilderTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "State": AppBlockBuilderStateType,
+    },
+)
+_OptionalAppBlockBuilderTypeDef = TypedDict(
+    "_OptionalAppBlockBuilderTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "CreatedTime": datetime,
+        "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
+        "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
+        "AccessEndpoints": List[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
+    pass
+
+_RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+)
+_OptionalCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Tags": Mapping[str, str],
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+class CreateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Platform": PlatformTypeType,
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
+    },
+    total=False,
+)
+
+class UpdateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
@@ -1187,21 +1600,19 @@
         "WorkingDirectory": str,
         "LaunchParameters": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredScriptDetailsTypeDef = TypedDict(
     "_RequiredScriptDetailsTypeDef",
     {
         "ScriptS3Location": S3LocationTypeDef,
         "ExecutablePath": str,
         "TimeoutInSeconds": int,
     },
@@ -1210,19 +1621,17 @@
     "_OptionalScriptDetailsTypeDef",
     {
         "ExecutableParameters": str,
     },
     total=False,
 )
 
-
 class ScriptDetailsTypeDef(_RequiredScriptDetailsTypeDef, _OptionalScriptDetailsTypeDef):
     pass
 
-
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
@@ -1236,96 +1645,33 @@
         "LaunchParameters": str,
         "AppBlockArn": str,
         "AttributesToDelete": Sequence[ApplicationAttributeType],
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CopyImageResponseTypeDef = TypedDict(
-    "CopyImageResponseTypeDef",
-    {
-        "DestinationImageName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateImageBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStreamingURLResultTypeDef = TypedDict(
-    "CreateStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUsageReportSubscriptionResultTypeDef = TypedDict(
-    "CreateUsageReportSubscriptionResultTypeDef",
-    {
-        "S3BucketName": str,
-        "Schedule": Literal["DAILY"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedFleetsResultTypeDef = TypedDict(
-    "ListAssociatedFleetsResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedStacksResultTypeDef = TypedDict(
-    "ListAssociatedStacksResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
     "BatchAssociateUserStackRequestRequestTypeDef",
     {
         "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
@@ -1340,15 +1686,15 @@
 )
 
 DescribeUserStackAssociationsResultTypeDef = TypedDict(
     "DescribeUserStackAssociationsResultTypeDef",
     {
         "UserStackAssociations": List[UserStackAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserStackAssociationErrorTypeDef = TypedDict(
     "UserStackAssociationErrorTypeDef",
     {
         "UserStackAssociation": UserStackAssociationTypeDef,
@@ -1370,22 +1716,20 @@
     {
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreateDirectoryConfigRequestRequestTypeDef(
     _RequiredCreateDirectoryConfigRequestRequestTypeDef,
     _OptionalCreateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDirectoryConfigTypeDef = TypedDict(
     "_RequiredDirectoryConfigTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalDirectoryConfigTypeDef = TypedDict(
@@ -1395,19 +1739,17 @@
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CreatedTime": datetime,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
     pass
 
-
 _RequiredUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
@@ -1416,22 +1758,20 @@
         "OrganizationalUnitDistinguishedNames": Sequence[str],
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDirectoryConfigRequestRequestTypeDef(
     _RequiredUpdateDirectoryConfigRequestRequestTypeDef,
     _OptionalUpdateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
@@ -1441,21 +1781,19 @@
     "_OptionalCreateEntitlementRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateEntitlementRequestRequestTypeDef(
     _RequiredCreateEntitlementRequestRequestTypeDef, _OptionalCreateEntitlementRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "StackName": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": List[EntitlementAttributeTypeDef],
@@ -1467,19 +1805,17 @@
         "Description": str,
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
-
 _RequiredUpdateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
     },
 )
@@ -1489,21 +1825,19 @@
         "Description": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
     },
     total=False,
 )
 
-
 class UpdateEntitlementRequestRequestTypeDef(
     _RequiredUpdateEntitlementRequestRequestTypeDef, _OptionalUpdateEntitlementRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -1529,21 +1863,19 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": Sequence[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateImageBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -1561,22 +1893,20 @@
         "AppstreamAgentVersion": str,
         "Tags": Mapping[str, str],
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
     },
     total=False,
 )
 
-
 class CreateImageBuilderRequestRequestTypeDef(
     _RequiredCreateImageBuilderRequestRequestTypeDef,
     _OptionalCreateImageBuilderRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateFleetRequestRequestTypeDef = TypedDict(
     "UpdateFleetRequestRequestTypeDef",
     {
         "ImageName": str,
         "ImageArn": str,
         "Name": str,
         "InstanceType": str,
@@ -1621,21 +1951,19 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateStackRequestRequestTypeDef(
     _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateStackRequestRequestTypeDef = TypedDict(
@@ -1653,170 +1981,19 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
-
-DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
-    {
-        "DirectoryNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "Arns": Sequence[str],
-        "Type": VisibilityTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "StackName": str,
-        "FleetName": str,
-    },
-)
-_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "UserId": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
-    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-):
-    pass
-
-
-DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
-    {
-        "StackName": str,
-        "UserName": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationType": AuthenticationTypeType,
-    },
-)
-_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeUsersRequestDescribeUsersPaginateTypeDef(
-    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
-    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
-    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "FleetName": str,
-    },
-)
-_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
-    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-):
-    pass
-
-
 DescribeFleetsRequestFleetStartedWaitTypeDef = TypedDict(
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     {
         "Names": Sequence[str],
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
@@ -1834,24 +2011,24 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitledApplicationsResultTypeDef = TypedDict(
     "ListEntitledApplicationsResultTypeDef",
     {
         "EntitledApplications": List[EntitledApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFleetTypeDef = TypedDict(
     "_RequiredFleetTypeDef",
     {
         "Arn": str,
@@ -1883,46 +2060,17 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": List[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
-
-_RequiredSessionTypeDef = TypedDict(
-    "_RequiredSessionTypeDef",
-    {
-        "Id": str,
-        "UserId": str,
-        "StackName": str,
-        "FleetName": str,
-        "State": SessionStateType,
-    },
-)
-_OptionalSessionTypeDef = TypedDict(
-    "_OptionalSessionTypeDef",
-    {
-        "ConnectionState": SessionConnectionStateType,
-        "StartTime": datetime,
-        "MaxExpirationTime": datetime,
-        "AuthenticationType": AuthenticationTypeType,
-        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
-    pass
-
-
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -1945,18 +2093,41 @@
         "ImageBuilderErrors": List[ResourceErrorTypeDef],
         "AppstreamAgentVersion": str,
         "AccessEndpoints": List[AccessEndpointTypeDef],
     },
     total=False,
 )
 
-
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
+_RequiredSessionTypeDef = TypedDict(
+    "_RequiredSessionTypeDef",
+    {
+        "Id": str,
+        "UserId": str,
+        "StackName": str,
+        "FleetName": str,
+        "State": SessionStateType,
+    },
+)
+_OptionalSessionTypeDef = TypedDict(
+    "_OptionalSessionTypeDef",
+    {
+        "ConnectionState": SessionConnectionStateType,
+        "StartTime": datetime,
+        "MaxExpirationTime": datetime,
+        "AuthenticationType": AuthenticationTypeType,
+        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
+    pass
 
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
         "imagePermissions": ImagePermissionsTypeDef,
     },
@@ -2004,33 +2175,72 @@
         "AccessEndpoints": List[AccessEndpointTypeDef],
         "EmbedHostDomains": List[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
+CreateAppBlockBuilderResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppBlockBuildersResultTypeDef = TypedDict(
+    "DescribeAppBlockBuildersResultTypeDef",
+    {
+        "AppBlockBuilders": List[AppBlockBuilderTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartAppBlockBuilderResultTypeDef = TypedDict(
+    "StartAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StopAppBlockBuilderResultTypeDef = TypedDict(
+    "StopAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAppBlockBuilderResultTypeDef = TypedDict(
+    "UpdateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeApplicationsResultTypeDef = TypedDict(
     "DescribeApplicationsResultTypeDef",
     {
         "Applications": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImageTypeDef = TypedDict(
     "_RequiredImageTypeDef",
     {
         "Name": str,
@@ -2055,296 +2265,296 @@
         "AppstreamAgentVersion": str,
         "ImagePermissions": ImagePermissionsTypeDef,
         "ImageErrors": List[ResourceErrorTypeDef],
     },
     total=False,
 )
 
-
 class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
     pass
 
-
 UpdateApplicationResultTypeDef = TypedDict(
     "UpdateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
         "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
+        "State": AppBlockStateType,
+        "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
-
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
-
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppBlockRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "Tags": Mapping[str, str],
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
-
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
 ):
     pass
 
-
 BatchAssociateUserStackResultTypeDef = TypedDict(
     "BatchAssociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateUserStackResultTypeDef = TypedDict(
     "BatchDisassociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDirectoryConfigResultTypeDef = TypedDict(
     "CreateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectoryConfigsResultTypeDef = TypedDict(
     "DescribeDirectoryConfigsResultTypeDef",
     {
         "DirectoryConfigs": List[DirectoryConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDirectoryConfigResultTypeDef = TypedDict(
     "UpdateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEntitlementResultTypeDef = TypedDict(
     "CreateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntitlementsResultTypeDef = TypedDict(
     "DescribeEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEntitlementResultTypeDef = TypedDict(
     "UpdateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFleetResultTypeDef = TypedDict(
     "CreateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "Fleets": List[FleetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFleetResultTypeDef = TypedDict(
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSessionsResultTypeDef = TypedDict(
-    "DescribeSessionsResultTypeDef",
-    {
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteImageBuilderResultTypeDef = TypedDict(
     "DeleteImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageBuildersResultTypeDef = TypedDict(
     "DescribeImageBuildersResultTypeDef",
     {
         "ImageBuilders": List[ImageBuilderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartImageBuilderResultTypeDef = TypedDict(
     "StartImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopImageBuilderResultTypeDef = TypedDict(
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeSessionsResultTypeDef = TypedDict(
+    "DescribeSessionsResultTypeDef",
+    {
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsageReportSubscriptionsResultTypeDef = TypedDict(
     "DescribeUsageReportSubscriptionsResultTypeDef",
     {
         "UsageReportSubscriptions": List[UsageReportSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStackResultTypeDef = TypedDict(
     "CreateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStackResultTypeDef = TypedDict(
     "UpdateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUpdatedImageResultTypeDef = TypedDict(
     "CreateUpdatedImageResultTypeDef",
     {
         "image": ImageTypeDef,
         "canUpdateImage": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteImageResultTypeDef = TypedDict(
     "DeleteImageResultTypeDef",
     {
         "Image": ImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppBlockResultTypeDef = TypedDict(
     "CreateAppBlockResultTypeDef",
     {
         "AppBlock": AppBlockTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppBlocksResultTypeDef = TypedDict(
     "DescribeAppBlocksResultTypeDef",
     {
         "AppBlocks": List[AppBlockTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.pyi` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     FleetAttributeType,
     FleetErrorCodeType,
     FleetStateType,
     FleetTypeType,
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -49,105 +53,133 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessEndpointTypeDef",
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    "ResourceErrorTypeDef",
+    "VpcConfigTypeDef",
+    "ErrorDetailsTypeDef",
     "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
+    "CopyImageResponseTypeDef",
+    "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
-    "VpcConfigTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
+    "CreateImageBuilderStreamingURLResultTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
+    "CreateStreamingURLResultTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
+    "CreateUsageReportSubscriptionResultTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteImageBuilderRequestRequestTypeDef",
     "DeleteImagePermissionsRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFleetsRequestRequestTypeDef",
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     "DescribeImageBuildersRequestRequestTypeDef",
     "DescribeImagePermissionsRequestRequestTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
+    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
     "DisableUserRequestRequestTypeDef",
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
-    "ResourceErrorTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
+    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
+    "ListAssociatedFleetsResultTypeDef",
+    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
+    "ListAssociatedStacksResultTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StackErrorTypeDef",
+    "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
+    "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    "AppBlockBuilderTypeDef",
+    "CreateAppBlockBuilderRequestRequestTypeDef",
+    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "AssociateApplicationFleetResultTypeDef",
-    "CopyImageResponseTypeDef",
-    "CreateImageBuilderStreamingURLResultTypeDef",
-    "CreateStreamingURLResultTypeDef",
-    "CreateUsageReportSubscriptionResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
-    "ListAssociatedFleetsResultTypeDef",
-    "ListAssociatedStacksResultTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
     "UserStackAssociationErrorTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
     "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
@@ -155,35 +187,30 @@
     "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
     "DescribeUsersResultTypeDef",
     "ListEntitledApplicationsResultTypeDef",
     "FleetTypeDef",
-    "SessionTypeDef",
     "ImageBuilderTypeDef",
+    "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
+    "CreateAppBlockBuilderResultTypeDef",
+    "DescribeAppBlockBuildersResultTypeDef",
+    "StartAppBlockBuilderResultTypeDef",
+    "StopAppBlockBuilderResultTypeDef",
+    "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
     "ImageTypeDef",
     "UpdateApplicationResultTypeDef",
     "AppBlockTypeDef",
     "CreateAppBlockRequestRequestTypeDef",
     "BatchAssociateUserStackResultTypeDef",
@@ -193,20 +220,20 @@
     "UpdateDirectoryConfigResultTypeDef",
     "CreateEntitlementResultTypeDef",
     "DescribeEntitlementsResultTypeDef",
     "UpdateEntitlementResultTypeDef",
     "CreateFleetResultTypeDef",
     "DescribeFleetsResultTypeDef",
     "UpdateFleetResultTypeDef",
-    "DescribeSessionsResultTypeDef",
     "CreateImageBuilderResultTypeDef",
     "DeleteImageBuilderResultTypeDef",
     "DescribeImageBuildersResultTypeDef",
     "StartImageBuilderResultTypeDef",
     "StopImageBuilderResultTypeDef",
+    "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
@@ -225,25 +252,83 @@
     "_OptionalAccessEndpointTypeDef",
     {
         "VpceId": str,
     },
     total=False,
 )
 
+
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+
+AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
+AppBlockBuilderStateChangeReasonTypeDef = TypedDict(
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    {
+        "Code": Literal["INTERNAL_ERROR"],
+        "Message": str,
+    },
+    total=False,
+)
+
+ResourceErrorTypeDef = TypedDict(
+    "ResourceErrorTypeDef",
+    {
+        "ErrorCode": FleetErrorCodeType,
+        "ErrorMessage": str,
+        "ErrorTimestamp": datetime,
+    },
+    total=False,
+)
+
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
+ErrorDetailsTypeDef = TypedDict(
+    "ErrorDetailsTypeDef",
+    {
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
     {
         "S3Bucket": str,
+    },
+)
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
+    {
         "S3Key": str,
     },
+    total=False,
 )
 
+
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+    pass
+
+
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -268,35 +353,34 @@
     "_OptionalApplicationSettingsTypeDef",
     {
         "SettingsGroup": str,
     },
     total=False,
 )
 
+
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
-AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationFleetRequestRequestTypeDef",
+
+AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     {
-        "FleetName": str,
-        "ApplicationArn": str,
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
+    "AssociateApplicationFleetRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FleetName": str,
+        "ApplicationArn": str,
     },
 )
 
 AssociateApplicationToEntitlementRequestRequestTypeDef = TypedDict(
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     {
         "StackName": str,
@@ -325,19 +409,21 @@
     "_OptionalUserStackAssociationTypeDef",
     {
         "SendEmailNotification": bool,
     },
     total=False,
 )
 
+
 class UserStackAssociationTypeDef(
     _RequiredUserStackAssociationTypeDef, _OptionalUserStackAssociationTypeDef
 ):
     pass
 
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusType,
         "CertificateAuthorityArn": str,
     },
     total=False,
@@ -355,19 +441,21 @@
         "Running": int,
         "InUse": int,
         "Available": int,
     },
     total=False,
 )
 
+
 class ComputeCapacityStatusTypeDef(
     _RequiredComputeCapacityStatusTypeDef, _OptionalComputeCapacityStatusTypeDef
 ):
     pass
 
+
 ComputeCapacityTypeDef = TypedDict(
     "ComputeCapacityTypeDef",
     {
         "DesiredInstances": int,
     },
 )
 
@@ -383,19 +471,60 @@
     "_OptionalCopyImageRequestRequestTypeDef",
     {
         "DestinationImageDescription": str,
     },
     total=False,
 )
 
+
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
+
+CopyImageResponseTypeDef = TypedDict(
+    "CopyImageResponseTypeDef",
+    {
+        "DestinationImageName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "AppBlockBuilderName": str,
+    },
+)
+_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "Validity": int,
+    },
+    total=False,
+)
+
+
+class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+):
+    pass
+
+
+CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -413,43 +542,45 @@
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedName": str,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Validity": int,
     },
     total=False,
 )
 
+
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
+
+CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateImageBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStorageConnectorTypeDef = TypedDict(
     "_RequiredStorageConnectorTypeDef",
     {
         "ConnectorType": StorageConnectorTypeType,
     },
 )
 _OptionalStorageConnectorTypeDef = TypedDict(
@@ -457,17 +588,19 @@
     {
         "ResourceIdentifier": str,
         "Domains": Sequence[str],
     },
     total=False,
 )
 
+
 class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
     pass
 
+
 StreamingExperienceSettingsTypeDef = TypedDict(
     "StreamingExperienceSettingsTypeDef",
     {
         "PreferredProtocol": PreferredProtocolType,
     },
     total=False,
 )
@@ -494,20 +627,31 @@
         "ApplicationId": str,
         "Validity": int,
         "SessionContext": str,
     },
     total=False,
 )
 
+
 class CreateStreamingURLRequestRequestTypeDef(
     _RequiredCreateStreamingURLRequestRequestTypeDef,
     _OptionalCreateStreamingURLRequestRequestTypeDef,
 ):
     pass
 
+
+CreateStreamingURLResultTypeDef = TypedDict(
+    "CreateStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUpdatedImageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUpdatedImageRequestRequestTypeDef",
     {
         "existingImageName": str,
         "newImageName": str,
     },
 )
@@ -518,20 +662,31 @@
         "newImageDisplayName": str,
         "newImageTags": Mapping[str, str],
         "dryRun": bool,
     },
     total=False,
 )
 
+
 class CreateUpdatedImageRequestRequestTypeDef(
     _RequiredCreateUpdatedImageRequestRequestTypeDef,
     _OptionalCreateUpdatedImageRequestRequestTypeDef,
 ):
     pass
 
+
+CreateUsageReportSubscriptionResultTypeDef = TypedDict(
+    "CreateUsageReportSubscriptionResultTypeDef",
+    {
+        "S3BucketName": str,
+        "Schedule": Literal["DAILY"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -541,19 +696,28 @@
         "MessageAction": MessageActionType,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
+DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 DeleteAppBlockRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -619,14 +783,35 @@
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+DescribeAppBlockBuildersRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeAppBlocksRequestRequestTypeDef = TypedDict(
     "DescribeAppBlocksRequestRequestTypeDef",
     {
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -650,20 +835,19 @@
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DirectoryNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDirectoryConfigsRequestRequestTypeDef = TypedDict(
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     {
@@ -686,20 +870,31 @@
         "Name": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeEntitlementsRequestRequestTypeDef(
     _RequiredDescribeEntitlementsRequestRequestTypeDef,
     _OptionalDescribeEntitlementsRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -710,14 +905,23 @@
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeImageBuildersRequestRequestTypeDef = TypedDict(
     "DescribeImageBuildersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -736,32 +940,70 @@
         "MaxResults": int,
         "SharedAwsAccountIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeImagePermissionsRequestRequestTypeDef(
     _RequiredDescribeImagePermissionsRequestRequestTypeDef,
     _OptionalDescribeImagePermissionsRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "Arns": Sequence[str],
+        "Type": VisibilityTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeImagesRequestRequestTypeDef = TypedDict(
     "DescribeImagesRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "Arns": Sequence[str],
         "Type": VisibilityTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    {
+        "StackName": str,
+        "FleetName": str,
+    },
+)
+_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    {
+        "UserId": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
+    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "StackName": str,
         "FleetName": str,
     },
 )
@@ -772,19 +1014,30 @@
         "NextToken": str,
         "Limit": int,
         "AuthenticationType": AuthenticationTypeType,
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
+
+DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeStacksRequestRequestTypeDef = TypedDict(
     "DescribeStacksRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -795,26 +1048,59 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
+    {
+        "StackName": str,
+        "UserName": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUserStackAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     {
         "StackName": str,
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationType": AuthenticationTypeType,
+    },
+)
+_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeUsersRequestDescribeUsersPaginateTypeDef(
+    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
+    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeUsersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalDescribeUsersRequestRequestTypeDef = TypedDict(
@@ -822,19 +1108,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeUsersRequestRequestTypeDef(
     _RequiredDescribeUsersRequestRequestTypeDef, _OptionalDescribeUsersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalUserTypeDef = TypedDict(
@@ -847,25 +1135,35 @@
         "FirstName": str,
         "LastName": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
+
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
+
 DisableUserRequestRequestTypeDef = TypedDict(
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
 DisassociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "DisassociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -932,24 +1230,14 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
-ResourceErrorTypeDef = TypedDict(
-    "ResourceErrorTypeDef",
-    {
-        "ErrorCode": FleetErrorCodeType,
-        "ErrorMessage": str,
-        "ErrorTimestamp": datetime,
-    },
-    total=False,
-)
-
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -969,54 +1257,120 @@
     {
         "ErrorCode": UsageReportExecutionErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
+    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedFleetsRequestRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_OptionalListAssociatedFleetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociatedFleetsRequestRequestTypeDef(
     _RequiredListAssociatedFleetsRequestRequestTypeDef,
     _OptionalListAssociatedFleetsRequestRequestTypeDef,
 ):
     pass
 
+
+ListAssociatedFleetsResultTypeDef = TypedDict(
+    "ListAssociatedFleetsResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
+    {
+        "FleetName": str,
+    },
+)
+_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
+    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociatedStacksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedStacksRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalListAssociatedStacksRequestRequestTypeDef = TypedDict(
     "_OptionalListAssociatedStacksRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociatedStacksRequestRequestTypeDef(
     _RequiredListAssociatedStacksRequestRequestTypeDef,
     _OptionalListAssociatedStacksRequestRequestTypeDef,
 ):
     pass
 
+
+ListAssociatedStacksResultTypeDef = TypedDict(
+    "ListAssociatedStacksResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListEntitledApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitledApplicationsRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
     },
 )
@@ -1025,36 +1379,74 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEntitledApplicationsRequestRequestTypeDef(
     _RequiredListEntitledApplicationsRequestRequestTypeDef,
     _OptionalListEntitledApplicationsRequestRequestTypeDef,
 ):
     pass
 
+
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
 StackErrorTypeDef = TypedDict(
     "StackErrorTypeDef",
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StartAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StartFleetRequestRequestTypeDef = TypedDict(
     "StartFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1068,19 +1460,28 @@
     "_OptionalStartImageBuilderRequestRequestTypeDef",
     {
         "AppstreamAgentVersion": str,
     },
     total=False,
 )
 
+
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
+
+StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StopAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StopFleetRequestRequestTypeDef = TypedDict(
     "StopFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1103,14 +1504,122 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredAppBlockBuilderTypeDef = TypedDict(
+    "_RequiredAppBlockBuilderTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "State": AppBlockBuilderStateType,
+    },
+)
+_OptionalAppBlockBuilderTypeDef = TypedDict(
+    "_OptionalAppBlockBuilderTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "CreatedTime": datetime,
+        "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
+        "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
+        "AccessEndpoints": List[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+
+class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
+    pass
+
+
+_RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+)
+_OptionalCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Tags": Mapping[str, str],
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Platform": PlatformTypeType,
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
+    },
+    total=False,
+)
+
+
+class UpdateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
+
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
@@ -1148,19 +1657,21 @@
         "WorkingDirectory": str,
         "LaunchParameters": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredScriptDetailsTypeDef = TypedDict(
     "_RequiredScriptDetailsTypeDef",
     {
         "ScriptS3Location": S3LocationTypeDef,
         "ExecutablePath": str,
         "TimeoutInSeconds": int,
     },
@@ -1169,17 +1680,19 @@
     "_OptionalScriptDetailsTypeDef",
     {
         "ExecutableParameters": str,
     },
     total=False,
 )
 
+
 class ScriptDetailsTypeDef(_RequiredScriptDetailsTypeDef, _OptionalScriptDetailsTypeDef):
     pass
 
+
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
@@ -1193,94 +1706,35 @@
         "LaunchParameters": str,
         "AppBlockArn": str,
         "AttributesToDelete": Sequence[ApplicationAttributeType],
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CopyImageResponseTypeDef = TypedDict(
-    "CopyImageResponseTypeDef",
-    {
-        "DestinationImageName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateImageBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStreamingURLResultTypeDef = TypedDict(
-    "CreateStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUsageReportSubscriptionResultTypeDef = TypedDict(
-    "CreateUsageReportSubscriptionResultTypeDef",
-    {
-        "S3BucketName": str,
-        "Schedule": Literal["DAILY"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedFleetsResultTypeDef = TypedDict(
-    "ListAssociatedFleetsResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedStacksResultTypeDef = TypedDict(
-    "ListAssociatedStacksResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
     "BatchAssociateUserStackRequestRequestTypeDef",
     {
         "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
@@ -1295,15 +1749,15 @@
 )
 
 DescribeUserStackAssociationsResultTypeDef = TypedDict(
     "DescribeUserStackAssociationsResultTypeDef",
     {
         "UserStackAssociations": List[UserStackAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserStackAssociationErrorTypeDef = TypedDict(
     "UserStackAssociationErrorTypeDef",
     {
         "UserStackAssociation": UserStackAssociationTypeDef,
@@ -1325,20 +1779,22 @@
     {
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreateDirectoryConfigRequestRequestTypeDef(
     _RequiredCreateDirectoryConfigRequestRequestTypeDef,
     _OptionalCreateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDirectoryConfigTypeDef = TypedDict(
     "_RequiredDirectoryConfigTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalDirectoryConfigTypeDef = TypedDict(
@@ -1348,17 +1804,19 @@
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CreatedTime": datetime,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
     pass
 
+
 _RequiredUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
@@ -1367,20 +1825,22 @@
         "OrganizationalUnitDistinguishedNames": Sequence[str],
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDirectoryConfigRequestRequestTypeDef(
     _RequiredUpdateDirectoryConfigRequestRequestTypeDef,
     _OptionalUpdateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
@@ -1390,19 +1850,21 @@
     "_OptionalCreateEntitlementRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateEntitlementRequestRequestTypeDef(
     _RequiredCreateEntitlementRequestRequestTypeDef, _OptionalCreateEntitlementRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "StackName": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": List[EntitlementAttributeTypeDef],
@@ -1414,17 +1876,19 @@
         "Description": str,
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
+
 _RequiredUpdateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
     },
 )
@@ -1434,19 +1898,21 @@
         "Description": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
     },
     total=False,
 )
 
+
 class UpdateEntitlementRequestRequestTypeDef(
     _RequiredUpdateEntitlementRequestRequestTypeDef, _OptionalUpdateEntitlementRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -1472,19 +1938,21 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": Sequence[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateImageBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -1502,20 +1970,22 @@
         "AppstreamAgentVersion": str,
         "Tags": Mapping[str, str],
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
     },
     total=False,
 )
 
+
 class CreateImageBuilderRequestRequestTypeDef(
     _RequiredCreateImageBuilderRequestRequestTypeDef,
     _OptionalCreateImageBuilderRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateFleetRequestRequestTypeDef = TypedDict(
     "UpdateFleetRequestRequestTypeDef",
     {
         "ImageName": str,
         "ImageArn": str,
         "Name": str,
         "InstanceType": str,
@@ -1560,19 +2030,21 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateStackRequestRequestTypeDef(
     _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateStackRequestRequestTypeDef = TypedDict(
@@ -1590,159 +2062,20 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
-DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
-    {
-        "DirectoryNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "Arns": Sequence[str],
-        "Type": VisibilityTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "StackName": str,
-        "FleetName": str,
-    },
-)
-_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "UserId": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
-    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-):
-    pass
-
-DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
-    {
-        "StackName": str,
-        "UserName": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationType": AuthenticationTypeType,
-    },
-)
-_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeUsersRequestDescribeUsersPaginateTypeDef(
-    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
-    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
-):
-    pass
-
-_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
-    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "FleetName": str,
-    },
-)
-_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
-    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-):
-    pass
 
 DescribeFleetsRequestFleetStartedWaitTypeDef = TypedDict(
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     {
         "Names": Sequence[str],
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
@@ -1761,24 +2094,24 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitledApplicationsResultTypeDef = TypedDict(
     "ListEntitledApplicationsResultTypeDef",
     {
         "EntitledApplications": List[EntitledApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFleetTypeDef = TypedDict(
     "_RequiredFleetTypeDef",
     {
         "Arn": str,
@@ -1810,41 +2143,18 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": List[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
-_RequiredSessionTypeDef = TypedDict(
-    "_RequiredSessionTypeDef",
-    {
-        "Id": str,
-        "UserId": str,
-        "StackName": str,
-        "FleetName": str,
-        "State": SessionStateType,
-    },
-)
-_OptionalSessionTypeDef = TypedDict(
-    "_OptionalSessionTypeDef",
-    {
-        "ConnectionState": SessionConnectionStateType,
-        "StartTime": datetime,
-        "MaxExpirationTime": datetime,
-        "AuthenticationType": AuthenticationTypeType,
-        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
-    pass
 
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
@@ -1868,17 +2178,46 @@
         "ImageBuilderErrors": List[ResourceErrorTypeDef],
         "AppstreamAgentVersion": str,
         "AccessEndpoints": List[AccessEndpointTypeDef],
     },
     total=False,
 )
 
+
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
+
+_RequiredSessionTypeDef = TypedDict(
+    "_RequiredSessionTypeDef",
+    {
+        "Id": str,
+        "UserId": str,
+        "StackName": str,
+        "FleetName": str,
+        "State": SessionStateType,
+    },
+)
+_OptionalSessionTypeDef = TypedDict(
+    "_OptionalSessionTypeDef",
+    {
+        "ConnectionState": SessionConnectionStateType,
+        "StartTime": datetime,
+        "MaxExpirationTime": datetime,
+        "AuthenticationType": AuthenticationTypeType,
+        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
+    pass
+
+
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
         "imagePermissions": ImagePermissionsTypeDef,
     },
 )
@@ -1925,31 +2264,74 @@
         "AccessEndpoints": List[AccessEndpointTypeDef],
         "EmbedHostDomains": List[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
+
+CreateAppBlockBuilderResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppBlockBuildersResultTypeDef = TypedDict(
+    "DescribeAppBlockBuildersResultTypeDef",
+    {
+        "AppBlockBuilders": List[AppBlockBuilderTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartAppBlockBuilderResultTypeDef = TypedDict(
+    "StartAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StopAppBlockBuilderResultTypeDef = TypedDict(
+    "StopAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAppBlockBuilderResultTypeDef = TypedDict(
+    "UpdateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeApplicationsResultTypeDef = TypedDict(
     "DescribeApplicationsResultTypeDef",
     {
         "Applications": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImageTypeDef = TypedDict(
     "_RequiredImageTypeDef",
     {
         "Name": str,
@@ -1974,290 +2356,302 @@
         "AppstreamAgentVersion": str,
         "ImagePermissions": ImagePermissionsTypeDef,
         "ImageErrors": List[ResourceErrorTypeDef],
     },
     total=False,
 )
 
+
 class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
     pass
 
+
 UpdateApplicationResultTypeDef = TypedDict(
     "UpdateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
         "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
+        "State": AppBlockStateType,
+        "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
+
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
+
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppBlockRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "Tags": Mapping[str, str],
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
+
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
 ):
     pass
 
+
 BatchAssociateUserStackResultTypeDef = TypedDict(
     "BatchAssociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateUserStackResultTypeDef = TypedDict(
     "BatchDisassociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDirectoryConfigResultTypeDef = TypedDict(
     "CreateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectoryConfigsResultTypeDef = TypedDict(
     "DescribeDirectoryConfigsResultTypeDef",
     {
         "DirectoryConfigs": List[DirectoryConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDirectoryConfigResultTypeDef = TypedDict(
     "UpdateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEntitlementResultTypeDef = TypedDict(
     "CreateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntitlementsResultTypeDef = TypedDict(
     "DescribeEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEntitlementResultTypeDef = TypedDict(
     "UpdateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFleetResultTypeDef = TypedDict(
     "CreateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "Fleets": List[FleetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFleetResultTypeDef = TypedDict(
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSessionsResultTypeDef = TypedDict(
-    "DescribeSessionsResultTypeDef",
-    {
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteImageBuilderResultTypeDef = TypedDict(
     "DeleteImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageBuildersResultTypeDef = TypedDict(
     "DescribeImageBuildersResultTypeDef",
     {
         "ImageBuilders": List[ImageBuilderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartImageBuilderResultTypeDef = TypedDict(
     "StartImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopImageBuilderResultTypeDef = TypedDict(
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeSessionsResultTypeDef = TypedDict(
+    "DescribeSessionsResultTypeDef",
+    {
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsageReportSubscriptionsResultTypeDef = TypedDict(
     "DescribeUsageReportSubscriptionsResultTypeDef",
     {
         "UsageReportSubscriptions": List[UsageReportSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStackResultTypeDef = TypedDict(
     "CreateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStackResultTypeDef = TypedDict(
     "UpdateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUpdatedImageResultTypeDef = TypedDict(
     "CreateUpdatedImageResultTypeDef",
     {
         "image": ImageTypeDef,
         "canUpdateImage": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteImageResultTypeDef = TypedDict(
     "DeleteImageResultTypeDef",
     {
         "Image": ImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppBlockResultTypeDef = TypedDict(
     "CreateAppBlockResultTypeDef",
     {
         "AppBlock": AppBlockTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppBlocksResultTypeDef = TypedDict(
     "DescribeAppBlocksResultTypeDef",
     {
         "AppBlocks": List[AppBlockTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.py` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.pyi` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/PKG-INFO` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.26.59
-Summary: Type annotations for boto3.AppStream 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppStream 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,14 +349,19 @@
 `mypy_boto3_appstream.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_appstream.literals import (
     AccessEndpointTypeType,
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderPlatformTypeType,
+    AppBlockBuilderStateChangeReasonCodeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     AppVisibilityType,
     ApplicationAttributeType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     DescribeDirectoryConfigsPaginatorName,
     DescribeFleetsPaginatorName,
     DescribeImageBuildersPaginatorName,
@@ -374,14 +379,15 @@
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     ListAssociatedFleetsPaginatorName,
     ListAssociatedStacksPaginatorName,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -410,103 +416,130 @@
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
+    AppBlockBuilderAppBlockAssociationTypeDef,
+    AppBlockBuilderStateChangeReasonTypeDef,
+    ResourceErrorTypeDef,
+    VpcConfigTypeDef,
+    ErrorDetailsTypeDef,
     S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
+    CopyImageResponseTypeDef,
+    CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
-    VpcConfigTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
+    CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
+    CreateStreamingURLResultTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
+    CreateUsageReportSubscriptionResultTypeDef,
     CreateUserRequestRequestTypeDef,
+    DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteImageBuilderRequestRequestTypeDef,
     DeleteImagePermissionsRequestRequestTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
+    DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
+    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeFleetsRequestRequestTypeDef,
+    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImageBuildersRequestRequestTypeDef,
     DescribeImagePermissionsRequestRequestTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
+    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
+    DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
+    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
     DisableUserRequestRequestTypeDef,
+    DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
-    ResourceErrorTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
+    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
+    ListAssociatedFleetsResultTypeDef,
+    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
+    ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StackErrorTypeDef,
+    StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
+    StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    AppBlockBuilderTypeDef,
+    CreateAppBlockBuilderRequestRequestTypeDef,
+    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     AssociateApplicationFleetResultTypeDef,
-    CopyImageResponseTypeDef,
-    CreateImageBuilderStreamingURLResultTypeDef,
-    CreateStreamingURLResultTypeDef,
-    CreateUsageReportSubscriptionResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
-    ListAssociatedFleetsResultTypeDef,
-    ListAssociatedStacksResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
     UserStackAssociationErrorTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
     DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
@@ -514,35 +547,30 @@
     EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
-    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
-    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
-    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    DescribeStacksRequestDescribeStacksPaginateTypeDef,
-    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
-    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
     DescribeUsersResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     FleetTypeDef,
-    SessionTypeDef,
     ImageBuilderTypeDef,
+    SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
+    StartAppBlockBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
     ImageTypeDef,
     UpdateApplicationResultTypeDef,
     AppBlockTypeDef,
     CreateAppBlockRequestRequestTypeDef,
     BatchAssociateUserStackResultTypeDef,
@@ -552,20 +580,20 @@
     UpdateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     UpdateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     DescribeFleetsResultTypeDef,
     UpdateFleetResultTypeDef,
-    DescribeSessionsResultTypeDef,
     CreateImageBuilderResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DescribeImageBuildersResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
+    DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
@@ -582,42 +610,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/SOURCES.txt` & `mypy-boto3-appstream-1.27.0/mypy_boto3_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.59/setup.py` & `mypy-boto3-appstream-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-appstream.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appstream",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppStream 1.26.59 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.AppStream 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```


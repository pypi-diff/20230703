# Comparing `tmp/mypy-boto3-securitylake-1.26.92.tar.gz` & `tmp/mypy-boto3-securitylake-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securitylake-1.26.92.tar", last modified: Wed Mar 15 19:32:09 2023, max compression
+gzip compressed data, was "mypy-boto3-securitylake-1.27.0.tar", last modified: Mon Jul  3 19:51:26 2023, max compression
```

## Comparing `mypy-boto3-securitylake-1.26.92.tar` & `mypy-boto3-securitylake-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.763555 mypy-boto3-securitylake-1.26.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-03-15 19:32:09.763555 mypy-boto3-securitylake-1.26.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.755555 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-03-15 19:32:01.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.763555 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-03-15 19:32:09.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-15 19:32:09.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 19:32:09.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-15 19:32:09.000000 mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 19:32:09.763555 mypy-boto3-securitylake-1.26.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-15 19:32:00.000000 mypy-boto3-securitylake-1.26.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.399980 mypy-boto3-securitylake-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-07-03 19:51:26.399980 mypy-boto3-securitylake-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.391980 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23969 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-03 19:47:52.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-03 19:47:52.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-03 19:47:52.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-07-03 19:47:52.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-07-03 19:47:52.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.399980 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-07-03 19:51:26.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:51:26.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:26.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:26.000000 mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:26.399980 mypy-boto3-securitylake-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:47:51.000000 mypy-boto3-securitylake-1.27.0/setup.py
```

### Comparing `mypy-boto3-securitylake-1.26.92/LICENSE` & `mypy-boto3-securitylake-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-securitylake-1.26.92/PKG-INFO` & `mypy-boto3-securitylake-1.27.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securitylake
-Version: 1.26.92
-Summary: Type annotations for boto3.SecurityLake 1.26.92 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SecurityLake 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-securitylake"></a>
 
 # mypy-boto3-securitylake
 
 [![PyPI - mypy-boto3-securitylake](https://img.shields.io/pypi/v/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,29 +280,29 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_securitylake import SecurityLakeClient
 from mypy_boto3_securitylake.paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 
 client: SecurityLakeClient = Session().client("securitylake")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
-get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator(
-    "get_datalake_status"
+get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator(
+    "get_data_lake_sources"
 )
-list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator(
-    "list_datalake_exceptions"
+list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator(
+    "list_data_lake_exceptions"
 )
 list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
 list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
 ```
 
 <a id="literals"></a>
 
@@ -310,29 +310,23 @@
 
 `mypy_boto3_securitylake.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securitylake.literals import (
     AccessTypeType,
-    AwsLogSourceTypeType,
-    DimensionType,
-    EndpointProtocolType,
-    GetDatalakeStatusPaginatorName,
-    HttpsMethodType,
-    ListDatalakeExceptionsPaginatorName,
+    AwsLogSourceNameType,
+    DataLakeStatusType,
+    GetDataLakeSourcesPaginatorName,
+    HttpMethodType,
+    ListDataLakeExceptionsPaginatorName,
     ListLogSourcesPaginatorName,
     ListSubscribersPaginatorName,
-    OcsfEventClassType,
-    RegionType,
-    SourceStatusType,
-    StorageClassType,
-    SubscriptionProtocolTypeType,
-    SubscriptionStatusType,
-    settingsStatusType,
+    SourceCollectionStatusType,
+    SubscriberStatusType,
     SecurityLakeServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -346,117 +340,129 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
-    LogsStatusTypeDef,
-    AutoEnableNewRegionConfigurationTypeDef,
-    CreateAwsLogSourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateCustomLogSourceRequestRequestTypeDef,
-    CreateDatalakeDelegatedAdminRequestRequestTypeDef,
-    CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef,
-    SourceTypeTypeDef,
-    CreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    DeleteAwsLogSourceRequestRequestTypeDef,
+    AwsIdentityTypeDef,
+    AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    CustomLogSourceAttributesTypeDef,
+    CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderTypeDef,
+    DataLakeEncryptionConfigurationTypeDef,
+    DataLakeReplicationConfigurationTypeDef,
+    DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationTypeDef,
+    DataLakeLifecycleTransitionTypeDef,
+    DataLakeSourceStatusTypeDef,
+    DataLakeUpdateExceptionTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
-    DeleteDatalakeDelegatedAdminRequestRequestTypeDef,
+    DeleteDataLakeRequestRequestTypeDef,
+    DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    FailuresTypeDef,
-    ProtocolAndNotificationEndpointTypeDef,
-    PaginatorConfigTypeDef,
-    GetDatalakeStatusRequestRequestTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
-    RetentionSettingTypeDef,
-    LastUpdateFailureTypeDef,
-    ListDatalakeExceptionsRequestRequestTypeDef,
-    ListLogSourcesRequestRequestTypeDef,
+    HttpsNotificationConfigurationTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListDataLakeExceptionsRequestRequestTypeDef,
+    ListDataLakesRequestRequestTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    UpdateDatalakeExceptionsExpiryRequestRequestTypeDef,
-    UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef,
-    UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    AccountSourcesTypeDef,
-    CreateDatalakeAutoEnableRequestRequestTypeDef,
-    DeleteDatalakeAutoEnableRequestRequestTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
+    CreateAwsLogSourceRequestRequestTypeDef,
+    DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationTypeDef,
+    DataLakeSourceTypeDef,
+    DataLakeUpdateStatusTypeDef,
+    NotificationConfigurationTypeDef,
+    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
+    CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
-    CreateSubscriberResponseTypeDef,
-    CreateSubscriptionNotificationConfigurationResponseTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
-    DeleteCustomLogSourceResponseTypeDef,
-    DeleteDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeAutoEnableResponseTypeDef,
-    GetDatalakeExceptionsExpiryResponseTypeDef,
-    ListLogSourcesResponseTypeDef,
-    UpdateSubscriptionNotificationConfigurationResponseTypeDef,
+    LogSourceResourceTypeDef,
+    DataLakeConfigurationTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
+    DataLakeResourceTypeDef,
+    CreateSubscriberNotificationRequestRequestTypeDef,
+    UpdateSubscriberNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
+    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
+    ListLogSourcesRequestRequestTypeDef,
+    LogSourceTypeDef,
     SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
-    FailuresResponseTypeDef,
-    GetDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef,
-    ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef,
-    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
-    LakeConfigurationRequestTypeDef,
-    UpdateStatusTypeDef,
-    GetDatalakeStatusResponseTypeDef,
+    CreateDataLakeRequestRequestTypeDef,
+    UpdateDataLakeRequestRequestTypeDef,
+    CreateDataLakeResponseTypeDef,
+    ListDataLakesResponseTypeDef,
+    UpdateDataLakeResponseTypeDef,
+    ListLogSourcesResponseTypeDef,
+    CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
-    CreateDatalakeRequestRequestTypeDef,
-    UpdateDatalakeRequestRequestTypeDef,
-    LakeConfigurationResponseTypeDef,
-    GetDatalakeResponseTypeDef,
 )
 
 
-def get_structure() -> LogsStatusTypeDef:
+def get_structure() -> AwsIdentityTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-securitylake-1.26.92/README.md` & `mypy-boto3-securitylake-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-securitylake"></a>
 
 # mypy-boto3-securitylake
 
 [![PyPI - mypy-boto3-securitylake](https://img.shields.io/pypi/v/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -248,29 +248,29 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_securitylake import SecurityLakeClient
 from mypy_boto3_securitylake.paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 
 client: SecurityLakeClient = Session().client("securitylake")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
-get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator(
-    "get_datalake_status"
+get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator(
+    "get_data_lake_sources"
 )
-list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator(
-    "list_datalake_exceptions"
+list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator(
+    "list_data_lake_exceptions"
 )
 list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
 list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
 ```
 
 <a id="literals"></a>
 
@@ -278,29 +278,23 @@
 
 `mypy_boto3_securitylake.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securitylake.literals import (
     AccessTypeType,
-    AwsLogSourceTypeType,
-    DimensionType,
-    EndpointProtocolType,
-    GetDatalakeStatusPaginatorName,
-    HttpsMethodType,
-    ListDatalakeExceptionsPaginatorName,
+    AwsLogSourceNameType,
+    DataLakeStatusType,
+    GetDataLakeSourcesPaginatorName,
+    HttpMethodType,
+    ListDataLakeExceptionsPaginatorName,
     ListLogSourcesPaginatorName,
     ListSubscribersPaginatorName,
-    OcsfEventClassType,
-    RegionType,
-    SourceStatusType,
-    StorageClassType,
-    SubscriptionProtocolTypeType,
-    SubscriptionStatusType,
-    settingsStatusType,
+    SourceCollectionStatusType,
+    SubscriberStatusType,
     SecurityLakeServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -314,117 +308,129 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
-    LogsStatusTypeDef,
-    AutoEnableNewRegionConfigurationTypeDef,
-    CreateAwsLogSourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateCustomLogSourceRequestRequestTypeDef,
-    CreateDatalakeDelegatedAdminRequestRequestTypeDef,
-    CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef,
-    SourceTypeTypeDef,
-    CreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    DeleteAwsLogSourceRequestRequestTypeDef,
+    AwsIdentityTypeDef,
+    AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    CustomLogSourceAttributesTypeDef,
+    CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderTypeDef,
+    DataLakeEncryptionConfigurationTypeDef,
+    DataLakeReplicationConfigurationTypeDef,
+    DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationTypeDef,
+    DataLakeLifecycleTransitionTypeDef,
+    DataLakeSourceStatusTypeDef,
+    DataLakeUpdateExceptionTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
-    DeleteDatalakeDelegatedAdminRequestRequestTypeDef,
+    DeleteDataLakeRequestRequestTypeDef,
+    DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    FailuresTypeDef,
-    ProtocolAndNotificationEndpointTypeDef,
-    PaginatorConfigTypeDef,
-    GetDatalakeStatusRequestRequestTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
-    RetentionSettingTypeDef,
-    LastUpdateFailureTypeDef,
-    ListDatalakeExceptionsRequestRequestTypeDef,
-    ListLogSourcesRequestRequestTypeDef,
+    HttpsNotificationConfigurationTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListDataLakeExceptionsRequestRequestTypeDef,
+    ListDataLakesRequestRequestTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    UpdateDatalakeExceptionsExpiryRequestRequestTypeDef,
-    UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef,
-    UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    AccountSourcesTypeDef,
-    CreateDatalakeAutoEnableRequestRequestTypeDef,
-    DeleteDatalakeAutoEnableRequestRequestTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
+    CreateAwsLogSourceRequestRequestTypeDef,
+    DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationTypeDef,
+    DataLakeSourceTypeDef,
+    DataLakeUpdateStatusTypeDef,
+    NotificationConfigurationTypeDef,
+    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
+    CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
-    CreateSubscriberResponseTypeDef,
-    CreateSubscriptionNotificationConfigurationResponseTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
-    DeleteCustomLogSourceResponseTypeDef,
-    DeleteDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeAutoEnableResponseTypeDef,
-    GetDatalakeExceptionsExpiryResponseTypeDef,
-    ListLogSourcesResponseTypeDef,
-    UpdateSubscriptionNotificationConfigurationResponseTypeDef,
+    LogSourceResourceTypeDef,
+    DataLakeConfigurationTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
+    DataLakeResourceTypeDef,
+    CreateSubscriberNotificationRequestRequestTypeDef,
+    UpdateSubscriberNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
+    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
+    ListLogSourcesRequestRequestTypeDef,
+    LogSourceTypeDef,
     SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
-    FailuresResponseTypeDef,
-    GetDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef,
-    ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef,
-    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
-    LakeConfigurationRequestTypeDef,
-    UpdateStatusTypeDef,
-    GetDatalakeStatusResponseTypeDef,
+    CreateDataLakeRequestRequestTypeDef,
+    UpdateDataLakeRequestRequestTypeDef,
+    CreateDataLakeResponseTypeDef,
+    ListDataLakesResponseTypeDef,
+    UpdateDataLakeResponseTypeDef,
+    ListLogSourcesResponseTypeDef,
+    CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
-    CreateDatalakeRequestRequestTypeDef,
-    UpdateDatalakeRequestRequestTypeDef,
-    LakeConfigurationResponseTypeDef,
-    GetDatalakeResponseTypeDef,
 )
 
 
-def get_structure() -> LogsStatusTypeDef:
+def get_structure() -> AwsIdentityTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/__init__.py` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_securitylake import (
         Client,
-        GetDatalakeStatusPaginator,
-        ListDatalakeExceptionsPaginator,
+        GetDataLakeSourcesPaginator,
+        ListDataLakeExceptionsPaginator,
         ListLogSourcesPaginator,
         ListSubscribersPaginator,
         SecurityLakeClient,
     )
 
     session = Session()
     client: SecurityLakeClient = session.client("securitylake")
 
-    get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator("get_datalake_status")
-    list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator("list_datalake_exceptions")
+    get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")
+    list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator("list_data_lake_exceptions")
     list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
     list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
     ```
 """
 from .client import SecurityLakeClient
 from .paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 
 Client = SecurityLakeClient
 
 
 __all__ = (
     "Client",
-    "GetDatalakeStatusPaginator",
-    "ListDatalakeExceptionsPaginator",
+    "GetDataLakeSourcesPaginator",
+    "ListDataLakeExceptionsPaginator",
     "ListLogSourcesPaginator",
     "ListSubscribersPaginator",
     "SecurityLakeClient",
 )
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/__init__.pyi` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_securitylake import (
         Client,
-        GetDatalakeStatusPaginator,
-        ListDatalakeExceptionsPaginator,
+        GetDataLakeSourcesPaginator,
+        ListDataLakeExceptionsPaginator,
         ListLogSourcesPaginator,
         ListSubscribersPaginator,
         SecurityLakeClient,
     )
 
     session = Session()
     client: SecurityLakeClient = session.client("securitylake")
 
-    get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator("get_datalake_status")
-    list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator("list_datalake_exceptions")
+    get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")
+    list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator("list_data_lake_exceptions")
     list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
     list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
     ```
 """
 from .client import SecurityLakeClient
 from .paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 
 Client = SecurityLakeClient
 
 __all__ = (
     "Client",
-    "GetDatalakeStatusPaginator",
-    "ListDatalakeExceptionsPaginator",
+    "GetDataLakeSourcesPaginator",
+    "ListDataLakeExceptionsPaginator",
     "ListLogSourcesPaginator",
     "ListSubscribersPaginator",
     "SecurityLakeClient",
 )
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/__main__.py` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityLake 1.26.92\nVersion:         1.26.92\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.SecurityLake 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.92")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/client.py` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,50 +14,46 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import (
-    AccessTypeType,
-    DimensionType,
-    HttpsMethodType,
-    OcsfEventClassType,
-    RegionType,
-    SubscriptionProtocolTypeType,
-)
+from .literals import AccessTypeType
 from .paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 from .type_defs import (
-    AutoEnableNewRegionConfigurationTypeDef,
+    AwsIdentityTypeDef,
+    AwsLogSourceConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    CreateDataLakeResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
     CreateSubscriberResponseTypeDef,
-    CreateSubscriptionNotificationConfigurationResponseTypeDef,
+    CustomLogSourceConfigurationTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    DataLakeConfigurationTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
-    DeleteCustomLogSourceResponseTypeDef,
-    DeleteDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeAutoEnableResponseTypeDef,
-    GetDatalakeExceptionsExpiryResponseTypeDef,
-    GetDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeResponseTypeDef,
-    GetDatalakeStatusResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
-    LakeConfigurationRequestTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
+    ListDataLakesResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
-    SourceTypeTypeDef,
+    LogSourceResourceTypeDef,
+    NotificationConfigurationTypeDef,
+    UpdateDataLakeResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
-    UpdateSubscriptionNotificationConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -71,29 +67,20 @@
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
-    AccountNotFoundException: Type[BotocoreClientError]
-    BucketNotFoundException: Type[BotocoreClientError]
+    BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
-    ConcurrentModificationException: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
-    ConflictSourceNamesException: Type[BotocoreClientError]
-    ConflictSubscriptionException: Type[BotocoreClientError]
-    EventBridgeException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
-    InvalidInputException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
-    S3Exception: Type[BotocoreClientError]
-    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
-    ValidationException: Type[BotocoreClientError]
 
 
 class SecurityLakeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/)
     """
@@ -122,215 +109,185 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#close)
         """
 
     def create_aws_log_source(
-        self,
-        *,
-        inputOrder: Sequence[DimensionType],
-        enableAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        enableSingleDimension: Sequence[str] = ...,
-        enableTwoDimensions: Mapping[str, Sequence[str]] = ...
+        self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> CreateAwsLogSourceResponseTypeDef:
         """
         Adds a natively supported Amazon Web Service as an Amazon Security Lake source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_aws_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_aws_log_source)
         """
 
     def create_custom_log_source(
         self,
         *,
-        customSourceName: str,
-        eventClass: OcsfEventClassType,
-        glueInvocationRoleArn: str,
-        logProviderAccountId: str
+        sourceName: str,
+        configuration: CustomLogSourceConfigurationTypeDef = ...,
+        eventClasses: Sequence[str] = ...,
+        sourceVersion: str = ...
     ) -> CreateCustomLogSourceResponseTypeDef:
         """
         Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
         Services Region where you want to create a custom source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_custom_log_source)
         """
 
-    def create_datalake(
+    def create_data_lake(
         self,
         *,
-        configurations: Mapping[RegionType, LakeConfigurationRequestTypeDef] = ...,
-        enableAll: bool = ...,
-        metaStoreManagerRoleArn: str = ...,
-        regions: Sequence[RegionType] = ...
-    ) -> Dict[str, Any]:
+        configurations: Sequence[DataLakeConfigurationTypeDef],
+        metaStoreManagerRoleArn: str
+    ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake)
         """
 
-    def create_datalake_auto_enable(
-        self, *, configurationForNewAccounts: Sequence[AutoEnableNewRegionConfigurationTypeDef]
+    def create_data_lake_exception_subscription(
+        self,
+        *,
+        notificationEndpoint: str,
+        subscriptionProtocol: str,
+        exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
-        Automatically enables Amazon Security Lake for new member accounts in your
-        organization.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake_auto_enable)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake_auto_enable)
-        """
-
-    def create_datalake_delegated_admin(self, *, account: str) -> Dict[str, Any]:
-        """
-        Designates the Amazon Security Lake delegated administrator account for the
-        organization.
+        Creates the specified notification subscription in Amazon Security Lake for the
+        organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake_delegated_admin)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake_delegated_admin)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake_exception_subscription)
         """
 
-    def create_datalake_exceptions_subscription(
-        self, *, notificationEndpoint: str, subscriptionProtocol: SubscriptionProtocolTypeType
+    def create_data_lake_organization_configuration(
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
-        Creates the specified notification subscription in Amazon Security Lake for the
-        organization you specify.
+        Automatically enables Amazon Security Lake for new member accounts in your
+        organization.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake_exceptions_subscription)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_organization_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake_organization_configuration)
         """
 
     def create_subscriber(
         self,
         *,
-        accountId: str,
-        externalId: str,
-        sourceTypes: Sequence[SourceTypeTypeDef],
+        sources: Sequence[LogSourceResourceTypeDef],
+        subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
         subscriberDescription: str = ...
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscriber)
         """
 
-    def create_subscription_notification_configuration(
-        self,
-        *,
-        subscriptionId: str,
-        createSqs: bool = ...,
-        httpsApiKeyName: str = ...,
-        httpsApiKeyValue: str = ...,
-        httpsMethod: HttpsMethodType = ...,
-        roleArn: str = ...,
-        subscriptionEndpoint: str = ...
-    ) -> CreateSubscriptionNotificationConfigurationResponseTypeDef:
+    def create_subscriber_notification(
+        self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
+    ) -> CreateSubscriberNotificationResponseTypeDef:
         """
         Notifies the subscriber when new data is written to the data lake for the
         sources that the subscriber consumes in Security Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscription_notification_configuration)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscription_notification_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber_notification)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscriber_notification)
         """
 
     def delete_aws_log_source(
-        self,
-        *,
-        inputOrder: Sequence[DimensionType],
-        disableAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        disableSingleDimension: Sequence[str] = ...,
-        disableTwoDimensions: Mapping[str, Sequence[str]] = ...
+        self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> DeleteAwsLogSourceResponseTypeDef:
         """
         Removes a natively supported Amazon Web Service as an Amazon Security Lake
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_aws_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_aws_log_source)
         """
 
     def delete_custom_log_source(
-        self, *, customSourceName: str
-    ) -> DeleteCustomLogSourceResponseTypeDef:
+        self, *, sourceName: str, sourceVersion: str = ...
+    ) -> Dict[str, Any]:
         """
-        Removes a custom log source from Amazon Security Lake.
+        Removes a custom log source from Amazon Security Lake, to stop sending data from
+        the custom source to Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_custom_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_custom_log_source)
         """
 
-    def delete_datalake(self) -> Dict[str, Any]:
-        """
-        When you delete Amazon Security Lake from your account, Security Lake is
-        disabled in all Amazon Web Services Regions.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake)
+    def delete_data_lake(self, *, regions: Sequence[str]) -> Dict[str, Any]:
         """
+        When you disable Amazon Security Lake from your account, Security Lake is
+        disabled in all Amazon Web Services Regions and it stops collecting data from
+        your sources.
 
-    def delete_datalake_auto_enable(
-        self,
-        *,
-        removeFromConfigurationForNewAccounts: Sequence[AutoEnableNewRegionConfigurationTypeDef]
-    ) -> Dict[str, Any]:
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake)
         """
-        `DeleteDatalakeAutoEnable` removes automatic enablement of configuration
-        settings for new member accounts (but keeps settings for the delegated
-        administrator) from Amazon Security Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake_auto_enable)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake_auto_enable)
+    def delete_data_lake_exception_subscription(self) -> Dict[str, Any]:
         """
+        Deletes the specified notification subscription in Amazon Security Lake for the
+        organization you specify.
 
-    def delete_datalake_delegated_admin(self, *, account: str) -> Dict[str, Any]:
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_exception_subscription)
         """
-        Deletes the Amazon Security Lake delegated administrator account for the
-        organization.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake_delegated_admin)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake_delegated_admin)
+    def delete_data_lake_organization_configuration(
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
+    ) -> Dict[str, Any]:
         """
+        Removes automatic the enablement of configuration settings for new member
+        accounts (but retains the settings for the delegated administrator) from Amazon
+        Security Lake.
 
-    def delete_datalake_exceptions_subscription(
-        self,
-    ) -> DeleteDatalakeExceptionsSubscriptionResponseTypeDef:
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_organization_configuration)
         """
-        Deletes the specified notification subscription in Amazon Security Lake for the
-        organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake_exceptions_subscription)
+    def delete_subscriber(self, *, subscriberId: str) -> Dict[str, Any]:
         """
-
-    def delete_subscriber(self, *, id: str) -> Dict[str, Any]:
-        """
-        Deletes the subscription permission for accounts that are already enabled in
-        Amazon Security Lake.
+        Deletes the subscription permission and all notification settings for accounts
+        that are already enabled in Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_subscriber)
         """
 
-    def delete_subscription_notification_configuration(
-        self, *, subscriptionId: str
-    ) -> Dict[str, Any]:
+    def delete_subscriber_notification(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscription_notification_configuration)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_subscription_notification_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber_notification)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_subscriber_notification)
+        """
+
+    def deregister_data_lake_delegated_administrator(self) -> Dict[str, Any]:
+        """
+        Deletes the Amazon Security Lake delegated administrator account for the
+        organization.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.deregister_data_lake_delegated_administrator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#deregister_data_lake_delegated_administrator)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
@@ -339,93 +296,85 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#generate_presigned_url)
         """
 
-    def get_datalake(self) -> GetDatalakeResponseTypeDef:
+    def get_data_lake_exception_subscription(
+        self,
+    ) -> GetDataLakeExceptionSubscriptionResponseTypeDef:
         """
-        Retrieves the Amazon Security Lake configuration object for the specified Amazon
-        Web Services account ID.
+        Retrieves the details of exception notifications for the account in Amazon
+        Security Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_data_lake_exception_subscription)
         """
 
-    def get_datalake_auto_enable(self) -> GetDatalakeAutoEnableResponseTypeDef:
+    def get_data_lake_organization_configuration(
+        self,
+    ) -> GetDataLakeOrganizationConfigurationResponseTypeDef:
         """
         Retrieves the configuration that will be automatically set up for accounts added
         to the organization after the organization has onboarded to Amazon Security
         Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_auto_enable)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_auto_enable)
-        """
-
-    def get_datalake_exceptions_expiry(self) -> GetDatalakeExceptionsExpiryResponseTypeDef:
-        """
-        Retrieves the expiration period and time-to-live (TTL) for which the exception
-        message will remain.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_exceptions_expiry)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_exceptions_expiry)
-        """
-
-    def get_datalake_exceptions_subscription(
-        self,
-    ) -> GetDatalakeExceptionsSubscriptionResponseTypeDef:
-        """
-        Retrieves the details of exception notifications for the account in Amazon
-        Security Lake.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_exceptions_subscription)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_organization_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_data_lake_organization_configuration)
         """
 
-    def get_datalake_status(
-        self, *, accountSet: Sequence[str] = ..., maxAccountResults: int = ..., nextToken: str = ...
-    ) -> GetDatalakeStatusResponseTypeDef:
+    def get_data_lake_sources(
+        self, *, accounts: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
+    ) -> GetDataLakeSourcesResponseTypeDef:
         """
         Retrieves a snapshot of the current Region, including whether Amazon Security
         Lake is enabled for those accounts and which sources Security Lake is collecting
         data from.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_status)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_status)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_data_lake_sources)
         """
 
-    def get_subscriber(self, *, id: str) -> GetSubscriberResponseTypeDef:
+    def get_subscriber(self, *, subscriberId: str) -> GetSubscriberResponseTypeDef:
         """
         Retrieves the subscription information for the specified subscription ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_subscriber)
         """
 
-    def list_datalake_exceptions(
-        self, *, maxFailures: int = ..., nextToken: str = ..., regionSet: Sequence[RegionType] = ...
-    ) -> ListDatalakeExceptionsResponseTypeDef:
+    def list_data_lake_exceptions(
+        self, *, maxResults: int = ..., nextToken: str = ..., regions: Sequence[str] = ...
+    ) -> ListDataLakeExceptionsResponseTypeDef:
         """
         Lists the Amazon Security Lake exceptions that you can use to find the source of
         problems and fix them.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_datalake_exceptions)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_datalake_exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lake_exceptions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lake_exceptions)
+        """
+
+    def list_data_lakes(self, *, regions: Sequence[str] = ...) -> ListDataLakesResponseTypeDef:
+        """
+        Retrieves the Amazon Security Lake configuration object for the specified Amazon
+        Web Services account ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lakes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lakes)
         """
 
     def list_log_sources(
         self,
         *,
-        inputOrder: Sequence[DimensionType] = ...,
-        listAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        listSingleDimension: Sequence[str] = ...,
-        listTwoDimensions: Mapping[str, Sequence[str]] = ...,
+        accounts: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
+        regions: Sequence[str] = ...,
+        sources: Sequence[LogSourceResourceTypeDef] = ...
     ) -> ListLogSourcesResponseTypeDef:
         """
         Retrieves the log sources in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_log_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_log_sources)
         """
@@ -436,92 +385,88 @@
         """
         List all subscribers for the specific Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_subscribers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_subscribers)
         """
 
-    def update_datalake(
-        self, *, configurations: Mapping[RegionType, LakeConfigurationRequestTypeDef]
-    ) -> Dict[str, Any]:
+    def register_data_lake_delegated_administrator(self, *, accountId: str) -> Dict[str, Any]:
         """
-        Specifies where to store your security data and for how long.
+        Designates the Amazon Security Lake delegated administrator account for the
+        organization.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.register_data_lake_delegated_administrator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#register_data_lake_delegated_administrator)
         """
 
-    def update_datalake_exceptions_expiry(self, *, exceptionMessageExpiry: int) -> Dict[str, Any]:
+    def update_data_lake(
+        self, *, configurations: Sequence[DataLakeConfigurationTypeDef]
+    ) -> UpdateDataLakeResponseTypeDef:
         """
-        Update the expiration period for the exception message to your preferred time,
-        and control the time-to-live (TTL) for the exception message to remain.
+        Specifies where to store your security data and for how long.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_datalake_exceptions_expiry)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_datalake_exceptions_expiry)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_data_lake)
         """
 
-    def update_datalake_exceptions_subscription(
-        self, *, notificationEndpoint: str, subscriptionProtocol: SubscriptionProtocolTypeType
+    def update_data_lake_exception_subscription(
+        self,
+        *,
+        notificationEndpoint: str,
+        subscriptionProtocol: str,
+        exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_datalake_exceptions_subscription)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_data_lake_exception_subscription)
         """
 
     def update_subscriber(
         self,
         *,
-        id: str,
-        sourceTypes: Sequence[SourceTypeTypeDef],
-        externalId: str = ...,
+        subscriberId: str,
+        sources: Sequence[LogSourceResourceTypeDef] = ...,
         subscriberDescription: str = ...,
+        subscriberIdentity: AwsIdentityTypeDef = ...,
         subscriberName: str = ...
     ) -> UpdateSubscriberResponseTypeDef:
         """
         Updates an existing subscription for the given Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_subscriber)
         """
 
-    def update_subscription_notification_configuration(
-        self,
-        *,
-        subscriptionId: str,
-        createSqs: bool = ...,
-        httpsApiKeyName: str = ...,
-        httpsApiKeyValue: str = ...,
-        httpsMethod: HttpsMethodType = ...,
-        roleArn: str = ...,
-        subscriptionEndpoint: str = ...
-    ) -> UpdateSubscriptionNotificationConfigurationResponseTypeDef:
+    def update_subscriber_notification(
+        self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
+    ) -> UpdateSubscriberNotificationResponseTypeDef:
         """
         Updates an existing notification method for the subscription (SQS or HTTPs
         endpoint) or switches the notification subscription endpoint for a subscriber.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscription_notification_configuration)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_subscription_notification_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber_notification)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_subscriber_notification)
         """
 
     @overload
     def get_paginator(
-        self, operation_name: Literal["get_datalake_status"]
-    ) -> GetDatalakeStatusPaginator:
+        self, operation_name: Literal["get_data_lake_sources"]
+    ) -> GetDataLakeSourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
-        self, operation_name: Literal["list_datalake_exceptions"]
-    ) -> ListDatalakeExceptionsPaginator:
+        self, operation_name: Literal["list_data_lake_exceptions"]
+    ) -> ListDataLakeExceptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_paginator)
         """
 
     @overload
     def get_paginator(self, operation_name: Literal["list_log_sources"]) -> ListLogSourcesPaginator:
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/client.pyi` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/client.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -14,50 +14,46 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import (
-    AccessTypeType,
-    DimensionType,
-    HttpsMethodType,
-    OcsfEventClassType,
-    RegionType,
-    SubscriptionProtocolTypeType,
-)
+from .literals import AccessTypeType
 from .paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 from .type_defs import (
-    AutoEnableNewRegionConfigurationTypeDef,
+    AwsIdentityTypeDef,
+    AwsLogSourceConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    CreateDataLakeResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
     CreateSubscriberResponseTypeDef,
-    CreateSubscriptionNotificationConfigurationResponseTypeDef,
+    CustomLogSourceConfigurationTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    DataLakeConfigurationTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
-    DeleteCustomLogSourceResponseTypeDef,
-    DeleteDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeAutoEnableResponseTypeDef,
-    GetDatalakeExceptionsExpiryResponseTypeDef,
-    GetDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeResponseTypeDef,
-    GetDatalakeStatusResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
-    LakeConfigurationRequestTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
+    ListDataLakesResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
-    SourceTypeTypeDef,
+    LogSourceResourceTypeDef,
+    NotificationConfigurationTypeDef,
+    UpdateDataLakeResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
-    UpdateSubscriptionNotificationConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -68,29 +64,20 @@
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
-    AccountNotFoundException: Type[BotocoreClientError]
-    BucketNotFoundException: Type[BotocoreClientError]
+    BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
-    ConcurrentModificationException: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
-    ConflictSourceNamesException: Type[BotocoreClientError]
-    ConflictSubscriptionException: Type[BotocoreClientError]
-    EventBridgeException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
-    InvalidInputException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
-    S3Exception: Type[BotocoreClientError]
-    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
-    ValidationException: Type[BotocoreClientError]
 
 class SecurityLakeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/)
     """
 
@@ -115,286 +102,250 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#close)
         """
     def create_aws_log_source(
-        self,
-        *,
-        inputOrder: Sequence[DimensionType],
-        enableAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        enableSingleDimension: Sequence[str] = ...,
-        enableTwoDimensions: Mapping[str, Sequence[str]] = ...
+        self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> CreateAwsLogSourceResponseTypeDef:
         """
         Adds a natively supported Amazon Web Service as an Amazon Security Lake source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_aws_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_aws_log_source)
         """
     def create_custom_log_source(
         self,
         *,
-        customSourceName: str,
-        eventClass: OcsfEventClassType,
-        glueInvocationRoleArn: str,
-        logProviderAccountId: str
+        sourceName: str,
+        configuration: CustomLogSourceConfigurationTypeDef = ...,
+        eventClasses: Sequence[str] = ...,
+        sourceVersion: str = ...
     ) -> CreateCustomLogSourceResponseTypeDef:
         """
         Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
         Services Region where you want to create a custom source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_custom_log_source)
         """
-    def create_datalake(
+    def create_data_lake(
         self,
         *,
-        configurations: Mapping[RegionType, LakeConfigurationRequestTypeDef] = ...,
-        enableAll: bool = ...,
-        metaStoreManagerRoleArn: str = ...,
-        regions: Sequence[RegionType] = ...
-    ) -> Dict[str, Any]:
+        configurations: Sequence[DataLakeConfigurationTypeDef],
+        metaStoreManagerRoleArn: str
+    ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake)
         """
-    def create_datalake_auto_enable(
-        self, *, configurationForNewAccounts: Sequence[AutoEnableNewRegionConfigurationTypeDef]
+    def create_data_lake_exception_subscription(
+        self,
+        *,
+        notificationEndpoint: str,
+        subscriptionProtocol: str,
+        exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
-        Automatically enables Amazon Security Lake for new member accounts in your
-        organization.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake_auto_enable)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake_auto_enable)
-        """
-    def create_datalake_delegated_admin(self, *, account: str) -> Dict[str, Any]:
-        """
-        Designates the Amazon Security Lake delegated administrator account for the
-        organization.
+        Creates the specified notification subscription in Amazon Security Lake for the
+        organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake_delegated_admin)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake_delegated_admin)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake_exception_subscription)
         """
-    def create_datalake_exceptions_subscription(
-        self, *, notificationEndpoint: str, subscriptionProtocol: SubscriptionProtocolTypeType
+    def create_data_lake_organization_configuration(
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
-        Creates the specified notification subscription in Amazon Security Lake for the
-        organization you specify.
+        Automatically enables Amazon Security Lake for new member accounts in your
+        organization.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_datalake_exceptions_subscription)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_organization_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake_organization_configuration)
         """
     def create_subscriber(
         self,
         *,
-        accountId: str,
-        externalId: str,
-        sourceTypes: Sequence[SourceTypeTypeDef],
+        sources: Sequence[LogSourceResourceTypeDef],
+        subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
         subscriberDescription: str = ...
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscriber)
         """
-    def create_subscription_notification_configuration(
-        self,
-        *,
-        subscriptionId: str,
-        createSqs: bool = ...,
-        httpsApiKeyName: str = ...,
-        httpsApiKeyValue: str = ...,
-        httpsMethod: HttpsMethodType = ...,
-        roleArn: str = ...,
-        subscriptionEndpoint: str = ...
-    ) -> CreateSubscriptionNotificationConfigurationResponseTypeDef:
+    def create_subscriber_notification(
+        self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
+    ) -> CreateSubscriberNotificationResponseTypeDef:
         """
         Notifies the subscriber when new data is written to the data lake for the
         sources that the subscriber consumes in Security Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscription_notification_configuration)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscription_notification_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber_notification)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscriber_notification)
         """
     def delete_aws_log_source(
-        self,
-        *,
-        inputOrder: Sequence[DimensionType],
-        disableAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        disableSingleDimension: Sequence[str] = ...,
-        disableTwoDimensions: Mapping[str, Sequence[str]] = ...
+        self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> DeleteAwsLogSourceResponseTypeDef:
         """
         Removes a natively supported Amazon Web Service as an Amazon Security Lake
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_aws_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_aws_log_source)
         """
     def delete_custom_log_source(
-        self, *, customSourceName: str
-    ) -> DeleteCustomLogSourceResponseTypeDef:
+        self, *, sourceName: str, sourceVersion: str = ...
+    ) -> Dict[str, Any]:
         """
-        Removes a custom log source from Amazon Security Lake.
+        Removes a custom log source from Amazon Security Lake, to stop sending data from
+        the custom source to Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_custom_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_custom_log_source)
         """
-    def delete_datalake(self) -> Dict[str, Any]:
+    def delete_data_lake(self, *, regions: Sequence[str]) -> Dict[str, Any]:
         """
-        When you delete Amazon Security Lake from your account, Security Lake is
-        disabled in all Amazon Web Services Regions.
+        When you disable Amazon Security Lake from your account, Security Lake is
+        disabled in all Amazon Web Services Regions and it stops collecting data from
+        your sources.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake)
         """
-    def delete_datalake_auto_enable(
-        self,
-        *,
-        removeFromConfigurationForNewAccounts: Sequence[AutoEnableNewRegionConfigurationTypeDef]
-    ) -> Dict[str, Any]:
-        """
-        `DeleteDatalakeAutoEnable` removes automatic enablement of configuration
-        settings for new member accounts (but keeps settings for the delegated
-        administrator) from Amazon Security Lake.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake_auto_enable)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake_auto_enable)
+    def delete_data_lake_exception_subscription(self) -> Dict[str, Any]:
         """
-    def delete_datalake_delegated_admin(self, *, account: str) -> Dict[str, Any]:
-        """
-        Deletes the Amazon Security Lake delegated administrator account for the
-        organization.
+        Deletes the specified notification subscription in Amazon Security Lake for the
+        organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake_delegated_admin)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake_delegated_admin)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_exception_subscription)
         """
-    def delete_datalake_exceptions_subscription(
-        self,
-    ) -> DeleteDatalakeExceptionsSubscriptionResponseTypeDef:
+    def delete_data_lake_organization_configuration(
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
+    ) -> Dict[str, Any]:
         """
-        Deletes the specified notification subscription in Amazon Security Lake for the
-        organization you specify.
+        Removes automatic the enablement of configuration settings for new member
+        accounts (but retains the settings for the delegated administrator) from Amazon
+        Security Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_datalake_exceptions_subscription)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_organization_configuration)
         """
-    def delete_subscriber(self, *, id: str) -> Dict[str, Any]:
+    def delete_subscriber(self, *, subscriberId: str) -> Dict[str, Any]:
         """
-        Deletes the subscription permission for accounts that are already enabled in
-        Amazon Security Lake.
+        Deletes the subscription permission and all notification settings for accounts
+        that are already enabled in Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_subscriber)
         """
-    def delete_subscription_notification_configuration(
-        self, *, subscriptionId: str
-    ) -> Dict[str, Any]:
+    def delete_subscriber_notification(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscription_notification_configuration)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_subscription_notification_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber_notification)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_subscriber_notification)
+        """
+    def deregister_data_lake_delegated_administrator(self) -> Dict[str, Any]:
+        """
+        Deletes the Amazon Security Lake delegated administrator account for the
+        organization.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.deregister_data_lake_delegated_administrator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#deregister_data_lake_delegated_administrator)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#generate_presigned_url)
         """
-    def get_datalake(self) -> GetDatalakeResponseTypeDef:
+    def get_data_lake_exception_subscription(
+        self,
+    ) -> GetDataLakeExceptionSubscriptionResponseTypeDef:
         """
-        Retrieves the Amazon Security Lake configuration object for the specified Amazon
-        Web Services account ID.
+        Retrieves the details of exception notifications for the account in Amazon
+        Security Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_data_lake_exception_subscription)
         """
-    def get_datalake_auto_enable(self) -> GetDatalakeAutoEnableResponseTypeDef:
+    def get_data_lake_organization_configuration(
+        self,
+    ) -> GetDataLakeOrganizationConfigurationResponseTypeDef:
         """
         Retrieves the configuration that will be automatically set up for accounts added
         to the organization after the organization has onboarded to Amazon Security
         Lake.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_auto_enable)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_auto_enable)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_organization_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_data_lake_organization_configuration)
         """
-    def get_datalake_exceptions_expiry(self) -> GetDatalakeExceptionsExpiryResponseTypeDef:
-        """
-        Retrieves the expiration period and time-to-live (TTL) for which the exception
-        message will remain.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_exceptions_expiry)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_exceptions_expiry)
-        """
-    def get_datalake_exceptions_subscription(
-        self,
-    ) -> GetDatalakeExceptionsSubscriptionResponseTypeDef:
-        """
-        Retrieves the details of exception notifications for the account in Amazon
-        Security Lake.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_exceptions_subscription)
-        """
-    def get_datalake_status(
-        self, *, accountSet: Sequence[str] = ..., maxAccountResults: int = ..., nextToken: str = ...
-    ) -> GetDatalakeStatusResponseTypeDef:
+    def get_data_lake_sources(
+        self, *, accounts: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
+    ) -> GetDataLakeSourcesResponseTypeDef:
         """
         Retrieves a snapshot of the current Region, including whether Amazon Security
         Lake is enabled for those accounts and which sources Security Lake is collecting
         data from.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_datalake_status)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_datalake_status)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_data_lake_sources)
         """
-    def get_subscriber(self, *, id: str) -> GetSubscriberResponseTypeDef:
+    def get_subscriber(self, *, subscriberId: str) -> GetSubscriberResponseTypeDef:
         """
         Retrieves the subscription information for the specified subscription ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_subscriber)
         """
-    def list_datalake_exceptions(
-        self, *, maxFailures: int = ..., nextToken: str = ..., regionSet: Sequence[RegionType] = ...
-    ) -> ListDatalakeExceptionsResponseTypeDef:
+    def list_data_lake_exceptions(
+        self, *, maxResults: int = ..., nextToken: str = ..., regions: Sequence[str] = ...
+    ) -> ListDataLakeExceptionsResponseTypeDef:
         """
         Lists the Amazon Security Lake exceptions that you can use to find the source of
         problems and fix them.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_datalake_exceptions)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_datalake_exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lake_exceptions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lake_exceptions)
+        """
+    def list_data_lakes(self, *, regions: Sequence[str] = ...) -> ListDataLakesResponseTypeDef:
+        """
+        Retrieves the Amazon Security Lake configuration object for the specified Amazon
+        Web Services account ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lakes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lakes)
         """
     def list_log_sources(
         self,
         *,
-        inputOrder: Sequence[DimensionType] = ...,
-        listAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        listSingleDimension: Sequence[str] = ...,
-        listTwoDimensions: Mapping[str, Sequence[str]] = ...,
+        accounts: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
+        regions: Sequence[str] = ...,
+        sources: Sequence[LogSourceResourceTypeDef] = ...
     ) -> ListLogSourcesResponseTypeDef:
         """
         Retrieves the log sources in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_log_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_log_sources)
         """
@@ -403,86 +354,82 @@
     ) -> ListSubscribersResponseTypeDef:
         """
         List all subscribers for the specific Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_subscribers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_subscribers)
         """
-    def update_datalake(
-        self, *, configurations: Mapping[RegionType, LakeConfigurationRequestTypeDef]
-    ) -> Dict[str, Any]:
+    def register_data_lake_delegated_administrator(self, *, accountId: str) -> Dict[str, Any]:
         """
-        Specifies where to store your security data and for how long.
+        Designates the Amazon Security Lake delegated administrator account for the
+        organization.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_datalake)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_datalake)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.register_data_lake_delegated_administrator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#register_data_lake_delegated_administrator)
         """
-    def update_datalake_exceptions_expiry(self, *, exceptionMessageExpiry: int) -> Dict[str, Any]:
+    def update_data_lake(
+        self, *, configurations: Sequence[DataLakeConfigurationTypeDef]
+    ) -> UpdateDataLakeResponseTypeDef:
         """
-        Update the expiration period for the exception message to your preferred time,
-        and control the time-to-live (TTL) for the exception message to remain.
+        Specifies where to store your security data and for how long.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_datalake_exceptions_expiry)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_datalake_exceptions_expiry)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_data_lake)
         """
-    def update_datalake_exceptions_subscription(
-        self, *, notificationEndpoint: str, subscriptionProtocol: SubscriptionProtocolTypeType
+    def update_data_lake_exception_subscription(
+        self,
+        *,
+        notificationEndpoint: str,
+        subscriptionProtocol: str,
+        exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_datalake_exceptions_subscription)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_datalake_exceptions_subscription)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake_exception_subscription)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_data_lake_exception_subscription)
         """
     def update_subscriber(
         self,
         *,
-        id: str,
-        sourceTypes: Sequence[SourceTypeTypeDef],
-        externalId: str = ...,
+        subscriberId: str,
+        sources: Sequence[LogSourceResourceTypeDef] = ...,
         subscriberDescription: str = ...,
+        subscriberIdentity: AwsIdentityTypeDef = ...,
         subscriberName: str = ...
     ) -> UpdateSubscriberResponseTypeDef:
         """
         Updates an existing subscription for the given Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_subscriber)
         """
-    def update_subscription_notification_configuration(
-        self,
-        *,
-        subscriptionId: str,
-        createSqs: bool = ...,
-        httpsApiKeyName: str = ...,
-        httpsApiKeyValue: str = ...,
-        httpsMethod: HttpsMethodType = ...,
-        roleArn: str = ...,
-        subscriptionEndpoint: str = ...
-    ) -> UpdateSubscriptionNotificationConfigurationResponseTypeDef:
+    def update_subscriber_notification(
+        self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
+    ) -> UpdateSubscriberNotificationResponseTypeDef:
         """
         Updates an existing notification method for the subscription (SQS or HTTPs
         endpoint) or switches the notification subscription endpoint for a subscriber.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscription_notification_configuration)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_subscription_notification_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber_notification)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#update_subscriber_notification)
         """
     @overload
     def get_paginator(
-        self, operation_name: Literal["get_datalake_status"]
-    ) -> GetDatalakeStatusPaginator:
+        self, operation_name: Literal["get_data_lake_sources"]
+    ) -> GetDataLakeSourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_paginator)
         """
     @overload
     def get_paginator(
-        self, operation_name: Literal["list_datalake_exceptions"]
-    ) -> ListDatalakeExceptionsPaginator:
+        self, operation_name: Literal["list_data_lake_exceptions"]
+    ) -> ListDataLakeExceptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#get_paginator)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_log_sources"]) -> ListLogSourcesPaginator:
         """
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/literals.py` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/literals.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,105 +17,43 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccessTypeType",
-    "AwsLogSourceTypeType",
-    "DimensionType",
-    "EndpointProtocolType",
-    "GetDatalakeStatusPaginatorName",
-    "HttpsMethodType",
-    "ListDatalakeExceptionsPaginatorName",
+    "AwsLogSourceNameType",
+    "DataLakeStatusType",
+    "GetDataLakeSourcesPaginatorName",
+    "HttpMethodType",
+    "ListDataLakeExceptionsPaginatorName",
     "ListLogSourcesPaginatorName",
     "ListSubscribersPaginatorName",
-    "OcsfEventClassType",
-    "RegionType",
-    "SourceStatusType",
-    "StorageClassType",
-    "SubscriptionProtocolTypeType",
-    "SubscriptionStatusType",
-    "settingsStatusType",
+    "SourceCollectionStatusType",
+    "SubscriberStatusType",
     "SecurityLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AccessTypeType = Literal["LAKEFORMATION", "S3"]
-AwsLogSourceTypeType = Literal["CLOUD_TRAIL", "ROUTE53", "SH_FINDINGS", "VPC_FLOW"]
-DimensionType = Literal["MEMBER", "REGION", "SOURCE_TYPE"]
-EndpointProtocolType = Literal["HTTPS", "SQS"]
-GetDatalakeStatusPaginatorName = Literal["get_datalake_status"]
-HttpsMethodType = Literal["POST", "PUT"]
-ListDatalakeExceptionsPaginatorName = Literal["list_datalake_exceptions"]
+AwsLogSourceNameType = Literal[
+    "CLOUD_TRAIL_MGMT", "LAMBDA_EXECUTION", "ROUTE53", "S3_DATA", "SH_FINDINGS", "VPC_FLOW"
+]
+DataLakeStatusType = Literal["COMPLETED", "FAILED", "INITIALIZED", "PENDING"]
+GetDataLakeSourcesPaginatorName = Literal["get_data_lake_sources"]
+HttpMethodType = Literal["POST", "PUT"]
+ListDataLakeExceptionsPaginatorName = Literal["list_data_lake_exceptions"]
 ListLogSourcesPaginatorName = Literal["list_log_sources"]
 ListSubscribersPaginatorName = Literal["list_subscribers"]
-OcsfEventClassType = Literal[
-    "ACCESS_ACTIVITY",
-    "ACCOUNT_CHANGE",
-    "AUTHENTICATION",
-    "AUTHORIZATION",
-    "CLOUD_API",
-    "CLOUD_STORAGE",
-    "CONFIG_STATE",
-    "CONTAINER_LIFECYCLE",
-    "DATABASE_LIFECYCLE",
-    "DHCP_ACTIVITY",
-    "DNS_ACTIVITY",
-    "ENTITY_MANAGEMENT_AUDIT",
-    "FILE_ACTIVITY",
-    "FTP_ACTIVITY",
-    "HTTP_ACTIVITY",
-    "INVENTORY_INFO",
-    "KERNEL_ACTIVITY",
-    "KERNEL_EXTENSION",
-    "MEMORY_ACTIVITY",
-    "MODULE_ACTIVITY",
-    "NETWORK_ACTIVITY",
-    "PROCESS_ACTIVITY",
-    "RDP_ACTIVITY",
-    "REGISTRY_KEY_ACTIVITY",
-    "REGISTRY_VALUE_ACTIVITY",
-    "RESOURCE_ACTIVITY",
-    "RFB_ACTIVITY",
-    "SCHEDULED_JOB_ACTIVITY",
-    "SECURITY_FINDING",
-    "SMB_ACTIVITY",
-    "SMTP_ACTIVITY",
-    "SSH_ACTIVITY",
-    "VIRTUAL_MACHINE_ACTIVITY",
-]
-RegionType = Literal[
-    "ap-northeast-1",
-    "ap-southeast-2",
-    "eu-central-1",
-    "eu-west-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-2",
-]
-SourceStatusType = Literal["ACTIVE", "DEACTIVATED", "PENDING"]
-StorageClassType = Literal[
-    "DEEP_ARCHIVE",
-    "EXPIRE",
-    "GLACIER",
-    "GLACIER_IR",
-    "INTELLIGENT_TIERING",
-    "ONEZONE_IA",
-    "STANDARD_IA",
-]
-SubscriptionProtocolTypeType = Literal[
-    "APP", "EMAIL", "EMAIL_JSON", "FIREHOSE", "HTTP", "HTTPS", "LAMBDA", "SMS", "SQS"
-]
-SubscriptionStatusType = Literal["ACTIVE", "DEACTIVATED", "PENDING", "READY"]
-settingsStatusType = Literal["COMPLETED", "FAILED", "INITIALIZED", "PENDING"]
+SourceCollectionStatusType = Literal["COLLECTING", "MISCONFIGURED", "NOT_COLLECTING"]
+SubscriberStatusType = Literal["ACTIVE", "DEACTIVATED", "PENDING", "READY"]
 SecurityLakeServiceName = Literal["securitylake"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -124,14 +62,15 @@
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
@@ -171,14 +110,15 @@
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
@@ -276,14 +216,15 @@
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
@@ -319,14 +260,15 @@
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
@@ -345,16 +287,19 @@
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
@@ -438,15 +383,17 @@
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
@@ -465,18 +412,24 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "get_datalake_status", "list_datalake_exceptions", "list_log_sources", "list_subscribers"
+    "get_data_lake_sources", "list_data_lake_exceptions", "list_log_sources", "list_subscribers"
 ]
 RegionName = Literal[
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
+    "eu-west-2",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/literals.pyi` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/literals.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -16,104 +16,42 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccessTypeType",
-    "AwsLogSourceTypeType",
-    "DimensionType",
-    "EndpointProtocolType",
-    "GetDatalakeStatusPaginatorName",
-    "HttpsMethodType",
-    "ListDatalakeExceptionsPaginatorName",
+    "AwsLogSourceNameType",
+    "DataLakeStatusType",
+    "GetDataLakeSourcesPaginatorName",
+    "HttpMethodType",
+    "ListDataLakeExceptionsPaginatorName",
     "ListLogSourcesPaginatorName",
     "ListSubscribersPaginatorName",
-    "OcsfEventClassType",
-    "RegionType",
-    "SourceStatusType",
-    "StorageClassType",
-    "SubscriptionProtocolTypeType",
-    "SubscriptionStatusType",
-    "settingsStatusType",
+    "SourceCollectionStatusType",
+    "SubscriberStatusType",
     "SecurityLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AccessTypeType = Literal["LAKEFORMATION", "S3"]
-AwsLogSourceTypeType = Literal["CLOUD_TRAIL", "ROUTE53", "SH_FINDINGS", "VPC_FLOW"]
-DimensionType = Literal["MEMBER", "REGION", "SOURCE_TYPE"]
-EndpointProtocolType = Literal["HTTPS", "SQS"]
-GetDatalakeStatusPaginatorName = Literal["get_datalake_status"]
-HttpsMethodType = Literal["POST", "PUT"]
-ListDatalakeExceptionsPaginatorName = Literal["list_datalake_exceptions"]
+AwsLogSourceNameType = Literal[
+    "CLOUD_TRAIL_MGMT", "LAMBDA_EXECUTION", "ROUTE53", "S3_DATA", "SH_FINDINGS", "VPC_FLOW"
+]
+DataLakeStatusType = Literal["COMPLETED", "FAILED", "INITIALIZED", "PENDING"]
+GetDataLakeSourcesPaginatorName = Literal["get_data_lake_sources"]
+HttpMethodType = Literal["POST", "PUT"]
+ListDataLakeExceptionsPaginatorName = Literal["list_data_lake_exceptions"]
 ListLogSourcesPaginatorName = Literal["list_log_sources"]
 ListSubscribersPaginatorName = Literal["list_subscribers"]
-OcsfEventClassType = Literal[
-    "ACCESS_ACTIVITY",
-    "ACCOUNT_CHANGE",
-    "AUTHENTICATION",
-    "AUTHORIZATION",
-    "CLOUD_API",
-    "CLOUD_STORAGE",
-    "CONFIG_STATE",
-    "CONTAINER_LIFECYCLE",
-    "DATABASE_LIFECYCLE",
-    "DHCP_ACTIVITY",
-    "DNS_ACTIVITY",
-    "ENTITY_MANAGEMENT_AUDIT",
-    "FILE_ACTIVITY",
-    "FTP_ACTIVITY",
-    "HTTP_ACTIVITY",
-    "INVENTORY_INFO",
-    "KERNEL_ACTIVITY",
-    "KERNEL_EXTENSION",
-    "MEMORY_ACTIVITY",
-    "MODULE_ACTIVITY",
-    "NETWORK_ACTIVITY",
-    "PROCESS_ACTIVITY",
-    "RDP_ACTIVITY",
-    "REGISTRY_KEY_ACTIVITY",
-    "REGISTRY_VALUE_ACTIVITY",
-    "RESOURCE_ACTIVITY",
-    "RFB_ACTIVITY",
-    "SCHEDULED_JOB_ACTIVITY",
-    "SECURITY_FINDING",
-    "SMB_ACTIVITY",
-    "SMTP_ACTIVITY",
-    "SSH_ACTIVITY",
-    "VIRTUAL_MACHINE_ACTIVITY",
-]
-RegionType = Literal[
-    "ap-northeast-1",
-    "ap-southeast-2",
-    "eu-central-1",
-    "eu-west-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-2",
-]
-SourceStatusType = Literal["ACTIVE", "DEACTIVATED", "PENDING"]
-StorageClassType = Literal[
-    "DEEP_ARCHIVE",
-    "EXPIRE",
-    "GLACIER",
-    "GLACIER_IR",
-    "INTELLIGENT_TIERING",
-    "ONEZONE_IA",
-    "STANDARD_IA",
-]
-SubscriptionProtocolTypeType = Literal[
-    "APP", "EMAIL", "EMAIL_JSON", "FIREHOSE", "HTTP", "HTTPS", "LAMBDA", "SMS", "SQS"
-]
-SubscriptionStatusType = Literal["ACTIVE", "DEACTIVATED", "PENDING", "READY"]
-settingsStatusType = Literal["COMPLETED", "FAILED", "INITIALIZED", "PENDING"]
+SourceCollectionStatusType = Literal["COLLECTING", "MISCONFIGURED", "NOT_COLLECTING"]
+SubscriberStatusType = Literal["ACTIVE", "DEACTIVATED", "PENDING", "READY"]
 SecurityLakeServiceName = Literal["securitylake"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -122,14 +60,15 @@
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
@@ -169,14 +108,15 @@
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
@@ -274,14 +214,15 @@
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
@@ -317,14 +258,15 @@
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
@@ -343,16 +285,19 @@
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
@@ -436,15 +381,17 @@
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
@@ -463,18 +410,24 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "get_datalake_status", "list_datalake_exceptions", "list_log_sources", "list_subscribers"
+    "get_data_lake_sources", "list_data_lake_exceptions", "list_log_sources", "list_subscribers"
 ]
 RegionName = Literal[
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
+    "eu-west-2",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/paginator.py` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_securitylake.client import SecurityLakeClient
     from mypy_boto3_securitylake.paginator import (
-        GetDatalakeStatusPaginator,
-        ListDatalakeExceptionsPaginator,
+        GetDataLakeSourcesPaginator,
+        ListDataLakeExceptionsPaginator,
         ListLogSourcesPaginator,
         ListSubscribersPaginator,
     )
 
     session = Session()
     client: SecurityLakeClient = session.client("securitylake")
 
-    get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator("get_datalake_status")
-    list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator("list_datalake_exceptions")
+    get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")
+    list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator("list_data_lake_exceptions")
     list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
     list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
     ```
 """
-from typing import Generic, Iterator, Mapping, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import DimensionType, RegionType
 from .type_defs import (
-    GetDatalakeStatusResponseTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
+    LogSourceResourceTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
-    "GetDatalakeStatusPaginator",
-    "ListDatalakeExceptionsPaginator",
+    "GetDataLakeSourcesPaginator",
+    "ListDataLakeExceptionsPaginator",
     "ListLogSourcesPaginator",
     "ListSubscribersPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -52,74 +52,70 @@
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
 
-class GetDatalakeStatusPaginator(Paginator):
+class GetDataLakeSourcesPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDatalakeStatus)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakestatuspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
     """
 
     def paginate(
-        self, *, accountSet: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[GetDatalakeStatusResponseTypeDef]:
+        self, *, accounts: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[GetDataLakeSourcesResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDatalakeStatus.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakestatuspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
         """
 
 
-class ListDatalakeExceptionsPaginator(Paginator):
+class ListDataLakeExceptionsPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDatalakeExceptions)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        regionSet: Sequence[RegionType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListDatalakeExceptionsResponseTypeDef]:
+        self, *, regions: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDataLakeExceptionsResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDatalakeExceptions.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
         """
 
 
 class ListLogSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listlogsourcespaginator)
     """
 
     def paginate(
         self,
         *,
-        inputOrder: Sequence[DimensionType] = ...,
-        listAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        listSingleDimension: Sequence[str] = ...,
-        listTwoDimensions: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        accounts: Sequence[str] = ...,
+        regions: Sequence[str] = ...,
+        sources: Sequence[LogSourceResourceTypeDef] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listlogsourcespaginator)
         """
 
 
 class ListSubscribersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscribersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
         """
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/paginator.pyi` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -6,114 +6,110 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_securitylake.client import SecurityLakeClient
     from mypy_boto3_securitylake.paginator import (
-        GetDatalakeStatusPaginator,
-        ListDatalakeExceptionsPaginator,
+        GetDataLakeSourcesPaginator,
+        ListDataLakeExceptionsPaginator,
         ListLogSourcesPaginator,
         ListSubscribersPaginator,
     )
 
     session = Session()
     client: SecurityLakeClient = session.client("securitylake")
 
-    get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator("get_datalake_status")
-    list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator("list_datalake_exceptions")
+    get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")
+    list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator("list_data_lake_exceptions")
     list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
     list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
     ```
 """
-from typing import Generic, Iterator, Mapping, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import DimensionType, RegionType
 from .type_defs import (
-    GetDatalakeStatusResponseTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
+    LogSourceResourceTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
-    "GetDatalakeStatusPaginator",
-    "ListDatalakeExceptionsPaginator",
+    "GetDataLakeSourcesPaginator",
+    "ListDataLakeExceptionsPaginator",
     "ListLogSourcesPaginator",
     "ListSubscribersPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-class GetDatalakeStatusPaginator(Paginator):
+class GetDataLakeSourcesPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDatalakeStatus)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakestatuspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
     """
 
     def paginate(
-        self, *, accountSet: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[GetDatalakeStatusResponseTypeDef]:
+        self, *, accounts: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[GetDataLakeSourcesResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDatalakeStatus.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakestatuspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
         """
 
-class ListDatalakeExceptionsPaginator(Paginator):
+class ListDataLakeExceptionsPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDatalakeExceptions)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        regionSet: Sequence[RegionType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListDatalakeExceptionsResponseTypeDef]:
+        self, *, regions: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDataLakeExceptionsResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDatalakeExceptions.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
         """
 
 class ListLogSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listlogsourcespaginator)
     """
 
     def paginate(
         self,
         *,
-        inputOrder: Sequence[DimensionType] = ...,
-        listAllDimensions: Mapping[str, Mapping[str, Sequence[str]]] = ...,
-        listSingleDimension: Sequence[str] = ...,
-        listTwoDimensions: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        accounts: Sequence[str] = ...,
+        regions: Sequence[str] = ...,
+        sources: Sequence[LogSourceResourceTypeDef] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listlogsourcespaginator)
         """
 
 class ListSubscribersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscribersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
         """
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/type_defs.py` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,782 +2,887 @@
 Type annotations for securitylake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_securitylake.type_defs import LogsStatusTypeDef
+    from mypy_boto3_securitylake.type_defs import AwsIdentityTypeDef
 
-    data: LogsStatusTypeDef = {...}
+    data: AwsIdentityTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccessTypeType,
-    AwsLogSourceTypeType,
-    DimensionType,
-    EndpointProtocolType,
-    HttpsMethodType,
-    OcsfEventClassType,
-    RegionType,
-    SourceStatusType,
-    StorageClassType,
-    SubscriptionProtocolTypeType,
-    SubscriptionStatusType,
-    settingsStatusType,
+    AwsLogSourceNameType,
+    DataLakeStatusType,
+    HttpMethodType,
+    SourceCollectionStatusType,
+    SubscriberStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "LogsStatusTypeDef",
-    "AutoEnableNewRegionConfigurationTypeDef",
-    "CreateAwsLogSourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "CreateCustomLogSourceRequestRequestTypeDef",
-    "CreateDatalakeDelegatedAdminRequestRequestTypeDef",
-    "CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
-    "SourceTypeTypeDef",
-    "CreateSubscriptionNotificationConfigurationRequestRequestTypeDef",
-    "DeleteAwsLogSourceRequestRequestTypeDef",
+    "AwsIdentityTypeDef",
+    "AwsLogSourceConfigurationTypeDef",
+    "AwsLogSourceResourceTypeDef",
+    "CreateAwsLogSourceResponseTypeDef",
+    "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    "CreateSubscriberNotificationResponseTypeDef",
+    "CustomLogSourceAttributesTypeDef",
+    "CustomLogSourceCrawlerConfigurationTypeDef",
+    "CustomLogSourceProviderTypeDef",
+    "DataLakeEncryptionConfigurationTypeDef",
+    "DataLakeReplicationConfigurationTypeDef",
+    "DataLakeExceptionTypeDef",
+    "DataLakeLifecycleExpirationTypeDef",
+    "DataLakeLifecycleTransitionTypeDef",
+    "DataLakeSourceStatusTypeDef",
+    "DataLakeUpdateExceptionTypeDef",
+    "DeleteAwsLogSourceResponseTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
-    "DeleteDatalakeDelegatedAdminRequestRequestTypeDef",
+    "DeleteDataLakeRequestRequestTypeDef",
+    "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef",
-    "FailuresTypeDef",
-    "ProtocolAndNotificationEndpointTypeDef",
-    "PaginatorConfigTypeDef",
-    "GetDatalakeStatusRequestRequestTypeDef",
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
-    "RetentionSettingTypeDef",
-    "LastUpdateFailureTypeDef",
-    "ListDatalakeExceptionsRequestRequestTypeDef",
-    "ListLogSourcesRequestRequestTypeDef",
+    "HttpsNotificationConfigurationTypeDef",
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    "ListDataLakeExceptionsRequestRequestTypeDef",
+    "ListDataLakesRequestRequestTypeDef",
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "ListSubscribersRequestRequestTypeDef",
-    "UpdateDatalakeExceptionsExpiryRequestRequestTypeDef",
-    "UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
-    "UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef",
-    "AccountSourcesTypeDef",
-    "CreateDatalakeAutoEnableRequestRequestTypeDef",
-    "DeleteDatalakeAutoEnableRequestRequestTypeDef",
-    "CreateAwsLogSourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    "UpdateSubscriberNotificationResponseTypeDef",
+    "CreateAwsLogSourceRequestRequestTypeDef",
+    "DeleteAwsLogSourceRequestRequestTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    "CustomLogSourceConfigurationTypeDef",
+    "CustomLogSourceResourceTypeDef",
+    "ListDataLakeExceptionsResponseTypeDef",
+    "DataLakeLifecycleConfigurationTypeDef",
+    "DataLakeSourceTypeDef",
+    "DataLakeUpdateStatusTypeDef",
+    "NotificationConfigurationTypeDef",
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
+    "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
-    "CreateSubscriberResponseTypeDef",
-    "CreateSubscriptionNotificationConfigurationResponseTypeDef",
-    "DeleteAwsLogSourceResponseTypeDef",
-    "DeleteCustomLogSourceResponseTypeDef",
-    "DeleteDatalakeExceptionsSubscriptionResponseTypeDef",
-    "GetDatalakeAutoEnableResponseTypeDef",
-    "GetDatalakeExceptionsExpiryResponseTypeDef",
-    "ListLogSourcesResponseTypeDef",
-    "UpdateSubscriptionNotificationConfigurationResponseTypeDef",
+    "LogSourceResourceTypeDef",
+    "DataLakeConfigurationTypeDef",
+    "GetDataLakeSourcesResponseTypeDef",
+    "DataLakeResourceTypeDef",
+    "CreateSubscriberNotificationRequestRequestTypeDef",
+    "UpdateSubscriberNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
+    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
+    "ListLogSourcesRequestRequestTypeDef",
+    "LogSourceTypeDef",
     "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
-    "FailuresResponseTypeDef",
-    "GetDatalakeExceptionsSubscriptionResponseTypeDef",
-    "GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef",
-    "ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef",
-    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    "LakeConfigurationRequestTypeDef",
-    "UpdateStatusTypeDef",
-    "GetDatalakeStatusResponseTypeDef",
+    "CreateDataLakeRequestRequestTypeDef",
+    "UpdateDataLakeRequestRequestTypeDef",
+    "CreateDataLakeResponseTypeDef",
+    "ListDataLakesResponseTypeDef",
+    "UpdateDataLakeResponseTypeDef",
+    "ListLogSourcesResponseTypeDef",
+    "CreateSubscriberResponseTypeDef",
     "GetSubscriberResponseTypeDef",
     "ListSubscribersResponseTypeDef",
     "UpdateSubscriberResponseTypeDef",
-    "ListDatalakeExceptionsResponseTypeDef",
-    "CreateDatalakeRequestRequestTypeDef",
-    "UpdateDatalakeRequestRequestTypeDef",
-    "LakeConfigurationResponseTypeDef",
-    "GetDatalakeResponseTypeDef",
 )
 
-LogsStatusTypeDef = TypedDict(
-    "LogsStatusTypeDef",
+AwsIdentityTypeDef = TypedDict(
+    "AwsIdentityTypeDef",
     {
-        "healthStatus": SourceStatusType,
-        "pathToLogs": str,
+        "externalId": str,
+        "principal": str,
     },
 )
 
-AutoEnableNewRegionConfigurationTypeDef = TypedDict(
-    "AutoEnableNewRegionConfigurationTypeDef",
+_RequiredAwsLogSourceConfigurationTypeDef = TypedDict(
+    "_RequiredAwsLogSourceConfigurationTypeDef",
     {
-        "region": RegionType,
-        "sources": Sequence[AwsLogSourceTypeType],
+        "regions": Sequence[str],
+        "sourceName": AwsLogSourceNameType,
     },
 )
-
-_RequiredCreateAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAwsLogSourceRequestRequestTypeDef",
+_OptionalAwsLogSourceConfigurationTypeDef = TypedDict(
+    "_OptionalAwsLogSourceConfigurationTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
+        "accounts": Sequence[str],
+        "sourceVersion": str,
     },
+    total=False,
 )
-_OptionalCreateAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAwsLogSourceRequestRequestTypeDef",
+
+class AwsLogSourceConfigurationTypeDef(
+    _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
+):
+    pass
+
+AwsLogSourceResourceTypeDef = TypedDict(
+    "AwsLogSourceResourceTypeDef",
     {
-        "enableAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "enableSingleDimension": Sequence[str],
-        "enableTwoDimensions": Mapping[str, Sequence[str]],
+        "sourceName": AwsLogSourceNameType,
+        "sourceVersion": str,
     },
     total=False,
 )
 
+CreateAwsLogSourceResponseTypeDef = TypedDict(
+    "CreateAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-class CreateAwsLogSourceRequestRequestTypeDef(
-    _RequiredCreateAwsLogSourceRequestRequestTypeDef,
-    _OptionalCreateAwsLogSourceRequestRequestTypeDef,
+_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    {
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+    },
+)
+_OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    {
+        "exceptionTimeToLive": int,
+    },
+    total=False,
+)
+
+class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
+    _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+CreateSubscriberNotificationResponseTypeDef = TypedDict(
+    "CreateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CustomLogSourceAttributesTypeDef = TypedDict(
+    "CustomLogSourceAttributesTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "crawlerArn": str,
+        "databaseArn": str,
+        "tableArn": str,
     },
+    total=False,
 )
 
-CreateCustomLogSourceRequestRequestTypeDef = TypedDict(
-    "CreateCustomLogSourceRequestRequestTypeDef",
+CustomLogSourceCrawlerConfigurationTypeDef = TypedDict(
+    "CustomLogSourceCrawlerConfigurationTypeDef",
     {
-        "customSourceName": str,
-        "eventClass": OcsfEventClassType,
-        "glueInvocationRoleArn": str,
-        "logProviderAccountId": str,
+        "roleArn": str,
     },
 )
 
-CreateDatalakeDelegatedAdminRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeDelegatedAdminRequestRequestTypeDef",
+CustomLogSourceProviderTypeDef = TypedDict(
+    "CustomLogSourceProviderTypeDef",
     {
-        "account": str,
+        "location": str,
+        "roleArn": str,
     },
+    total=False,
 )
 
-CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
+DataLakeEncryptionConfigurationTypeDef = TypedDict(
+    "DataLakeEncryptionConfigurationTypeDef",
     {
-        "notificationEndpoint": str,
-        "subscriptionProtocol": SubscriptionProtocolTypeType,
+        "kmsKeyId": str,
     },
+    total=False,
 )
 
-SourceTypeTypeDef = TypedDict(
-    "SourceTypeTypeDef",
+DataLakeReplicationConfigurationTypeDef = TypedDict(
+    "DataLakeReplicationConfigurationTypeDef",
     {
-        "awsSourceType": AwsLogSourceTypeType,
-        "customSourceType": str,
+        "regions": Sequence[str],
+        "roleArn": str,
     },
     total=False,
 )
 
-_RequiredCreateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+DataLakeExceptionTypeDef = TypedDict(
+    "DataLakeExceptionTypeDef",
     {
-        "subscriptionId": str,
+        "exception": str,
+        "region": str,
+        "remediation": str,
+        "timestamp": datetime,
     },
+    total=False,
 )
-_OptionalCreateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+
+DataLakeLifecycleExpirationTypeDef = TypedDict(
+    "DataLakeLifecycleExpirationTypeDef",
     {
-        "createSqs": bool,
-        "httpsApiKeyName": str,
-        "httpsApiKeyValue": str,
-        "httpsMethod": HttpsMethodType,
-        "roleArn": str,
-        "subscriptionEndpoint": str,
+        "days": int,
     },
     total=False,
 )
 
+DataLakeLifecycleTransitionTypeDef = TypedDict(
+    "DataLakeLifecycleTransitionTypeDef",
+    {
+        "days": int,
+        "storageClass": str,
+    },
+    total=False,
+)
 
-class CreateSubscriptionNotificationConfigurationRequestRequestTypeDef(
-    _RequiredCreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    _OptionalCreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-):
-    pass
+DataLakeSourceStatusTypeDef = TypedDict(
+    "DataLakeSourceStatusTypeDef",
+    {
+        "resource": str,
+        "status": SourceCollectionStatusType,
+    },
+    total=False,
+)
 
+DataLakeUpdateExceptionTypeDef = TypedDict(
+    "DataLakeUpdateExceptionTypeDef",
+    {
+        "code": str,
+        "reason": str,
+    },
+    total=False,
+)
 
-_RequiredDeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAwsLogSourceRequestRequestTypeDef",
+DeleteAwsLogSourceResponseTypeDef = TypedDict(
+    "DeleteAwsLogSourceResponseTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
+        "failed": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalDeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAwsLogSourceRequestRequestTypeDef",
+
+_RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
-        "disableAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "disableSingleDimension": Sequence[str],
-        "disableTwoDimensions": Mapping[str, Sequence[str]],
+        "sourceName": str,
+    },
+)
+_OptionalDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteCustomLogSourceRequestRequestTypeDef",
+    {
+        "sourceVersion": str,
     },
     total=False,
 )
 
-
-class DeleteAwsLogSourceRequestRequestTypeDef(
-    _RequiredDeleteAwsLogSourceRequestRequestTypeDef,
-    _OptionalDeleteAwsLogSourceRequestRequestTypeDef,
+class DeleteCustomLogSourceRequestRequestTypeDef(
+    _RequiredDeleteCustomLogSourceRequestRequestTypeDef,
+    _OptionalDeleteCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
-    "DeleteCustomLogSourceRequestRequestTypeDef",
+DeleteDataLakeRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeRequestRequestTypeDef",
     {
-        "customSourceName": str,
+        "regions": Sequence[str],
     },
 )
 
-DeleteDatalakeDelegatedAdminRequestRequestTypeDef = TypedDict(
-    "DeleteDatalakeDelegatedAdminRequestRequestTypeDef",
+DeleteSubscriberNotificationRequestRequestTypeDef = TypedDict(
+    "DeleteSubscriberNotificationRequestRequestTypeDef",
     {
-        "account": str,
+        "subscriberId": str,
     },
 )
 
 DeleteSubscriberRequestRequestTypeDef = TypedDict(
     "DeleteSubscriberRequestRequestTypeDef",
     {
-        "id": str,
+        "subscriberId": str,
     },
 )
 
-DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef",
+GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
     {
-        "subscriptionId": str,
+        "exceptionTimeToLive": int,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FailuresTypeDef = TypedDict(
-    "FailuresTypeDef",
+GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     {
-        "exceptionMessage": str,
-        "remediation": str,
-        "timestamp": datetime,
+        "accounts": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
-ProtocolAndNotificationEndpointTypeDef = TypedDict(
-    "ProtocolAndNotificationEndpointTypeDef",
+GetDataLakeSourcesRequestRequestTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestRequestTypeDef",
     {
-        "endpoint": str,
-        "protocol": str,
+        "accounts": Sequence[str],
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetSubscriberRequestRequestTypeDef = TypedDict(
+    "GetSubscriberRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "subscriberId": str,
     },
-    total=False,
 )
 
-GetDatalakeStatusRequestRequestTypeDef = TypedDict(
-    "GetDatalakeStatusRequestRequestTypeDef",
+_RequiredHttpsNotificationConfigurationTypeDef = TypedDict(
+    "_RequiredHttpsNotificationConfigurationTypeDef",
     {
-        "accountSet": Sequence[str],
-        "maxAccountResults": int,
-        "nextToken": str,
+        "endpoint": str,
+        "targetRoleArn": str,
     },
-    total=False,
 )
-
-GetSubscriberRequestRequestTypeDef = TypedDict(
-    "GetSubscriberRequestRequestTypeDef",
+_OptionalHttpsNotificationConfigurationTypeDef = TypedDict(
+    "_OptionalHttpsNotificationConfigurationTypeDef",
     {
-        "id": str,
+        "authorizationApiKeyName": str,
+        "authorizationApiKeyValue": str,
+        "httpMethod": HttpMethodType,
     },
+    total=False,
 )
 
-RetentionSettingTypeDef = TypedDict(
-    "RetentionSettingTypeDef",
+class HttpsNotificationConfigurationTypeDef(
+    _RequiredHttpsNotificationConfigurationTypeDef, _OptionalHttpsNotificationConfigurationTypeDef
+):
+    pass
+
+ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     {
-        "retentionPeriod": int,
-        "storageClass": StorageClassType,
+        "regions": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-LastUpdateFailureTypeDef = TypedDict(
-    "LastUpdateFailureTypeDef",
+ListDataLakeExceptionsRequestRequestTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestRequestTypeDef",
     {
-        "code": str,
-        "reason": str,
+        "maxResults": int,
+        "nextToken": str,
+        "regions": Sequence[str],
     },
     total=False,
 )
 
-ListDatalakeExceptionsRequestRequestTypeDef = TypedDict(
-    "ListDatalakeExceptionsRequestRequestTypeDef",
+ListDataLakesRequestRequestTypeDef = TypedDict(
+    "ListDataLakesRequestRequestTypeDef",
     {
-        "maxFailures": int,
-        "nextToken": str,
-        "regionSet": Sequence[RegionType],
+        "regions": Sequence[str],
     },
     total=False,
 )
 
-ListLogSourcesRequestRequestTypeDef = TypedDict(
-    "ListLogSourcesRequestRequestTypeDef",
+ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
-        "listAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "listSingleDimension": Sequence[str],
-        "listTwoDimensions": Mapping[str, Sequence[str]],
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSubscribersRequestRequestTypeDef = TypedDict(
     "ListSubscribersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-UpdateDatalakeExceptionsExpiryRequestRequestTypeDef = TypedDict(
-    "UpdateDatalakeExceptionsExpiryRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "exceptionMessageExpiry": int,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef = TypedDict(
-    "UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
+RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
+    "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
-        "notificationEndpoint": str,
-        "subscriptionProtocol": SubscriptionProtocolTypeType,
+        "accountId": str,
     },
 )
 
-_RequiredUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "subscriptionId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
-_OptionalUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+
+_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
-        "createSqs": bool,
-        "httpsApiKeyName": str,
-        "httpsApiKeyValue": str,
-        "httpsMethod": HttpsMethodType,
-        "roleArn": str,
-        "subscriptionEndpoint": str,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+    },
+)
+_OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    {
+        "exceptionTimeToLive": int,
     },
     total=False,
 )
 
-
-class UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef(
-    _RequiredUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    _OptionalUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
+class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(
+    _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    _OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+UpdateSubscriberNotificationResponseTypeDef = TypedDict(
+    "UpdateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-_RequiredAccountSourcesTypeDef = TypedDict(
-    "_RequiredAccountSourcesTypeDef",
+CreateAwsLogSourceRequestRequestTypeDef = TypedDict(
+    "CreateAwsLogSourceRequestRequestTypeDef",
     {
-        "account": str,
-        "sourceType": str,
+        "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
-_OptionalAccountSourcesTypeDef = TypedDict(
-    "_OptionalAccountSourcesTypeDef",
+
+DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
+    "DeleteAwsLogSourceRequestRequestTypeDef",
     {
-        "eventClass": OcsfEventClassType,
-        "logsStatus": List[LogsStatusTypeDef],
+        "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
-    total=False,
 )
 
+DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
+    "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    {
+        "region": str,
+        "sources": Sequence[AwsLogSourceResourceTypeDef],
+    },
+)
 
-class AccountSourcesTypeDef(_RequiredAccountSourcesTypeDef, _OptionalAccountSourcesTypeDef):
-    pass
+CustomLogSourceConfigurationTypeDef = TypedDict(
+    "CustomLogSourceConfigurationTypeDef",
+    {
+        "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
+        "providerIdentity": AwsIdentityTypeDef,
+    },
+)
 
+CustomLogSourceResourceTypeDef = TypedDict(
+    "CustomLogSourceResourceTypeDef",
+    {
+        "attributes": CustomLogSourceAttributesTypeDef,
+        "provider": CustomLogSourceProviderTypeDef,
+        "sourceName": str,
+        "sourceVersion": str,
+    },
+    total=False,
+)
 
-CreateDatalakeAutoEnableRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeAutoEnableRequestRequestTypeDef",
+ListDataLakeExceptionsResponseTypeDef = TypedDict(
+    "ListDataLakeExceptionsResponseTypeDef",
     {
-        "configurationForNewAccounts": Sequence[AutoEnableNewRegionConfigurationTypeDef],
+        "exceptions": List[DataLakeExceptionTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDatalakeAutoEnableRequestRequestTypeDef = TypedDict(
-    "DeleteDatalakeAutoEnableRequestRequestTypeDef",
+DataLakeLifecycleConfigurationTypeDef = TypedDict(
+    "DataLakeLifecycleConfigurationTypeDef",
     {
-        "removeFromConfigurationForNewAccounts": Sequence[AutoEnableNewRegionConfigurationTypeDef],
+        "expiration": DataLakeLifecycleExpirationTypeDef,
+        "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
     },
+    total=False,
 )
 
-CreateAwsLogSourceResponseTypeDef = TypedDict(
-    "CreateAwsLogSourceResponseTypeDef",
+DataLakeSourceTypeDef = TypedDict(
+    "DataLakeSourceTypeDef",
     {
-        "failed": List[str],
-        "processing": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "account": str,
+        "eventClasses": List[str],
+        "sourceName": str,
+        "sourceStatuses": List[DataLakeSourceStatusTypeDef],
     },
+    total=False,
 )
 
-CreateCustomLogSourceResponseTypeDef = TypedDict(
-    "CreateCustomLogSourceResponseTypeDef",
+DataLakeUpdateStatusTypeDef = TypedDict(
+    "DataLakeUpdateStatusTypeDef",
     {
-        "customDataLocation": str,
-        "glueCrawlerName": str,
-        "glueDatabaseName": str,
-        "glueTableName": str,
-        "logProviderAccessRoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "exception": DataLakeUpdateExceptionTypeDef,
+        "requestId": str,
+        "status": DataLakeStatusType,
     },
+    total=False,
 )
 
-CreateSubscriberResponseTypeDef = TypedDict(
-    "CreateSubscriberResponseTypeDef",
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
     {
-        "resourceShareArn": str,
-        "resourceShareName": str,
-        "roleArn": str,
-        "s3BucketArn": str,
-        "snsArn": str,
-        "subscriptionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
+        "sqsNotificationConfiguration": Mapping[str, Any],
     },
+    total=False,
 )
 
-CreateSubscriptionNotificationConfigurationResponseTypeDef = TypedDict(
-    "CreateSubscriptionNotificationConfigurationResponseTypeDef",
+CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
-        "queueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
-DeleteAwsLogSourceResponseTypeDef = TypedDict(
-    "DeleteAwsLogSourceResponseTypeDef",
+DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
-        "failed": List[str],
-        "processing": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
-DeleteCustomLogSourceResponseTypeDef = TypedDict(
-    "DeleteCustomLogSourceResponseTypeDef",
+GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
-        "customDataLocation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDatalakeExceptionsSubscriptionResponseTypeDef = TypedDict(
-    "DeleteDatalakeExceptionsSubscriptionResponseTypeDef",
+_RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
+    {
+        "sourceName": str,
+    },
+)
+_OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCustomLogSourceRequestRequestTypeDef",
     {
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "configuration": CustomLogSourceConfigurationTypeDef,
+        "eventClasses": Sequence[str],
+        "sourceVersion": str,
     },
+    total=False,
 )
 
-GetDatalakeAutoEnableResponseTypeDef = TypedDict(
-    "GetDatalakeAutoEnableResponseTypeDef",
+class CreateCustomLogSourceRequestRequestTypeDef(
+    _RequiredCreateCustomLogSourceRequestRequestTypeDef,
+    _OptionalCreateCustomLogSourceRequestRequestTypeDef,
+):
+    pass
+
+CreateCustomLogSourceResponseTypeDef = TypedDict(
+    "CreateCustomLogSourceResponseTypeDef",
     {
-        "autoEnableNewAccounts": List[AutoEnableNewRegionConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "source": CustomLogSourceResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDatalakeExceptionsExpiryResponseTypeDef = TypedDict(
-    "GetDatalakeExceptionsExpiryResponseTypeDef",
+LogSourceResourceTypeDef = TypedDict(
+    "LogSourceResourceTypeDef",
     {
-        "exceptionMessageExpiry": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "awsLogSource": AwsLogSourceResourceTypeDef,
+        "customLogSource": CustomLogSourceResourceTypeDef,
     },
+    total=False,
 )
 
-ListLogSourcesResponseTypeDef = TypedDict(
-    "ListLogSourcesResponseTypeDef",
+_RequiredDataLakeConfigurationTypeDef = TypedDict(
+    "_RequiredDataLakeConfigurationTypeDef",
+    {
+        "region": str,
+    },
+)
+_OptionalDataLakeConfigurationTypeDef = TypedDict(
+    "_OptionalDataLakeConfigurationTypeDef",
     {
+        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class DataLakeConfigurationTypeDef(
+    _RequiredDataLakeConfigurationTypeDef, _OptionalDataLakeConfigurationTypeDef
+):
+    pass
+
+GetDataLakeSourcesResponseTypeDef = TypedDict(
+    "GetDataLakeSourcesResponseTypeDef",
+    {
+        "dataLakeArn": str,
+        "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
-        "regionSourceTypesAccountsList": List[Dict[str, Dict[str, List[str]]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDataLakeResourceTypeDef = TypedDict(
+    "_RequiredDataLakeResourceTypeDef",
+    {
+        "dataLakeArn": str,
+        "region": str,
+    },
+)
+_OptionalDataLakeResourceTypeDef = TypedDict(
+    "_OptionalDataLakeResourceTypeDef",
+    {
+        "createStatus": DataLakeStatusType,
+        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+        "s3BucketArn": str,
+        "updateStatus": DataLakeUpdateStatusTypeDef,
+    },
+    total=False,
+)
+
+class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
+    pass
+
+CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
+    "CreateSubscriberNotificationRequestRequestTypeDef",
+    {
+        "configuration": NotificationConfigurationTypeDef,
+        "subscriberId": str,
     },
 )
 
-UpdateSubscriptionNotificationConfigurationResponseTypeDef = TypedDict(
-    "UpdateSubscriptionNotificationConfigurationResponseTypeDef",
+UpdateSubscriberNotificationRequestRequestTypeDef = TypedDict(
+    "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
-        "queueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "configuration": NotificationConfigurationTypeDef,
+        "subscriberId": str,
     },
 )
 
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
-        "accountId": str,
-        "externalId": str,
-        "sourceTypes": Sequence[SourceTypeTypeDef],
+        "sources": Sequence[LogSourceResourceTypeDef],
+        "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
 )
 _OptionalCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSubscriberRequestRequestTypeDef",
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
     },
     total=False,
 )
 
-
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
 ):
     pass
 
+ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
+    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
+    {
+        "accounts": Sequence[str],
+        "regions": Sequence[str],
+        "sources": Sequence[LogSourceResourceTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListLogSourcesRequestRequestTypeDef = TypedDict(
+    "ListLogSourcesRequestRequestTypeDef",
+    {
+        "accounts": Sequence[str],
+        "maxResults": int,
+        "nextToken": str,
+        "regions": Sequence[str],
+        "sources": Sequence[LogSourceResourceTypeDef],
+    },
+    total=False,
+)
+
+LogSourceTypeDef = TypedDict(
+    "LogSourceTypeDef",
+    {
+        "account": str,
+        "region": str,
+        "sources": List[LogSourceResourceTypeDef],
+    },
+    total=False,
+)
 
 _RequiredSubscriberResourceTypeDef = TypedDict(
     "_RequiredSubscriberResourceTypeDef",
     {
-        "accountId": str,
-        "sourceTypes": List[SourceTypeTypeDef],
-        "subscriptionId": str,
+        "sources": List[LogSourceResourceTypeDef],
+        "subscriberArn": str,
+        "subscriberId": str,
+        "subscriberIdentity": AwsIdentityTypeDef,
+        "subscriberName": str,
     },
 )
 _OptionalSubscriberResourceTypeDef = TypedDict(
     "_OptionalSubscriberResourceTypeDef",
     {
         "accessTypes": List[AccessTypeType],
         "createdAt": datetime,
-        "externalId": str,
         "resourceShareArn": str,
         "resourceShareName": str,
         "roleArn": str,
         "s3BucketArn": str,
-        "snsArn": str,
         "subscriberDescription": str,
-        "subscriberName": str,
-        "subscriptionEndpoint": str,
-        "subscriptionProtocol": EndpointProtocolType,
-        "subscriptionStatus": SubscriptionStatusType,
+        "subscriberEndpoint": str,
+        "subscriberStatus": SubscriberStatusType,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-
 class SubscriberResourceTypeDef(
     _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
 ):
     pass
 
-
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
-        "id": str,
-        "sourceTypes": Sequence[SourceTypeTypeDef],
+        "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSubscriberRequestRequestTypeDef",
     {
-        "externalId": str,
+        "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberDescription": str,
+        "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
     total=False,
 )
 
-
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
-
-FailuresResponseTypeDef = TypedDict(
-    "FailuresResponseTypeDef",
+CreateDataLakeRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeRequestRequestTypeDef",
     {
-        "failures": List[FailuresTypeDef],
-        "region": str,
+        "configurations": Sequence[DataLakeConfigurationTypeDef],
+        "metaStoreManagerRoleArn": str,
     },
-    total=False,
 )
 
-GetDatalakeExceptionsSubscriptionResponseTypeDef = TypedDict(
-    "GetDatalakeExceptionsSubscriptionResponseTypeDef",
+UpdateDataLakeRequestRequestTypeDef = TypedDict(
+    "UpdateDataLakeRequestRequestTypeDef",
     {
-        "protocolAndNotificationEndpoint": ProtocolAndNotificationEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "configurations": Sequence[DataLakeConfigurationTypeDef],
     },
 )
 
-GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef = TypedDict(
-    "GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef",
+CreateDataLakeResponseTypeDef = TypedDict(
+    "CreateDataLakeResponseTypeDef",
     {
-        "accountSet": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "dataLakes": List[DataLakeResourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef = TypedDict(
-    "ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef",
+ListDataLakesResponseTypeDef = TypedDict(
+    "ListDataLakesResponseTypeDef",
     {
-        "regionSet": Sequence[RegionType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "dataLakes": List[DataLakeResourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
-    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
+UpdateDataLakeResponseTypeDef = TypedDict(
+    "UpdateDataLakeResponseTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
-        "listAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "listSingleDimension": Sequence[str],
-        "listTwoDimensions": Mapping[str, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "dataLakes": List[DataLakeResourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-LakeConfigurationRequestTypeDef = TypedDict(
-    "LakeConfigurationRequestTypeDef",
-    {
-        "encryptionKey": str,
-        "replicationDestinationRegions": Sequence[RegionType],
-        "replicationRoleArn": str,
-        "retentionSettings": Sequence[RetentionSettingTypeDef],
-        "tagsMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-UpdateStatusTypeDef = TypedDict(
-    "UpdateStatusTypeDef",
+ListLogSourcesResponseTypeDef = TypedDict(
+    "ListLogSourcesResponseTypeDef",
     {
-        "lastUpdateFailure": LastUpdateFailureTypeDef,
-        "lastUpdateRequestId": str,
-        "lastUpdateStatus": settingsStatusType,
+        "nextToken": str,
+        "sources": List[LogSourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-GetDatalakeStatusResponseTypeDef = TypedDict(
-    "GetDatalakeStatusResponseTypeDef",
+CreateSubscriberResponseTypeDef = TypedDict(
+    "CreateSubscriberResponseTypeDef",
     {
-        "accountSourcesList": List[AccountSourcesTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "subscriber": SubscriberResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSubscriberResponseTypeDef = TypedDict(
     "GetSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscribersResponseTypeDef = TypedDict(
     "ListSubscribersResponseTypeDef",
     {
         "nextToken": str,
         "subscribers": List[SubscriberResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSubscriberResponseTypeDef = TypedDict(
     "UpdateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatalakeExceptionsResponseTypeDef = TypedDict(
-    "ListDatalakeExceptionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "nonRetryableFailures": List[FailuresResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatalakeRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeRequestRequestTypeDef",
-    {
-        "configurations": Mapping[RegionType, LakeConfigurationRequestTypeDef],
-        "enableAll": bool,
-        "metaStoreManagerRoleArn": str,
-        "regions": Sequence[RegionType],
-    },
-    total=False,
-)
-
-UpdateDatalakeRequestRequestTypeDef = TypedDict(
-    "UpdateDatalakeRequestRequestTypeDef",
-    {
-        "configurations": Mapping[RegionType, LakeConfigurationRequestTypeDef],
-    },
-)
-
-LakeConfigurationResponseTypeDef = TypedDict(
-    "LakeConfigurationResponseTypeDef",
-    {
-        "encryptionKey": str,
-        "replicationDestinationRegions": List[RegionType],
-        "replicationRoleArn": str,
-        "retentionSettings": List[RetentionSettingTypeDef],
-        "s3BucketArn": str,
-        "status": settingsStatusType,
-        "tagsMap": Dict[str, str],
-        "updateStatus": UpdateStatusTypeDef,
-    },
-    total=False,
-)
-
-GetDatalakeResponseTypeDef = TypedDict(
-    "GetDatalakeResponseTypeDef",
-    {
-        "configurations": Dict[RegionType, LakeConfigurationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake/type_defs.pyi` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,765 +2,910 @@
 Type annotations for securitylake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_securitylake.type_defs import LogsStatusTypeDef
+    from mypy_boto3_securitylake.type_defs import AwsIdentityTypeDef
 
-    data: LogsStatusTypeDef = {...}
+    data: AwsIdentityTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccessTypeType,
-    AwsLogSourceTypeType,
-    DimensionType,
-    EndpointProtocolType,
-    HttpsMethodType,
-    OcsfEventClassType,
-    RegionType,
-    SourceStatusType,
-    StorageClassType,
-    SubscriptionProtocolTypeType,
-    SubscriptionStatusType,
-    settingsStatusType,
+    AwsLogSourceNameType,
+    DataLakeStatusType,
+    HttpMethodType,
+    SourceCollectionStatusType,
+    SubscriberStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "LogsStatusTypeDef",
-    "AutoEnableNewRegionConfigurationTypeDef",
-    "CreateAwsLogSourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "CreateCustomLogSourceRequestRequestTypeDef",
-    "CreateDatalakeDelegatedAdminRequestRequestTypeDef",
-    "CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
-    "SourceTypeTypeDef",
-    "CreateSubscriptionNotificationConfigurationRequestRequestTypeDef",
-    "DeleteAwsLogSourceRequestRequestTypeDef",
+    "AwsIdentityTypeDef",
+    "AwsLogSourceConfigurationTypeDef",
+    "AwsLogSourceResourceTypeDef",
+    "CreateAwsLogSourceResponseTypeDef",
+    "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    "CreateSubscriberNotificationResponseTypeDef",
+    "CustomLogSourceAttributesTypeDef",
+    "CustomLogSourceCrawlerConfigurationTypeDef",
+    "CustomLogSourceProviderTypeDef",
+    "DataLakeEncryptionConfigurationTypeDef",
+    "DataLakeReplicationConfigurationTypeDef",
+    "DataLakeExceptionTypeDef",
+    "DataLakeLifecycleExpirationTypeDef",
+    "DataLakeLifecycleTransitionTypeDef",
+    "DataLakeSourceStatusTypeDef",
+    "DataLakeUpdateExceptionTypeDef",
+    "DeleteAwsLogSourceResponseTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
-    "DeleteDatalakeDelegatedAdminRequestRequestTypeDef",
+    "DeleteDataLakeRequestRequestTypeDef",
+    "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef",
-    "FailuresTypeDef",
-    "ProtocolAndNotificationEndpointTypeDef",
-    "PaginatorConfigTypeDef",
-    "GetDatalakeStatusRequestRequestTypeDef",
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
-    "RetentionSettingTypeDef",
-    "LastUpdateFailureTypeDef",
-    "ListDatalakeExceptionsRequestRequestTypeDef",
-    "ListLogSourcesRequestRequestTypeDef",
+    "HttpsNotificationConfigurationTypeDef",
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    "ListDataLakeExceptionsRequestRequestTypeDef",
+    "ListDataLakesRequestRequestTypeDef",
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "ListSubscribersRequestRequestTypeDef",
-    "UpdateDatalakeExceptionsExpiryRequestRequestTypeDef",
-    "UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
-    "UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef",
-    "AccountSourcesTypeDef",
-    "CreateDatalakeAutoEnableRequestRequestTypeDef",
-    "DeleteDatalakeAutoEnableRequestRequestTypeDef",
-    "CreateAwsLogSourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    "UpdateSubscriberNotificationResponseTypeDef",
+    "CreateAwsLogSourceRequestRequestTypeDef",
+    "DeleteAwsLogSourceRequestRequestTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    "CustomLogSourceConfigurationTypeDef",
+    "CustomLogSourceResourceTypeDef",
+    "ListDataLakeExceptionsResponseTypeDef",
+    "DataLakeLifecycleConfigurationTypeDef",
+    "DataLakeSourceTypeDef",
+    "DataLakeUpdateStatusTypeDef",
+    "NotificationConfigurationTypeDef",
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
+    "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
-    "CreateSubscriberResponseTypeDef",
-    "CreateSubscriptionNotificationConfigurationResponseTypeDef",
-    "DeleteAwsLogSourceResponseTypeDef",
-    "DeleteCustomLogSourceResponseTypeDef",
-    "DeleteDatalakeExceptionsSubscriptionResponseTypeDef",
-    "GetDatalakeAutoEnableResponseTypeDef",
-    "GetDatalakeExceptionsExpiryResponseTypeDef",
-    "ListLogSourcesResponseTypeDef",
-    "UpdateSubscriptionNotificationConfigurationResponseTypeDef",
+    "LogSourceResourceTypeDef",
+    "DataLakeConfigurationTypeDef",
+    "GetDataLakeSourcesResponseTypeDef",
+    "DataLakeResourceTypeDef",
+    "CreateSubscriberNotificationRequestRequestTypeDef",
+    "UpdateSubscriberNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
+    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
+    "ListLogSourcesRequestRequestTypeDef",
+    "LogSourceTypeDef",
     "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
-    "FailuresResponseTypeDef",
-    "GetDatalakeExceptionsSubscriptionResponseTypeDef",
-    "GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef",
-    "ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef",
-    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    "LakeConfigurationRequestTypeDef",
-    "UpdateStatusTypeDef",
-    "GetDatalakeStatusResponseTypeDef",
+    "CreateDataLakeRequestRequestTypeDef",
+    "UpdateDataLakeRequestRequestTypeDef",
+    "CreateDataLakeResponseTypeDef",
+    "ListDataLakesResponseTypeDef",
+    "UpdateDataLakeResponseTypeDef",
+    "ListLogSourcesResponseTypeDef",
+    "CreateSubscriberResponseTypeDef",
     "GetSubscriberResponseTypeDef",
     "ListSubscribersResponseTypeDef",
     "UpdateSubscriberResponseTypeDef",
-    "ListDatalakeExceptionsResponseTypeDef",
-    "CreateDatalakeRequestRequestTypeDef",
-    "UpdateDatalakeRequestRequestTypeDef",
-    "LakeConfigurationResponseTypeDef",
-    "GetDatalakeResponseTypeDef",
 )
 
-LogsStatusTypeDef = TypedDict(
-    "LogsStatusTypeDef",
+AwsIdentityTypeDef = TypedDict(
+    "AwsIdentityTypeDef",
+    {
+        "externalId": str,
+        "principal": str,
+    },
+)
+
+_RequiredAwsLogSourceConfigurationTypeDef = TypedDict(
+    "_RequiredAwsLogSourceConfigurationTypeDef",
+    {
+        "regions": Sequence[str],
+        "sourceName": AwsLogSourceNameType,
+    },
+)
+_OptionalAwsLogSourceConfigurationTypeDef = TypedDict(
+    "_OptionalAwsLogSourceConfigurationTypeDef",
+    {
+        "accounts": Sequence[str],
+        "sourceVersion": str,
+    },
+    total=False,
+)
+
+
+class AwsLogSourceConfigurationTypeDef(
+    _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
+):
+    pass
+
+
+AwsLogSourceResourceTypeDef = TypedDict(
+    "AwsLogSourceResourceTypeDef",
     {
-        "healthStatus": SourceStatusType,
-        "pathToLogs": str,
+        "sourceName": AwsLogSourceNameType,
+        "sourceVersion": str,
     },
+    total=False,
 )
 
-AutoEnableNewRegionConfigurationTypeDef = TypedDict(
-    "AutoEnableNewRegionConfigurationTypeDef",
+CreateAwsLogSourceResponseTypeDef = TypedDict(
+    "CreateAwsLogSourceResponseTypeDef",
     {
-        "region": RegionType,
-        "sources": Sequence[AwsLogSourceTypeType],
+        "failed": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAwsLogSourceRequestRequestTypeDef",
+_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
     },
 )
-_OptionalCreateAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAwsLogSourceRequestRequestTypeDef",
+_OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
-        "enableAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "enableSingleDimension": Sequence[str],
-        "enableTwoDimensions": Mapping[str, Sequence[str]],
+        "exceptionTimeToLive": int,
     },
     total=False,
 )
 
-class CreateAwsLogSourceRequestRequestTypeDef(
-    _RequiredCreateAwsLogSourceRequestRequestTypeDef,
-    _OptionalCreateAwsLogSourceRequestRequestTypeDef,
+
+class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
+    _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+CreateSubscriberNotificationResponseTypeDef = TypedDict(
+    "CreateSubscriberNotificationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "subscriberEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCustomLogSourceRequestRequestTypeDef = TypedDict(
-    "CreateCustomLogSourceRequestRequestTypeDef",
+CustomLogSourceAttributesTypeDef = TypedDict(
+    "CustomLogSourceAttributesTypeDef",
     {
-        "customSourceName": str,
-        "eventClass": OcsfEventClassType,
-        "glueInvocationRoleArn": str,
-        "logProviderAccountId": str,
+        "crawlerArn": str,
+        "databaseArn": str,
+        "tableArn": str,
     },
+    total=False,
 )
 
-CreateDatalakeDelegatedAdminRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeDelegatedAdminRequestRequestTypeDef",
+CustomLogSourceCrawlerConfigurationTypeDef = TypedDict(
+    "CustomLogSourceCrawlerConfigurationTypeDef",
     {
-        "account": str,
+        "roleArn": str,
     },
 )
 
-CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
+CustomLogSourceProviderTypeDef = TypedDict(
+    "CustomLogSourceProviderTypeDef",
     {
-        "notificationEndpoint": str,
-        "subscriptionProtocol": SubscriptionProtocolTypeType,
+        "location": str,
+        "roleArn": str,
     },
+    total=False,
 )
 
-SourceTypeTypeDef = TypedDict(
-    "SourceTypeTypeDef",
+DataLakeEncryptionConfigurationTypeDef = TypedDict(
+    "DataLakeEncryptionConfigurationTypeDef",
     {
-        "awsSourceType": AwsLogSourceTypeType,
-        "customSourceType": str,
+        "kmsKeyId": str,
     },
     total=False,
 )
 
-_RequiredCreateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+DataLakeReplicationConfigurationTypeDef = TypedDict(
+    "DataLakeReplicationConfigurationTypeDef",
     {
-        "subscriptionId": str,
+        "regions": Sequence[str],
+        "roleArn": str,
     },
+    total=False,
 )
-_OptionalCreateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+
+DataLakeExceptionTypeDef = TypedDict(
+    "DataLakeExceptionTypeDef",
     {
-        "createSqs": bool,
-        "httpsApiKeyName": str,
-        "httpsApiKeyValue": str,
-        "httpsMethod": HttpsMethodType,
-        "roleArn": str,
-        "subscriptionEndpoint": str,
+        "exception": str,
+        "region": str,
+        "remediation": str,
+        "timestamp": datetime,
     },
     total=False,
 )
 
-class CreateSubscriptionNotificationConfigurationRequestRequestTypeDef(
-    _RequiredCreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    _OptionalCreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-):
-    pass
+DataLakeLifecycleExpirationTypeDef = TypedDict(
+    "DataLakeLifecycleExpirationTypeDef",
+    {
+        "days": int,
+    },
+    total=False,
+)
 
-_RequiredDeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAwsLogSourceRequestRequestTypeDef",
+DataLakeLifecycleTransitionTypeDef = TypedDict(
+    "DataLakeLifecycleTransitionTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
+        "days": int,
+        "storageClass": str,
     },
+    total=False,
 )
-_OptionalDeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAwsLogSourceRequestRequestTypeDef",
+
+DataLakeSourceStatusTypeDef = TypedDict(
+    "DataLakeSourceStatusTypeDef",
     {
-        "disableAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "disableSingleDimension": Sequence[str],
-        "disableTwoDimensions": Mapping[str, Sequence[str]],
+        "resource": str,
+        "status": SourceCollectionStatusType,
     },
     total=False,
 )
 
-class DeleteAwsLogSourceRequestRequestTypeDef(
-    _RequiredDeleteAwsLogSourceRequestRequestTypeDef,
-    _OptionalDeleteAwsLogSourceRequestRequestTypeDef,
-):
-    pass
+DataLakeUpdateExceptionTypeDef = TypedDict(
+    "DataLakeUpdateExceptionTypeDef",
+    {
+        "code": str,
+        "reason": str,
+    },
+    total=False,
+)
 
-DeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
-    "DeleteCustomLogSourceRequestRequestTypeDef",
+DeleteAwsLogSourceResponseTypeDef = TypedDict(
+    "DeleteAwsLogSourceResponseTypeDef",
     {
-        "customSourceName": str,
+        "failed": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDatalakeDelegatedAdminRequestRequestTypeDef = TypedDict(
-    "DeleteDatalakeDelegatedAdminRequestRequestTypeDef",
+_RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
-        "account": str,
+        "sourceName": str,
     },
 )
+_OptionalDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteCustomLogSourceRequestRequestTypeDef",
+    {
+        "sourceVersion": str,
+    },
+    total=False,
+)
 
-DeleteSubscriberRequestRequestTypeDef = TypedDict(
-    "DeleteSubscriberRequestRequestTypeDef",
+
+class DeleteCustomLogSourceRequestRequestTypeDef(
+    _RequiredDeleteCustomLogSourceRequestRequestTypeDef,
+    _OptionalDeleteCustomLogSourceRequestRequestTypeDef,
+):
+    pass
+
+
+DeleteDataLakeRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeRequestRequestTypeDef",
     {
-        "id": str,
+        "regions": Sequence[str],
     },
 )
 
-DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef",
+DeleteSubscriberNotificationRequestRequestTypeDef = TypedDict(
+    "DeleteSubscriberNotificationRequestRequestTypeDef",
     {
-        "subscriptionId": str,
+        "subscriberId": str,
     },
 )
 
-FailuresTypeDef = TypedDict(
-    "FailuresTypeDef",
+DeleteSubscriberRequestRequestTypeDef = TypedDict(
+    "DeleteSubscriberRequestRequestTypeDef",
     {
-        "exceptionMessage": str,
-        "remediation": str,
-        "timestamp": datetime,
+        "subscriberId": str,
     },
 )
 
-ProtocolAndNotificationEndpointTypeDef = TypedDict(
-    "ProtocolAndNotificationEndpointTypeDef",
+GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
     {
-        "endpoint": str,
-        "protocol": str,
+        "exceptionTimeToLive": int,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "accounts": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-GetDatalakeStatusRequestRequestTypeDef = TypedDict(
-    "GetDatalakeStatusRequestRequestTypeDef",
+GetDataLakeSourcesRequestRequestTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestRequestTypeDef",
     {
-        "accountSet": Sequence[str],
-        "maxAccountResults": int,
+        "accounts": Sequence[str],
+        "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 GetSubscriberRequestRequestTypeDef = TypedDict(
     "GetSubscriberRequestRequestTypeDef",
     {
-        "id": str,
+        "subscriberId": str,
     },
 )
 
-RetentionSettingTypeDef = TypedDict(
-    "RetentionSettingTypeDef",
+_RequiredHttpsNotificationConfigurationTypeDef = TypedDict(
+    "_RequiredHttpsNotificationConfigurationTypeDef",
     {
-        "retentionPeriod": int,
-        "storageClass": StorageClassType,
+        "endpoint": str,
+        "targetRoleArn": str,
+    },
+)
+_OptionalHttpsNotificationConfigurationTypeDef = TypedDict(
+    "_OptionalHttpsNotificationConfigurationTypeDef",
+    {
+        "authorizationApiKeyName": str,
+        "authorizationApiKeyValue": str,
+        "httpMethod": HttpMethodType,
     },
     total=False,
 )
 
-LastUpdateFailureTypeDef = TypedDict(
-    "LastUpdateFailureTypeDef",
+
+class HttpsNotificationConfigurationTypeDef(
+    _RequiredHttpsNotificationConfigurationTypeDef, _OptionalHttpsNotificationConfigurationTypeDef
+):
+    pass
+
+
+ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     {
-        "code": str,
-        "reason": str,
+        "regions": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatalakeExceptionsRequestRequestTypeDef = TypedDict(
-    "ListDatalakeExceptionsRequestRequestTypeDef",
+ListDataLakeExceptionsRequestRequestTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestRequestTypeDef",
     {
-        "maxFailures": int,
+        "maxResults": int,
         "nextToken": str,
-        "regionSet": Sequence[RegionType],
+        "regions": Sequence[str],
     },
     total=False,
 )
 
-ListLogSourcesRequestRequestTypeDef = TypedDict(
-    "ListLogSourcesRequestRequestTypeDef",
+ListDataLakesRequestRequestTypeDef = TypedDict(
+    "ListDataLakesRequestRequestTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
-        "listAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "listSingleDimension": Sequence[str],
-        "listTwoDimensions": Mapping[str, Sequence[str]],
-        "maxResults": int,
-        "nextToken": str,
+        "regions": Sequence[str],
+    },
+    total=False,
+)
+
+ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSubscribersRequestRequestTypeDef = TypedDict(
     "ListSubscribersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-UpdateDatalakeExceptionsExpiryRequestRequestTypeDef = TypedDict(
-    "UpdateDatalakeExceptionsExpiryRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "exceptionMessageExpiry": int,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef = TypedDict(
-    "UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef",
+RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
+    "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
-        "notificationEndpoint": str,
-        "subscriptionProtocol": SubscriptionProtocolTypeType,
+        "accountId": str,
     },
 )
 
-_RequiredUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "subscriptionId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
-_OptionalUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef",
+
+_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
-        "createSqs": bool,
-        "httpsApiKeyName": str,
-        "httpsApiKeyValue": str,
-        "httpsMethod": HttpsMethodType,
-        "roleArn": str,
-        "subscriptionEndpoint": str,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+    },
+)
+_OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    {
+        "exceptionTimeToLive": int,
     },
     total=False,
 )
 
-class UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef(
-    _RequiredUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    _OptionalUpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
+
+class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(
+    _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    _OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAccountSourcesTypeDef = TypedDict(
-    "_RequiredAccountSourcesTypeDef",
+
+UpdateSubscriberNotificationResponseTypeDef = TypedDict(
+    "UpdateSubscriberNotificationResponseTypeDef",
     {
-        "account": str,
-        "sourceType": str,
+        "subscriberEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAwsLogSourceRequestRequestTypeDef = TypedDict(
+    "CreateAwsLogSourceRequestRequestTypeDef",
+    {
+        "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
-_OptionalAccountSourcesTypeDef = TypedDict(
-    "_OptionalAccountSourcesTypeDef",
+
+DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
+    "DeleteAwsLogSourceRequestRequestTypeDef",
+    {
+        "sources": Sequence[AwsLogSourceConfigurationTypeDef],
+    },
+)
+
+DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
+    "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    {
+        "region": str,
+        "sources": Sequence[AwsLogSourceResourceTypeDef],
+    },
+)
+
+CustomLogSourceConfigurationTypeDef = TypedDict(
+    "CustomLogSourceConfigurationTypeDef",
     {
-        "eventClass": OcsfEventClassType,
-        "logsStatus": List[LogsStatusTypeDef],
+        "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
+        "providerIdentity": AwsIdentityTypeDef,
+    },
+)
+
+CustomLogSourceResourceTypeDef = TypedDict(
+    "CustomLogSourceResourceTypeDef",
+    {
+        "attributes": CustomLogSourceAttributesTypeDef,
+        "provider": CustomLogSourceProviderTypeDef,
+        "sourceName": str,
+        "sourceVersion": str,
     },
     total=False,
 )
 
-class AccountSourcesTypeDef(_RequiredAccountSourcesTypeDef, _OptionalAccountSourcesTypeDef):
-    pass
+ListDataLakeExceptionsResponseTypeDef = TypedDict(
+    "ListDataLakeExceptionsResponseTypeDef",
+    {
+        "exceptions": List[DataLakeExceptionTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-CreateDatalakeAutoEnableRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeAutoEnableRequestRequestTypeDef",
+DataLakeLifecycleConfigurationTypeDef = TypedDict(
+    "DataLakeLifecycleConfigurationTypeDef",
     {
-        "configurationForNewAccounts": Sequence[AutoEnableNewRegionConfigurationTypeDef],
+        "expiration": DataLakeLifecycleExpirationTypeDef,
+        "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
     },
+    total=False,
 )
 
-DeleteDatalakeAutoEnableRequestRequestTypeDef = TypedDict(
-    "DeleteDatalakeAutoEnableRequestRequestTypeDef",
+DataLakeSourceTypeDef = TypedDict(
+    "DataLakeSourceTypeDef",
     {
-        "removeFromConfigurationForNewAccounts": Sequence[AutoEnableNewRegionConfigurationTypeDef],
+        "account": str,
+        "eventClasses": List[str],
+        "sourceName": str,
+        "sourceStatuses": List[DataLakeSourceStatusTypeDef],
     },
+    total=False,
 )
 
-CreateAwsLogSourceResponseTypeDef = TypedDict(
-    "CreateAwsLogSourceResponseTypeDef",
+DataLakeUpdateStatusTypeDef = TypedDict(
+    "DataLakeUpdateStatusTypeDef",
     {
-        "failed": List[str],
-        "processing": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "exception": DataLakeUpdateExceptionTypeDef,
+        "requestId": str,
+        "status": DataLakeStatusType,
     },
+    total=False,
 )
 
-CreateCustomLogSourceResponseTypeDef = TypedDict(
-    "CreateCustomLogSourceResponseTypeDef",
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
     {
-        "customDataLocation": str,
-        "glueCrawlerName": str,
-        "glueDatabaseName": str,
-        "glueTableName": str,
-        "logProviderAccessRoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
+        "sqsNotificationConfiguration": Mapping[str, Any],
     },
+    total=False,
 )
 
-CreateSubscriberResponseTypeDef = TypedDict(
-    "CreateSubscriberResponseTypeDef",
+CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
-        "resourceShareArn": str,
-        "resourceShareName": str,
-        "roleArn": str,
-        "s3BucketArn": str,
-        "snsArn": str,
-        "subscriptionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
-CreateSubscriptionNotificationConfigurationResponseTypeDef = TypedDict(
-    "CreateSubscriptionNotificationConfigurationResponseTypeDef",
+DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
-        "queueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
-DeleteAwsLogSourceResponseTypeDef = TypedDict(
-    "DeleteAwsLogSourceResponseTypeDef",
+GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
-        "failed": List[str],
-        "processing": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteCustomLogSourceResponseTypeDef = TypedDict(
-    "DeleteCustomLogSourceResponseTypeDef",
+_RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
+    {
+        "sourceName": str,
+    },
+)
+_OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCustomLogSourceRequestRequestTypeDef",
     {
-        "customDataLocation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "configuration": CustomLogSourceConfigurationTypeDef,
+        "eventClasses": Sequence[str],
+        "sourceVersion": str,
     },
+    total=False,
 )
 
-DeleteDatalakeExceptionsSubscriptionResponseTypeDef = TypedDict(
-    "DeleteDatalakeExceptionsSubscriptionResponseTypeDef",
+
+class CreateCustomLogSourceRequestRequestTypeDef(
+    _RequiredCreateCustomLogSourceRequestRequestTypeDef,
+    _OptionalCreateCustomLogSourceRequestRequestTypeDef,
+):
+    pass
+
+
+CreateCustomLogSourceResponseTypeDef = TypedDict(
+    "CreateCustomLogSourceResponseTypeDef",
     {
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "source": CustomLogSourceResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDatalakeAutoEnableResponseTypeDef = TypedDict(
-    "GetDatalakeAutoEnableResponseTypeDef",
+LogSourceResourceTypeDef = TypedDict(
+    "LogSourceResourceTypeDef",
     {
-        "autoEnableNewAccounts": List[AutoEnableNewRegionConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "awsLogSource": AwsLogSourceResourceTypeDef,
+        "customLogSource": CustomLogSourceResourceTypeDef,
     },
+    total=False,
 )
 
-GetDatalakeExceptionsExpiryResponseTypeDef = TypedDict(
-    "GetDatalakeExceptionsExpiryResponseTypeDef",
+_RequiredDataLakeConfigurationTypeDef = TypedDict(
+    "_RequiredDataLakeConfigurationTypeDef",
     {
-        "exceptionMessageExpiry": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "region": str,
     },
 )
+_OptionalDataLakeConfigurationTypeDef = TypedDict(
+    "_OptionalDataLakeConfigurationTypeDef",
+    {
+        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+    },
+    total=False,
+)
 
-ListLogSourcesResponseTypeDef = TypedDict(
-    "ListLogSourcesResponseTypeDef",
+
+class DataLakeConfigurationTypeDef(
+    _RequiredDataLakeConfigurationTypeDef, _OptionalDataLakeConfigurationTypeDef
+):
+    pass
+
+
+GetDataLakeSourcesResponseTypeDef = TypedDict(
+    "GetDataLakeSourcesResponseTypeDef",
     {
+        "dataLakeArn": str,
+        "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
-        "regionSourceTypesAccountsList": List[Dict[str, Dict[str, List[str]]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSubscriptionNotificationConfigurationResponseTypeDef = TypedDict(
-    "UpdateSubscriptionNotificationConfigurationResponseTypeDef",
+_RequiredDataLakeResourceTypeDef = TypedDict(
+    "_RequiredDataLakeResourceTypeDef",
     {
-        "queueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "dataLakeArn": str,
+        "region": str,
+    },
+)
+_OptionalDataLakeResourceTypeDef = TypedDict(
+    "_OptionalDataLakeResourceTypeDef",
+    {
+        "createStatus": DataLakeStatusType,
+        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+        "s3BucketArn": str,
+        "updateStatus": DataLakeUpdateStatusTypeDef,
+    },
+    total=False,
+)
+
+
+class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
+    pass
+
+
+CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
+    "CreateSubscriberNotificationRequestRequestTypeDef",
+    {
+        "configuration": NotificationConfigurationTypeDef,
+        "subscriberId": str,
+    },
+)
+
+UpdateSubscriberNotificationRequestRequestTypeDef = TypedDict(
+    "UpdateSubscriberNotificationRequestRequestTypeDef",
+    {
+        "configuration": NotificationConfigurationTypeDef,
+        "subscriberId": str,
     },
 )
 
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
-        "accountId": str,
-        "externalId": str,
-        "sourceTypes": Sequence[SourceTypeTypeDef],
+        "sources": Sequence[LogSourceResourceTypeDef],
+        "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
 )
 _OptionalCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSubscriberRequestRequestTypeDef",
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
     },
     total=False,
 )
 
+
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
 ):
     pass
 
+
+ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
+    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
+    {
+        "accounts": Sequence[str],
+        "regions": Sequence[str],
+        "sources": Sequence[LogSourceResourceTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListLogSourcesRequestRequestTypeDef = TypedDict(
+    "ListLogSourcesRequestRequestTypeDef",
+    {
+        "accounts": Sequence[str],
+        "maxResults": int,
+        "nextToken": str,
+        "regions": Sequence[str],
+        "sources": Sequence[LogSourceResourceTypeDef],
+    },
+    total=False,
+)
+
+LogSourceTypeDef = TypedDict(
+    "LogSourceTypeDef",
+    {
+        "account": str,
+        "region": str,
+        "sources": List[LogSourceResourceTypeDef],
+    },
+    total=False,
+)
+
 _RequiredSubscriberResourceTypeDef = TypedDict(
     "_RequiredSubscriberResourceTypeDef",
     {
-        "accountId": str,
-        "sourceTypes": List[SourceTypeTypeDef],
-        "subscriptionId": str,
+        "sources": List[LogSourceResourceTypeDef],
+        "subscriberArn": str,
+        "subscriberId": str,
+        "subscriberIdentity": AwsIdentityTypeDef,
+        "subscriberName": str,
     },
 )
 _OptionalSubscriberResourceTypeDef = TypedDict(
     "_OptionalSubscriberResourceTypeDef",
     {
         "accessTypes": List[AccessTypeType],
         "createdAt": datetime,
-        "externalId": str,
         "resourceShareArn": str,
         "resourceShareName": str,
         "roleArn": str,
         "s3BucketArn": str,
-        "snsArn": str,
         "subscriberDescription": str,
-        "subscriberName": str,
-        "subscriptionEndpoint": str,
-        "subscriptionProtocol": EndpointProtocolType,
-        "subscriptionStatus": SubscriptionStatusType,
+        "subscriberEndpoint": str,
+        "subscriberStatus": SubscriberStatusType,
         "updatedAt": datetime,
     },
     total=False,
 )
 
+
 class SubscriberResourceTypeDef(
     _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
 ):
     pass
 
+
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
-        "id": str,
-        "sourceTypes": Sequence[SourceTypeTypeDef],
+        "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSubscriberRequestRequestTypeDef",
     {
-        "externalId": str,
+        "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberDescription": str,
+        "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
     total=False,
 )
 
+
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
-FailuresResponseTypeDef = TypedDict(
-    "FailuresResponseTypeDef",
-    {
-        "failures": List[FailuresTypeDef],
-        "region": str,
-    },
-    total=False,
-)
 
-GetDatalakeExceptionsSubscriptionResponseTypeDef = TypedDict(
-    "GetDatalakeExceptionsSubscriptionResponseTypeDef",
+CreateDataLakeRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeRequestRequestTypeDef",
     {
-        "protocolAndNotificationEndpoint": ProtocolAndNotificationEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef = TypedDict(
-    "GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef",
-    {
-        "accountSet": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "configurations": Sequence[DataLakeConfigurationTypeDef],
+        "metaStoreManagerRoleArn": str,
     },
-    total=False,
 )
 
-ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef = TypedDict(
-    "ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef",
+UpdateDataLakeRequestRequestTypeDef = TypedDict(
+    "UpdateDataLakeRequestRequestTypeDef",
     {
-        "regionSet": Sequence[RegionType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "configurations": Sequence[DataLakeConfigurationTypeDef],
     },
-    total=False,
 )
 
-ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
-    "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
+CreateDataLakeResponseTypeDef = TypedDict(
+    "CreateDataLakeResponseTypeDef",
     {
-        "inputOrder": Sequence[DimensionType],
-        "listAllDimensions": Mapping[str, Mapping[str, Sequence[str]]],
-        "listSingleDimension": Sequence[str],
-        "listTwoDimensions": Mapping[str, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "dataLakes": List[DataLakeResourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
+ListDataLakesResponseTypeDef = TypedDict(
+    "ListDataLakesResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "dataLakes": List[DataLakeResourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-LakeConfigurationRequestTypeDef = TypedDict(
-    "LakeConfigurationRequestTypeDef",
+UpdateDataLakeResponseTypeDef = TypedDict(
+    "UpdateDataLakeResponseTypeDef",
     {
-        "encryptionKey": str,
-        "replicationDestinationRegions": Sequence[RegionType],
-        "replicationRoleArn": str,
-        "retentionSettings": Sequence[RetentionSettingTypeDef],
-        "tagsMap": Mapping[str, str],
+        "dataLakes": List[DataLakeResourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateStatusTypeDef = TypedDict(
-    "UpdateStatusTypeDef",
+ListLogSourcesResponseTypeDef = TypedDict(
+    "ListLogSourcesResponseTypeDef",
     {
-        "lastUpdateFailure": LastUpdateFailureTypeDef,
-        "lastUpdateRequestId": str,
-        "lastUpdateStatus": settingsStatusType,
+        "nextToken": str,
+        "sources": List[LogSourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-GetDatalakeStatusResponseTypeDef = TypedDict(
-    "GetDatalakeStatusResponseTypeDef",
+CreateSubscriberResponseTypeDef = TypedDict(
+    "CreateSubscriberResponseTypeDef",
     {
-        "accountSourcesList": List[AccountSourcesTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "subscriber": SubscriberResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSubscriberResponseTypeDef = TypedDict(
     "GetSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscribersResponseTypeDef = TypedDict(
     "ListSubscribersResponseTypeDef",
     {
         "nextToken": str,
         "subscribers": List[SubscriberResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSubscriberResponseTypeDef = TypedDict(
     "UpdateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatalakeExceptionsResponseTypeDef = TypedDict(
-    "ListDatalakeExceptionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "nonRetryableFailures": List[FailuresResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatalakeRequestRequestTypeDef = TypedDict(
-    "CreateDatalakeRequestRequestTypeDef",
-    {
-        "configurations": Mapping[RegionType, LakeConfigurationRequestTypeDef],
-        "enableAll": bool,
-        "metaStoreManagerRoleArn": str,
-        "regions": Sequence[RegionType],
-    },
-    total=False,
-)
-
-UpdateDatalakeRequestRequestTypeDef = TypedDict(
-    "UpdateDatalakeRequestRequestTypeDef",
-    {
-        "configurations": Mapping[RegionType, LakeConfigurationRequestTypeDef],
-    },
-)
-
-LakeConfigurationResponseTypeDef = TypedDict(
-    "LakeConfigurationResponseTypeDef",
-    {
-        "encryptionKey": str,
-        "replicationDestinationRegions": List[RegionType],
-        "replicationRoleArn": str,
-        "retentionSettings": List[RetentionSettingTypeDef],
-        "s3BucketArn": str,
-        "status": settingsStatusType,
-        "tagsMap": Dict[str, str],
-        "updateStatus": UpdateStatusTypeDef,
-    },
-    total=False,
-)
-
-GetDatalakeResponseTypeDef = TypedDict(
-    "GetDatalakeResponseTypeDef",
-    {
-        "configurations": Dict[RegionType, LakeConfigurationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/PKG-INFO` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securitylake
-Version: 1.26.92
-Summary: Type annotations for boto3.SecurityLake 1.26.92 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SecurityLake 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-securitylake"></a>
 
 # mypy-boto3-securitylake
 
 [![PyPI - mypy-boto3-securitylake](https://img.shields.io/pypi/v/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,29 +280,29 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_securitylake import SecurityLakeClient
 from mypy_boto3_securitylake.paginator import (
-    GetDatalakeStatusPaginator,
-    ListDatalakeExceptionsPaginator,
+    GetDataLakeSourcesPaginator,
+    ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 
 client: SecurityLakeClient = Session().client("securitylake")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
-get_datalake_status_paginator: GetDatalakeStatusPaginator = client.get_paginator(
-    "get_datalake_status"
+get_data_lake_sources_paginator: GetDataLakeSourcesPaginator = client.get_paginator(
+    "get_data_lake_sources"
 )
-list_datalake_exceptions_paginator: ListDatalakeExceptionsPaginator = client.get_paginator(
-    "list_datalake_exceptions"
+list_data_lake_exceptions_paginator: ListDataLakeExceptionsPaginator = client.get_paginator(
+    "list_data_lake_exceptions"
 )
 list_log_sources_paginator: ListLogSourcesPaginator = client.get_paginator("list_log_sources")
 list_subscribers_paginator: ListSubscribersPaginator = client.get_paginator("list_subscribers")
 ```
 
 <a id="literals"></a>
 
@@ -310,29 +310,23 @@
 
 `mypy_boto3_securitylake.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securitylake.literals import (
     AccessTypeType,
-    AwsLogSourceTypeType,
-    DimensionType,
-    EndpointProtocolType,
-    GetDatalakeStatusPaginatorName,
-    HttpsMethodType,
-    ListDatalakeExceptionsPaginatorName,
+    AwsLogSourceNameType,
+    DataLakeStatusType,
+    GetDataLakeSourcesPaginatorName,
+    HttpMethodType,
+    ListDataLakeExceptionsPaginatorName,
     ListLogSourcesPaginatorName,
     ListSubscribersPaginatorName,
-    OcsfEventClassType,
-    RegionType,
-    SourceStatusType,
-    StorageClassType,
-    SubscriptionProtocolTypeType,
-    SubscriptionStatusType,
-    settingsStatusType,
+    SourceCollectionStatusType,
+    SubscriberStatusType,
     SecurityLakeServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -346,117 +340,129 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
-    LogsStatusTypeDef,
-    AutoEnableNewRegionConfigurationTypeDef,
-    CreateAwsLogSourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateCustomLogSourceRequestRequestTypeDef,
-    CreateDatalakeDelegatedAdminRequestRequestTypeDef,
-    CreateDatalakeExceptionsSubscriptionRequestRequestTypeDef,
-    SourceTypeTypeDef,
-    CreateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    DeleteAwsLogSourceRequestRequestTypeDef,
+    AwsIdentityTypeDef,
+    AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    CustomLogSourceAttributesTypeDef,
+    CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderTypeDef,
+    DataLakeEncryptionConfigurationTypeDef,
+    DataLakeReplicationConfigurationTypeDef,
+    DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationTypeDef,
+    DataLakeLifecycleTransitionTypeDef,
+    DataLakeSourceStatusTypeDef,
+    DataLakeUpdateExceptionTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
-    DeleteDatalakeDelegatedAdminRequestRequestTypeDef,
+    DeleteDataLakeRequestRequestTypeDef,
+    DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DeleteSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    FailuresTypeDef,
-    ProtocolAndNotificationEndpointTypeDef,
-    PaginatorConfigTypeDef,
-    GetDatalakeStatusRequestRequestTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
-    RetentionSettingTypeDef,
-    LastUpdateFailureTypeDef,
-    ListDatalakeExceptionsRequestRequestTypeDef,
-    ListLogSourcesRequestRequestTypeDef,
+    HttpsNotificationConfigurationTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListDataLakeExceptionsRequestRequestTypeDef,
+    ListDataLakesRequestRequestTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    UpdateDatalakeExceptionsExpiryRequestRequestTypeDef,
-    UpdateDatalakeExceptionsSubscriptionRequestRequestTypeDef,
-    UpdateSubscriptionNotificationConfigurationRequestRequestTypeDef,
-    AccountSourcesTypeDef,
-    CreateDatalakeAutoEnableRequestRequestTypeDef,
-    DeleteDatalakeAutoEnableRequestRequestTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
+    CreateAwsLogSourceRequestRequestTypeDef,
+    DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceTypeDef,
+    ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationTypeDef,
+    DataLakeSourceTypeDef,
+    DataLakeUpdateStatusTypeDef,
+    NotificationConfigurationTypeDef,
+    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
+    CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
-    CreateSubscriberResponseTypeDef,
-    CreateSubscriptionNotificationConfigurationResponseTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
-    DeleteCustomLogSourceResponseTypeDef,
-    DeleteDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeAutoEnableResponseTypeDef,
-    GetDatalakeExceptionsExpiryResponseTypeDef,
-    ListLogSourcesResponseTypeDef,
-    UpdateSubscriptionNotificationConfigurationResponseTypeDef,
+    LogSourceResourceTypeDef,
+    DataLakeConfigurationTypeDef,
+    GetDataLakeSourcesResponseTypeDef,
+    DataLakeResourceTypeDef,
+    CreateSubscriberNotificationRequestRequestTypeDef,
+    UpdateSubscriberNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
+    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
+    ListLogSourcesRequestRequestTypeDef,
+    LogSourceTypeDef,
     SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
-    FailuresResponseTypeDef,
-    GetDatalakeExceptionsSubscriptionResponseTypeDef,
-    GetDatalakeStatusRequestGetDatalakeStatusPaginateTypeDef,
-    ListDatalakeExceptionsRequestListDatalakeExceptionsPaginateTypeDef,
-    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
-    LakeConfigurationRequestTypeDef,
-    UpdateStatusTypeDef,
-    GetDatalakeStatusResponseTypeDef,
+    CreateDataLakeRequestRequestTypeDef,
+    UpdateDataLakeRequestRequestTypeDef,
+    CreateDataLakeResponseTypeDef,
+    ListDataLakesResponseTypeDef,
+    UpdateDataLakeResponseTypeDef,
+    ListLogSourcesResponseTypeDef,
+    CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
-    ListDatalakeExceptionsResponseTypeDef,
-    CreateDatalakeRequestRequestTypeDef,
-    UpdateDatalakeRequestRequestTypeDef,
-    LakeConfigurationResponseTypeDef,
-    GetDatalakeResponseTypeDef,
 )
 
 
-def get_structure() -> LogsStatusTypeDef:
+def get_structure() -> AwsIdentityTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-securitylake-1.26.92/mypy_boto3_securitylake.egg-info/SOURCES.txt` & `mypy-boto3-securitylake-1.27.0/mypy_boto3_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.26.92/setup.py` & `mypy-boto3-securitylake-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-securitylake.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securitylake",
-    version="1.26.92",
+    version="1.27.0",
     packages=["mypy_boto3_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityLake 1.26.92 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.SecurityLake 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/",
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


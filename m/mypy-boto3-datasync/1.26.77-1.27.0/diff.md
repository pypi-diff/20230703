# Comparing `tmp/mypy-boto3-datasync-1.26.77.tar.gz` & `tmp/mypy-boto3-datasync-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datasync-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-datasync-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-datasync-1.26.77.tar` & `mypy-boto3-datasync-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34899 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39738 2023-02-22 20:33:58.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39691 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.483106 mypy-boto3-datasync-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-03 19:50:38.483106 mypy-boto3-datasync-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.483106 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45375 2023-07-03 19:35:21.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45303 2023-07-03 19:35:21.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-03 19:35:21.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-03 19:35:21.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-03 19:35:21.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-07-03 19:35:21.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55433 2023-07-03 19:35:22.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55372 2023-07-03 19:35:22.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.483106 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-03 19:50:38.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:38.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:38.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:38.000000 mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.483106 mypy-boto3-datasync-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:35:20.000000 mypy-boto3-datasync-1.27.0/setup.py
```

### Comparing `mypy-boto3-datasync-1.26.77/LICENSE` & `mypy-boto3-datasync-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-datasync-1.26.77/PKG-INFO` & `mypy-boto3-datasync-1.27.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.26.77
-Summary: Type annotations for boto3.DataSync 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.DataSync 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-datasync"></a>
 
 # mypy-boto3-datasync
 
 [![PyPI - mypy-boto3-datasync](https://img.shields.io/pypi/v/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,27 +279,39 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_datasync import DataSyncClient
 from mypy_boto3_datasync.paginator import (
+    DescribeStorageSystemResourceMetricsPaginator,
     ListAgentsPaginator,
+    ListDiscoveryJobsPaginator,
     ListLocationsPaginator,
+    ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 
 client: DataSyncClient = Session().client("datasync")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+describe_storage_system_resource_metrics_paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator(
+    "describe_storage_system_resource_metrics"
+)
 list_agents_paginator: ListAgentsPaginator = client.get_paginator("list_agents")
+list_discovery_jobs_paginator: ListDiscoveryJobsPaginator = client.get_paginator(
+    "list_discovery_jobs"
+)
 list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
+list_storage_systems_paginator: ListStorageSystemsPaginator = client.get_paginator(
+    "list_storage_systems"
+)
 list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
     "list_tags_for_resource"
 )
 list_task_executions_paginator: ListTaskExecutionsPaginator = client.get_paginator(
     "list_task_executions"
 )
 list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
@@ -312,23 +324,30 @@
 `mypy_boto3_datasync.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_datasync.literals import (
     AgentStatusType,
     AtimeType,
+    DescribeStorageSystemResourceMetricsPaginatorName,
+    DiscoveryJobStatusType,
+    DiscoveryResourceFilterType,
+    DiscoveryResourceTypeType,
+    DiscoverySystemTypeType,
     EfsInTransitEncryptionType,
     EndpointTypeType,
     FilterTypeType,
     GidType,
     HdfsAuthenticationTypeType,
     HdfsDataTransferProtectionType,
     HdfsRpcProtectionType,
     ListAgentsPaginatorName,
+    ListDiscoveryJobsPaginatorName,
     ListLocationsPaginatorName,
+    ListStorageSystemsPaginatorName,
     ListTagsForResourcePaginatorName,
     ListTaskExecutionsPaginatorName,
     ListTasksPaginatorName,
     LocationFilterNameType,
     LogLevelType,
     MtimeType,
     NfsVersionType,
@@ -336,17 +355,19 @@
     ObjectTagsType,
     OperatorType,
     OverwriteModeType,
     PhaseStatusType,
     PosixPermissionsType,
     PreserveDeletedFilesType,
     PreserveDevicesType,
+    RecommendationStatusType,
     S3StorageClassType,
     SmbSecurityDescriptorCopyFlagsType,
     SmbVersionType,
+    StorageSystemConnectivityStatusType,
     TaskExecutionStatusType,
     TaskFilterNameType,
     TaskQueueingType,
     TaskStatusType,
     TransferModeType,
     UidType,
     VerifyModeType,
@@ -367,81 +388,114 @@
 ### Typed dictionaries
 
 `mypy_boto3_datasync.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
+    CredentialsTypeDef,
+    DiscoveryServerConfigurationTypeDef,
+    TagListEntryTypeDef,
+    AddStorageSystemResponseTypeDef,
     AgentListEntryTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    TagListEntryTypeDef,
-    ResponseMetadataTypeDef,
+    CapacityTypeDef,
+    CreateAgentResponseTypeDef,
     Ec2ConfigTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
+    CreateLocationHdfsResponseTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
     S3ConfigTypeDef,
+    CreateLocationS3ResponseTypeDef,
     SmbMountOptionsTypeDef,
+    CreateLocationSmbResponseTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
+    CreateTaskResponseTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
     PrivateLinkConfigTypeDef,
+    DescribeDiscoveryJobRequestRequestTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
+    DescribeStorageSystemRequestRequestTypeDef,
+    DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
+    DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
+    DescribeStorageSystemResourcesRequestRequestTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
     TaskExecutionResultDetailTypeDef,
     DescribeTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DiscoveryJobListEntryTypeDef,
+    GenerateRecommendationsRequestRequestTypeDef,
+    IOPSTypeDef,
+    LatencyTypeDef,
+    ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
+    ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
+    ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
     LocationListEntryTypeDef,
+    ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
+    ListStorageSystemsRequestRequestTypeDef,
+    StorageSystemListEntryTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
     TaskExecutionListEntryTypeDef,
     TaskFilterTypeDef,
     TaskListEntryTypeDef,
+    MaxP95PerformanceTypeDef,
+    RecommendationTypeDef,
+    ThroughputTypeDef,
+    PaginatorConfigTypeDef,
+    RemoveStorageSystemRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
+    StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
+    UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    UpdateStorageSystemRequestRequestTypeDef,
+    AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateAgentResponseTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
-    CreateLocationHdfsResponseTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
-    CreateLocationS3ResponseTypeDef,
-    CreateLocationSmbResponseTypeDef,
-    CreateTaskResponseTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
     ListAgentsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
     DescribeLocationEfsResponseTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
@@ -456,71 +510,78 @@
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
     DescribeTaskResponseTypeDef,
     UpdateTaskRequestRequestTypeDef,
     DescribeAgentResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
-    ListAgentsRequestListAgentsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
     ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
     ListTasksResponseTypeDef,
+    NetAppONTAPClusterTypeDef,
+    NetAppONTAPSVMTypeDef,
+    NetAppONTAPVolumeTypeDef,
+    P95MetricsTypeDef,
     FsxProtocolTypeDef,
+    ResourceDetailsTypeDef,
+    ResourceMetricsTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
 )
 
 
-def get_structure() -> AgentListEntryTypeDef:
+def get_structure() -> CredentialsTypeDef:
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

### Comparing `mypy-boto3-datasync-1.26.77/README.md` & `mypy-boto3-datasync-1.27.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-datasync"></a>
 
 # mypy-boto3-datasync
 
 [![PyPI - mypy-boto3-datasync](https://img.shields.io/pypi/v/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,27 +247,39 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_datasync import DataSyncClient
 from mypy_boto3_datasync.paginator import (
+    DescribeStorageSystemResourceMetricsPaginator,
     ListAgentsPaginator,
+    ListDiscoveryJobsPaginator,
     ListLocationsPaginator,
+    ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 
 client: DataSyncClient = Session().client("datasync")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+describe_storage_system_resource_metrics_paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator(
+    "describe_storage_system_resource_metrics"
+)
 list_agents_paginator: ListAgentsPaginator = client.get_paginator("list_agents")
+list_discovery_jobs_paginator: ListDiscoveryJobsPaginator = client.get_paginator(
+    "list_discovery_jobs"
+)
 list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
+list_storage_systems_paginator: ListStorageSystemsPaginator = client.get_paginator(
+    "list_storage_systems"
+)
 list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
     "list_tags_for_resource"
 )
 list_task_executions_paginator: ListTaskExecutionsPaginator = client.get_paginator(
     "list_task_executions"
 )
 list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
@@ -280,23 +292,30 @@
 `mypy_boto3_datasync.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_datasync.literals import (
     AgentStatusType,
     AtimeType,
+    DescribeStorageSystemResourceMetricsPaginatorName,
+    DiscoveryJobStatusType,
+    DiscoveryResourceFilterType,
+    DiscoveryResourceTypeType,
+    DiscoverySystemTypeType,
     EfsInTransitEncryptionType,
     EndpointTypeType,
     FilterTypeType,
     GidType,
     HdfsAuthenticationTypeType,
     HdfsDataTransferProtectionType,
     HdfsRpcProtectionType,
     ListAgentsPaginatorName,
+    ListDiscoveryJobsPaginatorName,
     ListLocationsPaginatorName,
+    ListStorageSystemsPaginatorName,
     ListTagsForResourcePaginatorName,
     ListTaskExecutionsPaginatorName,
     ListTasksPaginatorName,
     LocationFilterNameType,
     LogLevelType,
     MtimeType,
     NfsVersionType,
@@ -304,17 +323,19 @@
     ObjectTagsType,
     OperatorType,
     OverwriteModeType,
     PhaseStatusType,
     PosixPermissionsType,
     PreserveDeletedFilesType,
     PreserveDevicesType,
+    RecommendationStatusType,
     S3StorageClassType,
     SmbSecurityDescriptorCopyFlagsType,
     SmbVersionType,
+    StorageSystemConnectivityStatusType,
     TaskExecutionStatusType,
     TaskFilterNameType,
     TaskQueueingType,
     TaskStatusType,
     TransferModeType,
     UidType,
     VerifyModeType,
@@ -335,81 +356,114 @@
 ### Typed dictionaries
 
 `mypy_boto3_datasync.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
+    CredentialsTypeDef,
+    DiscoveryServerConfigurationTypeDef,
+    TagListEntryTypeDef,
+    AddStorageSystemResponseTypeDef,
     AgentListEntryTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    TagListEntryTypeDef,
-    ResponseMetadataTypeDef,
+    CapacityTypeDef,
+    CreateAgentResponseTypeDef,
     Ec2ConfigTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
+    CreateLocationHdfsResponseTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
     S3ConfigTypeDef,
+    CreateLocationS3ResponseTypeDef,
     SmbMountOptionsTypeDef,
+    CreateLocationSmbResponseTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
+    CreateTaskResponseTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
     PrivateLinkConfigTypeDef,
+    DescribeDiscoveryJobRequestRequestTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
+    DescribeStorageSystemRequestRequestTypeDef,
+    DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
+    DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
+    DescribeStorageSystemResourcesRequestRequestTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
     TaskExecutionResultDetailTypeDef,
     DescribeTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DiscoveryJobListEntryTypeDef,
+    GenerateRecommendationsRequestRequestTypeDef,
+    IOPSTypeDef,
+    LatencyTypeDef,
+    ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
+    ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
+    ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
     LocationListEntryTypeDef,
+    ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
+    ListStorageSystemsRequestRequestTypeDef,
+    StorageSystemListEntryTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
     TaskExecutionListEntryTypeDef,
     TaskFilterTypeDef,
     TaskListEntryTypeDef,
+    MaxP95PerformanceTypeDef,
+    RecommendationTypeDef,
+    ThroughputTypeDef,
+    PaginatorConfigTypeDef,
+    RemoveStorageSystemRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
+    StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
+    UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    UpdateStorageSystemRequestRequestTypeDef,
+    AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateAgentResponseTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
-    CreateLocationHdfsResponseTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
-    CreateLocationS3ResponseTypeDef,
-    CreateLocationSmbResponseTypeDef,
-    CreateTaskResponseTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
     ListAgentsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
     DescribeLocationEfsResponseTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
@@ -424,71 +478,78 @@
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
     DescribeTaskResponseTypeDef,
     UpdateTaskRequestRequestTypeDef,
     DescribeAgentResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
-    ListAgentsRequestListAgentsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
     ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
     ListTasksResponseTypeDef,
+    NetAppONTAPClusterTypeDef,
+    NetAppONTAPSVMTypeDef,
+    NetAppONTAPVolumeTypeDef,
+    P95MetricsTypeDef,
     FsxProtocolTypeDef,
+    ResourceDetailsTypeDef,
+    ResourceMetricsTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
 )
 
 
-def get_structure() -> AgentListEntryTypeDef:
+def get_structure() -> CredentialsTypeDef:
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

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.py` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,45 +4,57 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_datasync import (
         Client,
         DataSyncClient,
+        DescribeStorageSystemResourceMetricsPaginator,
         ListAgentsPaginator,
+        ListDiscoveryJobsPaginator,
         ListLocationsPaginator,
+        ListStorageSystemsPaginator,
         ListTagsForResourcePaginator,
         ListTaskExecutionsPaginator,
         ListTasksPaginator,
     )
 
     session = Session()
     client: DataSyncClient = session.client("datasync")
 
+    describe_storage_system_resource_metrics_paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator("describe_storage_system_resource_metrics")
     list_agents_paginator: ListAgentsPaginator = client.get_paginator("list_agents")
+    list_discovery_jobs_paginator: ListDiscoveryJobsPaginator = client.get_paginator("list_discovery_jobs")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
+    list_storage_systems_paginator: ListStorageSystemsPaginator = client.get_paginator("list_storage_systems")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     list_task_executions_paginator: ListTaskExecutionsPaginator = client.get_paginator("list_task_executions")
     list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
     ```
 """
 from .client import DataSyncClient
 from .paginator import (
+    DescribeStorageSystemResourceMetricsPaginator,
     ListAgentsPaginator,
+    ListDiscoveryJobsPaginator,
     ListLocationsPaginator,
+    ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 
 Client = DataSyncClient
 
 
 __all__ = (
     "Client",
     "DataSyncClient",
+    "DescribeStorageSystemResourceMetricsPaginator",
     "ListAgentsPaginator",
+    "ListDiscoveryJobsPaginator",
     "ListLocationsPaginator",
+    "ListStorageSystemsPaginator",
     "ListTagsForResourcePaginator",
     "ListTaskExecutionsPaginator",
     "ListTasksPaginator",
 )
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__main__.py` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataSync 1.26.77\nVersion:         1.26.77\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.DataSync 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.77")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.py` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,74 +10,89 @@
     from mypy_boto3_datasync.client import DataSyncClient
 
     session = Session()
     client: DataSyncClient = session.client("datasync")
     ```
 """
 import sys
+from datetime import datetime
 from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import (
+    DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     HdfsAuthenticationTypeType,
     ObjectStorageServerProtocolType,
     S3StorageClassType,
 )
 from .paginator import (
+    DescribeStorageSystemResourceMetricsPaginator,
     ListAgentsPaginator,
+    ListDiscoveryJobsPaginator,
     ListLocationsPaginator,
+    ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
+    AddStorageSystemResponseTypeDef,
     CreateAgentResponseTypeDef,
     CreateLocationEfsResponseTypeDef,
     CreateLocationFsxLustreResponseTypeDef,
     CreateLocationFsxOntapResponseTypeDef,
     CreateLocationFsxOpenZfsResponseTypeDef,
     CreateLocationFsxWindowsResponseTypeDef,
     CreateLocationHdfsResponseTypeDef,
     CreateLocationNfsResponseTypeDef,
     CreateLocationObjectStorageResponseTypeDef,
     CreateLocationS3ResponseTypeDef,
     CreateLocationSmbResponseTypeDef,
     CreateTaskResponseTypeDef,
+    CredentialsTypeDef,
     DescribeAgentResponseTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsResponseTypeDef,
     DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
     DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     DescribeLocationNfsResponseTypeDef,
     DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3ResponseTypeDef,
     DescribeLocationSmbResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
     DescribeTaskResponseTypeDef,
+    DiscoveryServerConfigurationTypeDef,
     Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
     ListAgentsResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
+    StartDiscoveryJobResponseTypeDef,
     StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
     TaskFilterTypeDef,
     TaskScheduleTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -116,14 +131,34 @@
         """
         DataSyncClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#exceptions)
         """
 
+    def add_storage_system(
+        self,
+        *,
+        ServerConfiguration: DiscoveryServerConfigurationTypeDef,
+        SystemType: Literal["NetAppONTAP"],
+        AgentArns: Sequence[str],
+        ClientToken: str,
+        Credentials: CredentialsTypeDef,
+        CloudWatchLogGroupArn: str = ...,
+        Tags: Sequence[TagListEntryTypeDef] = ...,
+        Name: str = ...
+    ) -> AddStorageSystemResponseTypeDef:
+        """
+        Creates an Amazon Web Services resource for an on-premises storage system that
+        you want DataSync Discovery to collect information about.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#add_storage_system)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#can_paginate)
         """
@@ -317,16 +352,15 @@
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationS3ResponseTypeDef:
         """
-        Creates an endpoint for an Amazon S3 bucket that DataSync can access for a
-        transfer.
+        A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_s3)
         """
 
     def create_location_smb(
         self,
@@ -397,14 +431,24 @@
         Returns metadata about an DataSync agent, such as its name, endpoint type, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_agent)
         """
 
+    def describe_discovery_job(
+        self, *, DiscoveryJobArn: str
+    ) -> DescribeDiscoveryJobResponseTypeDef:
+        """
+        Returns information about a DataSync discovery job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_discovery_job)
+        """
+
     def describe_location_efs(self, *, LocationArn: str) -> DescribeLocationEfsResponseTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_efs)
         """
@@ -492,14 +536,63 @@
         """
         Returns metadata, such as the path and user information about an SMB location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_smb)
         """
 
+    def describe_storage_system(
+        self, *, StorageSystemArn: str
+    ) -> DescribeStorageSystemResponseTypeDef:
+        """
+        Returns information about an on-premises storage system that you're using with
+        DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system)
+        """
+
+    def describe_storage_system_resource_metrics(
+        self,
+        *,
+        DiscoveryJobArn: str,
+        ResourceType: DiscoveryResourceTypeType,
+        ResourceId: str,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
+        """
+        Returns information, including performance data and capacity usage, which
+        DataSync Discovery collects about a specific resource in your-premises storage
+        system.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resource_metrics)
+        """
+
+    def describe_storage_system_resources(
+        self,
+        *,
+        DiscoveryJobArn: str,
+        ResourceType: DiscoveryResourceTypeType,
+        ResourceIds: Sequence[str] = ...,
+        Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeStorageSystemResourcesResponseTypeDef:
+        """
+        Returns information that DataSync Discovery collects about resources in your on-
+        premises storage system.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
+        """
+
     def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
         Returns metadata about a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
@@ -524,39 +617,75 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_presigned_url)
         """
 
+    def generate_recommendations(
+        self,
+        *,
+        DiscoveryJobArn: str,
+        ResourceIds: Sequence[str],
+        ResourceType: DiscoveryResourceTypeType
+    ) -> Dict[str, Any]:
+        """
+        Creates recommendations about where to migrate your data to in Amazon Web
+        Services.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_recommendations)
+        """
+
     def list_agents(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAgentsResponseTypeDef:
         """
         Returns a list of DataSync agents that belong to an Amazon Web Services account
         in the Amazon Web Services Region specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_agents)
         """
 
+    def list_discovery_jobs(
+        self, *, StorageSystemArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListDiscoveryJobsResponseTypeDef:
+        """
+        Provides a list of the existing discovery jobs in the Amazon Web Services Region
+        and Amazon Web Services account where you're using DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_discovery_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_discovery_jobs)
+        """
+
     def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[LocationFilterTypeDef] = ...
     ) -> ListLocationsResponseTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_locations)
         """
 
+    def list_storage_systems(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListStorageSystemsResponseTypeDef:
+        """
+        Lists the on-premises storage systems that you're using with DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_storage_systems)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_storage_systems)
+        """
+
     def list_tags_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags associated with an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tags_for_resource)
@@ -583,14 +712,38 @@
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tasks)
         """
 
+    def remove_storage_system(self, *, StorageSystemArn: str) -> Dict[str, Any]:
+        """
+        Permanently removes a storage system resource from DataSync Discovery, including
+        the associated discovery jobs, collected data, and recommendations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.remove_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#remove_storage_system)
+        """
+
+    def start_discovery_job(
+        self,
+        *,
+        StorageSystemArn: str,
+        CollectionDurationMinutes: int,
+        ClientToken: str,
+        Tags: Sequence[TagListEntryTypeDef] = ...
+    ) -> StartDiscoveryJobResponseTypeDef:
+        """
+        Runs a DataSync discovery job on your on-premises storage system.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_discovery_job)
+        """
+
     def start_task_execution(
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
@@ -599,14 +752,22 @@
         """
         Starts an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_task_execution)
         """
 
+    def stop_discovery_job(self, *, DiscoveryJobArn: str) -> Dict[str, Any]:
+        """
+        Stops a running DataSync discovery job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.stop_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#stop_discovery_job)
+        """
+
     def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagListEntryTypeDef]
     ) -> Dict[str, Any]:
         """
         Applies a *tag* to an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.tag_resource)
@@ -625,14 +786,24 @@
         """
         Updates the name of an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_agent)
         """
 
+    def update_discovery_job(
+        self, *, DiscoveryJobArn: str, CollectionDurationMinutes: int
+    ) -> Dict[str, Any]:
+        """
+        Edits a DataSync discovery job configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_discovery_job)
+        """
+
     def update_location_hdfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,
         BlockSize: int = ...,
@@ -705,14 +876,32 @@
         Updates some of the parameters of a previously created location for Server
         Message Block (SMB) file system access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_smb)
         """
 
+    def update_storage_system(
+        self,
+        *,
+        StorageSystemArn: str,
+        ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,
+        AgentArns: Sequence[str] = ...,
+        Name: str = ...,
+        CloudWatchLogGroupArn: str = ...,
+        Credentials: CredentialsTypeDef = ...
+    ) -> Dict[str, Any]:
+        """
+        Modifies some configurations of an on-premises storage system resource that
+        you're using with DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_storage_system)
+        """
+
     def update_task(
         self,
         *,
         TaskArn: str,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
@@ -727,36 +916,63 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task)
         """
 
     def update_task_execution(
         self, *, TaskExecutionArn: str, Options: OptionsTypeDef
     ) -> Dict[str, Any]:
         """
-        Updates execution of a task.
+        Modifies a running DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task_execution)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_storage_system_resource_metrics"]
+    ) -> DescribeStorageSystemResourceMetricsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_agents"]) -> ListAgentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_discovery_jobs"]
+    ) -> ListDiscoveryJobsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_locations"]) -> ListLocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_storage_systems"]
+    ) -> ListStorageSystemsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.pyi` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -10,74 +10,89 @@
     from mypy_boto3_datasync.client import DataSyncClient
 
     session = Session()
     client: DataSyncClient = session.client("datasync")
     ```
 """
 import sys
+from datetime import datetime
 from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import (
+    DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     HdfsAuthenticationTypeType,
     ObjectStorageServerProtocolType,
     S3StorageClassType,
 )
 from .paginator import (
+    DescribeStorageSystemResourceMetricsPaginator,
     ListAgentsPaginator,
+    ListDiscoveryJobsPaginator,
     ListLocationsPaginator,
+    ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
+    AddStorageSystemResponseTypeDef,
     CreateAgentResponseTypeDef,
     CreateLocationEfsResponseTypeDef,
     CreateLocationFsxLustreResponseTypeDef,
     CreateLocationFsxOntapResponseTypeDef,
     CreateLocationFsxOpenZfsResponseTypeDef,
     CreateLocationFsxWindowsResponseTypeDef,
     CreateLocationHdfsResponseTypeDef,
     CreateLocationNfsResponseTypeDef,
     CreateLocationObjectStorageResponseTypeDef,
     CreateLocationS3ResponseTypeDef,
     CreateLocationSmbResponseTypeDef,
     CreateTaskResponseTypeDef,
+    CredentialsTypeDef,
     DescribeAgentResponseTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsResponseTypeDef,
     DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
     DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     DescribeLocationNfsResponseTypeDef,
     DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3ResponseTypeDef,
     DescribeLocationSmbResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
     DescribeTaskResponseTypeDef,
+    DiscoveryServerConfigurationTypeDef,
     Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
     ListAgentsResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
+    StartDiscoveryJobResponseTypeDef,
     StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
     TaskFilterTypeDef,
     TaskScheduleTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -111,14 +126,33 @@
     def exceptions(self) -> Exceptions:
         """
         DataSyncClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#exceptions)
         """
+    def add_storage_system(
+        self,
+        *,
+        ServerConfiguration: DiscoveryServerConfigurationTypeDef,
+        SystemType: Literal["NetAppONTAP"],
+        AgentArns: Sequence[str],
+        ClientToken: str,
+        Credentials: CredentialsTypeDef,
+        CloudWatchLogGroupArn: str = ...,
+        Tags: Sequence[TagListEntryTypeDef] = ...,
+        Name: str = ...
+    ) -> AddStorageSystemResponseTypeDef:
+        """
+        Creates an Amazon Web Services resource for an on-premises storage system that
+        you want DataSync Discovery to collect information about.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#add_storage_system)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#can_paginate)
         """
@@ -300,16 +334,15 @@
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationS3ResponseTypeDef:
         """
-        Creates an endpoint for an Amazon S3 bucket that DataSync can access for a
-        transfer.
+        A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_s3)
         """
     def create_location_smb(
         self,
         *,
@@ -373,14 +406,23 @@
         """
         Returns metadata about an DataSync agent, such as its name, endpoint type, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_agent)
         """
+    def describe_discovery_job(
+        self, *, DiscoveryJobArn: str
+    ) -> DescribeDiscoveryJobResponseTypeDef:
+        """
+        Returns information about a DataSync discovery job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_discovery_job)
+        """
     def describe_location_efs(self, *, LocationArn: str) -> DescribeLocationEfsResponseTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_efs)
         """
@@ -458,14 +500,60 @@
     def describe_location_smb(self, *, LocationArn: str) -> DescribeLocationSmbResponseTypeDef:
         """
         Returns metadata, such as the path and user information about an SMB location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_smb)
         """
+    def describe_storage_system(
+        self, *, StorageSystemArn: str
+    ) -> DescribeStorageSystemResponseTypeDef:
+        """
+        Returns information about an on-premises storage system that you're using with
+        DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system)
+        """
+    def describe_storage_system_resource_metrics(
+        self,
+        *,
+        DiscoveryJobArn: str,
+        ResourceType: DiscoveryResourceTypeType,
+        ResourceId: str,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
+        """
+        Returns information, including performance data and capacity usage, which
+        DataSync Discovery collects about a specific resource in your-premises storage
+        system.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resource_metrics)
+        """
+    def describe_storage_system_resources(
+        self,
+        *,
+        DiscoveryJobArn: str,
+        ResourceType: DiscoveryResourceTypeType,
+        ResourceIds: Sequence[str] = ...,
+        Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeStorageSystemResourcesResponseTypeDef:
+        """
+        Returns information that DataSync Discovery collects about resources in your on-
+        premises storage system.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
+        """
     def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
         Returns metadata about a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
@@ -487,37 +575,70 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_presigned_url)
         """
+    def generate_recommendations(
+        self,
+        *,
+        DiscoveryJobArn: str,
+        ResourceIds: Sequence[str],
+        ResourceType: DiscoveryResourceTypeType
+    ) -> Dict[str, Any]:
+        """
+        Creates recommendations about where to migrate your data to in Amazon Web
+        Services.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_recommendations)
+        """
     def list_agents(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAgentsResponseTypeDef:
         """
         Returns a list of DataSync agents that belong to an Amazon Web Services account
         in the Amazon Web Services Region specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_agents)
         """
+    def list_discovery_jobs(
+        self, *, StorageSystemArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListDiscoveryJobsResponseTypeDef:
+        """
+        Provides a list of the existing discovery jobs in the Amazon Web Services Region
+        and Amazon Web Services account where you're using DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_discovery_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_discovery_jobs)
+        """
     def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[LocationFilterTypeDef] = ...
     ) -> ListLocationsResponseTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_locations)
         """
+    def list_storage_systems(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListStorageSystemsResponseTypeDef:
+        """
+        Lists the on-premises storage systems that you're using with DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_storage_systems)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_storage_systems)
+        """
     def list_tags_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags associated with an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tags_for_resource)
@@ -541,14 +662,36 @@
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tasks)
         """
+    def remove_storage_system(self, *, StorageSystemArn: str) -> Dict[str, Any]:
+        """
+        Permanently removes a storage system resource from DataSync Discovery, including
+        the associated discovery jobs, collected data, and recommendations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.remove_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#remove_storage_system)
+        """
+    def start_discovery_job(
+        self,
+        *,
+        StorageSystemArn: str,
+        CollectionDurationMinutes: int,
+        ClientToken: str,
+        Tags: Sequence[TagListEntryTypeDef] = ...
+    ) -> StartDiscoveryJobResponseTypeDef:
+        """
+        Runs a DataSync discovery job on your on-premises storage system.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_discovery_job)
+        """
     def start_task_execution(
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
@@ -556,14 +699,21 @@
     ) -> StartTaskExecutionResponseTypeDef:
         """
         Starts an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_task_execution)
         """
+    def stop_discovery_job(self, *, DiscoveryJobArn: str) -> Dict[str, Any]:
+        """
+        Stops a running DataSync discovery job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.stop_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#stop_discovery_job)
+        """
     def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagListEntryTypeDef]
     ) -> Dict[str, Any]:
         """
         Applies a *tag* to an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.tag_resource)
@@ -579,14 +729,23 @@
     def update_agent(self, *, AgentArn: str, Name: str = ...) -> Dict[str, Any]:
         """
         Updates the name of an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_agent)
         """
+    def update_discovery_job(
+        self, *, DiscoveryJobArn: str, CollectionDurationMinutes: int
+    ) -> Dict[str, Any]:
+        """
+        Edits a DataSync discovery job configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_discovery_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_discovery_job)
+        """
     def update_location_hdfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,
         BlockSize: int = ...,
@@ -655,14 +814,31 @@
         """
         Updates some of the parameters of a previously created location for Server
         Message Block (SMB) file system access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_smb)
         """
+    def update_storage_system(
+        self,
+        *,
+        StorageSystemArn: str,
+        ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,
+        AgentArns: Sequence[str] = ...,
+        Name: str = ...,
+        CloudWatchLogGroupArn: str = ...,
+        Credentials: CredentialsTypeDef = ...
+    ) -> Dict[str, Any]:
+        """
+        Modifies some configurations of an on-premises storage system resource that
+        you're using with DataSync Discovery.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_storage_system)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_storage_system)
+        """
     def update_task(
         self,
         *,
         TaskArn: str,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
@@ -676,33 +852,57 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task)
         """
     def update_task_execution(
         self, *, TaskExecutionArn: str, Options: OptionsTypeDef
     ) -> Dict[str, Any]:
         """
-        Updates execution of a task.
+        Modifies a running DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task_execution)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_storage_system_resource_metrics"]
+    ) -> DescribeStorageSystemResourceMetricsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_agents"]) -> ListAgentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_discovery_jobs"]
+    ) -> ListDiscoveryJobsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_locations"]) -> ListLocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_storage_systems"]
+    ) -> ListStorageSystemsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.py` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/literals.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,30 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AgentStatusType",
     "AtimeType",
+    "DescribeStorageSystemResourceMetricsPaginatorName",
+    "DiscoveryJobStatusType",
+    "DiscoveryResourceFilterType",
+    "DiscoveryResourceTypeType",
+    "DiscoverySystemTypeType",
     "EfsInTransitEncryptionType",
     "EndpointTypeType",
     "FilterTypeType",
     "GidType",
     "HdfsAuthenticationTypeType",
     "HdfsDataTransferProtectionType",
     "HdfsRpcProtectionType",
     "ListAgentsPaginatorName",
+    "ListDiscoveryJobsPaginatorName",
     "ListLocationsPaginatorName",
+    "ListStorageSystemsPaginatorName",
     "ListTagsForResourcePaginatorName",
     "ListTaskExecutionsPaginatorName",
     "ListTasksPaginatorName",
     "LocationFilterNameType",
     "LogLevelType",
     "MtimeType",
     "NfsVersionType",
@@ -42,17 +49,19 @@
     "ObjectTagsType",
     "OperatorType",
     "OverwriteModeType",
     "PhaseStatusType",
     "PosixPermissionsType",
     "PreserveDeletedFilesType",
     "PreserveDevicesType",
+    "RecommendationStatusType",
     "S3StorageClassType",
     "SmbSecurityDescriptorCopyFlagsType",
     "SmbVersionType",
+    "StorageSystemConnectivityStatusType",
     "TaskExecutionStatusType",
     "TaskFilterNameType",
     "TaskQueueingType",
     "TaskStatusType",
     "TransferModeType",
     "UidType",
     "VerifyModeType",
@@ -62,23 +71,34 @@
     "PaginatorName",
     "RegionName",
 )
 
 
 AgentStatusType = Literal["OFFLINE", "ONLINE"]
 AtimeType = Literal["BEST_EFFORT", "NONE"]
+DescribeStorageSystemResourceMetricsPaginatorName = Literal[
+    "describe_storage_system_resource_metrics"
+]
+DiscoveryJobStatusType = Literal[
+    "COMPLETED", "COMPLETED_WITH_ISSUES", "FAILED", "RUNNING", "STOPPED", "TERMINATED", "WARNING"
+]
+DiscoveryResourceFilterType = Literal["SVM"]
+DiscoveryResourceTypeType = Literal["CLUSTER", "SVM", "VOLUME"]
+DiscoverySystemTypeType = Literal["NetAppONTAP"]
 EfsInTransitEncryptionType = Literal["NONE", "TLS1_2"]
 EndpointTypeType = Literal["FIPS", "PRIVATE_LINK", "PUBLIC"]
 FilterTypeType = Literal["SIMPLE_PATTERN"]
 GidType = Literal["BOTH", "INT_VALUE", "NAME", "NONE"]
 HdfsAuthenticationTypeType = Literal["KERBEROS", "SIMPLE"]
 HdfsDataTransferProtectionType = Literal["AUTHENTICATION", "DISABLED", "INTEGRITY", "PRIVACY"]
 HdfsRpcProtectionType = Literal["AUTHENTICATION", "DISABLED", "INTEGRITY", "PRIVACY"]
 ListAgentsPaginatorName = Literal["list_agents"]
+ListDiscoveryJobsPaginatorName = Literal["list_discovery_jobs"]
 ListLocationsPaginatorName = Literal["list_locations"]
+ListStorageSystemsPaginatorName = Literal["list_storage_systems"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 ListTaskExecutionsPaginatorName = Literal["list_task_executions"]
 ListTasksPaginatorName = Literal["list_tasks"]
 LocationFilterNameType = Literal["CreationTime", "LocationType", "LocationUri"]
 LogLevelType = Literal["BASIC", "OFF", "TRANSFER"]
 MtimeType = Literal["NONE", "PRESERVE"]
 NfsVersionType = Literal["AUTOMATIC", "NFS3", "NFS4_0", "NFS4_1"]
@@ -97,26 +117,28 @@
     "NotEquals",
 ]
 OverwriteModeType = Literal["ALWAYS", "NEVER"]
 PhaseStatusType = Literal["ERROR", "PENDING", "SUCCESS"]
 PosixPermissionsType = Literal["NONE", "PRESERVE"]
 PreserveDeletedFilesType = Literal["PRESERVE", "REMOVE"]
 PreserveDevicesType = Literal["NONE", "PRESERVE"]
+RecommendationStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "NONE"]
 S3StorageClassType = Literal[
     "DEEP_ARCHIVE",
     "GLACIER",
     "GLACIER_INSTANT_RETRIEVAL",
     "INTELLIGENT_TIERING",
     "ONEZONE_IA",
     "OUTPOSTS",
     "STANDARD",
     "STANDARD_IA",
 ]
 SmbSecurityDescriptorCopyFlagsType = Literal["NONE", "OWNER_DACL", "OWNER_DACL_SACL"]
 SmbVersionType = Literal["AUTOMATIC", "SMB1", "SMB2", "SMB2_0", "SMB3"]
+StorageSystemConnectivityStatusType = Literal["FAIL", "PASS", "UNKNOWN"]
 TaskExecutionStatusType = Literal[
     "ERROR", "LAUNCHING", "PREPARING", "QUEUED", "SUCCESS", "TRANSFERRING", "VERIFYING"
 ]
 TaskFilterNameType = Literal["CreationTime", "LocationId"]
 TaskQueueingType = Literal["DISABLED", "ENABLED"]
 TaskStatusType = Literal["AVAILABLE", "CREATING", "QUEUED", "RUNNING", "UNAVAILABLE"]
 TransferModeType = Literal["ALL", "CHANGED"]
@@ -134,14 +156,15 @@
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
@@ -181,14 +204,15 @@
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
@@ -267,14 +291,15 @@
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
@@ -285,14 +310,15 @@
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
@@ -328,14 +354,15 @@
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
@@ -354,16 +381,19 @@
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
@@ -447,15 +477,17 @@
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
@@ -474,27 +506,35 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_agents", "list_locations", "list_tags_for_resource", "list_task_executions", "list_tasks"
+    "describe_storage_system_resource_metrics",
+    "list_agents",
+    "list_discovery_jobs",
+    "list_locations",
+    "list_storage_systems",
+    "list_tags_for_resource",
+    "list_task_executions",
+    "list_tasks",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.pyi` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/literals.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -17,23 +17,30 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AgentStatusType",
     "AtimeType",
+    "DescribeStorageSystemResourceMetricsPaginatorName",
+    "DiscoveryJobStatusType",
+    "DiscoveryResourceFilterType",
+    "DiscoveryResourceTypeType",
+    "DiscoverySystemTypeType",
     "EfsInTransitEncryptionType",
     "EndpointTypeType",
     "FilterTypeType",
     "GidType",
     "HdfsAuthenticationTypeType",
     "HdfsDataTransferProtectionType",
     "HdfsRpcProtectionType",
     "ListAgentsPaginatorName",
+    "ListDiscoveryJobsPaginatorName",
     "ListLocationsPaginatorName",
+    "ListStorageSystemsPaginatorName",
     "ListTagsForResourcePaginatorName",
     "ListTaskExecutionsPaginatorName",
     "ListTasksPaginatorName",
     "LocationFilterNameType",
     "LogLevelType",
     "MtimeType",
     "NfsVersionType",
@@ -41,17 +48,19 @@
     "ObjectTagsType",
     "OperatorType",
     "OverwriteModeType",
     "PhaseStatusType",
     "PosixPermissionsType",
     "PreserveDeletedFilesType",
     "PreserveDevicesType",
+    "RecommendationStatusType",
     "S3StorageClassType",
     "SmbSecurityDescriptorCopyFlagsType",
     "SmbVersionType",
+    "StorageSystemConnectivityStatusType",
     "TaskExecutionStatusType",
     "TaskFilterNameType",
     "TaskQueueingType",
     "TaskStatusType",
     "TransferModeType",
     "UidType",
     "VerifyModeType",
@@ -60,23 +69,34 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AgentStatusType = Literal["OFFLINE", "ONLINE"]
 AtimeType = Literal["BEST_EFFORT", "NONE"]
+DescribeStorageSystemResourceMetricsPaginatorName = Literal[
+    "describe_storage_system_resource_metrics"
+]
+DiscoveryJobStatusType = Literal[
+    "COMPLETED", "COMPLETED_WITH_ISSUES", "FAILED", "RUNNING", "STOPPED", "TERMINATED", "WARNING"
+]
+DiscoveryResourceFilterType = Literal["SVM"]
+DiscoveryResourceTypeType = Literal["CLUSTER", "SVM", "VOLUME"]
+DiscoverySystemTypeType = Literal["NetAppONTAP"]
 EfsInTransitEncryptionType = Literal["NONE", "TLS1_2"]
 EndpointTypeType = Literal["FIPS", "PRIVATE_LINK", "PUBLIC"]
 FilterTypeType = Literal["SIMPLE_PATTERN"]
 GidType = Literal["BOTH", "INT_VALUE", "NAME", "NONE"]
 HdfsAuthenticationTypeType = Literal["KERBEROS", "SIMPLE"]
 HdfsDataTransferProtectionType = Literal["AUTHENTICATION", "DISABLED", "INTEGRITY", "PRIVACY"]
 HdfsRpcProtectionType = Literal["AUTHENTICATION", "DISABLED", "INTEGRITY", "PRIVACY"]
 ListAgentsPaginatorName = Literal["list_agents"]
+ListDiscoveryJobsPaginatorName = Literal["list_discovery_jobs"]
 ListLocationsPaginatorName = Literal["list_locations"]
+ListStorageSystemsPaginatorName = Literal["list_storage_systems"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 ListTaskExecutionsPaginatorName = Literal["list_task_executions"]
 ListTasksPaginatorName = Literal["list_tasks"]
 LocationFilterNameType = Literal["CreationTime", "LocationType", "LocationUri"]
 LogLevelType = Literal["BASIC", "OFF", "TRANSFER"]
 MtimeType = Literal["NONE", "PRESERVE"]
 NfsVersionType = Literal["AUTOMATIC", "NFS3", "NFS4_0", "NFS4_1"]
@@ -95,26 +115,28 @@
     "NotEquals",
 ]
 OverwriteModeType = Literal["ALWAYS", "NEVER"]
 PhaseStatusType = Literal["ERROR", "PENDING", "SUCCESS"]
 PosixPermissionsType = Literal["NONE", "PRESERVE"]
 PreserveDeletedFilesType = Literal["PRESERVE", "REMOVE"]
 PreserveDevicesType = Literal["NONE", "PRESERVE"]
+RecommendationStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "NONE"]
 S3StorageClassType = Literal[
     "DEEP_ARCHIVE",
     "GLACIER",
     "GLACIER_INSTANT_RETRIEVAL",
     "INTELLIGENT_TIERING",
     "ONEZONE_IA",
     "OUTPOSTS",
     "STANDARD",
     "STANDARD_IA",
 ]
 SmbSecurityDescriptorCopyFlagsType = Literal["NONE", "OWNER_DACL", "OWNER_DACL_SACL"]
 SmbVersionType = Literal["AUTOMATIC", "SMB1", "SMB2", "SMB2_0", "SMB3"]
+StorageSystemConnectivityStatusType = Literal["FAIL", "PASS", "UNKNOWN"]
 TaskExecutionStatusType = Literal[
     "ERROR", "LAUNCHING", "PREPARING", "QUEUED", "SUCCESS", "TRANSFERRING", "VERIFYING"
 ]
 TaskFilterNameType = Literal["CreationTime", "LocationId"]
 TaskQueueingType = Literal["DISABLED", "ENABLED"]
 TaskStatusType = Literal["AVAILABLE", "CREATING", "QUEUED", "RUNNING", "UNAVAILABLE"]
 TransferModeType = Literal["ALL", "CHANGED"]
@@ -132,14 +154,15 @@
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
@@ -179,14 +202,15 @@
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
@@ -265,14 +289,15 @@
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
@@ -283,14 +308,15 @@
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
@@ -326,14 +352,15 @@
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
@@ -352,16 +379,19 @@
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
@@ -445,15 +475,17 @@
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
@@ -472,27 +504,35 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_agents", "list_locations", "list_tags_for_resource", "list_task_executions", "list_tasks"
+    "describe_storage_system_resource_metrics",
+    "list_agents",
+    "list_discovery_jobs",
+    "list_locations",
+    "list_storage_systems",
+    "list_tags_for_resource",
+    "list_task_executions",
+    "list_tasks",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.py` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Type annotations for datasync service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_datasync.type_defs import AgentListEntryTypeDef
+    from mypy_boto3_datasync.type_defs import CredentialsTypeDef
 
-    data: AgentListEntryTypeDef = {...}
+    data: CredentialsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AgentStatusType,
     AtimeType,
+    DiscoveryJobStatusType,
+    DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     EndpointTypeType,
     GidType,
     HdfsAuthenticationTypeType,
     HdfsDataTransferProtectionType,
     HdfsRpcProtectionType,
     LocationFilterNameType,
@@ -34,17 +36,19 @@
     ObjectTagsType,
     OperatorType,
     OverwriteModeType,
     PhaseStatusType,
     PosixPermissionsType,
     PreserveDeletedFilesType,
     PreserveDevicesType,
+    RecommendationStatusType,
     S3StorageClassType,
     SmbSecurityDescriptorCopyFlagsType,
     SmbVersionType,
+    StorageSystemConnectivityStatusType,
     TaskExecutionStatusType,
     TaskFilterNameType,
     TaskQueueingType,
     TaskStatusType,
     TransferModeType,
     UidType,
     VerifyModeType,
@@ -57,81 +61,114 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "CredentialsTypeDef",
+    "DiscoveryServerConfigurationTypeDef",
+    "TagListEntryTypeDef",
+    "AddStorageSystemResponseTypeDef",
     "AgentListEntryTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
-    "TagListEntryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CapacityTypeDef",
+    "CreateAgentResponseTypeDef",
     "Ec2ConfigTypeDef",
+    "CreateLocationEfsResponseTypeDef",
+    "CreateLocationFsxLustreResponseTypeDef",
+    "CreateLocationFsxOntapResponseTypeDef",
+    "CreateLocationFsxOpenZfsResponseTypeDef",
+    "CreateLocationFsxWindowsResponseTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
+    "CreateLocationHdfsResponseTypeDef",
     "NfsMountOptionsTypeDef",
     "OnPremConfigTypeDef",
+    "CreateLocationNfsResponseTypeDef",
+    "CreateLocationObjectStorageResponseTypeDef",
     "S3ConfigTypeDef",
+    "CreateLocationS3ResponseTypeDef",
     "SmbMountOptionsTypeDef",
+    "CreateLocationSmbResponseTypeDef",
     "FilterRuleTypeDef",
     "OptionsTypeDef",
     "TaskScheduleTypeDef",
+    "CreateTaskResponseTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
+    "DescribeDiscoveryJobRequestRequestTypeDef",
+    "DescribeDiscoveryJobResponseTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
+    "DescribeLocationFsxLustreResponseTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
+    "DescribeLocationFsxWindowsResponseTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
+    "DescribeLocationObjectStorageResponseTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
+    "DescribeStorageSystemRequestRequestTypeDef",
+    "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
+    "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
+    "DescribeStorageSystemResourcesRequestRequestTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
     "TaskExecutionResultDetailTypeDef",
     "DescribeTaskRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DiscoveryJobListEntryTypeDef",
+    "GenerateRecommendationsRequestRequestTypeDef",
+    "IOPSTypeDef",
+    "LatencyTypeDef",
+    "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListAgentsRequestRequestTypeDef",
+    "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
+    "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
     "LocationListEntryTypeDef",
+    "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
+    "ListStorageSystemsRequestRequestTypeDef",
+    "StorageSystemListEntryTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "ListTaskExecutionsRequestRequestTypeDef",
     "TaskExecutionListEntryTypeDef",
     "TaskFilterTypeDef",
     "TaskListEntryTypeDef",
+    "MaxP95PerformanceTypeDef",
+    "RecommendationTypeDef",
+    "ThroughputTypeDef",
+    "PaginatorConfigTypeDef",
+    "RemoveStorageSystemRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDiscoveryJobResponseTypeDef",
+    "StartTaskExecutionResponseTypeDef",
+    "StopDiscoveryJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentRequestRequestTypeDef",
+    "UpdateDiscoveryJobRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
+    "DescribeStorageSystemResponseTypeDef",
+    "UpdateStorageSystemRequestRequestTypeDef",
+    "AddStorageSystemRequestRequestTypeDef",
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateAgentResponseTypeDef",
-    "CreateLocationEfsResponseTypeDef",
-    "CreateLocationFsxLustreResponseTypeDef",
-    "CreateLocationFsxOntapResponseTypeDef",
-    "CreateLocationFsxOpenZfsResponseTypeDef",
-    "CreateLocationFsxWindowsResponseTypeDef",
-    "CreateLocationHdfsResponseTypeDef",
-    "CreateLocationNfsResponseTypeDef",
-    "CreateLocationObjectStorageResponseTypeDef",
-    "CreateLocationS3ResponseTypeDef",
-    "CreateLocationSmbResponseTypeDef",
-    "CreateTaskResponseTypeDef",
-    "DescribeLocationFsxLustreResponseTypeDef",
-    "DescribeLocationFsxWindowsResponseTypeDef",
-    "DescribeLocationObjectStorageResponseTypeDef",
     "ListAgentsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartTaskExecutionResponseTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
     "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
@@ -146,48 +183,67 @@
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
     "DescribeTaskResponseTypeDef",
     "UpdateTaskRequestRequestTypeDef",
     "DescribeAgentResponseTypeDef",
     "DescribeTaskExecutionResponseTypeDef",
-    "ListAgentsRequestListAgentsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
+    "ListDiscoveryJobsResponseTypeDef",
     "ListLocationsRequestListLocationsPaginateTypeDef",
     "ListLocationsRequestRequestTypeDef",
     "ListLocationsResponseTypeDef",
+    "ListStorageSystemsResponseTypeDef",
     "ListTaskExecutionsResponseTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ListTasksResponseTypeDef",
+    "NetAppONTAPClusterTypeDef",
+    "NetAppONTAPSVMTypeDef",
+    "NetAppONTAPVolumeTypeDef",
+    "P95MetricsTypeDef",
     "FsxProtocolTypeDef",
+    "ResourceDetailsTypeDef",
+    "ResourceMetricsTypeDef",
     "CreateLocationFsxOntapRequestRequestTypeDef",
     "CreateLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxOntapResponseTypeDef",
     "DescribeLocationFsxOpenZfsResponseTypeDef",
+    "DescribeStorageSystemResourcesResponseTypeDef",
+    "DescribeStorageSystemResourceMetricsResponseTypeDef",
 )
 
-AgentListEntryTypeDef = TypedDict(
-    "AgentListEntryTypeDef",
+CredentialsTypeDef = TypedDict(
+    "CredentialsTypeDef",
     {
-        "AgentArn": str,
-        "Name": str,
-        "Status": AgentStatusType,
+        "Username": str,
+        "Password": str,
     },
-    total=False,
 )
 
-CancelTaskExecutionRequestRequestTypeDef = TypedDict(
-    "CancelTaskExecutionRequestRequestTypeDef",
+_RequiredDiscoveryServerConfigurationTypeDef = TypedDict(
+    "_RequiredDiscoveryServerConfigurationTypeDef",
     {
-        "TaskExecutionArn": str,
+        "ServerHostname": str,
+    },
+)
+_OptionalDiscoveryServerConfigurationTypeDef = TypedDict(
+    "_OptionalDiscoveryServerConfigurationTypeDef",
+    {
+        "ServerPort": int,
     },
+    total=False,
 )
 
+
+class DiscoveryServerConfigurationTypeDef(
+    _RequiredDiscoveryServerConfigurationTypeDef, _OptionalDiscoveryServerConfigurationTypeDef
+):
+    pass
+
+
 _RequiredTagListEntryTypeDef = TypedDict(
     "_RequiredTagListEntryTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagListEntryTypeDef = TypedDict(
@@ -199,33 +255,105 @@
 )
 
 
 class TagListEntryTypeDef(_RequiredTagListEntryTypeDef, _OptionalTagListEntryTypeDef):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddStorageSystemResponseTypeDef = TypedDict(
+    "AddStorageSystemResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "StorageSystemArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AgentListEntryTypeDef = TypedDict(
+    "AgentListEntryTypeDef",
+    {
+        "AgentArn": str,
+        "Name": str,
+        "Status": AgentStatusType,
+    },
+    total=False,
+)
+
+CancelTaskExecutionRequestRequestTypeDef = TypedDict(
+    "CancelTaskExecutionRequestRequestTypeDef",
+    {
+        "TaskExecutionArn": str,
+    },
+)
+
+CapacityTypeDef = TypedDict(
+    "CapacityTypeDef",
+    {
+        "Used": int,
+        "Provisioned": int,
+        "LogicalUsed": int,
+    },
+    total=False,
+)
+
+CreateAgentResponseTypeDef = TypedDict(
+    "CreateAgentResponseTypeDef",
+    {
+        "AgentArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2ConfigTypeDef = TypedDict(
     "Ec2ConfigTypeDef",
     {
         "SubnetArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
 
+CreateLocationEfsResponseTypeDef = TypedDict(
+    "CreateLocationEfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLocationFsxLustreResponseTypeDef = TypedDict(
+    "CreateLocationFsxLustreResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLocationFsxOntapResponseTypeDef = TypedDict(
+    "CreateLocationFsxOntapResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLocationFsxOpenZfsResponseTypeDef = TypedDict(
+    "CreateLocationFsxOpenZfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLocationFsxWindowsResponseTypeDef = TypedDict(
+    "CreateLocationFsxWindowsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HdfsNameNodeTypeDef = TypedDict(
     "HdfsNameNodeTypeDef",
     {
         "Hostname": str,
         "Port": int,
     },
 )
@@ -235,14 +363,22 @@
     {
         "RpcProtection": HdfsRpcProtectionType,
         "DataTransferProtection": HdfsDataTransferProtectionType,
     },
     total=False,
 )
 
+CreateLocationHdfsResponseTypeDef = TypedDict(
+    "CreateLocationHdfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NfsMountOptionsTypeDef = TypedDict(
     "NfsMountOptionsTypeDef",
     {
         "Version": NfsVersionType,
     },
     total=False,
 )
@@ -250,29 +386,61 @@
 OnPremConfigTypeDef = TypedDict(
     "OnPremConfigTypeDef",
     {
         "AgentArns": Sequence[str],
     },
 )
 
+CreateLocationNfsResponseTypeDef = TypedDict(
+    "CreateLocationNfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLocationObjectStorageResponseTypeDef = TypedDict(
+    "CreateLocationObjectStorageResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketAccessRoleArn": str,
     },
 )
 
+CreateLocationS3ResponseTypeDef = TypedDict(
+    "CreateLocationS3ResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SmbMountOptionsTypeDef = TypedDict(
     "SmbMountOptionsTypeDef",
     {
         "Version": SmbVersionType,
     },
     total=False,
 )
 
+CreateLocationSmbResponseTypeDef = TypedDict(
+    "CreateLocationSmbResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FilterRuleTypeDef = TypedDict(
     "FilterRuleTypeDef",
     {
         "FilterType": Literal["SIMPLE_PATTERN"],
         "Value": str,
     },
     total=False,
@@ -303,14 +471,22 @@
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
+CreateTaskResponseTypeDef = TypedDict(
+    "CreateTaskResponseTypeDef",
+    {
+        "TaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAgentRequestRequestTypeDef = TypedDict(
     "DeleteAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
 )
 
@@ -342,28 +518,59 @@
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
     total=False,
 )
 
+DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
+    "DescribeDiscoveryJobRequestRequestTypeDef",
+    {
+        "DiscoveryJobArn": str,
+    },
+)
+
+DescribeDiscoveryJobResponseTypeDef = TypedDict(
+    "DescribeDiscoveryJobResponseTypeDef",
+    {
+        "StorageSystemArn": str,
+        "DiscoveryJobArn": str,
+        "CollectionDurationMinutes": int,
+        "Status": DiscoveryJobStatusType,
+        "JobStartTime": datetime,
+        "JobEndTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+DescribeLocationFsxLustreResponseTypeDef = TypedDict(
+    "DescribeLocationFsxLustreResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "SecurityGroupArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -377,14 +584,27 @@
 DescribeLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+DescribeLocationFsxWindowsResponseTypeDef = TypedDict(
+    "DescribeLocationFsxWindowsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "SecurityGroupArns": List[str],
+        "CreationTime": datetime,
+        "User": str,
+        "Domain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLocationHdfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationHdfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -398,28 +618,129 @@
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+DescribeLocationObjectStorageResponseTypeDef = TypedDict(
+    "DescribeLocationObjectStorageResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "AccessKey": str,
+        "ServerPort": int,
+        "ServerProtocol": ObjectStorageServerProtocolType,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ServerCertificate": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLocationS3RequestRequestTypeDef = TypedDict(
     "DescribeLocationS3RequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
 DescribeLocationSmbRequestRequestTypeDef = TypedDict(
     "DescribeLocationSmbRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+DescribeStorageSystemRequestRequestTypeDef = TypedDict(
+    "DescribeStorageSystemRequestRequestTypeDef",
+    {
+        "StorageSystemArn": str,
+    },
+)
+
+_RequiredDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
+    {
+        "DiscoveryJobArn": str,
+        "ResourceType": DiscoveryResourceTypeType,
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef(
+    _RequiredDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
+    _OptionalDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef",
+    {
+        "DiscoveryJobArn": str,
+        "ResourceType": DiscoveryResourceTypeType,
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeStorageSystemResourceMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeStorageSystemResourceMetricsRequestRequestTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeStorageSystemResourceMetricsRequestRequestTypeDef(
+    _RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef,
+    _OptionalDescribeStorageSystemResourceMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeStorageSystemResourcesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeStorageSystemResourcesRequestRequestTypeDef",
+    {
+        "DiscoveryJobArn": str,
+        "ResourceType": DiscoveryResourceTypeType,
+    },
+)
+_OptionalDescribeStorageSystemResourcesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeStorageSystemResourcesRequestRequestTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "Filter": Mapping[Literal["SVM"], Sequence[str]],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeStorageSystemResourcesRequestRequestTypeDef(
+    _RequiredDescribeStorageSystemResourcesRequestRequestTypeDef,
+    _OptionalDescribeStorageSystemResourcesRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeTaskExecutionRequestRequestTypeDef = TypedDict(
     "DescribeTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
@@ -442,33 +763,89 @@
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DiscoveryJobListEntryTypeDef = TypedDict(
+    "DiscoveryJobListEntryTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DiscoveryJobArn": str,
+        "Status": DiscoveryJobStatusType,
+    },
+    total=False,
+)
+
+GenerateRecommendationsRequestRequestTypeDef = TypedDict(
+    "GenerateRecommendationsRequestRequestTypeDef",
+    {
+        "DiscoveryJobArn": str,
+        "ResourceIds": Sequence[str],
+        "ResourceType": DiscoveryResourceTypeType,
+    },
+)
+
+IOPSTypeDef = TypedDict(
+    "IOPSTypeDef",
+    {
+        "Read": float,
+        "Write": float,
+        "Other": float,
+        "Total": float,
+    },
+    total=False,
+)
+
+LatencyTypeDef = TypedDict(
+    "LatencyTypeDef",
+    {
+        "Read": float,
+        "Write": float,
+        "Other": float,
+    },
+    total=False,
+)
+
+ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
+    "ListAgentsRequestListAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAgentsRequestRequestTypeDef = TypedDict(
     "ListAgentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef = TypedDict(
+    "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
+    {
+        "StorageSystemArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListDiscoveryJobsRequestRequestTypeDef = TypedDict(
+    "ListDiscoveryJobsRequestRequestTypeDef",
+    {
+        "StorageSystemArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 LocationFilterTypeDef = TypedDict(
     "LocationFilterTypeDef",
     {
         "Name": LocationFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
@@ -479,14 +856,62 @@
     {
         "LocationArn": str,
         "LocationUri": str,
     },
     total=False,
 )
 
+ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
+    "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListStorageSystemsRequestRequestTypeDef = TypedDict(
+    "ListStorageSystemsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+StorageSystemListEntryTypeDef = TypedDict(
+    "StorageSystemListEntryTypeDef",
+    {
+        "StorageSystemArn": str,
+        "Name": str,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -502,14 +927,23 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef = TypedDict(
+    "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
+    {
+        "TaskArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTaskExecutionsRequestRequestTypeDef = TypedDict(
     "ListTaskExecutionsRequestRequestTypeDef",
     {
         "TaskArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -540,14 +974,104 @@
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
     total=False,
 )
 
+MaxP95PerformanceTypeDef = TypedDict(
+    "MaxP95PerformanceTypeDef",
+    {
+        "IopsRead": float,
+        "IopsWrite": float,
+        "IopsOther": float,
+        "IopsTotal": float,
+        "ThroughputRead": float,
+        "ThroughputWrite": float,
+        "ThroughputOther": float,
+        "ThroughputTotal": float,
+        "LatencyRead": float,
+        "LatencyWrite": float,
+        "LatencyOther": float,
+    },
+    total=False,
+)
+
+RecommendationTypeDef = TypedDict(
+    "RecommendationTypeDef",
+    {
+        "StorageType": str,
+        "StorageConfiguration": Dict[str, str],
+        "EstimatedMonthlyStorageCost": str,
+    },
+    total=False,
+)
+
+ThroughputTypeDef = TypedDict(
+    "ThroughputTypeDef",
+    {
+        "Read": float,
+        "Write": float,
+        "Other": float,
+        "Total": float,
+    },
+    total=False,
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
+RemoveStorageSystemRequestRequestTypeDef = TypedDict(
+    "RemoveStorageSystemRequestRequestTypeDef",
+    {
+        "StorageSystemArn": str,
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
+StartDiscoveryJobResponseTypeDef = TypedDict(
+    "StartDiscoveryJobResponseTypeDef",
+    {
+        "DiscoveryJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartTaskExecutionResponseTypeDef = TypedDict(
+    "StartTaskExecutionResponseTypeDef",
+    {
+        "TaskExecutionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StopDiscoveryJobRequestRequestTypeDef = TypedDict(
+    "StopDiscoveryJobRequestRequestTypeDef",
+    {
+        "DiscoveryJobArn": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Keys": Sequence[str],
     },
 )
@@ -569,14 +1093,22 @@
 
 class UpdateAgentRequestRequestTypeDef(
     _RequiredUpdateAgentRequestRequestTypeDef, _OptionalUpdateAgentRequestRequestTypeDef
 ):
     pass
 
 
+UpdateDiscoveryJobRequestRequestTypeDef = TypedDict(
+    "UpdateDiscoveryJobRequestRequestTypeDef",
+    {
+        "DiscoveryJobArn": str,
+        "CollectionDurationMinutes": int,
+    },
+)
+
 _RequiredUpdateLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationObjectStorageRequestRequestTypeDef = TypedDict(
@@ -597,14 +1129,84 @@
 class UpdateLocationObjectStorageRequestRequestTypeDef(
     _RequiredUpdateLocationObjectStorageRequestRequestTypeDef,
     _OptionalUpdateLocationObjectStorageRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeStorageSystemResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResponseTypeDef",
+    {
+        "StorageSystemArn": str,
+        "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
+        "SystemType": Literal["NetAppONTAP"],
+        "AgentArns": List[str],
+        "Name": str,
+        "ErrorMessage": str,
+        "ConnectivityStatus": StorageSystemConnectivityStatusType,
+        "CloudWatchLogGroupArn": str,
+        "CreationTime": datetime,
+        "SecretsManagerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateStorageSystemRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStorageSystemRequestRequestTypeDef",
+    {
+        "StorageSystemArn": str,
+    },
+)
+_OptionalUpdateStorageSystemRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStorageSystemRequestRequestTypeDef",
+    {
+        "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
+        "AgentArns": Sequence[str],
+        "Name": str,
+        "CloudWatchLogGroupArn": str,
+        "Credentials": CredentialsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateStorageSystemRequestRequestTypeDef(
+    _RequiredUpdateStorageSystemRequestRequestTypeDef,
+    _OptionalUpdateStorageSystemRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredAddStorageSystemRequestRequestTypeDef = TypedDict(
+    "_RequiredAddStorageSystemRequestRequestTypeDef",
+    {
+        "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
+        "SystemType": Literal["NetAppONTAP"],
+        "AgentArns": Sequence[str],
+        "ClientToken": str,
+        "Credentials": CredentialsTypeDef,
+    },
+)
+_OptionalAddStorageSystemRequestRequestTypeDef = TypedDict(
+    "_OptionalAddStorageSystemRequestRequestTypeDef",
+    {
+        "CloudWatchLogGroupArn": str,
+        "Tags": Sequence[TagListEntryTypeDef],
+        "Name": str,
+    },
+    total=False,
+)
+
+
+class AddStorageSystemRequestRequestTypeDef(
+    _RequiredAddStorageSystemRequestRequestTypeDef, _OptionalAddStorageSystemRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAgentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAgentRequestRequestTypeDef",
     {
         "ActivationKey": str,
     },
 )
 _OptionalCreateAgentRequestRequestTypeDef = TypedDict(
@@ -703,180 +1305,60 @@
 class CreateLocationObjectStorageRequestRequestTypeDef(
     _RequiredCreateLocationObjectStorageRequestRequestTypeDef,
     _OptionalCreateLocationObjectStorageRequestRequestTypeDef,
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagListEntryTypeDef],
-    },
-)
-
-CreateAgentResponseTypeDef = TypedDict(
-    "CreateAgentResponseTypeDef",
-    {
-        "AgentArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationEfsResponseTypeDef = TypedDict(
-    "CreateLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationFsxLustreResponseTypeDef = TypedDict(
-    "CreateLocationFsxLustreResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationFsxOntapResponseTypeDef = TypedDict(
-    "CreateLocationFsxOntapResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationFsxOpenZfsResponseTypeDef = TypedDict(
-    "CreateLocationFsxOpenZfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationFsxWindowsResponseTypeDef = TypedDict(
-    "CreateLocationFsxWindowsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationHdfsResponseTypeDef = TypedDict(
-    "CreateLocationHdfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationNfsResponseTypeDef = TypedDict(
-    "CreateLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLocationObjectStorageResponseTypeDef = TypedDict(
-    "CreateLocationObjectStorageResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationS3ResponseTypeDef = TypedDict(
-    "CreateLocationS3ResponseTypeDef",
+_RequiredStartDiscoveryJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDiscoveryJobRequestRequestTypeDef",
     {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StorageSystemArn": str,
+        "CollectionDurationMinutes": int,
+        "ClientToken": str,
     },
 )
-
-CreateLocationSmbResponseTypeDef = TypedDict(
-    "CreateLocationSmbResponseTypeDef",
+_OptionalStartDiscoveryJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDiscoveryJobRequestRequestTypeDef",
     {
-        "LocationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Sequence[TagListEntryTypeDef],
     },
+    total=False,
 )
 
-CreateTaskResponseTypeDef = TypedDict(
-    "CreateTaskResponseTypeDef",
-    {
-        "TaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-DescribeLocationFsxLustreResponseTypeDef = TypedDict(
-    "DescribeLocationFsxLustreResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "SecurityGroupArns": List[str],
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class StartDiscoveryJobRequestRequestTypeDef(
+    _RequiredStartDiscoveryJobRequestRequestTypeDef, _OptionalStartDiscoveryJobRequestRequestTypeDef
+):
+    pass
 
-DescribeLocationFsxWindowsResponseTypeDef = TypedDict(
-    "DescribeLocationFsxWindowsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "SecurityGroupArns": List[str],
-        "CreationTime": datetime,
-        "User": str,
-        "Domain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-DescribeLocationObjectStorageResponseTypeDef = TypedDict(
-    "DescribeLocationObjectStorageResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "LocationArn": str,
-        "LocationUri": str,
-        "AccessKey": str,
-        "ServerPort": int,
-        "ServerProtocol": ObjectStorageServerProtocolType,
-        "AgentArns": List[str],
-        "CreationTime": datetime,
-        "ServerCertificate": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagListEntryTypeDef],
     },
 )
 
 ListAgentsResponseTypeDef = TypedDict(
     "ListAgentsResponseTypeDef",
     {
         "Agents": List[AgentListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTaskExecutionResponseTypeDef = TypedDict(
-    "StartTaskExecutionResponseTypeDef",
-    {
-        "TaskExecutionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationEfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationEfsRequestRequestTypeDef",
     {
         "EfsFilesystemArn": str,
@@ -908,15 +1390,15 @@
         "LocationArn": str,
         "LocationUri": str,
         "Ec2Config": Ec2ConfigTypeDef,
         "CreationTime": datetime,
         "AccessPointArn": str,
         "FileSystemAccessRoleArn": str,
         "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
@@ -960,15 +1442,15 @@
         "KmsKeyProviderUri": str,
         "QopConfiguration": QopConfigurationTypeDef,
         "AuthenticationType": HdfsAuthenticationTypeType,
         "SimpleUser": str,
         "KerberosPrincipal": str,
         "AgentArns": List[str],
         "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationHdfsRequestRequestTypeDef",
     {
         "LocationArn": str,
@@ -1037,15 +1519,15 @@
     "DescribeLocationNfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "OnPremConfig": OnPremConfigTypeDef,
         "MountOptions": NfsMountOptionsTypeDef,
         "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
@@ -1098,15 +1580,15 @@
     {
         "LocationArn": str,
         "LocationUri": str,
         "S3StorageClass": S3StorageClassType,
         "S3Config": S3ConfigTypeDef,
         "AgentArns": List[str],
         "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationSmbRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationSmbRequestRequestTypeDef",
     {
         "Subdirectory": str,
@@ -1139,15 +1621,15 @@
         "LocationArn": str,
         "LocationUri": str,
         "AgentArns": List[str],
         "User": str,
         "Domain": str,
         "MountOptions": SmbMountOptionsTypeDef,
         "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFsxProtocolSmbTypeDef = TypedDict(
     "_RequiredFsxProtocolSmbTypeDef",
     {
         "Password": str,
@@ -1270,15 +1752,15 @@
         "Options": OptionsTypeDef,
         "Excludes": List[FilterRuleTypeDef],
         "Schedule": TaskScheduleTypeDef,
         "ErrorCode": str,
         "ErrorDetail": str,
         "CreationTime": datetime,
         "Includes": List[FilterRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
@@ -1310,15 +1792,15 @@
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
         "LastConnectionTime": datetime,
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
         "PrivateLinkConfig": PrivateLinkConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTaskExecutionResponseTypeDef = TypedDict(
     "DescribeTaskExecutionResponseTypeDef",
     {
         "TaskExecutionArn": str,
@@ -1330,62 +1812,32 @@
         "EstimatedFilesToTransfer": int,
         "EstimatedBytesToTransfer": int,
         "FilesTransferred": int,
         "BytesWritten": int,
         "BytesTransferred": int,
         "Result": TaskExecutionResultDetailTypeDef,
         "BytesCompressed": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
-    "ListAgentsRequestListAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
-ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef = TypedDict(
-    "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
+ListDiscoveryJobsResponseTypeDef = TypedDict(
+    "ListDiscoveryJobsResponseTypeDef",
     {
-        "TaskArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
     {
         "Filters": Sequence[LocationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListLocationsRequestRequestTypeDef = TypedDict(
     "ListLocationsRequestRequestTypeDef",
     {
@@ -1397,32 +1849,41 @@
 )
 
 ListLocationsResponseTypeDef = TypedDict(
     "ListLocationsResponseTypeDef",
     {
         "Locations": List[LocationListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStorageSystemsResponseTypeDef = TypedDict(
+    "ListStorageSystemsResponseTypeDef",
+    {
+        "StorageSystems": List[StorageSystemListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTaskExecutionsResponseTypeDef = TypedDict(
     "ListTaskExecutionsResponseTypeDef",
     {
         "TaskExecutions": List[TaskExecutionListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
     {
         "Filters": Sequence[TaskFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
@@ -1434,27 +1895,117 @@
 )
 
 ListTasksResponseTypeDef = TypedDict(
     "ListTasksResponseTypeDef",
     {
         "Tasks": List[TaskListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+NetAppONTAPClusterTypeDef = TypedDict(
+    "NetAppONTAPClusterTypeDef",
+    {
+        "CifsShareCount": int,
+        "NfsExportedVolumes": int,
+        "ResourceId": str,
+        "ClusterName": str,
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "ClusterBlockStorageSize": int,
+        "ClusterBlockStorageUsed": int,
+        "ClusterBlockStorageLogicalUsed": int,
+        "Recommendations": List[RecommendationTypeDef],
+        "RecommendationStatus": RecommendationStatusType,
     },
+    total=False,
+)
+
+NetAppONTAPSVMTypeDef = TypedDict(
+    "NetAppONTAPSVMTypeDef",
+    {
+        "ClusterUuid": str,
+        "ResourceId": str,
+        "SvmName": str,
+        "CifsShareCount": int,
+        "EnabledProtocols": List[str],
+        "TotalCapacityUsed": int,
+        "TotalCapacityProvisioned": int,
+        "TotalLogicalCapacityUsed": int,
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "Recommendations": List[RecommendationTypeDef],
+        "NfsExportedVolumes": int,
+        "RecommendationStatus": RecommendationStatusType,
+        "TotalSnapshotCapacityUsed": int,
+    },
+    total=False,
+)
+
+NetAppONTAPVolumeTypeDef = TypedDict(
+    "NetAppONTAPVolumeTypeDef",
+    {
+        "VolumeName": str,
+        "ResourceId": str,
+        "CifsShareCount": int,
+        "SecurityStyle": str,
+        "SvmUuid": str,
+        "SvmName": str,
+        "CapacityUsed": int,
+        "CapacityProvisioned": int,
+        "LogicalCapacityUsed": int,
+        "NfsExported": bool,
+        "SnapshotCapacityUsed": int,
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "Recommendations": List[RecommendationTypeDef],
+        "RecommendationStatus": RecommendationStatusType,
+    },
+    total=False,
+)
+
+P95MetricsTypeDef = TypedDict(
+    "P95MetricsTypeDef",
+    {
+        "IOPS": IOPSTypeDef,
+        "Throughput": ThroughputTypeDef,
+        "Latency": LatencyTypeDef,
+    },
+    total=False,
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
         "SMB": FsxProtocolSmbTypeDef,
     },
     total=False,
 )
 
+ResourceDetailsTypeDef = TypedDict(
+    "ResourceDetailsTypeDef",
+    {
+        "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
+        "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
+        "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
+    },
+    total=False,
+)
+
+ResourceMetricsTypeDef = TypedDict(
+    "ResourceMetricsTypeDef",
+    {
+        "Timestamp": datetime,
+        "P95Metrics": P95MetricsTypeDef,
+        "Capacity": CapacityTypeDef,
+        "ResourceId": str,
+        "ResourceType": DiscoveryResourceTypeType,
+    },
+    total=False,
+)
+
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
     {
         "Protocol": FsxProtocolTypeDef,
         "SecurityGroupArns": Sequence[str],
         "StorageVirtualMachineArn": str,
     },
@@ -1507,22 +2058,40 @@
         "CreationTime": datetime,
         "LocationArn": str,
         "LocationUri": str,
         "Protocol": FsxProtocolTypeDef,
         "SecurityGroupArns": List[str],
         "StorageVirtualMachineArn": str,
         "FsxFilesystemArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLocationFsxOpenZfsResponseTypeDef = TypedDict(
     "DescribeLocationFsxOpenZfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "Protocol": FsxProtocolTypeDef,
         "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResourcesResponseTypeDef",
+    {
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResourceMetricsResponseTypeDef",
+    {
+        "Metrics": List[ResourceMetricsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.26.77
-Summary: Type annotations for boto3.DataSync 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.DataSync 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-datasync"></a>
 
 # mypy-boto3-datasync
 
 [![PyPI - mypy-boto3-datasync](https://img.shields.io/pypi/v/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,27 +279,39 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_datasync import DataSyncClient
 from mypy_boto3_datasync.paginator import (
+    DescribeStorageSystemResourceMetricsPaginator,
     ListAgentsPaginator,
+    ListDiscoveryJobsPaginator,
     ListLocationsPaginator,
+    ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 
 client: DataSyncClient = Session().client("datasync")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+describe_storage_system_resource_metrics_paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator(
+    "describe_storage_system_resource_metrics"
+)
 list_agents_paginator: ListAgentsPaginator = client.get_paginator("list_agents")
+list_discovery_jobs_paginator: ListDiscoveryJobsPaginator = client.get_paginator(
+    "list_discovery_jobs"
+)
 list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
+list_storage_systems_paginator: ListStorageSystemsPaginator = client.get_paginator(
+    "list_storage_systems"
+)
 list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
     "list_tags_for_resource"
 )
 list_task_executions_paginator: ListTaskExecutionsPaginator = client.get_paginator(
     "list_task_executions"
 )
 list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
@@ -312,23 +324,30 @@
 `mypy_boto3_datasync.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_datasync.literals import (
     AgentStatusType,
     AtimeType,
+    DescribeStorageSystemResourceMetricsPaginatorName,
+    DiscoveryJobStatusType,
+    DiscoveryResourceFilterType,
+    DiscoveryResourceTypeType,
+    DiscoverySystemTypeType,
     EfsInTransitEncryptionType,
     EndpointTypeType,
     FilterTypeType,
     GidType,
     HdfsAuthenticationTypeType,
     HdfsDataTransferProtectionType,
     HdfsRpcProtectionType,
     ListAgentsPaginatorName,
+    ListDiscoveryJobsPaginatorName,
     ListLocationsPaginatorName,
+    ListStorageSystemsPaginatorName,
     ListTagsForResourcePaginatorName,
     ListTaskExecutionsPaginatorName,
     ListTasksPaginatorName,
     LocationFilterNameType,
     LogLevelType,
     MtimeType,
     NfsVersionType,
@@ -336,17 +355,19 @@
     ObjectTagsType,
     OperatorType,
     OverwriteModeType,
     PhaseStatusType,
     PosixPermissionsType,
     PreserveDeletedFilesType,
     PreserveDevicesType,
+    RecommendationStatusType,
     S3StorageClassType,
     SmbSecurityDescriptorCopyFlagsType,
     SmbVersionType,
+    StorageSystemConnectivityStatusType,
     TaskExecutionStatusType,
     TaskFilterNameType,
     TaskQueueingType,
     TaskStatusType,
     TransferModeType,
     UidType,
     VerifyModeType,
@@ -367,81 +388,114 @@
 ### Typed dictionaries
 
 `mypy_boto3_datasync.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
+    CredentialsTypeDef,
+    DiscoveryServerConfigurationTypeDef,
+    TagListEntryTypeDef,
+    AddStorageSystemResponseTypeDef,
     AgentListEntryTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    TagListEntryTypeDef,
-    ResponseMetadataTypeDef,
+    CapacityTypeDef,
+    CreateAgentResponseTypeDef,
     Ec2ConfigTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
+    CreateLocationHdfsResponseTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
     S3ConfigTypeDef,
+    CreateLocationS3ResponseTypeDef,
     SmbMountOptionsTypeDef,
+    CreateLocationSmbResponseTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
+    CreateTaskResponseTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
     PrivateLinkConfigTypeDef,
+    DescribeDiscoveryJobRequestRequestTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
+    DescribeStorageSystemRequestRequestTypeDef,
+    DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
+    DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
+    DescribeStorageSystemResourcesRequestRequestTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
     TaskExecutionResultDetailTypeDef,
     DescribeTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DiscoveryJobListEntryTypeDef,
+    GenerateRecommendationsRequestRequestTypeDef,
+    IOPSTypeDef,
+    LatencyTypeDef,
+    ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
+    ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
+    ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
     LocationListEntryTypeDef,
+    ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
+    ListStorageSystemsRequestRequestTypeDef,
+    StorageSystemListEntryTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
     TaskExecutionListEntryTypeDef,
     TaskFilterTypeDef,
     TaskListEntryTypeDef,
+    MaxP95PerformanceTypeDef,
+    RecommendationTypeDef,
+    ThroughputTypeDef,
+    PaginatorConfigTypeDef,
+    RemoveStorageSystemRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
+    StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
+    UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    UpdateStorageSystemRequestRequestTypeDef,
+    AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateAgentResponseTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
-    CreateLocationHdfsResponseTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
-    CreateLocationS3ResponseTypeDef,
-    CreateLocationSmbResponseTypeDef,
-    CreateTaskResponseTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
     ListAgentsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
     DescribeLocationEfsResponseTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
@@ -456,71 +510,78 @@
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
     DescribeTaskResponseTypeDef,
     UpdateTaskRequestRequestTypeDef,
     DescribeAgentResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
-    ListAgentsRequestListAgentsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
     ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
     ListTasksResponseTypeDef,
+    NetAppONTAPClusterTypeDef,
+    NetAppONTAPSVMTypeDef,
+    NetAppONTAPVolumeTypeDef,
+    P95MetricsTypeDef,
     FsxProtocolTypeDef,
+    ResourceDetailsTypeDef,
+    ResourceMetricsTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
 )
 
 
-def get_structure() -> AgentListEntryTypeDef:
+def get_structure() -> CredentialsTypeDef:
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

### Comparing `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy-boto3-datasync-1.27.0/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.77/setup.py` & `mypy-boto3-datasync-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-datasync.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.26.77",
+    version="1.27.0",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataSync 1.26.77 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.DataSync 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/",
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


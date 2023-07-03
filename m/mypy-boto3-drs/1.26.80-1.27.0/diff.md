# Comparing `tmp/mypy-boto3-drs-1.26.80.tar.gz` & `tmp/mypy-boto3-drs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
+gzip compressed data, was "mypy-boto3-drs-1.27.0.tar", last modified: Mon Jul  3 19:50:40 2023, max compression
```

## Comparing `mypy-boto3-drs-1.26.80.tar` & `mypy-boto3-drs-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.144039 mypy-boto3-drs-1.26.80/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-02-27 20:35:29.140040 mypy-boto3-drs-1.26.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.132040 mypy-boto3-drs-1.26.80/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30488 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-02-27 20:35:05.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44692 2023-02-27 20:35:05.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.140040 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.144039 mypy-boto3-drs-1.26.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.815148 mypy-boto3-drs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-07-03 19:50:40.807148 mypy-boto3-drs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.803148 mypy-boto3-drs-1.27.0/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39630 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-03 19:35:51.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56958 2023-07-03 19:35:53.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56911 2023-07-03 19:35:52.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.807148 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-07-03 19:50:40.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:40.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:40.000000 mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:40.815148 mypy-boto3-drs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:35:50.000000 mypy-boto3-drs-1.27.0/setup.py
```

### Comparing `mypy-boto3-drs-1.26.80/LICENSE` & `mypy-boto3-drs-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-drs-1.26.80/PKG-INFO` & `mypy-boto3-drs-1.27.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.26.80
-Summary: Type annotations for boto3.drs 1.26.80 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.drs 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-drs"></a>
 
 # mypy-boto3-drs
 
 [![PyPI - mypy-boto3-drs](https://img.shields.io/pypi/v/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,39 +280,47 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_drs import drsClient
 from mypy_boto3_drs.paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 
 client: drsClient = Session().client("drs")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator(
     "describe_job_log_items"
 )
 describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = (
+    client.get_paginator("describe_launch_configuration_templates")
+)
 describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator(
     "describe_recovery_instances"
 )
 describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator(
     "describe_recovery_snapshots"
 )
 describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator(
     "describe_replication_configuration_templates"
 )
+describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator(
+    "describe_source_networks"
+)
 describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator(
     "describe_source_servers"
 )
 list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = (
     client.get_paginator("list_extensible_source_servers")
 )
 list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator(
@@ -331,17 +339,19 @@
 from mypy_boto3_drs.literals import (
     DataReplicationErrorStringType,
     DataReplicationInitiationStepNameType,
     DataReplicationInitiationStepStatusType,
     DataReplicationStateType,
     DescribeJobLogItemsPaginatorName,
     DescribeJobsPaginatorName,
+    DescribeLaunchConfigurationTemplatesPaginatorName,
     DescribeRecoveryInstancesPaginatorName,
     DescribeRecoverySnapshotsPaginatorName,
     DescribeReplicationConfigurationTemplatesPaginatorName,
+    DescribeSourceNetworksPaginatorName,
     DescribeSourceServersPaginatorName,
     EC2InstanceStateType,
     ExtensionStatusType,
     FailbackLaunchTypeType,
     FailbackReplicationErrorType,
     FailbackStateType,
     InitiatedByType,
@@ -355,20 +365,22 @@
     ListExtensibleSourceServersPaginatorName,
     ListStagingAccountsPaginatorName,
     OriginEnvironmentType,
     PITPolicyRuleUnitsType,
     RecoveryInstanceDataReplicationInitiationStepNameType,
     RecoveryInstanceDataReplicationInitiationStepStatusType,
     RecoveryInstanceDataReplicationStateType,
+    RecoveryResultType,
     RecoverySnapshotsOrderType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
     ReplicationDirectionType,
+    ReplicationStatusType,
     TargetInstanceTypeRightSizingMethodType,
     drsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -384,117 +396,150 @@
 
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
+    AssociateSourceNetworkStackRequestRequestTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    LicensingTypeDef,
     PITPolicyRuleTypeDef,
+    CreateSourceNetworkRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
+    DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
+    EmptyResponseMetadataTypeDef,
+    SourceNetworkDataTypeDef,
+    ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
-    LicensingTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PaginatorConfigTypeDef,
+    ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
+    RecoveryLifeCycleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
+    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
+    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
+    StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
+    StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
-    JobLogEventDataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReverseReplicationResponseTypeDef,
+    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
+    DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
+    DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
-    JobTypeDef,
-    LaunchConfigurationTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
+    EventResourceDataTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
+    ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
+    SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
-    JobLogTypeDef,
+    StartSourceNetworkRecoveryRequestRequestTypeDef,
+    CreateLaunchConfigurationTemplateResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
+    UpdateLaunchConfigurationTemplateResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DataReplicationInfoTypeDef,
-    DescribeJobsResponseTypeDef,
-    StartFailbackLaunchResponseTypeDef,
-    StartRecoveryResponseTypeDef,
-    TerminateRecoveryInstancesResponseTypeDef,
+    JobLogEventDataTypeDef,
     LifeCycleTypeDef,
+    JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
-    DescribeJobLogItemsResponseTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
+    StartSourceNetworkReplicationResponseTypeDef,
+    StopSourceNetworkReplicationResponseTypeDef,
+    JobLogTypeDef,
     SourceServerResponseMetadataTypeDef,
     SourceServerTypeDef,
+    AssociateSourceNetworkStackResponseTypeDef,
+    DescribeJobsResponseTypeDef,
+    StartFailbackLaunchResponseTypeDef,
+    StartRecoveryResponseTypeDef,
+    StartSourceNetworkRecoveryResponseTypeDef,
+    TerminateRecoveryInstancesResponseTypeDef,
     RecoveryInstanceTypeDef,
+    DescribeJobLogItemsResponseTypeDef,
     CreateExtendedSourceServerResponseTypeDef,
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
@@ -506,42 +551,42 @@
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

### Comparing `mypy-boto3-drs-1.26.80/README.md` & `mypy-boto3-drs-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-drs"></a>
 
 # mypy-boto3-drs
 
 [![PyPI - mypy-boto3-drs](https://img.shields.io/pypi/v/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -248,39 +248,47 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_drs import drsClient
 from mypy_boto3_drs.paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 
 client: drsClient = Session().client("drs")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator(
     "describe_job_log_items"
 )
 describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = (
+    client.get_paginator("describe_launch_configuration_templates")
+)
 describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator(
     "describe_recovery_instances"
 )
 describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator(
     "describe_recovery_snapshots"
 )
 describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator(
     "describe_replication_configuration_templates"
 )
+describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator(
+    "describe_source_networks"
+)
 describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator(
     "describe_source_servers"
 )
 list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = (
     client.get_paginator("list_extensible_source_servers")
 )
 list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator(
@@ -299,17 +307,19 @@
 from mypy_boto3_drs.literals import (
     DataReplicationErrorStringType,
     DataReplicationInitiationStepNameType,
     DataReplicationInitiationStepStatusType,
     DataReplicationStateType,
     DescribeJobLogItemsPaginatorName,
     DescribeJobsPaginatorName,
+    DescribeLaunchConfigurationTemplatesPaginatorName,
     DescribeRecoveryInstancesPaginatorName,
     DescribeRecoverySnapshotsPaginatorName,
     DescribeReplicationConfigurationTemplatesPaginatorName,
+    DescribeSourceNetworksPaginatorName,
     DescribeSourceServersPaginatorName,
     EC2InstanceStateType,
     ExtensionStatusType,
     FailbackLaunchTypeType,
     FailbackReplicationErrorType,
     FailbackStateType,
     InitiatedByType,
@@ -323,20 +333,22 @@
     ListExtensibleSourceServersPaginatorName,
     ListStagingAccountsPaginatorName,
     OriginEnvironmentType,
     PITPolicyRuleUnitsType,
     RecoveryInstanceDataReplicationInitiationStepNameType,
     RecoveryInstanceDataReplicationInitiationStepStatusType,
     RecoveryInstanceDataReplicationStateType,
+    RecoveryResultType,
     RecoverySnapshotsOrderType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
     ReplicationDirectionType,
+    ReplicationStatusType,
     TargetInstanceTypeRightSizingMethodType,
     drsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -352,117 +364,150 @@
 
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
+    AssociateSourceNetworkStackRequestRequestTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    LicensingTypeDef,
     PITPolicyRuleTypeDef,
+    CreateSourceNetworkRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
+    DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
+    EmptyResponseMetadataTypeDef,
+    SourceNetworkDataTypeDef,
+    ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
-    LicensingTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PaginatorConfigTypeDef,
+    ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
+    RecoveryLifeCycleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
+    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
+    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
+    StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
+    StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
-    JobLogEventDataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReverseReplicationResponseTypeDef,
+    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
+    DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
+    DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
-    JobTypeDef,
-    LaunchConfigurationTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
+    EventResourceDataTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
+    ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
+    SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
-    JobLogTypeDef,
+    StartSourceNetworkRecoveryRequestRequestTypeDef,
+    CreateLaunchConfigurationTemplateResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
+    UpdateLaunchConfigurationTemplateResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DataReplicationInfoTypeDef,
-    DescribeJobsResponseTypeDef,
-    StartFailbackLaunchResponseTypeDef,
-    StartRecoveryResponseTypeDef,
-    TerminateRecoveryInstancesResponseTypeDef,
+    JobLogEventDataTypeDef,
     LifeCycleTypeDef,
+    JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
-    DescribeJobLogItemsResponseTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
+    StartSourceNetworkReplicationResponseTypeDef,
+    StopSourceNetworkReplicationResponseTypeDef,
+    JobLogTypeDef,
     SourceServerResponseMetadataTypeDef,
     SourceServerTypeDef,
+    AssociateSourceNetworkStackResponseTypeDef,
+    DescribeJobsResponseTypeDef,
+    StartFailbackLaunchResponseTypeDef,
+    StartRecoveryResponseTypeDef,
+    StartSourceNetworkRecoveryResponseTypeDef,
+    TerminateRecoveryInstancesResponseTypeDef,
     RecoveryInstanceTypeDef,
+    DescribeJobLogItemsResponseTypeDef,
     CreateExtendedSourceServerResponseTypeDef,
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
@@ -474,42 +519,42 @@
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

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.py` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,56 +5,64 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_drs import (
         Client,
         DescribeJobLogItemsPaginator,
         DescribeJobsPaginator,
+        DescribeLaunchConfigurationTemplatesPaginator,
         DescribeRecoveryInstancesPaginator,
         DescribeRecoverySnapshotsPaginator,
         DescribeReplicationConfigurationTemplatesPaginator,
+        DescribeSourceNetworksPaginator,
         DescribeSourceServersPaginator,
         ListExtensibleSourceServersPaginator,
         ListStagingAccountsPaginator,
         drsClient,
     )
 
     session = Session()
     client: drsClient = session.client("drs")
 
     describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
     describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+    describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")
     describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")
     describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")
     describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
+    describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator("describe_source_networks")
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = client.get_paginator("list_extensible_source_servers")
     list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator("list_staging_accounts")
     ```
 """
 from .client import drsClient
 from .paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 
 Client = drsClient
 
 
 __all__ = (
     "Client",
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
+    "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeRecoveryInstancesPaginator",
     "DescribeRecoverySnapshotsPaginator",
     "DescribeReplicationConfigurationTemplatesPaginator",
+    "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListStagingAccountsPaginator",
     "drsClient",
 )
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.pyi` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -5,55 +5,63 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_drs import (
         Client,
         DescribeJobLogItemsPaginator,
         DescribeJobsPaginator,
+        DescribeLaunchConfigurationTemplatesPaginator,
         DescribeRecoveryInstancesPaginator,
         DescribeRecoverySnapshotsPaginator,
         DescribeReplicationConfigurationTemplatesPaginator,
+        DescribeSourceNetworksPaginator,
         DescribeSourceServersPaginator,
         ListExtensibleSourceServersPaginator,
         ListStagingAccountsPaginator,
         drsClient,
     )
 
     session = Session()
     client: drsClient = session.client("drs")
 
     describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
     describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+    describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")
     describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")
     describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")
     describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
+    describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator("describe_source_networks")
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = client.get_paginator("list_extensible_source_servers")
     list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator("list_staging_accounts")
     ```
 """
 from .client import drsClient
 from .paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 
 Client = drsClient
 
 __all__ = (
     "Client",
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
+    "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeRecoveryInstancesPaginator",
     "DescribeRecoverySnapshotsPaginator",
     "DescribeReplicationConfigurationTemplatesPaginator",
+    "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListStagingAccountsPaginator",
     "drsClient",
 )
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/__main__.py` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.26.80\nVersion:         1.26.80\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.drs 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.80")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.py` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,34 +25,43 @@
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     TargetInstanceTypeRightSizingMethodType,
 )
 from .paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 from .type_defs import (
+    AssociateSourceNetworkStackResponseTypeDef,
     CreateExtendedSourceServerResponseTypeDef,
+    CreateLaunchConfigurationTemplateResponseTypeDef,
+    CreateSourceNetworkResponseTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     DescribeJobsRequestFiltersTypeDef,
     DescribeJobsResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DescribeSourceServersResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationResponseTypeDef,
     LaunchConfigurationTypeDef,
     LicensingTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PITPolicyRuleTypeDef,
@@ -61,16 +70,21 @@
     ReplicationConfigurationTypeDef,
     ReverseReplicationResponseTypeDef,
     SourceServerResponseMetadataTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartRecoveryResponseTypeDef,
     StartReplicationResponseTypeDef,
+    StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    StartSourceNetworkRecoveryResponseTypeDef,
+    StartSourceNetworkReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
+    StopSourceNetworkReplicationResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
+    UpdateLaunchConfigurationTemplateResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -111,14 +125,25 @@
         """
         drsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#exceptions)
         """
 
+    def associate_source_network_stack(
+        self, *, cfnStackName: str, sourceNetworkID: str
+    ) -> AssociateSourceNetworkStackResponseTypeDef:
+        """
+        Associate a Source Network to an existing CloudFormation Stack and modify launch
+        templates to use this network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.associate_source_network_stack)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#associate_source_network_stack)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#can_paginate)
         """
@@ -138,14 +163,32 @@
         Create an extended source server in the target Account based on the source
         server in staging account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_extended_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_extended_source_server)
         """
 
+    def create_launch_configuration_template(
+        self,
+        *,
+        copyPrivateIp: bool = ...,
+        copyTags: bool = ...,
+        exportBucketArn: str = ...,
+        launchDisposition: LaunchDispositionType = ...,
+        licensing: LicensingTypeDef = ...,
+        tags: Mapping[str, str] = ...,
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+    ) -> CreateLaunchConfigurationTemplateResponseTypeDef:
+        """
+        Creates a new Launch Configuration Template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_launch_configuration_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_launch_configuration_template)
+        """
+
     def create_replication_configuration_template(
         self,
         *,
         associateDefaultSecurityGroup: bool,
         bandwidthThrottling: int,
         createPublicIP: bool,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,
@@ -153,32 +196,53 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType,
         pitPolicy: Sequence[PITPolicyRuleTypeDef],
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
+        autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_replication_configuration_template)
         """
 
+    def create_source_network(
+        self, *, originAccountID: str, originRegion: str, vpcID: str, tags: Mapping[str, str] = ...
+    ) -> CreateSourceNetworkResponseTypeDef:
+        """
+        Create a new Source Network resource for a provided VPC ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_source_network)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_source_network)
+        """
+
     def delete_job(self, *, jobID: str) -> Dict[str, Any]:
         """
         Deletes a single Job by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_job)
         """
 
+    def delete_launch_configuration_template(
+        self, *, launchConfigurationTemplateID: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes a single Launch Configuration Template by ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_launch_configuration_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_launch_configuration_template)
+        """
+
     def delete_recovery_instance(self, *, recoveryInstanceID: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a single Recovery Instance by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_recovery_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_recovery_instance)
         """
@@ -190,14 +254,22 @@
         Deletes a single Replication Configuration Template by ID See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DeleteReplicationConfigurationTemplate).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_replication_configuration_template)
         """
 
+    def delete_source_network(self, *, sourceNetworkID: str) -> Dict[str, Any]:
+        """
+        Delete Source Network resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_source_network)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_source_network)
+        """
+
     def delete_source_server(self, *, sourceServerID: str) -> Dict[str, Any]:
         """
         Deletes a single Source Server by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_source_server)
         """
@@ -222,14 +294,30 @@
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_jobs)
         """
 
+    def describe_launch_configuration_templates(
+        self,
+        *,
+        launchConfigurationTemplateIDs: Sequence[str] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
+        """
+        Lists all Launch Configuration Templates, filtered by Launch Configuration
+        Template IDs See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DescribeLaunchConfigurationTemplates).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_launch_configuration_templates)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_launch_configuration_templates)
+        """
+
     def describe_recovery_instances(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeRecoveryInstancesResponseTypeDef:
@@ -266,14 +354,28 @@
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_replication_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_replication_configuration_templates)
         """
 
+    def describe_source_networks(
+        self,
+        *,
+        filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> DescribeSourceNetworksResponseTypeDef:
+        """
+        Lists all Source Networks or multiple Source Networks filtered by ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_networks)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_source_networks)
+        """
+
     def describe_source_servers(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeSourceServersResponseTypeDef:
@@ -300,14 +402,24 @@
         """
         Disconnects a specific Source Server from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#disconnect_source_server)
         """
 
+    def export_source_network_cfn_template(
+        self, *, sourceNetworkID: str
+    ) -> ExportSourceNetworkCfnTemplateResponseTypeDef:
+        """
+        Export the Source Network CloudFormation template to an S3 bucket.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.export_source_network_cfn_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#export_source_network_cfn_template)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -381,17 +493,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#list_tags_for_resource)
         """
 
     def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
         """
-        Causes the data replication initiation sequence to begin immediately upon next
-        Handshake for the specified Source Server ID, regardless of when the previous
-        initiation started.
+        WARNING: RetryDataReplication is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#retry_data_replication)
         """
 
     def reverse_replication(self, *, recoveryInstanceID: str) -> ReverseReplicationResponseTypeDef:
         """
@@ -431,14 +541,39 @@
         """
         Starts replication for a stopped Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#start_replication)
         """
 
+    def start_source_network_recovery(
+        self,
+        *,
+        sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],
+        deployAsNew: bool = ...,
+        tags: Mapping[str, str] = ...
+    ) -> StartSourceNetworkRecoveryResponseTypeDef:
+        """
+        Deploy VPC for the specified Source Network and modify launch templates to use
+        this network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_recovery)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#start_source_network_recovery)
+        """
+
+    def start_source_network_replication(
+        self, *, sourceNetworkID: str
+    ) -> StartSourceNetworkReplicationResponseTypeDef:
+        """
+        Starts replication for a Source Network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#start_source_network_replication)
+        """
+
     def stop_failback(self, *, recoveryInstanceID: str) -> EmptyResponseMetadataTypeDef:
         """
         Stops the failback process for a specified Recovery Instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_failback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#stop_failback)
         """
@@ -447,14 +582,24 @@
         """
         Stops replication for a Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#stop_replication)
         """
 
+    def stop_source_network_replication(
+        self, *, sourceNetworkID: str
+    ) -> StopSourceNetworkReplicationResponseTypeDef:
+        """
+        Stops replication for a Source Network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_source_network_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#stop_source_network_replication)
+        """
+
     def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or overwrites only the specified tags for the specified Elastic Disaster
         Recovery resource or resources.
 
@@ -515,19 +660,38 @@
         """
         Updates a LaunchConfiguration by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#update_launch_configuration)
         """
 
+    def update_launch_configuration_template(
+        self,
+        *,
+        launchConfigurationTemplateID: str,
+        copyPrivateIp: bool = ...,
+        copyTags: bool = ...,
+        exportBucketArn: str = ...,
+        launchDisposition: LaunchDispositionType = ...,
+        licensing: LicensingTypeDef = ...,
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+    ) -> UpdateLaunchConfigurationTemplateResponseTypeDef:
+        """
+        Updates an existing Launch Configuration Template by ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#update_launch_configuration_template)
+        """
+
     def update_replication_configuration(
         self,
         *,
         sourceServerID: str,
         associateDefaultSecurityGroup: bool = ...,
+        autoReplicateNewDisks: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         name: str = ...,
@@ -548,14 +712,15 @@
 
     def update_replication_configuration_template(
         self,
         *,
         replicationConfigurationTemplateID: str,
         arn: str = ...,
         associateDefaultSecurityGroup: bool = ...,
+        autoReplicateNewDisks: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
@@ -586,14 +751,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_launch_configuration_templates"]
+    ) -> DescribeLaunchConfigurationTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_recovery_instances"]
     ) -> DescribeRecoveryInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
 
@@ -613,14 +787,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_source_networks"]
+    ) -> DescribeSourceNetworksPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_source_servers"]
     ) -> DescribeSourceServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.pyi` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/client.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -25,34 +25,43 @@
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     TargetInstanceTypeRightSizingMethodType,
 )
 from .paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 from .type_defs import (
+    AssociateSourceNetworkStackResponseTypeDef,
     CreateExtendedSourceServerResponseTypeDef,
+    CreateLaunchConfigurationTemplateResponseTypeDef,
+    CreateSourceNetworkResponseTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     DescribeJobsRequestFiltersTypeDef,
     DescribeJobsResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DescribeSourceServersResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationResponseTypeDef,
     LaunchConfigurationTypeDef,
     LicensingTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PITPolicyRuleTypeDef,
@@ -61,16 +70,21 @@
     ReplicationConfigurationTypeDef,
     ReverseReplicationResponseTypeDef,
     SourceServerResponseMetadataTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartRecoveryResponseTypeDef,
     StartReplicationResponseTypeDef,
+    StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    StartSourceNetworkRecoveryResponseTypeDef,
+    StartSourceNetworkReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
+    StopSourceNetworkReplicationResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
+    UpdateLaunchConfigurationTemplateResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -106,14 +120,24 @@
     def exceptions(self) -> Exceptions:
         """
         drsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#exceptions)
         """
+    def associate_source_network_stack(
+        self, *, cfnStackName: str, sourceNetworkID: str
+    ) -> AssociateSourceNetworkStackResponseTypeDef:
+        """
+        Associate a Source Network to an existing CloudFormation Stack and modify launch
+        templates to use this network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.associate_source_network_stack)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#associate_source_network_stack)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#can_paginate)
         """
@@ -130,14 +154,31 @@
         """
         Create an extended source server in the target Account based on the source
         server in staging account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_extended_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_extended_source_server)
         """
+    def create_launch_configuration_template(
+        self,
+        *,
+        copyPrivateIp: bool = ...,
+        copyTags: bool = ...,
+        exportBucketArn: str = ...,
+        launchDisposition: LaunchDispositionType = ...,
+        licensing: LicensingTypeDef = ...,
+        tags: Mapping[str, str] = ...,
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+    ) -> CreateLaunchConfigurationTemplateResponseTypeDef:
+        """
+        Creates a new Launch Configuration Template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_launch_configuration_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_launch_configuration_template)
+        """
     def create_replication_configuration_template(
         self,
         *,
         associateDefaultSecurityGroup: bool,
         bandwidthThrottling: int,
         createPublicIP: bool,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,
@@ -145,30 +186,49 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType,
         pitPolicy: Sequence[PITPolicyRuleTypeDef],
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
+        autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_replication_configuration_template)
         """
+    def create_source_network(
+        self, *, originAccountID: str, originRegion: str, vpcID: str, tags: Mapping[str, str] = ...
+    ) -> CreateSourceNetworkResponseTypeDef:
+        """
+        Create a new Source Network resource for a provided VPC ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_source_network)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_source_network)
+        """
     def delete_job(self, *, jobID: str) -> Dict[str, Any]:
         """
         Deletes a single Job by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_job)
         """
+    def delete_launch_configuration_template(
+        self, *, launchConfigurationTemplateID: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes a single Launch Configuration Template by ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_launch_configuration_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_launch_configuration_template)
+        """
     def delete_recovery_instance(self, *, recoveryInstanceID: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a single Recovery Instance by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_recovery_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_recovery_instance)
         """
@@ -178,14 +238,21 @@
         """
         Deletes a single Replication Configuration Template by ID See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DeleteReplicationConfigurationTemplate).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_replication_configuration_template)
         """
+    def delete_source_network(self, *, sourceNetworkID: str) -> Dict[str, Any]:
+        """
+        Delete Source Network resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_source_network)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_source_network)
+        """
     def delete_source_server(self, *, sourceServerID: str) -> Dict[str, Any]:
         """
         Deletes a single Source Server by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.delete_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#delete_source_server)
         """
@@ -207,14 +274,29 @@
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_jobs)
         """
+    def describe_launch_configuration_templates(
+        self,
+        *,
+        launchConfigurationTemplateIDs: Sequence[str] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
+        """
+        Lists all Launch Configuration Templates, filtered by Launch Configuration
+        Template IDs See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DescribeLaunchConfigurationTemplates).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_launch_configuration_templates)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_launch_configuration_templates)
+        """
     def describe_recovery_instances(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeRecoveryInstancesResponseTypeDef:
@@ -248,14 +330,27 @@
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_replication_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_replication_configuration_templates)
         """
+    def describe_source_networks(
+        self,
+        *,
+        filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> DescribeSourceNetworksResponseTypeDef:
+        """
+        Lists all Source Networks or multiple Source Networks filtered by ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_networks)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#describe_source_networks)
+        """
     def describe_source_servers(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeSourceServersResponseTypeDef:
@@ -279,14 +374,23 @@
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Disconnects a specific Source Server from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#disconnect_source_server)
         """
+    def export_source_network_cfn_template(
+        self, *, sourceNetworkID: str
+    ) -> ExportSourceNetworkCfnTemplateResponseTypeDef:
+        """
+        Export the Source Network CloudFormation template to an S3 bucket.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.export_source_network_cfn_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#export_source_network_cfn_template)
+        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -352,17 +456,15 @@
         List all tags for your Elastic Disaster Recovery resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#list_tags_for_resource)
         """
     def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
         """
-        Causes the data replication initiation sequence to begin immediately upon next
-        Handshake for the specified Source Server ID, regardless of when the previous
-        initiation started.
+        WARNING: RetryDataReplication is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#retry_data_replication)
         """
     def reverse_replication(self, *, recoveryInstanceID: str) -> ReverseReplicationResponseTypeDef:
         """
         Start replication to origin / target region - applies only to protected
@@ -397,28 +499,60 @@
     def start_replication(self, *, sourceServerID: str) -> StartReplicationResponseTypeDef:
         """
         Starts replication for a stopped Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#start_replication)
         """
+    def start_source_network_recovery(
+        self,
+        *,
+        sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],
+        deployAsNew: bool = ...,
+        tags: Mapping[str, str] = ...
+    ) -> StartSourceNetworkRecoveryResponseTypeDef:
+        """
+        Deploy VPC for the specified Source Network and modify launch templates to use
+        this network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_recovery)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#start_source_network_recovery)
+        """
+    def start_source_network_replication(
+        self, *, sourceNetworkID: str
+    ) -> StartSourceNetworkReplicationResponseTypeDef:
+        """
+        Starts replication for a Source Network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#start_source_network_replication)
+        """
     def stop_failback(self, *, recoveryInstanceID: str) -> EmptyResponseMetadataTypeDef:
         """
         Stops the failback process for a specified Recovery Instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_failback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#stop_failback)
         """
     def stop_replication(self, *, sourceServerID: str) -> StopReplicationResponseTypeDef:
         """
         Stops replication for a Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#stop_replication)
         """
+    def stop_source_network_replication(
+        self, *, sourceNetworkID: str
+    ) -> StopSourceNetworkReplicationResponseTypeDef:
+        """
+        Stops replication for a Source Network.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.stop_source_network_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#stop_source_network_replication)
+        """
     def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or overwrites only the specified tags for the specified Elastic Disaster
         Recovery resource or resources.
 
@@ -474,19 +608,37 @@
     ) -> LaunchConfigurationTypeDef:
         """
         Updates a LaunchConfiguration by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#update_launch_configuration)
         """
+    def update_launch_configuration_template(
+        self,
+        *,
+        launchConfigurationTemplateID: str,
+        copyPrivateIp: bool = ...,
+        copyTags: bool = ...,
+        exportBucketArn: str = ...,
+        launchDisposition: LaunchDispositionType = ...,
+        licensing: LicensingTypeDef = ...,
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+    ) -> UpdateLaunchConfigurationTemplateResponseTypeDef:
+        """
+        Updates an existing Launch Configuration Template by ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#update_launch_configuration_template)
+        """
     def update_replication_configuration(
         self,
         *,
         sourceServerID: str,
         associateDefaultSecurityGroup: bool = ...,
+        autoReplicateNewDisks: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         name: str = ...,
@@ -506,14 +658,15 @@
         """
     def update_replication_configuration_template(
         self,
         *,
         replicationConfigurationTemplateID: str,
         arn: str = ...,
         associateDefaultSecurityGroup: bool = ...,
+        autoReplicateNewDisks: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
@@ -541,14 +694,22 @@
     def get_paginator(self, operation_name: Literal["describe_jobs"]) -> DescribeJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_launch_configuration_templates"]
+    ) -> DescribeLaunchConfigurationTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_recovery_instances"]
     ) -> DescribeRecoveryInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
     @overload
@@ -565,14 +726,22 @@
     ) -> DescribeReplicationConfigurationTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_source_networks"]
+    ) -> DescribeSourceNetworksPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_source_servers"]
     ) -> DescribeSourceServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.py` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 __all__ = (
     "DataReplicationErrorStringType",
     "DataReplicationInitiationStepNameType",
     "DataReplicationInitiationStepStatusType",
     "DataReplicationStateType",
     "DescribeJobLogItemsPaginatorName",
     "DescribeJobsPaginatorName",
+    "DescribeLaunchConfigurationTemplatesPaginatorName",
     "DescribeRecoveryInstancesPaginatorName",
     "DescribeRecoverySnapshotsPaginatorName",
     "DescribeReplicationConfigurationTemplatesPaginatorName",
+    "DescribeSourceNetworksPaginatorName",
     "DescribeSourceServersPaginatorName",
     "EC2InstanceStateType",
     "ExtensionStatusType",
     "FailbackLaunchTypeType",
     "FailbackReplicationErrorType",
     "FailbackStateType",
     "InitiatedByType",
@@ -46,20 +48,22 @@
     "ListExtensibleSourceServersPaginatorName",
     "ListStagingAccountsPaginatorName",
     "OriginEnvironmentType",
     "PITPolicyRuleUnitsType",
     "RecoveryInstanceDataReplicationInitiationStepNameType",
     "RecoveryInstanceDataReplicationInitiationStepStatusType",
     "RecoveryInstanceDataReplicationStateType",
+    "RecoveryResultType",
     "RecoverySnapshotsOrderType",
     "ReplicationConfigurationDataPlaneRoutingType",
     "ReplicationConfigurationDefaultLargeStagingDiskTypeType",
     "ReplicationConfigurationEbsEncryptionType",
     "ReplicationConfigurationReplicatedDiskStagingDiskTypeType",
     "ReplicationDirectionType",
+    "ReplicationStatusType",
     "TargetInstanceTypeRightSizingMethodType",
     "drsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -107,19 +111,23 @@
     "PAUSED",
     "RESCAN",
     "STALLED",
     "STOPPED",
 ]
 DescribeJobLogItemsPaginatorName = Literal["describe_job_log_items"]
 DescribeJobsPaginatorName = Literal["describe_jobs"]
+DescribeLaunchConfigurationTemplatesPaginatorName = Literal[
+    "describe_launch_configuration_templates"
+]
 DescribeRecoveryInstancesPaginatorName = Literal["describe_recovery_instances"]
 DescribeRecoverySnapshotsPaginatorName = Literal["describe_recovery_snapshots"]
 DescribeReplicationConfigurationTemplatesPaginatorName = Literal[
     "describe_replication_configuration_templates"
 ]
+DescribeSourceNetworksPaginatorName = Literal["describe_source_networks"]
 DescribeSourceServersPaginatorName = Literal["describe_source_servers"]
 EC2InstanceStateType = Literal[
     "NOT_FOUND", "PENDING", "RUNNING", "SHUTTING-DOWN", "STOPPED", "STOPPING", "TERMINATED"
 ]
 ExtensionStatusType = Literal["EXTENDED", "EXTENSION_ERROR", "NOT_EXTENDED"]
 FailbackLaunchTypeType = Literal["DRILL", "RECOVERY"]
 FailbackReplicationErrorType = Literal[
@@ -151,37 +159,50 @@
     "FAILBACK_IN_PROGRESS",
     "FAILBACK_LAUNCH_STATE_NOT_AVAILABLE",
     "FAILBACK_NOT_READY_FOR_LAUNCH",
     "FAILBACK_NOT_STARTED",
     "FAILBACK_READY_FOR_LAUNCH",
 ]
 InitiatedByType = Literal[
+    "ASSOCIATE_NETWORK_RECOVERY",
+    "CREATE_NETWORK_RECOVERY",
     "DIAGNOSTIC",
     "FAILBACK",
     "START_DRILL",
     "START_RECOVERY",
     "TARGET_ACCOUNT",
     "TERMINATE_RECOVERY_INSTANCES",
+    "UPDATE_NETWORK_RECOVERY",
 ]
 JobLogEventType = Literal[
     "CLEANUP_END",
     "CLEANUP_FAIL",
     "CLEANUP_START",
     "CONVERSION_END",
     "CONVERSION_FAIL",
     "CONVERSION_START",
+    "DEPLOY_NETWORK_CONFIGURATION_END",
+    "DEPLOY_NETWORK_CONFIGURATION_FAILED",
+    "DEPLOY_NETWORK_CONFIGURATION_START",
     "JOB_CANCEL",
     "JOB_END",
     "JOB_START",
     "LAUNCH_FAILED",
     "LAUNCH_START",
+    "NETWORK_RECOVERY_FAIL",
     "SERVER_SKIPPED",
     "SNAPSHOT_END",
     "SNAPSHOT_FAIL",
     "SNAPSHOT_START",
+    "UPDATE_LAUNCH_TEMPLATE_END",
+    "UPDATE_LAUNCH_TEMPLATE_FAILED",
+    "UPDATE_LAUNCH_TEMPLATE_START",
+    "UPDATE_NETWORK_CONFIGURATION_END",
+    "UPDATE_NETWORK_CONFIGURATION_FAILED",
+    "UPDATE_NETWORK_CONFIGURATION_START",
     "USING_PREVIOUS_SNAPSHOT",
     "USING_PREVIOUS_SNAPSHOT_FAILED",
 ]
 JobStatusType = Literal["COMPLETED", "PENDING", "STARTED"]
 JobTypeType = Literal["CREATE_CONVERTED_SNAPSHOT", "LAUNCH", "TERMINATE"]
 LastLaunchResultType = Literal["FAILED", "NOT_STARTED", "PENDING", "SUCCEEDED"]
 LastLaunchTypeType = Literal["DRILL", "RECOVERY"]
@@ -224,22 +245,32 @@
     "NOT_STARTED",
     "PAUSED",
     "REPLICATION_STATE_NOT_AVAILABLE",
     "RESCAN",
     "STALLED",
     "STOPPED",
 ]
+RecoveryResultType = Literal[
+    "ASSOCIATE_FAIL",
+    "ASSOCIATE_SUCCESS",
+    "FAIL",
+    "IN_PROGRESS",
+    "NOT_STARTED",
+    "PARTIAL_SUCCESS",
+    "SUCCESS",
+]
 RecoverySnapshotsOrderType = Literal["ASC", "DESC"]
 ReplicationConfigurationDataPlaneRoutingType = Literal["PRIVATE_IP", "PUBLIC_IP"]
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["AUTO", "GP2", "GP3", "ST1"]
-ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT"]
+ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT", "NONE"]
 ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
     "AUTO", "GP2", "GP3", "IO1", "SC1", "ST1", "STANDARD"
 ]
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
+ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
 TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "NONE"]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -249,14 +280,15 @@
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
@@ -296,14 +328,15 @@
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
@@ -401,14 +434,15 @@
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
@@ -444,14 +478,15 @@
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
@@ -470,16 +505,19 @@
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
@@ -563,15 +601,17 @@
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
@@ -592,17 +632,19 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_job_log_items",
     "describe_jobs",
+    "describe_launch_configuration_templates",
     "describe_recovery_instances",
     "describe_recovery_snapshots",
     "describe_replication_configuration_templates",
+    "describe_source_networks",
     "describe_source_servers",
     "list_extensible_source_servers",
     "list_staging_accounts",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.pyi` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 __all__ = (
     "DataReplicationErrorStringType",
     "DataReplicationInitiationStepNameType",
     "DataReplicationInitiationStepStatusType",
     "DataReplicationStateType",
     "DescribeJobLogItemsPaginatorName",
     "DescribeJobsPaginatorName",
+    "DescribeLaunchConfigurationTemplatesPaginatorName",
     "DescribeRecoveryInstancesPaginatorName",
     "DescribeRecoverySnapshotsPaginatorName",
     "DescribeReplicationConfigurationTemplatesPaginatorName",
+    "DescribeSourceNetworksPaginatorName",
     "DescribeSourceServersPaginatorName",
     "EC2InstanceStateType",
     "ExtensionStatusType",
     "FailbackLaunchTypeType",
     "FailbackReplicationErrorType",
     "FailbackStateType",
     "InitiatedByType",
@@ -45,20 +47,22 @@
     "ListExtensibleSourceServersPaginatorName",
     "ListStagingAccountsPaginatorName",
     "OriginEnvironmentType",
     "PITPolicyRuleUnitsType",
     "RecoveryInstanceDataReplicationInitiationStepNameType",
     "RecoveryInstanceDataReplicationInitiationStepStatusType",
     "RecoveryInstanceDataReplicationStateType",
+    "RecoveryResultType",
     "RecoverySnapshotsOrderType",
     "ReplicationConfigurationDataPlaneRoutingType",
     "ReplicationConfigurationDefaultLargeStagingDiskTypeType",
     "ReplicationConfigurationEbsEncryptionType",
     "ReplicationConfigurationReplicatedDiskStagingDiskTypeType",
     "ReplicationDirectionType",
+    "ReplicationStatusType",
     "TargetInstanceTypeRightSizingMethodType",
     "drsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -105,19 +109,23 @@
     "PAUSED",
     "RESCAN",
     "STALLED",
     "STOPPED",
 ]
 DescribeJobLogItemsPaginatorName = Literal["describe_job_log_items"]
 DescribeJobsPaginatorName = Literal["describe_jobs"]
+DescribeLaunchConfigurationTemplatesPaginatorName = Literal[
+    "describe_launch_configuration_templates"
+]
 DescribeRecoveryInstancesPaginatorName = Literal["describe_recovery_instances"]
 DescribeRecoverySnapshotsPaginatorName = Literal["describe_recovery_snapshots"]
 DescribeReplicationConfigurationTemplatesPaginatorName = Literal[
     "describe_replication_configuration_templates"
 ]
+DescribeSourceNetworksPaginatorName = Literal["describe_source_networks"]
 DescribeSourceServersPaginatorName = Literal["describe_source_servers"]
 EC2InstanceStateType = Literal[
     "NOT_FOUND", "PENDING", "RUNNING", "SHUTTING-DOWN", "STOPPED", "STOPPING", "TERMINATED"
 ]
 ExtensionStatusType = Literal["EXTENDED", "EXTENSION_ERROR", "NOT_EXTENDED"]
 FailbackLaunchTypeType = Literal["DRILL", "RECOVERY"]
 FailbackReplicationErrorType = Literal[
@@ -149,37 +157,50 @@
     "FAILBACK_IN_PROGRESS",
     "FAILBACK_LAUNCH_STATE_NOT_AVAILABLE",
     "FAILBACK_NOT_READY_FOR_LAUNCH",
     "FAILBACK_NOT_STARTED",
     "FAILBACK_READY_FOR_LAUNCH",
 ]
 InitiatedByType = Literal[
+    "ASSOCIATE_NETWORK_RECOVERY",
+    "CREATE_NETWORK_RECOVERY",
     "DIAGNOSTIC",
     "FAILBACK",
     "START_DRILL",
     "START_RECOVERY",
     "TARGET_ACCOUNT",
     "TERMINATE_RECOVERY_INSTANCES",
+    "UPDATE_NETWORK_RECOVERY",
 ]
 JobLogEventType = Literal[
     "CLEANUP_END",
     "CLEANUP_FAIL",
     "CLEANUP_START",
     "CONVERSION_END",
     "CONVERSION_FAIL",
     "CONVERSION_START",
+    "DEPLOY_NETWORK_CONFIGURATION_END",
+    "DEPLOY_NETWORK_CONFIGURATION_FAILED",
+    "DEPLOY_NETWORK_CONFIGURATION_START",
     "JOB_CANCEL",
     "JOB_END",
     "JOB_START",
     "LAUNCH_FAILED",
     "LAUNCH_START",
+    "NETWORK_RECOVERY_FAIL",
     "SERVER_SKIPPED",
     "SNAPSHOT_END",
     "SNAPSHOT_FAIL",
     "SNAPSHOT_START",
+    "UPDATE_LAUNCH_TEMPLATE_END",
+    "UPDATE_LAUNCH_TEMPLATE_FAILED",
+    "UPDATE_LAUNCH_TEMPLATE_START",
+    "UPDATE_NETWORK_CONFIGURATION_END",
+    "UPDATE_NETWORK_CONFIGURATION_FAILED",
+    "UPDATE_NETWORK_CONFIGURATION_START",
     "USING_PREVIOUS_SNAPSHOT",
     "USING_PREVIOUS_SNAPSHOT_FAILED",
 ]
 JobStatusType = Literal["COMPLETED", "PENDING", "STARTED"]
 JobTypeType = Literal["CREATE_CONVERTED_SNAPSHOT", "LAUNCH", "TERMINATE"]
 LastLaunchResultType = Literal["FAILED", "NOT_STARTED", "PENDING", "SUCCEEDED"]
 LastLaunchTypeType = Literal["DRILL", "RECOVERY"]
@@ -222,22 +243,32 @@
     "NOT_STARTED",
     "PAUSED",
     "REPLICATION_STATE_NOT_AVAILABLE",
     "RESCAN",
     "STALLED",
     "STOPPED",
 ]
+RecoveryResultType = Literal[
+    "ASSOCIATE_FAIL",
+    "ASSOCIATE_SUCCESS",
+    "FAIL",
+    "IN_PROGRESS",
+    "NOT_STARTED",
+    "PARTIAL_SUCCESS",
+    "SUCCESS",
+]
 RecoverySnapshotsOrderType = Literal["ASC", "DESC"]
 ReplicationConfigurationDataPlaneRoutingType = Literal["PRIVATE_IP", "PUBLIC_IP"]
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["AUTO", "GP2", "GP3", "ST1"]
-ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT"]
+ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT", "NONE"]
 ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
     "AUTO", "GP2", "GP3", "IO1", "SC1", "ST1", "STANDARD"
 ]
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
+ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
 TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "NONE"]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -247,14 +278,15 @@
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
@@ -294,14 +326,15 @@
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
@@ -399,14 +432,15 @@
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
@@ -442,14 +476,15 @@
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
@@ -468,16 +503,19 @@
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
@@ -561,15 +599,17 @@
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
@@ -590,17 +630,19 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_job_log_items",
     "describe_jobs",
+    "describe_launch_configuration_templates",
     "describe_recovery_instances",
     "describe_recovery_snapshots",
     "describe_replication_configuration_templates",
+    "describe_source_networks",
     "describe_source_servers",
     "list_extensible_source_servers",
     "list_staging_accounts",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.py` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/paginator.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,62 +8,71 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_drs.client import drsClient
     from mypy_boto3_drs.paginator import (
         DescribeJobLogItemsPaginator,
         DescribeJobsPaginator,
+        DescribeLaunchConfigurationTemplatesPaginator,
         DescribeRecoveryInstancesPaginator,
         DescribeRecoverySnapshotsPaginator,
         DescribeReplicationConfigurationTemplatesPaginator,
+        DescribeSourceNetworksPaginator,
         DescribeSourceServersPaginator,
         ListExtensibleSourceServersPaginator,
         ListStagingAccountsPaginator,
     )
 
     session = Session()
     client: drsClient = session.client("drs")
 
     describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
     describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+    describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")
     describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")
     describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")
     describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
+    describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator("describe_source_networks")
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = client.get_paginator("list_extensible_source_servers")
     list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator("list_staging_accounts")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import RecoverySnapshotsOrderType
 from .type_defs import (
     DescribeJobLogItemsResponseTypeDef,
     DescribeJobsRequestFiltersTypeDef,
     DescribeJobsResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DescribeSourceServersResponseTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
+    "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeRecoveryInstancesPaginator",
     "DescribeRecoverySnapshotsPaginator",
     "DescribeReplicationConfigurationTemplatesPaginator",
+    "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListStagingAccountsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
@@ -79,15 +88,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
         """
 
 
@@ -97,33 +106,51 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
         """
 
 
+class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        launchConfigurationTemplateIDs: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
+        """
+
+
 class DescribeRecoveryInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
         """
 
 
@@ -135,15 +162,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
 
@@ -153,61 +180,79 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
+class DescribeSourceNetworksPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[DescribeSourceNetworksResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
+        """
+
+
 class DescribeSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
         """
 
 
 class ListExtensibleSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
     """
 
     def paginate(
-        self, *, stagingAccountID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, stagingAccountID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExtensibleSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
         """
 
 
 class ListStagingAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStagingAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
         """
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.pyi` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/paginator.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -8,62 +8,71 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_drs.client import drsClient
     from mypy_boto3_drs.paginator import (
         DescribeJobLogItemsPaginator,
         DescribeJobsPaginator,
+        DescribeLaunchConfigurationTemplatesPaginator,
         DescribeRecoveryInstancesPaginator,
         DescribeRecoverySnapshotsPaginator,
         DescribeReplicationConfigurationTemplatesPaginator,
+        DescribeSourceNetworksPaginator,
         DescribeSourceServersPaginator,
         ListExtensibleSourceServersPaginator,
         ListStagingAccountsPaginator,
     )
 
     session = Session()
     client: drsClient = session.client("drs")
 
     describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
     describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+    describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")
     describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")
     describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")
     describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
+    describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator("describe_source_networks")
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = client.get_paginator("list_extensible_source_servers")
     list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator("list_staging_accounts")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import RecoverySnapshotsOrderType
 from .type_defs import (
     DescribeJobLogItemsResponseTypeDef,
     DescribeJobsRequestFiltersTypeDef,
     DescribeJobsResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DescribeSourceServersResponseTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
+    "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeRecoveryInstancesPaginator",
     "DescribeRecoverySnapshotsPaginator",
     "DescribeReplicationConfigurationTemplatesPaginator",
+    "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListStagingAccountsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -76,15 +85,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
         """
 
 class DescribeJobsPaginator(Paginator):
@@ -93,32 +102,49 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
         """
 
+class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        launchConfigurationTemplateIDs: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
+        """
+
 class DescribeRecoveryInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
         """
 
 class DescribeRecoverySnapshotsPaginator(Paginator):
@@ -129,15 +155,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(Paginator):
@@ -146,58 +172,75 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
+class DescribeSourceNetworksPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[DescribeSourceNetworksResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
+        """
+
 class DescribeSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
         """
 
 class ListExtensibleSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
     """
 
     def paginate(
-        self, *, stagingAccountID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, stagingAccountID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExtensibleSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
         """
 
 class ListStagingAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStagingAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
         """
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.py` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from mypy_boto3_drs.type_defs import AccountTypeDef
 
     data: AccountTypeDef = {...}
     ```
 """
 import sys
+from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataReplicationErrorStringType,
     DataReplicationInitiationStepNameType,
     DataReplicationInitiationStepStatusType,
     DataReplicationStateType,
@@ -33,134 +34,169 @@
     LaunchDispositionType,
     LaunchStatusType,
     OriginEnvironmentType,
     PITPolicyRuleUnitsType,
     RecoveryInstanceDataReplicationInitiationStepNameType,
     RecoveryInstanceDataReplicationInitiationStepStatusType,
     RecoveryInstanceDataReplicationStateType,
+    RecoveryResultType,
     RecoverySnapshotsOrderType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
     ReplicationDirectionType,
+    ReplicationStatusType,
     TargetInstanceTypeRightSizingMethodType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountTypeDef",
+    "AssociateSourceNetworkStackRequestRequestTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "LicensingTypeDef",
     "PITPolicyRuleTypeDef",
+    "CreateSourceNetworkRequestRequestTypeDef",
+    "CreateSourceNetworkResponseTypeDef",
     "DataReplicationErrorTypeDef",
     "DataReplicationInfoReplicatedDiskTypeDef",
     "DataReplicationInitiationStepTypeDef",
     "DeleteJobRequestRequestTypeDef",
+    "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
+    "DeleteSourceNetworkRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     "DescribeRecoverySnapshotsRequestFiltersTypeDef",
     "RecoverySnapshotTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
+    "DescribeSourceNetworksRequestFiltersTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
     "DisconnectRecoveryInstanceRequestRequestTypeDef",
     "DisconnectSourceServerRequestRequestTypeDef",
     "DiskTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "SourceNetworkDataTypeDef",
+    "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
+    "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
-    "LicensingTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
+    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PaginatorConfigTypeDef",
+    "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
+    "RecoveryLifeCycleTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
+    "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
     "StartFailbackLaunchRequestRequestTypeDef",
     "StartRecoveryRequestSourceServerTypeDef",
     "StartReplicationRequestRequestTypeDef",
+    "StartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
+    "StartSourceNetworkReplicationRequestRequestTypeDef",
     "StopFailbackRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
+    "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
-    "JobLogEventDataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetFailbackReplicationConfigurationResponseTypeDef",
     "ListStagingAccountsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ReverseReplicationResponseTypeDef",
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "LaunchConfigurationTemplateTypeDef",
+    "LaunchConfigurationTypeDef",
+    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
+    "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
+    "DescribeSourceNetworksRequestRequestTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
-    "JobTypeDef",
-    "LaunchConfigurationTypeDef",
-    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "EventResourceDataTypeDef",
     "LifeCycleLastLaunchTypeDef",
     "ListExtensibleSourceServersResponseTypeDef",
     "SourcePropertiesTypeDef",
+    "ParticipatingResourceTypeDef",
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     "RecoveryInstancePropertiesTypeDef",
+    "SourceNetworkTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "StartRecoveryRequestRequestTypeDef",
-    "JobLogTypeDef",
+    "StartSourceNetworkRecoveryRequestRequestTypeDef",
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DataReplicationInfoTypeDef",
-    "DescribeJobsResponseTypeDef",
-    "StartFailbackLaunchResponseTypeDef",
-    "StartRecoveryResponseTypeDef",
-    "TerminateRecoveryInstancesResponseTypeDef",
+    "JobLogEventDataTypeDef",
     "LifeCycleTypeDef",
+    "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
-    "DescribeJobLogItemsResponseTypeDef",
+    "DescribeSourceNetworksResponseTypeDef",
+    "StartSourceNetworkReplicationResponseTypeDef",
+    "StopSourceNetworkReplicationResponseTypeDef",
+    "JobLogTypeDef",
     "SourceServerResponseMetadataTypeDef",
     "SourceServerTypeDef",
+    "AssociateSourceNetworkStackResponseTypeDef",
+    "DescribeJobsResponseTypeDef",
+    "StartFailbackLaunchResponseTypeDef",
+    "StartRecoveryResponseTypeDef",
+    "StartSourceNetworkRecoveryResponseTypeDef",
+    "TerminateRecoveryInstancesResponseTypeDef",
     "RecoveryInstanceTypeDef",
+    "DescribeJobLogItemsResponseTypeDef",
     "CreateExtendedSourceServerResponseTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "StartReplicationResponseTypeDef",
     "StopReplicationResponseTypeDef",
     "DescribeRecoveryInstancesResponseTypeDef",
 )
 
@@ -168,14 +204,22 @@
     "AccountTypeDef",
     {
         "accountID": str,
     },
     total=False,
 )
 
+AssociateSourceNetworkStackRequestRequestTypeDef = TypedDict(
+    "AssociateSourceNetworkStackRequestRequestTypeDef",
+    {
+        "cfnStackName": str,
+        "sourceNetworkID": str,
+    },
+)
+
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
     total=False,
@@ -211,23 +255,20 @@
 class CreateExtendedSourceServerRequestRequestTypeDef(
     _RequiredCreateExtendedSourceServerRequestRequestTypeDef,
     _OptionalCreateExtendedSourceServerRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+LicensingTypeDef = TypedDict(
+    "LicensingTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "osByol": bool,
     },
+    total=False,
 )
 
 _RequiredPITPolicyRuleTypeDef = TypedDict(
     "_RequiredPITPolicyRuleTypeDef",
     {
         "interval": int,
         "retentionDuration": int,
@@ -244,14 +285,46 @@
 )
 
 
 class PITPolicyRuleTypeDef(_RequiredPITPolicyRuleTypeDef, _OptionalPITPolicyRuleTypeDef):
     pass
 
 
+_RequiredCreateSourceNetworkRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceNetworkRequestRequestTypeDef",
+    {
+        "originAccountID": str,
+        "originRegion": str,
+        "vpcID": str,
+    },
+)
+_OptionalCreateSourceNetworkRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceNetworkRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateSourceNetworkRequestRequestTypeDef(
+    _RequiredCreateSourceNetworkRequestRequestTypeDef,
+    _OptionalCreateSourceNetworkRequestRequestTypeDef,
+):
+    pass
+
+
+CreateSourceNetworkResponseTypeDef = TypedDict(
+    "CreateSourceNetworkResponseTypeDef",
+    {
+        "sourceNetworkID": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataReplicationErrorTypeDef = TypedDict(
     "DataReplicationErrorTypeDef",
     {
         "error": DataReplicationErrorStringType,
         "rawError": str,
     },
     total=False,
@@ -281,45 +354,71 @@
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 
+DeleteLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "launchConfigurationTemplateID": str,
+    },
+)
+
 DeleteRecoveryInstanceRequestRequestTypeDef = TypedDict(
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
 DeleteReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 
+DeleteSourceNetworkRequestRequestTypeDef = TypedDict(
+    "DeleteSourceNetworkRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
 DeleteSourceServerRequestRequestTypeDef = TypedDict(
     "DeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -345,14 +444,33 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 DescribeRecoveryInstancesRequestFiltersTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     {
         "recoveryInstanceIDs": Sequence[str],
         "sourceServerIDs": Sequence[str],
     },
     total=False,
@@ -385,24 +503,43 @@
 )
 
 
 class RecoverySnapshotTypeDef(_RequiredRecoverySnapshotTypeDef, _OptionalRecoverySnapshotTypeDef):
     pass
 
 
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
     total=False,
 )
 
+DescribeSourceNetworksRequestFiltersTypeDef = TypedDict(
+    "DescribeSourceNetworksRequestFiltersTypeDef",
+    {
+        "originAccountID": str,
+        "originRegion": str,
+        "sourceNetworkIDs": Sequence[str],
+    },
+    total=False,
+)
+
 DescribeSourceServersRequestFiltersTypeDef = TypedDict(
     "DescribeSourceServersRequestFiltersTypeDef",
     {
         "hardwareId": str,
         "sourceServerIDs": Sequence[str],
         "stagingAccountIDs": Sequence[str],
     },
@@ -428,21 +565,65 @@
     {
         "bytes": int,
         "deviceName": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SourceNetworkDataTypeDef = TypedDict(
+    "SourceNetworkDataTypeDef",
+    {
+        "sourceNetworkID": str,
+        "sourceVpc": str,
+        "stackName": str,
+        "targetVpc": str,
+    },
+    total=False,
+)
+
+ExportSourceNetworkCfnTemplateRequestRequestTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
+ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    {
+        "s3DestinationUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFailbackReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
+GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetFailbackReplicationConfigurationResponseTypeDef",
+    {
+        "bandwidthThrottling": int,
+        "name": str,
+        "recoveryInstanceID": str,
+        "usePrivateIP": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "GetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -470,32 +651,46 @@
         "launchStatus": LaunchStatusType,
         "recoveryInstanceID": str,
         "sourceServerID": str,
     },
     total=False,
 )
 
-LicensingTypeDef = TypedDict(
-    "LicensingTypeDef",
-    {
-        "osByol": bool,
-    },
-    total=False,
-)
-
 LifeCycleLastLaunchInitiatedTypeDef = TypedDict(
     "LifeCycleLastLaunchInitiatedTypeDef",
     {
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
     total=False,
 )
 
+_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "stagingAccountID": str,
+    },
+)
+_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
+    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensibleSourceServersRequestRequestTypeDef",
     {
         "stagingAccountID": str,
     },
 )
 _OptionalListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
@@ -521,14 +716,22 @@
         "arn": str,
         "hostname": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStagingAccountsRequestRequestTypeDef = TypedDict(
     "ListStagingAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -537,14 +740,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
     },
@@ -555,14 +766,32 @@
     "OSTypeDef",
     {
         "fullString": str,
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
+ParticipatingResourceIDTypeDef = TypedDict(
+    "ParticipatingResourceIDTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+    total=False,
+)
+
 RecoveryInstanceDataReplicationErrorTypeDef = TypedDict(
     "RecoveryInstanceDataReplicationErrorTypeDef",
     {
         "error": FailbackReplicationErrorType,
         "rawError": str,
     },
     total=False,
@@ -612,41 +841,70 @@
         "failbackToOriginalServer": bool,
         "firstByteDateTime": str,
         "state": FailbackStateType,
     },
     total=False,
 )
 
+RecoveryLifeCycleTypeDef = TypedDict(
+    "RecoveryLifeCycleTypeDef",
+    {
+        "apiCallDateTime": datetime,
+        "jobID": str,
+        "lastRecoveryResult": RecoveryResultType,
+    },
+    total=False,
+)
+
 ReplicationConfigurationReplicatedDiskTypeDef = TypedDict(
     "ReplicationConfigurationReplicatedDiskTypeDef",
     {
         "deviceName": str,
         "iops": int,
         "isBootDisk": bool,
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
 ReverseReplicationRequestRequestTypeDef = TypedDict(
     "ReverseReplicationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
+ReverseReplicationResponseTypeDef = TypedDict(
+    "ReverseReplicationResponseTypeDef",
+    {
+        "reversedDirectionSourceServerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": str,
         "originAvailabilityZone": str,
         "originRegion": str,
     },
@@ -711,28 +969,64 @@
 StartReplicationRequestRequestTypeDef = TypedDict(
     "StartReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
+_RequiredStartSourceNetworkRecoveryRequestNetworkEntryTypeDef = TypedDict(
+    "_RequiredStartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+_OptionalStartSourceNetworkRecoveryRequestNetworkEntryTypeDef = TypedDict(
+    "_OptionalStartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
+    {
+        "cfnStackName": str,
+    },
+    total=False,
+)
+
+
+class StartSourceNetworkRecoveryRequestNetworkEntryTypeDef(
+    _RequiredStartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    _OptionalStartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+):
+    pass
+
+
+StartSourceNetworkReplicationRequestRequestTypeDef = TypedDict(
+    "StartSourceNetworkReplicationRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
 StopFailbackRequestRequestTypeDef = TypedDict(
     "StopFailbackRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
 StopReplicationRequestRequestTypeDef = TypedDict(
     "StopReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
+StopSourceNetworkReplicationRequestRequestTypeDef = TypedDict(
+    "StopSourceNetworkReplicationRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -772,68 +1066,121 @@
 class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-JobLogEventDataTypeDef = TypedDict(
-    "JobLogEventDataTypeDef",
+ListStagingAccountsResponseTypeDef = TypedDict(
+    "ListStagingAccountsResponseTypeDef",
     {
-        "conversionProperties": ConversionPropertiesTypeDef,
-        "conversionServerID": str,
-        "rawError": str,
-        "sourceServerID": str,
-        "targetInstanceID": str,
+        "accounts": List[AccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "tags": Mapping[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+LaunchConfigurationTemplateTypeDef = TypedDict(
+    "LaunchConfigurationTemplateTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "arn": str,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchConfigurationTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "tags": Dict[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
+    total=False,
 )
 
-GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetFailbackReplicationConfigurationResponseTypeDef",
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
     {
-        "bandwidthThrottling": int,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
         "name": str,
-        "recoveryInstanceID": str,
-        "usePrivateIP": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListStagingAccountsResponseTypeDef = TypedDict(
-    "ListStagingAccountsResponseTypeDef",
+_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "accounts": List[AccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sourceServerID": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "name": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
+    total=False,
 )
 
-ReverseReplicationResponseTypeDef = TypedDict(
-    "ReverseReplicationResponseTypeDef",
+
+class UpdateLaunchConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
-        "reversedDirectionSourceServerArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "launchConfigurationTemplateID": str,
     },
 )
+_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
+
+class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "associateDefaultSecurityGroup": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
@@ -847,14 +1194,15 @@
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
     },
 )
 _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
+        "autoReplicateNewDisks": bool,
         "ebsEncryptionKeyArn": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -866,43 +1214,45 @@
 
 
 ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "pitPolicy": List[PITPolicyRuleTypeDef],
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
     "_RequiredReplicationConfigurationTemplateTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 _OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
     "_OptionalReplicationConfigurationTemplateTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "pitPolicy": List[PITPolicyRuleTypeDef],
@@ -931,14 +1281,15 @@
     },
 )
 _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "pitPolicy": Sequence[PITPolicyRuleTypeDef],
@@ -965,80 +1316,19 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
-
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "stagingAccountID": str,
-    },
-)
-_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
-    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-):
-    pass
-
-
-ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1049,15 +1339,15 @@
     total=False,
 )
 
 DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     {
         "filters": DescribeRecoveryInstancesRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeRecoveryInstancesRequestRequestTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     {
@@ -1075,15 +1365,15 @@
     },
 )
 _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = TypedDict(
     "_OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     {
         "filters": DescribeRecoverySnapshotsRequestFiltersTypeDef,
         "order": RecoverySnapshotsOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(
     _RequiredDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
@@ -1118,134 +1408,103 @@
 
 
 DescribeRecoverySnapshotsResponseTypeDef = TypedDict(
     "DescribeRecoverySnapshotsResponseTypeDef",
     {
         "items": List[RecoverySnapshotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
-    "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
+DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef = TypedDict(
+    "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     {
-        "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "filters": DescribeSourceNetworksRequestFiltersTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeSourceServersRequestRequestTypeDef = TypedDict(
-    "DescribeSourceServersRequestRequestTypeDef",
+DescribeSourceNetworksRequestRequestTypeDef = TypedDict(
+    "DescribeSourceNetworksRequestRequestTypeDef",
     {
-        "filters": DescribeSourceServersRequestFiltersTypeDef,
+        "filters": DescribeSourceNetworksRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
+    "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
-        "arn": str,
-        "creationDateTime": str,
-        "endDateTime": str,
-        "initiatedBy": InitiatedByType,
-        "participatingServers": List[ParticipatingServerTypeDef],
-        "status": JobStatusType,
-        "tags": Dict[str, str],
-        "type": JobTypeType,
+        "filters": DescribeSourceServersRequestFiltersTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
+DescribeSourceServersRequestRequestTypeDef = TypedDict(
+    "DescribeSourceServersRequestRequestTypeDef",
     {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "name": str,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filters": DescribeSourceServersRequestFiltersTypeDef,
+        "maxResults": int,
+        "nextToken": str,
     },
+    total=False,
 )
 
-_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
-    {
-        "sourceServerID": str,
-    },
-)
-_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+EventResourceDataTypeDef = TypedDict(
+    "EventResourceDataTypeDef",
     {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "name": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "sourceNetworkData": SourceNetworkDataTypeDef,
     },
     total=False,
 )
 
-
-class UpdateLaunchConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
         "status": LaunchStatusType,
     },
     total=False,
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
         "items": List[StagingSourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourcePropertiesTypeDef = TypedDict(
     "SourcePropertiesTypeDef",
     {
         "cpus": List[CPUTypeDef],
         "disks": List[DiskTypeDef],
         "identificationHints": IdentificationHintsTypeDef,
         "lastUpdatedDateTime": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "os": OSTypeDef,
         "ramBytes": int,
         "recommendedInstanceType": str,
+        "supportsNitroInstances": bool,
+    },
+    total=False,
+)
+
+ParticipatingResourceTypeDef = TypedDict(
+    "ParticipatingResourceTypeDef",
+    {
+        "launchStatus": LaunchStatusType,
+        "participatingResourceID": ParticipatingResourceIDTypeDef,
     },
     total=False,
 )
 
 RecoveryInstanceDataReplicationInitiationTypeDef = TypedDict(
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     {
@@ -1265,18 +1524,37 @@
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "os": OSTypeDef,
         "ramBytes": int,
     },
     total=False,
 )
 
+SourceNetworkTypeDef = TypedDict(
+    "SourceNetworkTypeDef",
+    {
+        "arn": str,
+        "cfnStackName": str,
+        "lastRecovery": RecoveryLifeCycleTypeDef,
+        "launchedVpcID": str,
+        "replicationStatus": ReplicationStatusType,
+        "replicationStatusDetails": str,
+        "sourceAccountID": str,
+        "sourceNetworkID": str,
+        "sourceRegion": str,
+        "sourceVpcID": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
@@ -1284,28 +1562,29 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
@@ -1346,30 +1625,68 @@
 
 class StartRecoveryRequestRequestTypeDef(
     _RequiredStartRecoveryRequestRequestTypeDef, _OptionalStartRecoveryRequestRequestTypeDef
 ):
     pass
 
 
-JobLogTypeDef = TypedDict(
-    "JobLogTypeDef",
+_RequiredStartSourceNetworkRecoveryRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSourceNetworkRecoveryRequestRequestTypeDef",
     {
-        "event": JobLogEventType,
-        "eventData": JobLogEventDataTypeDef,
-        "logDateTime": str,
+        "sourceNetworks": Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],
+    },
+)
+_OptionalStartSourceNetworkRecoveryRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSourceNetworkRecoveryRequestRequestTypeDef",
+    {
+        "deployAsNew": bool,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class StartSourceNetworkRecoveryRequestRequestTypeDef(
+    _RequiredStartSourceNetworkRecoveryRequestRequestTypeDef,
+    _OptionalStartSourceNetworkRecoveryRequestRequestTypeDef,
+):
+    pass
+
+
+CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[LaunchConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -1379,120 +1696,204 @@
         "lagDuration": str,
         "replicatedDisks": List[DataReplicationInfoReplicatedDiskTypeDef],
         "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
-DescribeJobsResponseTypeDef = TypedDict(
-    "DescribeJobsResponseTypeDef",
-    {
-        "items": List[JobTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFailbackLaunchResponseTypeDef = TypedDict(
-    "StartFailbackLaunchResponseTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRecoveryResponseTypeDef = TypedDict(
-    "StartRecoveryResponseTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateRecoveryInstancesResponseTypeDef = TypedDict(
-    "TerminateRecoveryInstancesResponseTypeDef",
+JobLogEventDataTypeDef = TypedDict(
+    "JobLogEventDataTypeDef",
     {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "conversionProperties": ConversionPropertiesTypeDef,
+        "conversionServerID": str,
+        "eventResourceData": EventResourceDataTypeDef,
+        "rawError": str,
+        "sourceServerID": str,
+        "targetInstanceID": str,
     },
+    total=False,
 )
 
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
         "elapsedReplicationDuration": str,
         "firstByteDateTime": str,
         "lastLaunch": LifeCycleLastLaunchTypeDef,
         "lastSeenByServiceDateTime": str,
     },
     total=False,
 )
 
+_RequiredJobTypeDef = TypedDict(
+    "_RequiredJobTypeDef",
+    {
+        "jobID": str,
+    },
+)
+_OptionalJobTypeDef = TypedDict(
+    "_OptionalJobTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": str,
+        "endDateTime": str,
+        "initiatedBy": InitiatedByType,
+        "participatingResources": List[ParticipatingResourceTypeDef],
+        "participatingServers": List[ParticipatingServerTypeDef],
+        "status": JobStatusType,
+        "tags": Dict[str, str],
+        "type": JobTypeType,
+    },
+    total=False,
+)
+
+
+class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
+    pass
+
+
 RecoveryInstanceDataReplicationInfoTypeDef = TypedDict(
     "RecoveryInstanceDataReplicationInfoTypeDef",
     {
         "dataReplicationError": RecoveryInstanceDataReplicationErrorTypeDef,
         "dataReplicationInitiation": RecoveryInstanceDataReplicationInitiationTypeDef,
         "dataReplicationState": RecoveryInstanceDataReplicationStateType,
         "etaDateTime": str,
         "lagDuration": str,
         "replicatedDisks": List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef],
         "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
-DescribeJobLogItemsResponseTypeDef = TypedDict(
-    "DescribeJobLogItemsResponseTypeDef",
+DescribeSourceNetworksResponseTypeDef = TypedDict(
+    "DescribeSourceNetworksResponseTypeDef",
     {
-        "items": List[JobLogTypeDef],
+        "items": List[SourceNetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSourceNetworkReplicationResponseTypeDef = TypedDict(
+    "StartSourceNetworkReplicationResponseTypeDef",
+    {
+        "sourceNetwork": SourceNetworkTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StopSourceNetworkReplicationResponseTypeDef = TypedDict(
+    "StopSourceNetworkReplicationResponseTypeDef",
+    {
+        "sourceNetwork": SourceNetworkTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+JobLogTypeDef = TypedDict(
+    "JobLogTypeDef",
+    {
+        "event": JobLogEventType,
+        "eventData": JobLogEventDataTypeDef,
+        "logDateTime": str,
     },
+    total=False,
 )
 
 SourceServerResponseMetadataTypeDef = TypedDict(
     "SourceServerResponseMetadataTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
+        "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
+        "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+AssociateSourceNetworkStackResponseTypeDef = TypedDict(
+    "AssociateSourceNetworkStackResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeJobsResponseTypeDef = TypedDict(
+    "DescribeJobsResponseTypeDef",
+    {
+        "items": List[JobTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartFailbackLaunchResponseTypeDef = TypedDict(
+    "StartFailbackLaunchResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartRecoveryResponseTypeDef = TypedDict(
+    "StartRecoveryResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSourceNetworkRecoveryResponseTypeDef = TypedDict(
+    "StartSourceNetworkRecoveryResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TerminateRecoveryInstancesResponseTypeDef = TypedDict(
+    "TerminateRecoveryInstancesResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecoveryInstanceTypeDef = TypedDict(
     "RecoveryInstanceTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": RecoveryInstanceDataReplicationInfoTypeDef,
         "ec2InstanceID": str,
         "ec2InstanceState": EC2InstanceStateType,
@@ -1506,48 +1907,57 @@
         "recoveryInstanceProperties": RecoveryInstancePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+DescribeJobLogItemsResponseTypeDef = TypedDict(
+    "DescribeJobLogItemsResponseTypeDef",
+    {
+        "items": List[JobLogTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateExtendedSourceServerResponseTypeDef = TypedDict(
     "CreateExtendedSourceServerResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecoveryInstancesResponseTypeDef = TypedDict(
     "DescribeRecoveryInstancesResponseTypeDef",
     {
         "items": List[RecoveryInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.pyi` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from mypy_boto3_drs.type_defs import AccountTypeDef
 
     data: AccountTypeDef = {...}
     ```
 """
 import sys
+from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataReplicationErrorStringType,
     DataReplicationInitiationStepNameType,
     DataReplicationInitiationStepStatusType,
     DataReplicationStateType,
@@ -33,133 +34,168 @@
     LaunchDispositionType,
     LaunchStatusType,
     OriginEnvironmentType,
     PITPolicyRuleUnitsType,
     RecoveryInstanceDataReplicationInitiationStepNameType,
     RecoveryInstanceDataReplicationInitiationStepStatusType,
     RecoveryInstanceDataReplicationStateType,
+    RecoveryResultType,
     RecoverySnapshotsOrderType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
     ReplicationDirectionType,
+    ReplicationStatusType,
     TargetInstanceTypeRightSizingMethodType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountTypeDef",
+    "AssociateSourceNetworkStackRequestRequestTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "LicensingTypeDef",
     "PITPolicyRuleTypeDef",
+    "CreateSourceNetworkRequestRequestTypeDef",
+    "CreateSourceNetworkResponseTypeDef",
     "DataReplicationErrorTypeDef",
     "DataReplicationInfoReplicatedDiskTypeDef",
     "DataReplicationInitiationStepTypeDef",
     "DeleteJobRequestRequestTypeDef",
+    "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
+    "DeleteSourceNetworkRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     "DescribeRecoverySnapshotsRequestFiltersTypeDef",
     "RecoverySnapshotTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
+    "DescribeSourceNetworksRequestFiltersTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
     "DisconnectRecoveryInstanceRequestRequestTypeDef",
     "DisconnectSourceServerRequestRequestTypeDef",
     "DiskTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "SourceNetworkDataTypeDef",
+    "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
+    "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
-    "LicensingTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
+    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PaginatorConfigTypeDef",
+    "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
+    "RecoveryLifeCycleTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
+    "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
     "StartFailbackLaunchRequestRequestTypeDef",
     "StartRecoveryRequestSourceServerTypeDef",
     "StartReplicationRequestRequestTypeDef",
+    "StartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
+    "StartSourceNetworkReplicationRequestRequestTypeDef",
     "StopFailbackRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
+    "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
-    "JobLogEventDataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetFailbackReplicationConfigurationResponseTypeDef",
     "ListStagingAccountsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ReverseReplicationResponseTypeDef",
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "LaunchConfigurationTemplateTypeDef",
+    "LaunchConfigurationTypeDef",
+    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
+    "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
+    "DescribeSourceNetworksRequestRequestTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
-    "JobTypeDef",
-    "LaunchConfigurationTypeDef",
-    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "EventResourceDataTypeDef",
     "LifeCycleLastLaunchTypeDef",
     "ListExtensibleSourceServersResponseTypeDef",
     "SourcePropertiesTypeDef",
+    "ParticipatingResourceTypeDef",
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     "RecoveryInstancePropertiesTypeDef",
+    "SourceNetworkTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "StartRecoveryRequestRequestTypeDef",
-    "JobLogTypeDef",
+    "StartSourceNetworkRecoveryRequestRequestTypeDef",
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DataReplicationInfoTypeDef",
-    "DescribeJobsResponseTypeDef",
-    "StartFailbackLaunchResponseTypeDef",
-    "StartRecoveryResponseTypeDef",
-    "TerminateRecoveryInstancesResponseTypeDef",
+    "JobLogEventDataTypeDef",
     "LifeCycleTypeDef",
+    "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
-    "DescribeJobLogItemsResponseTypeDef",
+    "DescribeSourceNetworksResponseTypeDef",
+    "StartSourceNetworkReplicationResponseTypeDef",
+    "StopSourceNetworkReplicationResponseTypeDef",
+    "JobLogTypeDef",
     "SourceServerResponseMetadataTypeDef",
     "SourceServerTypeDef",
+    "AssociateSourceNetworkStackResponseTypeDef",
+    "DescribeJobsResponseTypeDef",
+    "StartFailbackLaunchResponseTypeDef",
+    "StartRecoveryResponseTypeDef",
+    "StartSourceNetworkRecoveryResponseTypeDef",
+    "TerminateRecoveryInstancesResponseTypeDef",
     "RecoveryInstanceTypeDef",
+    "DescribeJobLogItemsResponseTypeDef",
     "CreateExtendedSourceServerResponseTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "StartReplicationResponseTypeDef",
     "StopReplicationResponseTypeDef",
     "DescribeRecoveryInstancesResponseTypeDef",
 )
 
@@ -167,14 +203,22 @@
     "AccountTypeDef",
     {
         "accountID": str,
     },
     total=False,
 )
 
+AssociateSourceNetworkStackRequestRequestTypeDef = TypedDict(
+    "AssociateSourceNetworkStackRequestRequestTypeDef",
+    {
+        "cfnStackName": str,
+        "sourceNetworkID": str,
+    },
+)
+
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
     total=False,
@@ -208,23 +252,20 @@
 
 class CreateExtendedSourceServerRequestRequestTypeDef(
     _RequiredCreateExtendedSourceServerRequestRequestTypeDef,
     _OptionalCreateExtendedSourceServerRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+LicensingTypeDef = TypedDict(
+    "LicensingTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "osByol": bool,
     },
+    total=False,
 )
 
 _RequiredPITPolicyRuleTypeDef = TypedDict(
     "_RequiredPITPolicyRuleTypeDef",
     {
         "interval": int,
         "retentionDuration": int,
@@ -239,14 +280,44 @@
     },
     total=False,
 )
 
 class PITPolicyRuleTypeDef(_RequiredPITPolicyRuleTypeDef, _OptionalPITPolicyRuleTypeDef):
     pass
 
+_RequiredCreateSourceNetworkRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceNetworkRequestRequestTypeDef",
+    {
+        "originAccountID": str,
+        "originRegion": str,
+        "vpcID": str,
+    },
+)
+_OptionalCreateSourceNetworkRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceNetworkRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateSourceNetworkRequestRequestTypeDef(
+    _RequiredCreateSourceNetworkRequestRequestTypeDef,
+    _OptionalCreateSourceNetworkRequestRequestTypeDef,
+):
+    pass
+
+CreateSourceNetworkResponseTypeDef = TypedDict(
+    "CreateSourceNetworkResponseTypeDef",
+    {
+        "sourceNetworkID": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataReplicationErrorTypeDef = TypedDict(
     "DataReplicationErrorTypeDef",
     {
         "error": DataReplicationErrorStringType,
         "rawError": str,
     },
     total=False,
@@ -276,45 +347,69 @@
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 
+DeleteLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "launchConfigurationTemplateID": str,
+    },
+)
+
 DeleteRecoveryInstanceRequestRequestTypeDef = TypedDict(
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
 DeleteReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 
+DeleteSourceNetworkRequestRequestTypeDef = TypedDict(
+    "DeleteSourceNetworkRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
 DeleteSourceServerRequestRequestTypeDef = TypedDict(
     "DeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -338,14 +433,33 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 DescribeRecoveryInstancesRequestFiltersTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     {
         "recoveryInstanceIDs": Sequence[str],
         "sourceServerIDs": Sequence[str],
     },
     total=False,
@@ -376,24 +490,43 @@
     },
     total=False,
 )
 
 class RecoverySnapshotTypeDef(_RequiredRecoverySnapshotTypeDef, _OptionalRecoverySnapshotTypeDef):
     pass
 
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
     total=False,
 )
 
+DescribeSourceNetworksRequestFiltersTypeDef = TypedDict(
+    "DescribeSourceNetworksRequestFiltersTypeDef",
+    {
+        "originAccountID": str,
+        "originRegion": str,
+        "sourceNetworkIDs": Sequence[str],
+    },
+    total=False,
+)
+
 DescribeSourceServersRequestFiltersTypeDef = TypedDict(
     "DescribeSourceServersRequestFiltersTypeDef",
     {
         "hardwareId": str,
         "sourceServerIDs": Sequence[str],
         "stagingAccountIDs": Sequence[str],
     },
@@ -419,21 +552,65 @@
     {
         "bytes": int,
         "deviceName": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SourceNetworkDataTypeDef = TypedDict(
+    "SourceNetworkDataTypeDef",
+    {
+        "sourceNetworkID": str,
+        "sourceVpc": str,
+        "stackName": str,
+        "targetVpc": str,
+    },
+    total=False,
+)
+
+ExportSourceNetworkCfnTemplateRequestRequestTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
+ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    {
+        "s3DestinationUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFailbackReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
+GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetFailbackReplicationConfigurationResponseTypeDef",
+    {
+        "bandwidthThrottling": int,
+        "name": str,
+        "recoveryInstanceID": str,
+        "usePrivateIP": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "GetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -461,32 +638,44 @@
         "launchStatus": LaunchStatusType,
         "recoveryInstanceID": str,
         "sourceServerID": str,
     },
     total=False,
 )
 
-LicensingTypeDef = TypedDict(
-    "LicensingTypeDef",
-    {
-        "osByol": bool,
-    },
-    total=False,
-)
-
 LifeCycleLastLaunchInitiatedTypeDef = TypedDict(
     "LifeCycleLastLaunchInitiatedTypeDef",
     {
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
     total=False,
 )
 
+_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "stagingAccountID": str,
+    },
+)
+_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
+    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+):
+    pass
+
 _RequiredListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensibleSourceServersRequestRequestTypeDef",
     {
         "stagingAccountID": str,
     },
 )
 _OptionalListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
@@ -510,14 +699,22 @@
         "arn": str,
         "hostname": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStagingAccountsRequestRequestTypeDef = TypedDict(
     "ListStagingAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -526,14 +723,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
     },
@@ -544,14 +749,32 @@
     "OSTypeDef",
     {
         "fullString": str,
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
+ParticipatingResourceIDTypeDef = TypedDict(
+    "ParticipatingResourceIDTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+    total=False,
+)
+
 RecoveryInstanceDataReplicationErrorTypeDef = TypedDict(
     "RecoveryInstanceDataReplicationErrorTypeDef",
     {
         "error": FailbackReplicationErrorType,
         "rawError": str,
     },
     total=False,
@@ -601,41 +824,70 @@
         "failbackToOriginalServer": bool,
         "firstByteDateTime": str,
         "state": FailbackStateType,
     },
     total=False,
 )
 
+RecoveryLifeCycleTypeDef = TypedDict(
+    "RecoveryLifeCycleTypeDef",
+    {
+        "apiCallDateTime": datetime,
+        "jobID": str,
+        "lastRecoveryResult": RecoveryResultType,
+    },
+    total=False,
+)
+
 ReplicationConfigurationReplicatedDiskTypeDef = TypedDict(
     "ReplicationConfigurationReplicatedDiskTypeDef",
     {
         "deviceName": str,
         "iops": int,
         "isBootDisk": bool,
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
 ReverseReplicationRequestRequestTypeDef = TypedDict(
     "ReverseReplicationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
+ReverseReplicationResponseTypeDef = TypedDict(
+    "ReverseReplicationResponseTypeDef",
+    {
+        "reversedDirectionSourceServerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": str,
         "originAvailabilityZone": str,
         "originRegion": str,
     },
@@ -696,28 +948,62 @@
 StartReplicationRequestRequestTypeDef = TypedDict(
     "StartReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
+_RequiredStartSourceNetworkRecoveryRequestNetworkEntryTypeDef = TypedDict(
+    "_RequiredStartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+_OptionalStartSourceNetworkRecoveryRequestNetworkEntryTypeDef = TypedDict(
+    "_OptionalStartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
+    {
+        "cfnStackName": str,
+    },
+    total=False,
+)
+
+class StartSourceNetworkRecoveryRequestNetworkEntryTypeDef(
+    _RequiredStartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    _OptionalStartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+):
+    pass
+
+StartSourceNetworkReplicationRequestRequestTypeDef = TypedDict(
+    "StartSourceNetworkReplicationRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
 StopFailbackRequestRequestTypeDef = TypedDict(
     "StopFailbackRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
 StopReplicationRequestRequestTypeDef = TypedDict(
     "StopReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
+StopSourceNetworkReplicationRequestRequestTypeDef = TypedDict(
+    "StopSourceNetworkReplicationRequestRequestTypeDef",
+    {
+        "sourceNetworkID": str,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -755,68 +1041,117 @@
 
 class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-JobLogEventDataTypeDef = TypedDict(
-    "JobLogEventDataTypeDef",
+ListStagingAccountsResponseTypeDef = TypedDict(
+    "ListStagingAccountsResponseTypeDef",
     {
-        "conversionProperties": ConversionPropertiesTypeDef,
-        "conversionServerID": str,
-        "rawError": str,
-        "sourceServerID": str,
-        "targetInstanceID": str,
+        "accounts": List[AccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "tags": Mapping[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+LaunchConfigurationTemplateTypeDef = TypedDict(
+    "LaunchConfigurationTemplateTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "arn": str,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchConfigurationTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "tags": Dict[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
+    total=False,
 )
 
-GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetFailbackReplicationConfigurationResponseTypeDef",
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
     {
-        "bandwidthThrottling": int,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
         "name": str,
-        "recoveryInstanceID": str,
-        "usePrivateIP": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListStagingAccountsResponseTypeDef = TypedDict(
-    "ListStagingAccountsResponseTypeDef",
+_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "accounts": List[AccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sourceServerID": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "name": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
+    total=False,
 )
 
-ReverseReplicationResponseTypeDef = TypedDict(
-    "ReverseReplicationResponseTypeDef",
+class UpdateLaunchConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
-        "reversedDirectionSourceServerArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "launchConfigurationTemplateID": str,
     },
 )
+_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
+class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+):
+    pass
 
 _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "associateDefaultSecurityGroup": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
@@ -830,14 +1165,15 @@
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
     },
 )
 _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
+        "autoReplicateNewDisks": bool,
         "ebsEncryptionKeyArn": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
@@ -847,43 +1183,45 @@
     pass
 
 ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "pitPolicy": List[PITPolicyRuleTypeDef],
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
     "_RequiredReplicationConfigurationTemplateTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 _OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
     "_OptionalReplicationConfigurationTemplateTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "pitPolicy": List[PITPolicyRuleTypeDef],
@@ -910,14 +1248,15 @@
     },
 )
 _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "pitPolicy": Sequence[PITPolicyRuleTypeDef],
@@ -942,76 +1281,19 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "stagingAccountID": str,
-    },
-)
-_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
-    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-):
-    pass
-
-ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1022,15 +1304,15 @@
     total=False,
 )
 
 DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     {
         "filters": DescribeRecoveryInstancesRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeRecoveryInstancesRequestRequestTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     {
@@ -1048,15 +1330,15 @@
     },
 )
 _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = TypedDict(
     "_OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     {
         "filters": DescribeRecoverySnapshotsRequestFiltersTypeDef,
         "order": RecoverySnapshotsOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(
     _RequiredDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
@@ -1087,130 +1369,103 @@
     pass
 
 DescribeRecoverySnapshotsResponseTypeDef = TypedDict(
     "DescribeRecoverySnapshotsResponseTypeDef",
     {
         "items": List[RecoverySnapshotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
-    "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
+DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef = TypedDict(
+    "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     {
-        "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "filters": DescribeSourceNetworksRequestFiltersTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeSourceServersRequestRequestTypeDef = TypedDict(
-    "DescribeSourceServersRequestRequestTypeDef",
+DescribeSourceNetworksRequestRequestTypeDef = TypedDict(
+    "DescribeSourceNetworksRequestRequestTypeDef",
     {
-        "filters": DescribeSourceServersRequestFiltersTypeDef,
+        "filters": DescribeSourceNetworksRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
+    "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
-        "arn": str,
-        "creationDateTime": str,
-        "endDateTime": str,
-        "initiatedBy": InitiatedByType,
-        "participatingServers": List[ParticipatingServerTypeDef],
-        "status": JobStatusType,
-        "tags": Dict[str, str],
-        "type": JobTypeType,
+        "filters": DescribeSourceServersRequestFiltersTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
+DescribeSourceServersRequestRequestTypeDef = TypedDict(
+    "DescribeSourceServersRequestRequestTypeDef",
     {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "name": str,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filters": DescribeSourceServersRequestFiltersTypeDef,
+        "maxResults": int,
+        "nextToken": str,
     },
+    total=False,
 )
 
-_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
+EventResourceDataTypeDef = TypedDict(
+    "EventResourceDataTypeDef",
     {
-        "sourceServerID": str,
-    },
-)
-_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
-    {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "name": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "sourceNetworkData": SourceNetworkDataTypeDef,
     },
     total=False,
 )
 
-class UpdateLaunchConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
-):
-    pass
-
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
         "status": LaunchStatusType,
     },
     total=False,
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
         "items": List[StagingSourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourcePropertiesTypeDef = TypedDict(
     "SourcePropertiesTypeDef",
     {
         "cpus": List[CPUTypeDef],
         "disks": List[DiskTypeDef],
         "identificationHints": IdentificationHintsTypeDef,
         "lastUpdatedDateTime": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "os": OSTypeDef,
         "ramBytes": int,
         "recommendedInstanceType": str,
+        "supportsNitroInstances": bool,
+    },
+    total=False,
+)
+
+ParticipatingResourceTypeDef = TypedDict(
+    "ParticipatingResourceTypeDef",
+    {
+        "launchStatus": LaunchStatusType,
+        "participatingResourceID": ParticipatingResourceIDTypeDef,
     },
     total=False,
 )
 
 RecoveryInstanceDataReplicationInitiationTypeDef = TypedDict(
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     {
@@ -1230,18 +1485,37 @@
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "os": OSTypeDef,
         "ramBytes": int,
     },
     total=False,
 )
 
+SourceNetworkTypeDef = TypedDict(
+    "SourceNetworkTypeDef",
+    {
+        "arn": str,
+        "cfnStackName": str,
+        "lastRecovery": RecoveryLifeCycleTypeDef,
+        "launchedVpcID": str,
+        "replicationStatus": ReplicationStatusType,
+        "replicationStatusDetails": str,
+        "sourceAccountID": str,
+        "sourceNetworkID": str,
+        "sourceRegion": str,
+        "sourceVpcID": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
@@ -1249,28 +1523,29 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
@@ -1307,30 +1582,66 @@
 )
 
 class StartRecoveryRequestRequestTypeDef(
     _RequiredStartRecoveryRequestRequestTypeDef, _OptionalStartRecoveryRequestRequestTypeDef
 ):
     pass
 
-JobLogTypeDef = TypedDict(
-    "JobLogTypeDef",
+_RequiredStartSourceNetworkRecoveryRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSourceNetworkRecoveryRequestRequestTypeDef",
     {
-        "event": JobLogEventType,
-        "eventData": JobLogEventDataTypeDef,
-        "logDateTime": str,
+        "sourceNetworks": Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],
+    },
+)
+_OptionalStartSourceNetworkRecoveryRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSourceNetworkRecoveryRequestRequestTypeDef",
+    {
+        "deployAsNew": bool,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class StartSourceNetworkRecoveryRequestRequestTypeDef(
+    _RequiredStartSourceNetworkRecoveryRequestRequestTypeDef,
+    _OptionalStartSourceNetworkRecoveryRequestRequestTypeDef,
+):
+    pass
+
+CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[LaunchConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -1340,120 +1651,202 @@
         "lagDuration": str,
         "replicatedDisks": List[DataReplicationInfoReplicatedDiskTypeDef],
         "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
-DescribeJobsResponseTypeDef = TypedDict(
-    "DescribeJobsResponseTypeDef",
-    {
-        "items": List[JobTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFailbackLaunchResponseTypeDef = TypedDict(
-    "StartFailbackLaunchResponseTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRecoveryResponseTypeDef = TypedDict(
-    "StartRecoveryResponseTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateRecoveryInstancesResponseTypeDef = TypedDict(
-    "TerminateRecoveryInstancesResponseTypeDef",
+JobLogEventDataTypeDef = TypedDict(
+    "JobLogEventDataTypeDef",
     {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "conversionProperties": ConversionPropertiesTypeDef,
+        "conversionServerID": str,
+        "eventResourceData": EventResourceDataTypeDef,
+        "rawError": str,
+        "sourceServerID": str,
+        "targetInstanceID": str,
     },
+    total=False,
 )
 
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
         "elapsedReplicationDuration": str,
         "firstByteDateTime": str,
         "lastLaunch": LifeCycleLastLaunchTypeDef,
         "lastSeenByServiceDateTime": str,
     },
     total=False,
 )
 
+_RequiredJobTypeDef = TypedDict(
+    "_RequiredJobTypeDef",
+    {
+        "jobID": str,
+    },
+)
+_OptionalJobTypeDef = TypedDict(
+    "_OptionalJobTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": str,
+        "endDateTime": str,
+        "initiatedBy": InitiatedByType,
+        "participatingResources": List[ParticipatingResourceTypeDef],
+        "participatingServers": List[ParticipatingServerTypeDef],
+        "status": JobStatusType,
+        "tags": Dict[str, str],
+        "type": JobTypeType,
+    },
+    total=False,
+)
+
+class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
+    pass
+
 RecoveryInstanceDataReplicationInfoTypeDef = TypedDict(
     "RecoveryInstanceDataReplicationInfoTypeDef",
     {
         "dataReplicationError": RecoveryInstanceDataReplicationErrorTypeDef,
         "dataReplicationInitiation": RecoveryInstanceDataReplicationInitiationTypeDef,
         "dataReplicationState": RecoveryInstanceDataReplicationStateType,
         "etaDateTime": str,
         "lagDuration": str,
         "replicatedDisks": List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef],
         "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
-DescribeJobLogItemsResponseTypeDef = TypedDict(
-    "DescribeJobLogItemsResponseTypeDef",
+DescribeSourceNetworksResponseTypeDef = TypedDict(
+    "DescribeSourceNetworksResponseTypeDef",
     {
-        "items": List[JobLogTypeDef],
+        "items": List[SourceNetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSourceNetworkReplicationResponseTypeDef = TypedDict(
+    "StartSourceNetworkReplicationResponseTypeDef",
+    {
+        "sourceNetwork": SourceNetworkTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StopSourceNetworkReplicationResponseTypeDef = TypedDict(
+    "StopSourceNetworkReplicationResponseTypeDef",
+    {
+        "sourceNetwork": SourceNetworkTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+JobLogTypeDef = TypedDict(
+    "JobLogTypeDef",
+    {
+        "event": JobLogEventType,
+        "eventData": JobLogEventDataTypeDef,
+        "logDateTime": str,
+    },
+    total=False,
+)
+
 SourceServerResponseMetadataTypeDef = TypedDict(
     "SourceServerResponseMetadataTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
+        "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
+        "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+AssociateSourceNetworkStackResponseTypeDef = TypedDict(
+    "AssociateSourceNetworkStackResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeJobsResponseTypeDef = TypedDict(
+    "DescribeJobsResponseTypeDef",
+    {
+        "items": List[JobTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartFailbackLaunchResponseTypeDef = TypedDict(
+    "StartFailbackLaunchResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartRecoveryResponseTypeDef = TypedDict(
+    "StartRecoveryResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSourceNetworkRecoveryResponseTypeDef = TypedDict(
+    "StartSourceNetworkRecoveryResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TerminateRecoveryInstancesResponseTypeDef = TypedDict(
+    "TerminateRecoveryInstancesResponseTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecoveryInstanceTypeDef = TypedDict(
     "RecoveryInstanceTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": RecoveryInstanceDataReplicationInfoTypeDef,
         "ec2InstanceID": str,
         "ec2InstanceState": EC2InstanceStateType,
@@ -1467,48 +1860,57 @@
         "recoveryInstanceProperties": RecoveryInstancePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+DescribeJobLogItemsResponseTypeDef = TypedDict(
+    "DescribeJobLogItemsResponseTypeDef",
+    {
+        "items": List[JobLogTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateExtendedSourceServerResponseTypeDef = TypedDict(
     "CreateExtendedSourceServerResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecoveryInstancesResponseTypeDef = TypedDict(
     "DescribeRecoveryInstancesResponseTypeDef",
     {
         "items": List[RecoveryInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.26.80
-Summary: Type annotations for boto3.drs 1.26.80 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.drs 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-drs"></a>
 
 # mypy-boto3-drs
 
 [![PyPI - mypy-boto3-drs](https://img.shields.io/pypi/v/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,39 +280,47 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_drs import drsClient
 from mypy_boto3_drs.paginator import (
     DescribeJobLogItemsPaginator,
     DescribeJobsPaginator,
+    DescribeLaunchConfigurationTemplatesPaginator,
     DescribeRecoveryInstancesPaginator,
     DescribeRecoverySnapshotsPaginator,
     DescribeReplicationConfigurationTemplatesPaginator,
+    DescribeSourceNetworksPaginator,
     DescribeSourceServersPaginator,
     ListExtensibleSourceServersPaginator,
     ListStagingAccountsPaginator,
 )
 
 client: drsClient = Session().client("drs")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_job_log_items_paginator: DescribeJobLogItemsPaginator = client.get_paginator(
     "describe_job_log_items"
 )
 describe_jobs_paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
+describe_launch_configuration_templates_paginator: DescribeLaunchConfigurationTemplatesPaginator = (
+    client.get_paginator("describe_launch_configuration_templates")
+)
 describe_recovery_instances_paginator: DescribeRecoveryInstancesPaginator = client.get_paginator(
     "describe_recovery_instances"
 )
 describe_recovery_snapshots_paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator(
     "describe_recovery_snapshots"
 )
 describe_replication_configuration_templates_paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator(
     "describe_replication_configuration_templates"
 )
+describe_source_networks_paginator: DescribeSourceNetworksPaginator = client.get_paginator(
+    "describe_source_networks"
+)
 describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator(
     "describe_source_servers"
 )
 list_extensible_source_servers_paginator: ListExtensibleSourceServersPaginator = (
     client.get_paginator("list_extensible_source_servers")
 )
 list_staging_accounts_paginator: ListStagingAccountsPaginator = client.get_paginator(
@@ -331,17 +339,19 @@
 from mypy_boto3_drs.literals import (
     DataReplicationErrorStringType,
     DataReplicationInitiationStepNameType,
     DataReplicationInitiationStepStatusType,
     DataReplicationStateType,
     DescribeJobLogItemsPaginatorName,
     DescribeJobsPaginatorName,
+    DescribeLaunchConfigurationTemplatesPaginatorName,
     DescribeRecoveryInstancesPaginatorName,
     DescribeRecoverySnapshotsPaginatorName,
     DescribeReplicationConfigurationTemplatesPaginatorName,
+    DescribeSourceNetworksPaginatorName,
     DescribeSourceServersPaginatorName,
     EC2InstanceStateType,
     ExtensionStatusType,
     FailbackLaunchTypeType,
     FailbackReplicationErrorType,
     FailbackStateType,
     InitiatedByType,
@@ -355,20 +365,22 @@
     ListExtensibleSourceServersPaginatorName,
     ListStagingAccountsPaginatorName,
     OriginEnvironmentType,
     PITPolicyRuleUnitsType,
     RecoveryInstanceDataReplicationInitiationStepNameType,
     RecoveryInstanceDataReplicationInitiationStepStatusType,
     RecoveryInstanceDataReplicationStateType,
+    RecoveryResultType,
     RecoverySnapshotsOrderType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
     ReplicationConfigurationEbsEncryptionType,
     ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
     ReplicationDirectionType,
+    ReplicationStatusType,
     TargetInstanceTypeRightSizingMethodType,
     drsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -384,117 +396,150 @@
 
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
+    AssociateSourceNetworkStackRequestRequestTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    LicensingTypeDef,
     PITPolicyRuleTypeDef,
+    CreateSourceNetworkRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
+    DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
+    DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
+    EmptyResponseMetadataTypeDef,
+    SourceNetworkDataTypeDef,
+    ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
-    LicensingTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PaginatorConfigTypeDef,
+    ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
+    RecoveryLifeCycleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
+    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
+    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
+    StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
+    StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
+    StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
-    JobLogEventDataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReverseReplicationResponseTypeDef,
+    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
+    DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
+    DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
-    JobTypeDef,
-    LaunchConfigurationTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
+    EventResourceDataTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
+    ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
+    SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
-    JobLogTypeDef,
+    StartSourceNetworkRecoveryRequestRequestTypeDef,
+    CreateLaunchConfigurationTemplateResponseTypeDef,
+    DescribeLaunchConfigurationTemplatesResponseTypeDef,
+    UpdateLaunchConfigurationTemplateResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DataReplicationInfoTypeDef,
-    DescribeJobsResponseTypeDef,
-    StartFailbackLaunchResponseTypeDef,
-    StartRecoveryResponseTypeDef,
-    TerminateRecoveryInstancesResponseTypeDef,
+    JobLogEventDataTypeDef,
     LifeCycleTypeDef,
+    JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
-    DescribeJobLogItemsResponseTypeDef,
+    DescribeSourceNetworksResponseTypeDef,
+    StartSourceNetworkReplicationResponseTypeDef,
+    StopSourceNetworkReplicationResponseTypeDef,
+    JobLogTypeDef,
     SourceServerResponseMetadataTypeDef,
     SourceServerTypeDef,
+    AssociateSourceNetworkStackResponseTypeDef,
+    DescribeJobsResponseTypeDef,
+    StartFailbackLaunchResponseTypeDef,
+    StartRecoveryResponseTypeDef,
+    StartSourceNetworkRecoveryResponseTypeDef,
+    TerminateRecoveryInstancesResponseTypeDef,
     RecoveryInstanceTypeDef,
+    DescribeJobLogItemsResponseTypeDef,
     CreateExtendedSourceServerResponseTypeDef,
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
@@ -506,42 +551,42 @@
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

### Comparing `mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy-boto3-drs-1.27.0/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.80/setup.py` & `mypy-boto3-drs-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-drs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.26.80",
+    version="1.27.0",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.drs 1.26.80 service generated with mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.drs 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/",
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


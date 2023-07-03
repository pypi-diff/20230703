# Comparing `tmp/mypy-boto3-elasticache-1.26.4.tar.gz` & `tmp/mypy-boto3-elasticache-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.26.4.tar", last modified: Mon Nov  7 20:50:35 2022, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.27.0.tar", last modified: Mon Jul  3 19:50:43 2023, max compression
```

## Comparing `mypy-boto3-elasticache-1.26.4.tar` & `mypy-boto3-elasticache-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    27123 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25672 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    67591 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    67498 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13089 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13087 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22660 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    22641 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    85176 2022-11-07 20:49:47.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    85109 2022-11-07 20:49:46.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    27123 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-07 20:49:43.000000 mypy-boto3-elasticache-1.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.423196 mypy-boto3-elasticache-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-03 19:50:43.423196 mypy-boto3-elasticache-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25770 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.419196 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68059 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-07-03 19:37:13.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-07-03 19:37:13.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86384 2023-07-03 19:37:15.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86317 2023-07-03 19:37:15.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.423196 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-03 19:50:43.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 19:50:43.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:43.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:50:43.000000 mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:43.423196 mypy-boto3-elasticache-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:37:12.000000 mypy-boto3-elasticache-1.27.0/setup.py
```

### Comparing `mypy-boto3-elasticache-1.26.4/LICENSE` & `mypy-boto3-elasticache-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-elasticache-1.26.4/PKG-INFO` & `mypy-boto3-elasticache-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.26.4
-Summary: Type annotations for boto3.ElastiCache 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElastiCache 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-elasticache"></a>
 
 # mypy-boto3-elasticache
 
 [![PyPI - mypy-boto3-elasticache](https://img.shields.io/pypi/v/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -402,14 +403,15 @@
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AuthenticationTypeType,
     AutomaticFailoverStatusType,
     CacheClusterAvailableWaiterName,
     CacheClusterDeletedWaiterName,
     ChangeTypeType,
+    ClusterModeType,
     DataTieringStatusType,
     DescribeCacheClustersPaginatorName,
     DescribeCacheEngineVersionsPaginatorName,
     DescribeCacheParameterGroupsPaginatorName,
     DescribeCacheParametersPaginatorName,
     DescribeCacheSecurityGroupsPaginatorName,
     DescribeCacheSubnetGroupsPaginatorName,
@@ -421,14 +423,15 @@
     DescribeReservedCacheNodesPaginatorName,
     DescribeServiceUpdatesPaginatorName,
     DescribeSnapshotsPaginatorName,
     DescribeUpdateActionsPaginatorName,
     DescribeUserGroupsPaginatorName,
     DescribeUsersPaginatorName,
     DestinationTypeType,
+    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
@@ -438,14 +441,15 @@
     ReplicationGroupAvailableWaiterName,
     ReplicationGroupDeletedWaiterName,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SlaMetType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
     ElastiCacheServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
@@ -462,29 +466,31 @@
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
     CacheSecurityGroupMembershipTypeDef,
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
@@ -496,74 +502,88 @@
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
-    ModifyUserMessageRequestTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
+    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
+    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
-    CreateUserMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
-    EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
+    CreateUserMessageRequestTypeDef,
+    ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
@@ -573,29 +593,14 @@
     IncreaseReplicaCountMessageRequestTypeDef,
     NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
@@ -682,42 +687,42 @@
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

### Comparing `mypy-boto3-elasticache-1.26.4/README.md` & `mypy-boto3-elasticache-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elasticache"></a>
 
 # mypy-boto3-elasticache
 
 [![PyPI - mypy-boto3-elasticache](https://img.shields.io/pypi/v/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,14 +371,15 @@
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AuthenticationTypeType,
     AutomaticFailoverStatusType,
     CacheClusterAvailableWaiterName,
     CacheClusterDeletedWaiterName,
     ChangeTypeType,
+    ClusterModeType,
     DataTieringStatusType,
     DescribeCacheClustersPaginatorName,
     DescribeCacheEngineVersionsPaginatorName,
     DescribeCacheParameterGroupsPaginatorName,
     DescribeCacheParametersPaginatorName,
     DescribeCacheSecurityGroupsPaginatorName,
     DescribeCacheSubnetGroupsPaginatorName,
@@ -390,14 +391,15 @@
     DescribeReservedCacheNodesPaginatorName,
     DescribeServiceUpdatesPaginatorName,
     DescribeSnapshotsPaginatorName,
     DescribeUpdateActionsPaginatorName,
     DescribeUserGroupsPaginatorName,
     DescribeUsersPaginatorName,
     DestinationTypeType,
+    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
@@ -407,14 +409,15 @@
     ReplicationGroupAvailableWaiterName,
     ReplicationGroupDeletedWaiterName,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SlaMetType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
     ElastiCacheServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
@@ -431,29 +434,31 @@
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
     CacheSecurityGroupMembershipTypeDef,
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
@@ -465,74 +470,88 @@
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
-    ModifyUserMessageRequestTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
+    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
+    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
-    CreateUserMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
-    EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
+    CreateUserMessageRequestTypeDef,
+    ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
@@ -542,29 +561,14 @@
     IncreaseReplicaCountMessageRequestTypeDef,
     NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
@@ -651,42 +655,42 @@
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

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.26.4\nVersion:         1.26.4\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.4")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
+    ClusterModeType,
     IpDiscoveryType,
     NetworkTypeType,
     OutpostModeType,
     ServiceUpdateStatusType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 from .paginator import (
     DescribeCacheClustersPaginator,
     DescribeCacheEngineVersionsPaginator,
     DescribeCacheParameterGroupsPaginator,
     DescribeCacheParametersPaginator,
@@ -46,14 +48,15 @@
     DescribeSnapshotsPaginator,
     DescribeUpdateActionsPaginator,
     DescribeUserGroupsPaginator,
     DescribeUsersPaginator,
 )
 from .type_defs import (
     AllowedNodeTypeModificationsMessageTypeDef,
+    AuthenticationModeTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheClusterMessageTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheParameterGroupDetailsTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CacheSecurityGroupMessageTypeDef,
@@ -451,15 +454,17 @@
         TransitEncryptionEnabled: bool = ...,
         AtRestEncryptionEnabled: bool = ...,
         KmsKeyId: str = ...,
         UserGroupIds: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         DataTieringEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
+        TransitEncryptionMode: TransitEncryptionModeType = ...,
+        ClusterMode: ClusterModeType = ...
     ) -> CreateReplicationGroupResultTypeDef:
         """
         Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
         replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_replication_group)
@@ -487,15 +492,16 @@
         *,
         UserId: str,
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        AuthenticationMode: AuthenticationModeTypeDef = ...
     ) -> UserResponseMetadataTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user)
         """
@@ -590,15 +596,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_cache_subnet_group)
         """
 
     def delete_global_replication_group(
         self, *, GlobalReplicationGroupId: str, RetainPrimaryReplicationGroup: bool
     ) -> DeleteGlobalReplicationGroupResultTypeDef:
         """
-        Deleting a Global datastore is a two-step process * First, you must
+        Deleting a Global datastore is a two-step process: * First, you must
         DisassociateGlobalReplicationGroup to remove the secondary clusters in the
         Global datastore.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_global_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_global_replication_group)
         """
 
@@ -1083,15 +1089,18 @@
         CacheNodeType: str = ...,
         AuthToken: str = ...,
         AuthTokenUpdateStrategy: AuthTokenUpdateStrategyTypeType = ...,
         UserGroupIdsToAdd: Sequence[str] = ...,
         UserGroupIdsToRemove: Sequence[str] = ...,
         RemoveUserGroups: bool = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
+        TransitEncryptionEnabled: bool = ...,
+        TransitEncryptionMode: TransitEncryptionModeType = ...,
+        ClusterMode: ClusterModeType = ...
     ) -> ModifyReplicationGroupResultTypeDef:
         """
         Modifies the settings for a replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_replication_group)
         """
@@ -1117,15 +1126,16 @@
     def modify_user(
         self,
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
-        NoPasswordRequired: bool = ...
+        NoPasswordRequired: bool = ...,
+        AuthenticationMode: AuthenticationModeTypeDef = ...
     ) -> UserResponseMetadataTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user)
         """
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
+    ClusterModeType,
     IpDiscoveryType,
     NetworkTypeType,
     OutpostModeType,
     ServiceUpdateStatusType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 from .paginator import (
     DescribeCacheClustersPaginator,
     DescribeCacheEngineVersionsPaginator,
     DescribeCacheParameterGroupsPaginator,
     DescribeCacheParametersPaginator,
@@ -46,14 +48,15 @@
     DescribeSnapshotsPaginator,
     DescribeUpdateActionsPaginator,
     DescribeUserGroupsPaginator,
     DescribeUsersPaginator,
 )
 from .type_defs import (
     AllowedNodeTypeModificationsMessageTypeDef,
+    AuthenticationModeTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheClusterMessageTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheParameterGroupDetailsTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CacheSecurityGroupMessageTypeDef,
@@ -433,15 +436,17 @@
         TransitEncryptionEnabled: bool = ...,
         AtRestEncryptionEnabled: bool = ...,
         KmsKeyId: str = ...,
         UserGroupIds: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         DataTieringEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
+        TransitEncryptionMode: TransitEncryptionModeType = ...,
+        ClusterMode: ClusterModeType = ...
     ) -> CreateReplicationGroupResultTypeDef:
         """
         Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
         replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_replication_group)
@@ -467,15 +472,16 @@
         *,
         UserId: str,
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        AuthenticationMode: AuthenticationModeTypeDef = ...
     ) -> UserResponseMetadataTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user)
         """
@@ -562,15 +568,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_cache_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_cache_subnet_group)
         """
     def delete_global_replication_group(
         self, *, GlobalReplicationGroupId: str, RetainPrimaryReplicationGroup: bool
     ) -> DeleteGlobalReplicationGroupResultTypeDef:
         """
-        Deleting a Global datastore is a two-step process * First, you must
+        Deleting a Global datastore is a two-step process: * First, you must
         DisassociateGlobalReplicationGroup to remove the secondary clusters in the
         Global datastore.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_global_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_global_replication_group)
         """
     def delete_replication_group(
@@ -1022,15 +1028,18 @@
         CacheNodeType: str = ...,
         AuthToken: str = ...,
         AuthTokenUpdateStrategy: AuthTokenUpdateStrategyTypeType = ...,
         UserGroupIdsToAdd: Sequence[str] = ...,
         UserGroupIdsToRemove: Sequence[str] = ...,
         RemoveUserGroups: bool = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
+        TransitEncryptionEnabled: bool = ...,
+        TransitEncryptionMode: TransitEncryptionModeType = ...,
+        ClusterMode: ClusterModeType = ...
     ) -> ModifyReplicationGroupResultTypeDef:
         """
         Modifies the settings for a replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_replication_group)
         """
@@ -1054,15 +1063,16 @@
     def modify_user(
         self,
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
-        NoPasswordRequired: bool = ...
+        NoPasswordRequired: bool = ...,
+        AuthenticationMode: AuthenticationModeTypeDef = ...
     ) -> UserResponseMetadataTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user)
         """
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AZModeType",
     "AuthTokenUpdateStatusType",
     "AuthTokenUpdateStrategyTypeType",
     "AuthenticationTypeType",
     "AutomaticFailoverStatusType",
     "CacheClusterAvailableWaiterName",
     "CacheClusterDeletedWaiterName",
     "ChangeTypeType",
+    "ClusterModeType",
     "DataTieringStatusType",
     "DescribeCacheClustersPaginatorName",
     "DescribeCacheEngineVersionsPaginatorName",
     "DescribeCacheParameterGroupsPaginatorName",
     "DescribeCacheParametersPaginatorName",
     "DescribeCacheSecurityGroupsPaginatorName",
     "DescribeCacheSubnetGroupsPaginatorName",
@@ -43,14 +43,15 @@
     "DescribeReservedCacheNodesPaginatorName",
     "DescribeServiceUpdatesPaginatorName",
     "DescribeSnapshotsPaginatorName",
     "DescribeUpdateActionsPaginatorName",
     "DescribeUserGroupsPaginatorName",
     "DescribeUsersPaginatorName",
     "DestinationTypeType",
+    "InputAuthenticationTypeType",
     "IpDiscoveryType",
     "LogDeliveryConfigurationStatusType",
     "LogFormatType",
     "LogTypeType",
     "MultiAZStatusType",
     "NetworkTypeType",
     "NodeUpdateInitiatedByType",
@@ -60,32 +61,33 @@
     "ReplicationGroupAvailableWaiterName",
     "ReplicationGroupDeletedWaiterName",
     "ServiceUpdateSeverityType",
     "ServiceUpdateStatusType",
     "ServiceUpdateTypeType",
     "SlaMetType",
     "SourceTypeType",
+    "TransitEncryptionModeType",
     "UpdateActionStatusType",
     "ElastiCacheServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AZModeType = Literal["cross-az", "single-az"]
 AuthTokenUpdateStatusType = Literal["ROTATING", "SETTING"]
 AuthTokenUpdateStrategyTypeType = Literal["DELETE", "ROTATE", "SET"]
-AuthenticationTypeType = Literal["no-password", "password"]
+AuthenticationTypeType = Literal["iam", "no-password", "password"]
 AutomaticFailoverStatusType = Literal["disabled", "disabling", "enabled", "enabling"]
 CacheClusterAvailableWaiterName = Literal["cache_cluster_available"]
 CacheClusterDeletedWaiterName = Literal["cache_cluster_deleted"]
 ChangeTypeType = Literal["immediate", "requires-reboot"]
+ClusterModeType = Literal["compatible", "disabled", "enabled"]
 DataTieringStatusType = Literal["disabled", "enabled"]
 DescribeCacheClustersPaginatorName = Literal["describe_cache_clusters"]
 DescribeCacheEngineVersionsPaginatorName = Literal["describe_cache_engine_versions"]
 DescribeCacheParameterGroupsPaginatorName = Literal["describe_cache_parameter_groups"]
 DescribeCacheParametersPaginatorName = Literal["describe_cache_parameters"]
 DescribeCacheSecurityGroupsPaginatorName = Literal["describe_cache_security_groups"]
 DescribeCacheSubnetGroupsPaginatorName = Literal["describe_cache_subnet_groups"]
@@ -99,14 +101,15 @@
 DescribeReservedCacheNodesPaginatorName = Literal["describe_reserved_cache_nodes"]
 DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
 DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
 DescribeUpdateActionsPaginatorName = Literal["describe_update_actions"]
 DescribeUserGroupsPaginatorName = Literal["describe_user_groups"]
 DescribeUsersPaginatorName = Literal["describe_users"]
 DestinationTypeType = Literal["cloudwatch-logs", "kinesis-firehose"]
+InputAuthenticationTypeType = Literal["iam", "no-password-required", "password"]
 IpDiscoveryType = Literal["ipv4", "ipv6"]
 LogDeliveryConfigurationStatusType = Literal[
     "active", "disabling", "enabling", "error", "modifying"
 ]
 LogFormatType = Literal["json", "text"]
 LogTypeType = Literal["engine-log", "slow-log"]
 MultiAZStatusType = Literal["disabled", "enabled"]
@@ -128,14 +131,15 @@
     "cache-parameter-group",
     "cache-security-group",
     "cache-subnet-group",
     "replication-group",
     "user",
     "user-group",
 ]
+TransitEncryptionModeType = Literal["preferred", "required"]
 UpdateActionStatusType = Literal[
     "complete",
     "in-progress",
     "not-applicable",
     "not-applied",
     "scheduled",
     "scheduling",
@@ -155,23 +159,25 @@
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
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -181,30 +187,35 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
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
+    "codecatalyst",
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
@@ -230,14 +241,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -282,51 +294,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
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
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -339,14 +357,15 @@
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
@@ -358,28 +377,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -388,14 +414,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -406,55 +433,64 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
@@ -504,21 +540,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AZModeType",
     "AuthTokenUpdateStatusType",
     "AuthTokenUpdateStrategyTypeType",
     "AuthenticationTypeType",
     "AutomaticFailoverStatusType",
     "CacheClusterAvailableWaiterName",
     "CacheClusterDeletedWaiterName",
     "ChangeTypeType",
+    "ClusterModeType",
     "DataTieringStatusType",
     "DescribeCacheClustersPaginatorName",
     "DescribeCacheEngineVersionsPaginatorName",
     "DescribeCacheParameterGroupsPaginatorName",
     "DescribeCacheParametersPaginatorName",
     "DescribeCacheSecurityGroupsPaginatorName",
     "DescribeCacheSubnetGroupsPaginatorName",
@@ -42,14 +44,15 @@
     "DescribeReservedCacheNodesPaginatorName",
     "DescribeServiceUpdatesPaginatorName",
     "DescribeSnapshotsPaginatorName",
     "DescribeUpdateActionsPaginatorName",
     "DescribeUserGroupsPaginatorName",
     "DescribeUsersPaginatorName",
     "DestinationTypeType",
+    "InputAuthenticationTypeType",
     "IpDiscoveryType",
     "LogDeliveryConfigurationStatusType",
     "LogFormatType",
     "LogTypeType",
     "MultiAZStatusType",
     "NetworkTypeType",
     "NodeUpdateInitiatedByType",
@@ -59,31 +62,34 @@
     "ReplicationGroupAvailableWaiterName",
     "ReplicationGroupDeletedWaiterName",
     "ServiceUpdateSeverityType",
     "ServiceUpdateStatusType",
     "ServiceUpdateTypeType",
     "SlaMetType",
     "SourceTypeType",
+    "TransitEncryptionModeType",
     "UpdateActionStatusType",
     "ElastiCacheServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AZModeType = Literal["cross-az", "single-az"]
 AuthTokenUpdateStatusType = Literal["ROTATING", "SETTING"]
 AuthTokenUpdateStrategyTypeType = Literal["DELETE", "ROTATE", "SET"]
-AuthenticationTypeType = Literal["no-password", "password"]
+AuthenticationTypeType = Literal["iam", "no-password", "password"]
 AutomaticFailoverStatusType = Literal["disabled", "disabling", "enabled", "enabling"]
 CacheClusterAvailableWaiterName = Literal["cache_cluster_available"]
 CacheClusterDeletedWaiterName = Literal["cache_cluster_deleted"]
 ChangeTypeType = Literal["immediate", "requires-reboot"]
+ClusterModeType = Literal["compatible", "disabled", "enabled"]
 DataTieringStatusType = Literal["disabled", "enabled"]
 DescribeCacheClustersPaginatorName = Literal["describe_cache_clusters"]
 DescribeCacheEngineVersionsPaginatorName = Literal["describe_cache_engine_versions"]
 DescribeCacheParameterGroupsPaginatorName = Literal["describe_cache_parameter_groups"]
 DescribeCacheParametersPaginatorName = Literal["describe_cache_parameters"]
 DescribeCacheSecurityGroupsPaginatorName = Literal["describe_cache_security_groups"]
 DescribeCacheSubnetGroupsPaginatorName = Literal["describe_cache_subnet_groups"]
@@ -97,14 +103,15 @@
 DescribeReservedCacheNodesPaginatorName = Literal["describe_reserved_cache_nodes"]
 DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
 DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
 DescribeUpdateActionsPaginatorName = Literal["describe_update_actions"]
 DescribeUserGroupsPaginatorName = Literal["describe_user_groups"]
 DescribeUsersPaginatorName = Literal["describe_users"]
 DestinationTypeType = Literal["cloudwatch-logs", "kinesis-firehose"]
+InputAuthenticationTypeType = Literal["iam", "no-password-required", "password"]
 IpDiscoveryType = Literal["ipv4", "ipv6"]
 LogDeliveryConfigurationStatusType = Literal[
     "active", "disabling", "enabling", "error", "modifying"
 ]
 LogFormatType = Literal["json", "text"]
 LogTypeType = Literal["engine-log", "slow-log"]
 MultiAZStatusType = Literal["disabled", "enabled"]
@@ -126,14 +133,15 @@
     "cache-parameter-group",
     "cache-security-group",
     "cache-subnet-group",
     "replication-group",
     "user",
     "user-group",
 ]
+TransitEncryptionModeType = Literal["preferred", "required"]
 UpdateActionStatusType = Literal[
     "complete",
     "in-progress",
     "not-applicable",
     "not-applied",
     "scheduled",
     "scheduling",
@@ -153,23 +161,25 @@
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
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -179,30 +189,35 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
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
+    "codecatalyst",
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
@@ -228,14 +243,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -280,51 +296,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
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
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -337,14 +359,15 @@
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
@@ -356,28 +379,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -386,14 +416,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -404,55 +435,64 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
@@ -502,21 +542,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 
@@ -140,30 +140,33 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 
 class DescribeCacheParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        CacheParameterGroupName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
         """
 
 
@@ -174,60 +177,60 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 
 class DescribeCacheSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
         """
 
 
 class DescribeCacheSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
         """
 
 
 class DescribeEngineDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CacheParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
         """
 
 
@@ -241,15 +244,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeeventspaginator)
         """
 
 
@@ -260,30 +263,30 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 
 class DescribeReplicationGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
     """
 
     def paginate(
-        self, *, ReplicationGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReplicationGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReplicationGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
         """
 
 
@@ -298,15 +301,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 
@@ -320,15 +323,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 
@@ -339,15 +342,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 
@@ -361,15 +364,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describesnapshotspaginator)
         """
 
 
@@ -386,30 +389,30 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 
 class DescribeUserGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
     """
 
     def paginate(
-        self, *, UserGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUserGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
         """
 
 
@@ -421,13 +424,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 class DescribeCacheEngineVersionsPaginator(Paginator):
@@ -136,29 +136,32 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 class DescribeCacheParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        CacheParameterGroupName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
         """
 
 class DescribeCacheParametersPaginator(Paginator):
@@ -168,57 +171,57 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 class DescribeCacheSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
         """
 
 class DescribeCacheSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[CacheSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
         """
 
 class DescribeEngineDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CacheParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -231,15 +234,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalReplicationGroupsPaginator(Paginator):
@@ -249,29 +252,29 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 class DescribeReplicationGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
     """
 
     def paginate(
-        self, *, ReplicationGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReplicationGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReplicationGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
         """
 
 class DescribeReservedCacheNodesPaginator(Paginator):
@@ -285,15 +288,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 class DescribeReservedCacheNodesOfferingsPaginator(Paginator):
@@ -306,15 +309,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 class DescribeServiceUpdatesPaginator(Paginator):
@@ -324,15 +327,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 class DescribeSnapshotsPaginator(Paginator):
@@ -345,15 +348,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describesnapshotspaginator)
         """
 
 class DescribeUpdateActionsPaginator(Paginator):
@@ -369,29 +372,29 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 class DescribeUserGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
     """
 
     def paginate(
-        self, *, UserGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUserGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -402,13 +405,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,60 +18,64 @@
 from .literals import (
     AuthenticationTypeType,
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AutomaticFailoverStatusType,
     AZModeType,
     ChangeTypeType,
+    ClusterModeType,
     DataTieringStatusType,
     DestinationTypeType,
+    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
     NodeUpdateStatusType,
     OutpostModeType,
     PendingAutomaticFailoverStatusType,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     SlaMetType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
     "CacheSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "SecurityGroupMembershipTypeDef",
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
+    "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
     "NodeGroupConfigurationTypeDef",
@@ -83,74 +87,88 @@
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteReplicationGroupMessageRequestTypeDef",
     "DeleteSnapshotMessageRequestTypeDef",
     "DeleteUserGroupMessageRequestTypeDef",
     "DeleteUserMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheClustersMessageRequestTypeDef",
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
+    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
     "TimeRangeFilterTypeDef",
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
     "GlobalReplicationGroupMemberTypeDef",
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "ModifyUserMessageRequestTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
+    "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
-    "CreateUserMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
-    "AllowedNodeTypeModificationsMessageTypeDef",
-    "CacheParameterGroupNameMessageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "TagListMessageTypeDef",
+    "CreateUserMessageRequestTypeDef",
+    "ModifyUserMessageRequestTypeDef",
     "UserResponseMetadataTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
@@ -160,29 +178,14 @@
     "IncreaseReplicaCountMessageRequestTypeDef",
     "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
@@ -266,25 +269,32 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
+    "AllowedNodeTypeModificationsMessageTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScaleUpModifications": List[str],
+        "ScaleDownModifications": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AuthenticationModeTypeDef = TypedDict(
+    "AuthenticationModeTypeDef",
+    {
+        "Type": InputAuthenticationTypeType,
+        "Passwords": Sequence[str],
+    },
+    total=False,
+)
+
 AuthenticationTypeDef = TypedDict(
     "AuthenticationTypeDef",
     {
         "Type": AuthenticationTypeType,
         "PasswordCount": int,
     },
     total=False,
@@ -318,22 +328,20 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchApplyUpdateActionMessageRequestTypeDef(
     _RequiredBatchApplyUpdateActionMessageRequestTypeDef,
     _OptionalBatchApplyUpdateActionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
     "_RequiredBatchStopUpdateActionMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
     },
 )
 _OptionalBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
@@ -341,22 +349,20 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchStopUpdateActionMessageRequestTypeDef(
     _RequiredBatchStopUpdateActionMessageRequestTypeDef,
     _OptionalBatchStopUpdateActionMessageRequestTypeDef,
 ):
     pass
 
-
 CacheParameterGroupStatusTypeDef = TypedDict(
     "CacheParameterGroupStatusTypeDef",
     {
         "CacheParameterGroupName": str,
         "ParameterApplyStatus": str,
         "CacheNodeIdsToReboot": List[str],
     },
@@ -447,14 +453,22 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ChangeType": ChangeTypeType,
     },
     total=False,
 )
 
+CacheParameterGroupNameMessageTypeDef = TypedDict(
+    "CacheParameterGroupNameMessageTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CacheParameterGroupTypeDef = TypedDict(
     "CacheParameterGroupTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
         "IsGlobal": bool,
@@ -491,21 +505,19 @@
     "_OptionalCompleteMigrationMessageRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
-
 class CompleteMigrationMessageRequestTypeDef(
     _RequiredCompleteMigrationMessageRequestTypeDef, _OptionalCompleteMigrationMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredConfigureShardTypeDef = TypedDict(
     "_RequiredConfigureShardTypeDef",
     {
         "NodeGroupId": str,
         "NewReplicaCount": int,
     },
 )
@@ -514,19 +526,17 @@
     {
         "PreferredAvailabilityZones": Sequence[str],
         "PreferredOutpostArns": Sequence[str],
     },
     total=False,
 )
 
-
 class ConfigureShardTypeDef(_RequiredConfigureShardTypeDef, _OptionalConfigureShardTypeDef):
     pass
 
-
 _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupIdSuffix": str,
         "PrimaryReplicationGroupId": str,
     },
 )
@@ -534,22 +544,20 @@
     "_OptionalCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupDescription": str,
     },
     total=False,
 )
 
-
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
@@ -582,44 +590,40 @@
     {
         "GlobalNodeGroupsToRemove": Sequence[str],
         "GlobalNodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteCacheClusterMessageRequestTypeDef",
     {
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteCacheClusterMessageRequestTypeDef(
     _RequiredDeleteCacheClusterMessageRequestTypeDef,
     _OptionalDeleteCacheClusterMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 
@@ -656,22 +660,20 @@
     {
         "RetainPrimaryCluster": bool,
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteReplicationGroupMessageRequestTypeDef(
     _RequiredDeleteReplicationGroupMessageRequestTypeDef,
     _OptionalDeleteReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteSnapshotMessageRequestTypeDef = TypedDict(
     "DeleteSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 
@@ -694,20 +696,21 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CacheClusterId": str,
+        "ShowCacheNodeInfo": bool,
+        "ShowCacheClustersNotInReplicationGroups": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeCacheClustersMessageRequestTypeDef = TypedDict(
     "DescribeCacheClustersMessageRequestTypeDef",
     {
@@ -716,37 +719,79 @@
         "Marker": str,
         "ShowCacheNodeInfo": bool,
         "ShowCacheClustersNotInReplicationGroups": bool,
     },
     total=False,
 )
 
+DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    {
+        "Engine": str,
+        "EngineVersion": str,
+        "CacheParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
         "DefaultOnly": bool,
     },
     total=False,
 )
 
+DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+    },
+)
+_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
+    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeCacheParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeCacheParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 _OptionalDescribeCacheParametersMessageRequestTypeDef = TypedDict(
@@ -755,42 +800,78 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
+DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    {
+        "CacheSecurityGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    {
+        "CacheSubnetGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -798,21 +879,32 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
@@ -820,35 +912,68 @@
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    {
+        "GlobalReplicationGroupId": str,
+        "ShowMemberInfo": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
     },
     total=False,
 )
 
+DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationGroupsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    {
+        "ReservedCacheNodeId": str,
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedCacheNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     {
         "ReservedCacheNodeId": str,
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
@@ -856,39 +981,75 @@
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedCacheNodesOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeServiceUpdatesMessageRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CacheClusterId": str,
+        "SnapshotName": str,
+        "SnapshotSource": str,
+        "ShowNodeGroupConfig": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "SnapshotName": str,
         "SnapshotSource": str,
@@ -904,14 +1065,23 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
+DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    {
+        "UserGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -939,14 +1109,21 @@
     {
         "GlobalReplicationGroupId": str,
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1029,22 +1206,20 @@
     {
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyCacheSubnetGroupMessageRequestTypeDef(
     _RequiredModifyCacheSubnetGroupMessageRequestTypeDef,
     _OptionalModifyCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1056,22 +1231,20 @@
         "CacheParameterGroupName": str,
         "GlobalReplicationGroupDescription": str,
         "AutomaticFailoverEnabled": bool,
     },
     total=False,
 )
 
-
 class ModifyGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalModifyGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 ReshardingConfigurationTypeDef = TypedDict(
     "ReshardingConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "PreferredAvailabilityZones": Sequence[str],
     },
     total=False,
@@ -1088,45 +1261,19 @@
     {
         "UserIdsToAdd": Sequence[str],
         "UserIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
-
-_RequiredModifyUserMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalModifyUserMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyUserMessageRequestTypeDef",
-    {
-        "AccessString": str,
-        "AppendAccessString": str,
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-    },
-    total=False,
-)
-
-
-class ModifyUserMessageRequestTypeDef(
-    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
-):
-    pass
-
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1135,14 +1282,24 @@
         "NodeUpdateInitiatedBy": NodeUpdateInitiatedByType,
         "NodeUpdateInitiatedDate": datetime,
         "NodeUpdateStatusModifiedDate": datetime,
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
 ProcessedUpdateActionTypeDef = TypedDict(
     "ProcessedUpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "UpdateActionStatus": UpdateActionStatusType,
@@ -1196,14 +1353,25 @@
     "SlotMigrationTypeDef",
     {
         "ProgressPercentage": float,
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
 RevokeCacheSecurityGroupIngressMessageRequestTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
@@ -1286,21 +1454,19 @@
         "TargetBucket": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopySnapshotMessageRequestTypeDef(
     _RequiredCopySnapshotMessageRequestTypeDef, _OptionalCopySnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
     },
@@ -1309,22 +1475,20 @@
     "_OptionalCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCacheParameterGroupMessageRequestTypeDef(
     _RequiredCreateCacheParameterGroupMessageRequestTypeDef,
     _OptionalCreateCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateCacheSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -1332,22 +1496,20 @@
     "_OptionalCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCacheSecurityGroupMessageRequestTypeDef(
     _RequiredCreateCacheSecurityGroupMessageRequestTypeDef,
     _OptionalCreateCacheSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateCacheSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1356,22 +1518,20 @@
     "_OptionalCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCacheSubnetGroupMessageRequestTypeDef(
     _RequiredCreateCacheSubnetGroupMessageRequestTypeDef,
     _OptionalCreateCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 _OptionalCreateSnapshotMessageRequestTypeDef = TypedDict(
@@ -1381,21 +1541,19 @@
         "CacheClusterId": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotMessageRequestTypeDef(
     _RequiredCreateSnapshotMessageRequestTypeDef, _OptionalCreateSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateUserGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserGroupMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "Engine": str,
     },
 )
@@ -1404,47 +1562,19 @@
     {
         "UserIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserGroupMessageRequestTypeDef(
     _RequiredCreateUserGroupMessageRequestTypeDef, _OptionalCreateUserGroupMessageRequestTypeDef
 ):
     pass
 
-
-_RequiredCreateUserMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-        "UserName": str,
-        "Engine": str,
-        "AccessString": str,
-    },
-)
-_OptionalCreateUserMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateUserMessageRequestTypeDef",
-    {
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateUserMessageRequestTypeDef(
-    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
-):
-    pass
-
-
 _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
     },
 )
 _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef = TypedDict(
@@ -1453,67 +1583,89 @@
         "ReservedCacheNodeId": str,
         "CacheNodeCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
-
-AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
-    "AllowedNodeTypeModificationsMessageTypeDef",
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
     {
-        "ScaleUpModifications": List[str],
-        "ScaleDownModifications": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CacheParameterGroupNameMessageTypeDef = TypedDict(
-    "CacheParameterGroupNameMessageTypeDef",
+_RequiredCreateUserMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateUserMessageRequestTypeDef",
     {
-        "CacheParameterGroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "UserId": str,
+        "UserName": str,
+        "Engine": str,
+        "AccessString": str,
     },
 )
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_OptionalCreateUserMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateUserMessageRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+        "Tags": Sequence[TagTypeDef],
+        "AuthenticationMode": AuthenticationModeTypeDef,
     },
+    total=False,
 )
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
+class CreateUserMessageRequestTypeDef(
+    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
+):
+    pass
+
+_RequiredModifyUserMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyUserMessageRequestTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "UserId": str,
     },
 )
+_OptionalModifyUserMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyUserMessageRequestTypeDef",
+    {
+        "AccessString": str,
+        "AppendAccessString": str,
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+        "AuthenticationMode": AuthenticationModeTypeDef,
+    },
+    total=False,
+)
+
+class ModifyUserMessageRequestTypeDef(
+    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
+):
+    pass
 
 UserResponseMetadataTypeDef = TypedDict(
     "UserResponseMetadataTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
         "MinimumEngineVersion": str,
         "AccessString": str,
         "UserGroupIds": List[str],
         "Authentication": AuthenticationTypeDef,
         "ARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
@@ -1558,15 +1710,15 @@
 )
 
 CacheEngineVersionMessageTypeDef = TypedDict(
     "CacheEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "CacheEngineVersions": List[CacheEngineVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheNodeTypeSpecificParameterTypeDef = TypedDict(
     "CacheNodeTypeSpecificParameterTypeDef",
     {
         "ParameterName": str,
@@ -1583,23 +1735,23 @@
 )
 
 CacheParameterGroupsMessageTypeDef = TypedDict(
     "CacheParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "CacheParameterGroups": List[CacheParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheParameterGroupResultTypeDef = TypedDict(
     "CreateCacheParameterGroupResultTypeDef",
     {
         "CacheParameterGroup": CacheParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSecurityGroupTypeDef = TypedDict(
     "CacheSecurityGroupTypeDef",
     {
         "OwnerId": str,
@@ -1624,22 +1776,20 @@
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
         "ReplicasToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseReplicaCountMessageRequestTypeDef(
     _RequiredDecreaseReplicaCountMessageRequestTypeDef,
     _OptionalDecreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredIncreaseReplicaCountMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseReplicaCountMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1648,22 +1798,20 @@
     {
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
     },
     total=False,
 )
 
-
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-
 NodeSnapshotTypeDef = TypedDict(
     "NodeSnapshotTypeDef",
     {
         "CacheClusterId": str,
         "NodeGroupId": str,
         "CacheNodeId": str,
         "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
@@ -1726,212 +1874,26 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
-    {
-        "CacheClusterId": str,
-        "ShowCacheNodeInfo": bool,
-        "ShowCacheClustersNotInReplicationGroups": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "CacheParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-    },
-)
-_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
-    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-):
-    pass
-
-
-DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    {
-        "CacheSecurityGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    {
-        "CacheSubnetGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-):
-    pass
-
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    {
-        "GlobalReplicationGroupId": str,
-        "ShowMemberInfo": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    {
-        "ReservedCacheNodeId": str,
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "CacheClusterId": str,
-        "SnapshotName": str,
-        "SnapshotSource": str,
-        "ShowNodeGroupConfig": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    {
-        "UserGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
         "UpdateActionStatus": Sequence[UpdateActionStatusType],
         "ShowNodeLevelUpdateStatus": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
     "DescribeUpdateActionsMessageRequestTypeDef",
     {
@@ -1951,15 +1913,15 @@
 
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeUsersMessageRequestTypeDef = TypedDict(
     "DescribeUsersMessageRequestTypeDef",
     {
@@ -1982,15 +1944,15 @@
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalReplicationGroupTypeDef = TypedDict(
     "GlobalReplicationGroupTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2029,22 +1991,20 @@
     {
         "ResetAllParameters": bool,
         "ParameterNameValues": Sequence[ParameterNameValueTypeDef],
     },
     total=False,
 )
 
-
 class ResetCacheParameterGroupMessageRequestTypeDef(
     _RequiredResetCacheParameterGroupMessageRequestTypeDef,
     _OptionalResetCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupCount": int,
         "ApplyImmediately": bool,
     },
@@ -2055,22 +2015,20 @@
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
         "NodeGroupsToRemove": Sequence[str],
         "NodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyReplicationGroupShardConfigurationMessageRequestTypeDef(
     _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     _OptionalModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
 ):
     pass
 
-
 RegionalConfigurationTypeDef = TypedDict(
     "RegionalConfigurationTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
@@ -2129,15 +2087,15 @@
 )
 
 ServiceUpdatesMessageTypeDef = TypedDict(
     "ServiceUpdatesMessageTypeDef",
     {
         "Marker": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -2149,30 +2107,30 @@
 )
 
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserGroupResponseMetadataTypeDef = TypedDict(
     "UserGroupResponseMetadataTypeDef",
     {
         "UserGroupId": str,
         "Status": str,
         "Engine": str,
         "UserIds": List[str],
         "MinimumEngineVersion": str,
         "PendingChanges": UserGroupPendingChangesTypeDef,
         "ReplicationGroups": List[str],
         "ARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserGroupTypeDef = TypedDict(
     "UserGroupTypeDef",
     {
         "UserGroupId": str,
@@ -2188,15 +2146,15 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodeGroupTypeDef = TypedDict(
     "NodeGroupTypeDef",
     {
         "NodeGroupId": str,
@@ -2211,15 +2169,15 @@
 
 CacheParameterGroupDetailsTypeDef = TypedDict(
     "CacheParameterGroupDetailsTypeDef",
     {
         "Marker": str,
         "Parameters": List[ParameterTypeDef],
         "CacheNodeTypeSpecificParameters": List[CacheNodeTypeSpecificParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "CacheParameterGroupFamily": str,
@@ -2230,40 +2188,40 @@
     total=False,
 )
 
 AuthorizeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSecurityGroupMessageTypeDef = TypedDict(
     "CacheSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSecurityGroups": List[CacheSecurityGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheSecurityGroupResultTypeDef = TypedDict(
     "CreateCacheSecurityGroupResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RevokeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotName": str,
@@ -2334,80 +2292,80 @@
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGlobalReplicationGroupResultTypeDef = TypedDict(
     "DeleteGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGlobalReplicationGroupsResultTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsResultTypeDef",
     {
         "Marker": str,
         "GlobalReplicationGroups": List[GlobalReplicationGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateGlobalReplicationGroupResultTypeDef = TypedDict(
     "DisassociateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailoverGlobalReplicationGroupResultTypeDef = TypedDict(
     "FailoverGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyGlobalReplicationGroupResultTypeDef = TypedDict(
     "ModifyGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebalanceSlotsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2419,22 +2377,20 @@
     "_OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "RegionalConfigurations": Sequence[RegionalConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2455,33 +2411,33 @@
     total=False,
 )
 
 PurchaseReservedCacheNodesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     {
         "ReservedCacheNode": ReservedCacheNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedCacheNodeMessageTypeDef = TypedDict(
     "ReservedCacheNodeMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodes": List[ReservedCacheNodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedCacheNodesOfferingMessageTypeDef = TypedDict(
     "ReservedCacheNodesOfferingMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodesOfferings": List[ReservedCacheNodesOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSubnetGroupTypeDef = TypedDict(
     "CacheSubnetGroupTypeDef",
     {
         "CacheSubnetGroupName": str,
@@ -2495,56 +2451,56 @@
 )
 
 DescribeUserGroupsResultTypeDef = TypedDict(
     "DescribeUserGroupsResultTypeDef",
     {
         "UserGroups": List[UserGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSnapshotResultTypeDef = TypedDict(
     "DeleteSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotsListMessageTypeDef = TypedDict(
     "DescribeSnapshotsListMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
@@ -2582,22 +2538,20 @@
         "TransitEncryptionEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
-
 class CreateCacheClusterMessageRequestTypeDef(
     _RequiredCreateCacheClusterMessageRequestTypeDef,
     _OptionalCreateCacheClusterMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupDescription": str,
     },
 )
@@ -2634,26 +2588,26 @@
         "AtRestEncryptionEnabled": bool,
         "KmsKeyId": str,
         "UserGroupIds": Sequence[str],
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "DataTieringEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMessageRequestTypeDef(
     _RequiredCreateReplicationGroupMessageRequestTypeDef,
     _OptionalCreateReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalModifyCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2679,22 +2633,20 @@
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
-
 class ModifyCacheClusterMessageRequestTypeDef(
     _RequiredModifyCacheClusterMessageRequestTypeDef,
     _OptionalModifyCacheClusterMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
     },
 )
 _OptionalModifyReplicationGroupMessageRequestTypeDef = TypedDict(
@@ -2721,83 +2673,89 @@
         "AuthToken": str,
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "UserGroupIdsToAdd": Sequence[str],
         "UserGroupIdsToRemove": Sequence[str],
         "RemoveUserGroups": bool,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "NumCacheNodes": int,
         "CacheNodeIdsToRemove": List[str],
         "EngineVersion": str,
         "CacheNodeType": str,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
     "ReplicationGroupPendingModifiedValuesTypeDef",
     {
         "PrimaryClusterId": str,
         "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
         "Resharding": ReshardingStatusTypeDef,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "UserGroups": UserGroupsUpdateStatusTypeDef,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSubnetGroupMessageTypeDef = TypedDict(
     "CacheSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSubnetGroups": List[CacheSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheSubnetGroupResultTypeDef = TypedDict(
     "CreateCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyCacheSubnetGroupResultTypeDef = TypedDict(
     "ModifyCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheClusterTypeDef = TypedDict(
     "CacheClusterTypeDef",
     {
         "CacheClusterId": str,
@@ -2828,14 +2786,15 @@
         "TransitEncryptionEnabled": bool,
         "AtRestEncryptionEnabled": bool,
         "ARN": str,
         "ReplicationGroupLogDeliveryEnabled": bool,
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupTypeDef = TypedDict(
     "ReplicationGroupTypeDef",
     {
@@ -2864,132 +2823,134 @@
         "UserGroupIds": List[str],
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "ReplicationGroupCreateTime": datetime,
         "DataTiering": DataTieringStatusType,
         "AutoMinorVersionUpgrade": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
         "Marker": str,
         "CacheClusters": List[CacheClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheClusterResultTypeDef = TypedDict(
     "CreateCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCacheClusterResultTypeDef = TypedDict(
     "DeleteCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyCacheClusterResultTypeDef = TypedDict(
     "ModifyCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootCacheClusterResultTypeDef = TypedDict(
     "RebootCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompleteMigrationResponseTypeDef = TypedDict(
     "CompleteMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationGroupResultTypeDef = TypedDict(
     "CreateReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DecreaseReplicaCountResultTypeDef = TypedDict(
     "DecreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationGroupResultTypeDef = TypedDict(
     "DeleteReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IncreaseReplicaCountResultTypeDef = TypedDict(
     "IncreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationGroupResultTypeDef = TypedDict(
     "ModifyReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationGroupShardConfigurationResultTypeDef = TypedDict(
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationGroupMessageTypeDef = TypedDict(
     "ReplicationGroupMessageTypeDef",
     {
         "Marker": str,
         "ReplicationGroups": List[ReplicationGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,59 +18,65 @@
 from .literals import (
     AuthenticationTypeType,
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AutomaticFailoverStatusType,
     AZModeType,
     ChangeTypeType,
+    ClusterModeType,
     DataTieringStatusType,
     DestinationTypeType,
+    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
     NodeUpdateStatusType,
     OutpostModeType,
     PendingAutomaticFailoverStatusType,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     SlaMetType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
     "CacheSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "SecurityGroupMembershipTypeDef",
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
+    "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
     "NodeGroupConfigurationTypeDef",
@@ -82,74 +88,88 @@
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteReplicationGroupMessageRequestTypeDef",
     "DeleteSnapshotMessageRequestTypeDef",
     "DeleteUserGroupMessageRequestTypeDef",
     "DeleteUserMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheClustersMessageRequestTypeDef",
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
+    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
     "TimeRangeFilterTypeDef",
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
     "GlobalReplicationGroupMemberTypeDef",
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "ModifyUserMessageRequestTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
+    "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
-    "CreateUserMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
-    "AllowedNodeTypeModificationsMessageTypeDef",
-    "CacheParameterGroupNameMessageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "TagListMessageTypeDef",
+    "CreateUserMessageRequestTypeDef",
+    "ModifyUserMessageRequestTypeDef",
     "UserResponseMetadataTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
@@ -159,29 +179,14 @@
     "IncreaseReplicaCountMessageRequestTypeDef",
     "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
@@ -265,25 +270,32 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
+    "AllowedNodeTypeModificationsMessageTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScaleUpModifications": List[str],
+        "ScaleDownModifications": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AuthenticationModeTypeDef = TypedDict(
+    "AuthenticationModeTypeDef",
+    {
+        "Type": InputAuthenticationTypeType,
+        "Passwords": Sequence[str],
+    },
+    total=False,
+)
+
 AuthenticationTypeDef = TypedDict(
     "AuthenticationTypeDef",
     {
         "Type": AuthenticationTypeType,
         "PasswordCount": int,
     },
     total=False,
@@ -317,20 +329,22 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchApplyUpdateActionMessageRequestTypeDef(
     _RequiredBatchApplyUpdateActionMessageRequestTypeDef,
     _OptionalBatchApplyUpdateActionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
     "_RequiredBatchStopUpdateActionMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
     },
 )
 _OptionalBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
@@ -338,20 +352,22 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchStopUpdateActionMessageRequestTypeDef(
     _RequiredBatchStopUpdateActionMessageRequestTypeDef,
     _OptionalBatchStopUpdateActionMessageRequestTypeDef,
 ):
     pass
 
+
 CacheParameterGroupStatusTypeDef = TypedDict(
     "CacheParameterGroupStatusTypeDef",
     {
         "CacheParameterGroupName": str,
         "ParameterApplyStatus": str,
         "CacheNodeIdsToReboot": List[str],
     },
@@ -442,14 +458,22 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ChangeType": ChangeTypeType,
     },
     total=False,
 )
 
+CacheParameterGroupNameMessageTypeDef = TypedDict(
+    "CacheParameterGroupNameMessageTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CacheParameterGroupTypeDef = TypedDict(
     "CacheParameterGroupTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
         "IsGlobal": bool,
@@ -486,19 +510,21 @@
     "_OptionalCompleteMigrationMessageRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
+
 class CompleteMigrationMessageRequestTypeDef(
     _RequiredCompleteMigrationMessageRequestTypeDef, _OptionalCompleteMigrationMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredConfigureShardTypeDef = TypedDict(
     "_RequiredConfigureShardTypeDef",
     {
         "NodeGroupId": str,
         "NewReplicaCount": int,
     },
 )
@@ -507,17 +533,19 @@
     {
         "PreferredAvailabilityZones": Sequence[str],
         "PreferredOutpostArns": Sequence[str],
     },
     total=False,
 )
 
+
 class ConfigureShardTypeDef(_RequiredConfigureShardTypeDef, _OptionalConfigureShardTypeDef):
     pass
 
+
 _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupIdSuffix": str,
         "PrimaryReplicationGroupId": str,
     },
 )
@@ -525,20 +553,22 @@
     "_OptionalCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupDescription": str,
     },
     total=False,
 )
 
+
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
@@ -571,40 +601,44 @@
     {
         "GlobalNodeGroupsToRemove": Sequence[str],
         "GlobalNodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteCacheClusterMessageRequestTypeDef",
     {
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteCacheClusterMessageRequestTypeDef(
     _RequiredDeleteCacheClusterMessageRequestTypeDef,
     _OptionalDeleteCacheClusterMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 
@@ -641,20 +675,22 @@
     {
         "RetainPrimaryCluster": bool,
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteReplicationGroupMessageRequestTypeDef(
     _RequiredDeleteReplicationGroupMessageRequestTypeDef,
     _OptionalDeleteReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteSnapshotMessageRequestTypeDef = TypedDict(
     "DeleteSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 
@@ -677,20 +713,21 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CacheClusterId": str,
+        "ShowCacheNodeInfo": bool,
+        "ShowCacheClustersNotInReplicationGroups": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeCacheClustersMessageRequestTypeDef = TypedDict(
     "DescribeCacheClustersMessageRequestTypeDef",
     {
@@ -699,37 +736,81 @@
         "Marker": str,
         "ShowCacheNodeInfo": bool,
         "ShowCacheClustersNotInReplicationGroups": bool,
     },
     total=False,
 )
 
+DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    {
+        "Engine": str,
+        "EngineVersion": str,
+        "CacheParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
         "DefaultOnly": bool,
     },
     total=False,
 )
 
+DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+    },
+)
+_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
+    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeCacheParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeCacheParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 _OptionalDescribeCacheParametersMessageRequestTypeDef = TypedDict(
@@ -738,40 +819,82 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
+
+DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    {
+        "CacheSecurityGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    {
+        "CacheSubnetGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCacheSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -779,55 +902,103 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    {
+        "GlobalReplicationGroupId": str,
+        "ShowMemberInfo": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
     },
     total=False,
 )
 
+DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationGroupsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    {
+        "ReservedCacheNodeId": str,
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedCacheNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     {
         "ReservedCacheNodeId": str,
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
@@ -835,39 +1006,75 @@
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedCacheNodesOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeServiceUpdatesMessageRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CacheClusterId": str,
+        "SnapshotName": str,
+        "SnapshotSource": str,
+        "ShowNodeGroupConfig": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "SnapshotName": str,
         "SnapshotSource": str,
@@ -883,14 +1090,23 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
+DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    {
+        "UserGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -918,14 +1134,21 @@
     {
         "GlobalReplicationGroupId": str,
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1008,20 +1231,22 @@
     {
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyCacheSubnetGroupMessageRequestTypeDef(
     _RequiredModifyCacheSubnetGroupMessageRequestTypeDef,
     _OptionalModifyCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1033,20 +1258,22 @@
         "CacheParameterGroupName": str,
         "GlobalReplicationGroupDescription": str,
         "AutomaticFailoverEnabled": bool,
     },
     total=False,
 )
 
+
 class ModifyGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalModifyGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 ReshardingConfigurationTypeDef = TypedDict(
     "ReshardingConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "PreferredAvailabilityZones": Sequence[str],
     },
     total=False,
@@ -1063,40 +1290,20 @@
     {
         "UserIdsToAdd": Sequence[str],
         "UserIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
-_RequiredModifyUserMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalModifyUserMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyUserMessageRequestTypeDef",
-    {
-        "AccessString": str,
-        "AppendAccessString": str,
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-    },
-    total=False,
-)
-
-class ModifyUserMessageRequestTypeDef(
-    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
-):
-    pass
 
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
@@ -1106,14 +1313,24 @@
         "NodeUpdateInitiatedBy": NodeUpdateInitiatedByType,
         "NodeUpdateInitiatedDate": datetime,
         "NodeUpdateStatusModifiedDate": datetime,
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
 ProcessedUpdateActionTypeDef = TypedDict(
     "ProcessedUpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "UpdateActionStatus": UpdateActionStatusType,
@@ -1167,14 +1384,25 @@
     "SlotMigrationTypeDef",
     {
         "ProgressPercentage": float,
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
 RevokeCacheSecurityGroupIngressMessageRequestTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
@@ -1257,19 +1485,21 @@
         "TargetBucket": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopySnapshotMessageRequestTypeDef(
     _RequiredCopySnapshotMessageRequestTypeDef, _OptionalCopySnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
     },
@@ -1278,20 +1508,22 @@
     "_OptionalCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCacheParameterGroupMessageRequestTypeDef(
     _RequiredCreateCacheParameterGroupMessageRequestTypeDef,
     _OptionalCreateCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateCacheSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -1299,20 +1531,22 @@
     "_OptionalCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCacheSecurityGroupMessageRequestTypeDef(
     _RequiredCreateCacheSecurityGroupMessageRequestTypeDef,
     _OptionalCreateCacheSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateCacheSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1321,20 +1555,22 @@
     "_OptionalCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCacheSubnetGroupMessageRequestTypeDef(
     _RequiredCreateCacheSubnetGroupMessageRequestTypeDef,
     _OptionalCreateCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 _OptionalCreateSnapshotMessageRequestTypeDef = TypedDict(
@@ -1344,19 +1580,21 @@
         "CacheClusterId": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotMessageRequestTypeDef(
     _RequiredCreateSnapshotMessageRequestTypeDef, _OptionalCreateSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateUserGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserGroupMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "Engine": str,
     },
 )
@@ -1365,42 +1603,20 @@
     {
         "UserIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserGroupMessageRequestTypeDef(
     _RequiredCreateUserGroupMessageRequestTypeDef, _OptionalCreateUserGroupMessageRequestTypeDef
 ):
     pass
 
-_RequiredCreateUserMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-        "UserName": str,
-        "Engine": str,
-        "AccessString": str,
-    },
-)
-_OptionalCreateUserMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateUserMessageRequestTypeDef",
-    {
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateUserMessageRequestTypeDef(
-    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
-):
-    pass
 
 _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
     },
 )
@@ -1410,65 +1626,95 @@
         "ReservedCacheNodeId": str,
         "CacheNodeCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
-AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
-    "AllowedNodeTypeModificationsMessageTypeDef",
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
     {
-        "ScaleUpModifications": List[str],
-        "ScaleDownModifications": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CacheParameterGroupNameMessageTypeDef = TypedDict(
-    "CacheParameterGroupNameMessageTypeDef",
+_RequiredCreateUserMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateUserMessageRequestTypeDef",
     {
-        "CacheParameterGroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "UserId": str,
+        "UserName": str,
+        "Engine": str,
+        "AccessString": str,
     },
 )
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_OptionalCreateUserMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateUserMessageRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+        "Tags": Sequence[TagTypeDef],
+        "AuthenticationMode": AuthenticationModeTypeDef,
     },
+    total=False,
 )
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
+
+class CreateUserMessageRequestTypeDef(
+    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
+):
+    pass
+
+
+_RequiredModifyUserMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyUserMessageRequestTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "UserId": str,
     },
 )
+_OptionalModifyUserMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyUserMessageRequestTypeDef",
+    {
+        "AccessString": str,
+        "AppendAccessString": str,
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+        "AuthenticationMode": AuthenticationModeTypeDef,
+    },
+    total=False,
+)
+
+
+class ModifyUserMessageRequestTypeDef(
+    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
+):
+    pass
+
 
 UserResponseMetadataTypeDef = TypedDict(
     "UserResponseMetadataTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
         "MinimumEngineVersion": str,
         "AccessString": str,
         "UserGroupIds": List[str],
         "Authentication": AuthenticationTypeDef,
         "ARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
@@ -1513,15 +1759,15 @@
 )
 
 CacheEngineVersionMessageTypeDef = TypedDict(
     "CacheEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "CacheEngineVersions": List[CacheEngineVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheNodeTypeSpecificParameterTypeDef = TypedDict(
     "CacheNodeTypeSpecificParameterTypeDef",
     {
         "ParameterName": str,
@@ -1538,23 +1784,23 @@
 )
 
 CacheParameterGroupsMessageTypeDef = TypedDict(
     "CacheParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "CacheParameterGroups": List[CacheParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheParameterGroupResultTypeDef = TypedDict(
     "CreateCacheParameterGroupResultTypeDef",
     {
         "CacheParameterGroup": CacheParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSecurityGroupTypeDef = TypedDict(
     "CacheSecurityGroupTypeDef",
     {
         "OwnerId": str,
@@ -1579,20 +1825,22 @@
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
         "ReplicasToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseReplicaCountMessageRequestTypeDef(
     _RequiredDecreaseReplicaCountMessageRequestTypeDef,
     _OptionalDecreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredIncreaseReplicaCountMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseReplicaCountMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1601,20 +1849,22 @@
     {
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
     },
     total=False,
 )
 
+
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+
 NodeSnapshotTypeDef = TypedDict(
     "NodeSnapshotTypeDef",
     {
         "CacheClusterId": str,
         "NodeGroupId": str,
         "CacheNodeId": str,
         "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
@@ -1677,208 +1927,26 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
-    {
-        "CacheClusterId": str,
-        "ShowCacheNodeInfo": bool,
-        "ShowCacheClustersNotInReplicationGroups": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "CacheParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-    },
-)
-_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
-    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-):
-    pass
-
-DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    {
-        "CacheSecurityGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    {
-        "CacheSubnetGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-):
-    pass
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    {
-        "GlobalReplicationGroupId": str,
-        "ShowMemberInfo": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    {
-        "ReservedCacheNodeId": str,
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "CacheClusterId": str,
-        "SnapshotName": str,
-        "SnapshotSource": str,
-        "ShowNodeGroupConfig": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    {
-        "UserGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
         "UpdateActionStatus": Sequence[UpdateActionStatusType],
         "ShowNodeLevelUpdateStatus": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
     "DescribeUpdateActionsMessageRequestTypeDef",
     {
@@ -1898,15 +1966,15 @@
 
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeUsersMessageRequestTypeDef = TypedDict(
     "DescribeUsersMessageRequestTypeDef",
     {
@@ -1929,15 +1997,15 @@
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalReplicationGroupTypeDef = TypedDict(
     "GlobalReplicationGroupTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -1976,20 +2044,22 @@
     {
         "ResetAllParameters": bool,
         "ParameterNameValues": Sequence[ParameterNameValueTypeDef],
     },
     total=False,
 )
 
+
 class ResetCacheParameterGroupMessageRequestTypeDef(
     _RequiredResetCacheParameterGroupMessageRequestTypeDef,
     _OptionalResetCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupCount": int,
         "ApplyImmediately": bool,
     },
@@ -2000,20 +2070,22 @@
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
         "NodeGroupsToRemove": Sequence[str],
         "NodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyReplicationGroupShardConfigurationMessageRequestTypeDef(
     _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     _OptionalModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
 ):
     pass
 
+
 RegionalConfigurationTypeDef = TypedDict(
     "RegionalConfigurationTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
@@ -2072,15 +2144,15 @@
 )
 
 ServiceUpdatesMessageTypeDef = TypedDict(
     "ServiceUpdatesMessageTypeDef",
     {
         "Marker": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -2092,30 +2164,30 @@
 )
 
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserGroupResponseMetadataTypeDef = TypedDict(
     "UserGroupResponseMetadataTypeDef",
     {
         "UserGroupId": str,
         "Status": str,
         "Engine": str,
         "UserIds": List[str],
         "MinimumEngineVersion": str,
         "PendingChanges": UserGroupPendingChangesTypeDef,
         "ReplicationGroups": List[str],
         "ARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserGroupTypeDef = TypedDict(
     "UserGroupTypeDef",
     {
         "UserGroupId": str,
@@ -2131,15 +2203,15 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodeGroupTypeDef = TypedDict(
     "NodeGroupTypeDef",
     {
         "NodeGroupId": str,
@@ -2154,15 +2226,15 @@
 
 CacheParameterGroupDetailsTypeDef = TypedDict(
     "CacheParameterGroupDetailsTypeDef",
     {
         "Marker": str,
         "Parameters": List[ParameterTypeDef],
         "CacheNodeTypeSpecificParameters": List[CacheNodeTypeSpecificParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "CacheParameterGroupFamily": str,
@@ -2173,40 +2245,40 @@
     total=False,
 )
 
 AuthorizeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSecurityGroupMessageTypeDef = TypedDict(
     "CacheSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSecurityGroups": List[CacheSecurityGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheSecurityGroupResultTypeDef = TypedDict(
     "CreateCacheSecurityGroupResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RevokeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotName": str,
@@ -2277,80 +2349,80 @@
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGlobalReplicationGroupResultTypeDef = TypedDict(
     "DeleteGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGlobalReplicationGroupsResultTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsResultTypeDef",
     {
         "Marker": str,
         "GlobalReplicationGroups": List[GlobalReplicationGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateGlobalReplicationGroupResultTypeDef = TypedDict(
     "DisassociateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailoverGlobalReplicationGroupResultTypeDef = TypedDict(
     "FailoverGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyGlobalReplicationGroupResultTypeDef = TypedDict(
     "ModifyGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebalanceSlotsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2362,20 +2434,22 @@
     "_OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "RegionalConfigurations": Sequence[RegionalConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2396,33 +2470,33 @@
     total=False,
 )
 
 PurchaseReservedCacheNodesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     {
         "ReservedCacheNode": ReservedCacheNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedCacheNodeMessageTypeDef = TypedDict(
     "ReservedCacheNodeMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodes": List[ReservedCacheNodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedCacheNodesOfferingMessageTypeDef = TypedDict(
     "ReservedCacheNodesOfferingMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodesOfferings": List[ReservedCacheNodesOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSubnetGroupTypeDef = TypedDict(
     "CacheSubnetGroupTypeDef",
     {
         "CacheSubnetGroupName": str,
@@ -2436,56 +2510,56 @@
 )
 
 DescribeUserGroupsResultTypeDef = TypedDict(
     "DescribeUserGroupsResultTypeDef",
     {
         "UserGroups": List[UserGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSnapshotResultTypeDef = TypedDict(
     "DeleteSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotsListMessageTypeDef = TypedDict(
     "DescribeSnapshotsListMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
@@ -2523,20 +2597,22 @@
         "TransitEncryptionEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
+
 class CreateCacheClusterMessageRequestTypeDef(
     _RequiredCreateCacheClusterMessageRequestTypeDef,
     _OptionalCreateCacheClusterMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupDescription": str,
     },
 )
@@ -2573,24 +2649,28 @@
         "AtRestEncryptionEnabled": bool,
         "KmsKeyId": str,
         "UserGroupIds": Sequence[str],
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "DataTieringEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMessageRequestTypeDef(
     _RequiredCreateReplicationGroupMessageRequestTypeDef,
     _OptionalCreateReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalModifyCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2616,20 +2696,22 @@
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
+
 class ModifyCacheClusterMessageRequestTypeDef(
     _RequiredModifyCacheClusterMessageRequestTypeDef,
     _OptionalModifyCacheClusterMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
     },
 )
 _OptionalModifyReplicationGroupMessageRequestTypeDef = TypedDict(
@@ -2656,81 +2738,91 @@
         "AuthToken": str,
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "UserGroupIdsToAdd": Sequence[str],
         "UserGroupIdsToRemove": Sequence[str],
         "RemoveUserGroups": bool,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
+
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "NumCacheNodes": int,
         "CacheNodeIdsToRemove": List[str],
         "EngineVersion": str,
         "CacheNodeType": str,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
     "ReplicationGroupPendingModifiedValuesTypeDef",
     {
         "PrimaryClusterId": str,
         "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
         "Resharding": ReshardingStatusTypeDef,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "UserGroups": UserGroupsUpdateStatusTypeDef,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSubnetGroupMessageTypeDef = TypedDict(
     "CacheSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSubnetGroups": List[CacheSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheSubnetGroupResultTypeDef = TypedDict(
     "CreateCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyCacheSubnetGroupResultTypeDef = TypedDict(
     "ModifyCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheClusterTypeDef = TypedDict(
     "CacheClusterTypeDef",
     {
         "CacheClusterId": str,
@@ -2761,14 +2853,15 @@
         "TransitEncryptionEnabled": bool,
         "AtRestEncryptionEnabled": bool,
         "ARN": str,
         "ReplicationGroupLogDeliveryEnabled": bool,
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupTypeDef = TypedDict(
     "ReplicationGroupTypeDef",
     {
@@ -2797,132 +2890,134 @@
         "UserGroupIds": List[str],
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "ReplicationGroupCreateTime": datetime,
         "DataTiering": DataTieringStatusType,
         "AutoMinorVersionUpgrade": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
         "Marker": str,
         "CacheClusters": List[CacheClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCacheClusterResultTypeDef = TypedDict(
     "CreateCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCacheClusterResultTypeDef = TypedDict(
     "DeleteCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyCacheClusterResultTypeDef = TypedDict(
     "ModifyCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootCacheClusterResultTypeDef = TypedDict(
     "RebootCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompleteMigrationResponseTypeDef = TypedDict(
     "CompleteMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationGroupResultTypeDef = TypedDict(
     "CreateReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DecreaseReplicaCountResultTypeDef = TypedDict(
     "DecreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationGroupResultTypeDef = TypedDict(
     "DeleteReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IncreaseReplicaCountResultTypeDef = TypedDict(
     "IncreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationGroupResultTypeDef = TypedDict(
     "ModifyReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationGroupShardConfigurationResultTypeDef = TypedDict(
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationGroupMessageTypeDef = TypedDict(
     "ReplicationGroupMessageTypeDef",
     {
         "Marker": str,
         "ReplicationGroups": List[ReplicationGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.26.4
-Summary: Type annotations for boto3.ElastiCache 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElastiCache 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-elasticache"></a>
 
 # mypy-boto3-elasticache
 
 [![PyPI - mypy-boto3-elasticache](https://img.shields.io/pypi/v/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -402,14 +403,15 @@
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AuthenticationTypeType,
     AutomaticFailoverStatusType,
     CacheClusterAvailableWaiterName,
     CacheClusterDeletedWaiterName,
     ChangeTypeType,
+    ClusterModeType,
     DataTieringStatusType,
     DescribeCacheClustersPaginatorName,
     DescribeCacheEngineVersionsPaginatorName,
     DescribeCacheParameterGroupsPaginatorName,
     DescribeCacheParametersPaginatorName,
     DescribeCacheSecurityGroupsPaginatorName,
     DescribeCacheSubnetGroupsPaginatorName,
@@ -421,14 +423,15 @@
     DescribeReservedCacheNodesPaginatorName,
     DescribeServiceUpdatesPaginatorName,
     DescribeSnapshotsPaginatorName,
     DescribeUpdateActionsPaginatorName,
     DescribeUserGroupsPaginatorName,
     DescribeUsersPaginatorName,
     DestinationTypeType,
+    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
@@ -438,14 +441,15 @@
     ReplicationGroupAvailableWaiterName,
     ReplicationGroupDeletedWaiterName,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SlaMetType,
     SourceTypeType,
+    TransitEncryptionModeType,
     UpdateActionStatusType,
     ElastiCacheServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
@@ -462,29 +466,31 @@
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
     CacheSecurityGroupMembershipTypeDef,
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
@@ -496,74 +502,88 @@
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
-    ModifyUserMessageRequestTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
+    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
+    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
-    CreateUserMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
-    EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
+    CreateUserMessageRequestTypeDef,
+    ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
@@ -573,29 +593,14 @@
     IncreaseReplicaCountMessageRequestTypeDef,
     NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
@@ -682,42 +687,42 @@
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

### Comparing `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.27.0/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.4/setup.py` & `mypy-boto3-elasticache-1.27.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-elasticache.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.26.4",
+    version="1.27.0",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElastiCache 1.26.4 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.ElastiCache 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 elasticache type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_elasticache": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_elasticache": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/",
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


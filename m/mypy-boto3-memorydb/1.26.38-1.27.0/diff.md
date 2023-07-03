# Comparing `tmp/mypy-boto3-memorydb-1.26.38.tar.gz` & `tmp/mypy-boto3-memorydb-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-memorydb-1.26.38.tar", last modified: Tue Dec 27 20:32:14 2022, max compression
+gzip compressed data, was "mypy-boto3-memorydb-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
```

## Comparing `mypy-boto3-memorydb-1.26.38.tar` & `mypy-boto3-memorydb-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36248 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41309 2022-12-27 20:32:03.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41274 2022-12-27 20:32:03.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.183680 mypy-boto3-memorydb-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-03 19:51:08.183680 mypy-boto3-memorydb-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.175680 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-07-03 19:42:15.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-03 19:42:15.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-03 19:42:15.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-03 19:42:15.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-03 19:42:15.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-07-03 19:42:15.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41450 2023-07-03 19:42:16.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41415 2023-07-03 19:42:16.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.183680 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-03 19:51:08.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:08.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:08.000000 mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.183680 mypy-boto3-memorydb-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:42:13.000000 mypy-boto3-memorydb-1.27.0/setup.py
```

### Comparing `mypy-boto3-memorydb-1.26.38/LICENSE` & `mypy-boto3-memorydb-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-memorydb-1.26.38/PKG-INFO` & `mypy-boto3-memorydb-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.26.38
-Summary: Type annotations for boto3.MemoryDB 1.26.38 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.MemoryDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,63 +382,74 @@
 from mypy_boto3_memorydb.type_defs import (
     ACLPendingChangesTypeDef,
     ACLsUpdateStatusTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AvailabilityZoneTypeDef,
     ServiceUpdateRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedClusterTypeDef,
     PendingModifiedServiceUpdateTypeDef,
     EndpointTypeDef,
     SecurityGroupMembershipTypeDef,
     TagTypeDef,
     ParameterGroupTypeDef,
     DeleteACLRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeACLsRequestDescribeACLsPaginateTypeDef,
     DescribeACLsRequestRequestTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
+    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
+    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
     DescribeReservedNodesOfferingsRequestRequestTypeDef,
+    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesRequestRequestTypeDef,
+    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
     ServiceUpdateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
+    ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
+    ResponseMetadataTypeDef,
     ShardConfigurationRequestTypeDef,
     ShardConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateACLRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     ACLTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     SubnetTypeDef,
     BatchUpdateClusterRequestRequestTypeDef,
-    ListAllowedNodeTypeUpdatesResponseTypeDef,
     NodeTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
@@ -449,25 +460,14 @@
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
-    DescribeACLsRequestDescribeACLsPaginateTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
-    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
-    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
@@ -517,42 +517,42 @@
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

### Comparing `mypy-boto3-memorydb-1.26.38/README.md` & `mypy-boto3-memorydb-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,63 +350,74 @@
 from mypy_boto3_memorydb.type_defs import (
     ACLPendingChangesTypeDef,
     ACLsUpdateStatusTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AvailabilityZoneTypeDef,
     ServiceUpdateRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedClusterTypeDef,
     PendingModifiedServiceUpdateTypeDef,
     EndpointTypeDef,
     SecurityGroupMembershipTypeDef,
     TagTypeDef,
     ParameterGroupTypeDef,
     DeleteACLRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeACLsRequestDescribeACLsPaginateTypeDef,
     DescribeACLsRequestRequestTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
+    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
+    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
     DescribeReservedNodesOfferingsRequestRequestTypeDef,
+    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesRequestRequestTypeDef,
+    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
     ServiceUpdateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
+    ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
+    ResponseMetadataTypeDef,
     ShardConfigurationRequestTypeDef,
     ShardConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateACLRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     ACLTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     SubnetTypeDef,
     BatchUpdateClusterRequestRequestTypeDef,
-    ListAllowedNodeTypeUpdatesResponseTypeDef,
     NodeTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
@@ -417,25 +428,14 @@
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
-    DescribeACLsRequestDescribeACLsPaginateTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
-    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
-    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
@@ -485,42 +485,42 @@
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

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__init__.py` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__init__.pyi` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__main__.py` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MemoryDB 1.26.38\nVersion:         1.26.38\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.MemoryDB 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.38")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.py` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.pyi` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.py` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,29 +44,29 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AZStatusType = Literal["multiaz", "singleaz"]
-AuthenticationTypeType = Literal["no-password", "password"]
+AuthenticationTypeType = Literal["iam", "no-password", "password"]
 DataTieringStatusType = Literal["false", "true"]
 DescribeACLsPaginatorName = Literal["describe_acls"]
 DescribeClustersPaginatorName = Literal["describe_clusters"]
 DescribeEngineVersionsPaginatorName = Literal["describe_engine_versions"]
 DescribeEventsPaginatorName = Literal["describe_events"]
 DescribeParameterGroupsPaginatorName = Literal["describe_parameter_groups"]
 DescribeParametersPaginatorName = Literal["describe_parameters"]
 DescribeReservedNodesOfferingsPaginatorName = Literal["describe_reserved_nodes_offerings"]
 DescribeReservedNodesPaginatorName = Literal["describe_reserved_nodes"]
 DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
 DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
 DescribeSubnetGroupsPaginatorName = Literal["describe_subnet_groups"]
 DescribeUsersPaginatorName = Literal["describe_users"]
-InputAuthenticationTypeType = Literal["password"]
+InputAuthenticationTypeType = Literal["iam", "password"]
 ServiceUpdateStatusType = Literal["available", "complete", "in-progress", "scheduled"]
 ServiceUpdateTypeType = Literal["security-update"]
 SourceTypeType = Literal["acl", "cluster", "node", "parameter-group", "subnet-group", "user"]
 MemoryDBServiceName = Literal["memorydb"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -78,14 +78,15 @@
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
@@ -106,31 +107,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -209,14 +213,15 @@
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
@@ -227,18 +232,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -269,14 +276,15 @@
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
@@ -295,16 +303,19 @@
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
@@ -384,18 +395,21 @@
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

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.pyi` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -42,29 +42,29 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AZStatusType = Literal["multiaz", "singleaz"]
-AuthenticationTypeType = Literal["no-password", "password"]
+AuthenticationTypeType = Literal["iam", "no-password", "password"]
 DataTieringStatusType = Literal["false", "true"]
 DescribeACLsPaginatorName = Literal["describe_acls"]
 DescribeClustersPaginatorName = Literal["describe_clusters"]
 DescribeEngineVersionsPaginatorName = Literal["describe_engine_versions"]
 DescribeEventsPaginatorName = Literal["describe_events"]
 DescribeParameterGroupsPaginatorName = Literal["describe_parameter_groups"]
 DescribeParametersPaginatorName = Literal["describe_parameters"]
 DescribeReservedNodesOfferingsPaginatorName = Literal["describe_reserved_nodes_offerings"]
 DescribeReservedNodesPaginatorName = Literal["describe_reserved_nodes"]
 DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
 DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
 DescribeSubnetGroupsPaginatorName = Literal["describe_subnet_groups"]
 DescribeUsersPaginatorName = Literal["describe_users"]
-InputAuthenticationTypeType = Literal["password"]
+InputAuthenticationTypeType = Literal["iam", "password"]
 ServiceUpdateStatusType = Literal["available", "complete", "in-progress", "scheduled"]
 ServiceUpdateTypeType = Literal["security-update"]
 SourceTypeType = Literal["acl", "cluster", "node", "parameter-group", "subnet-group", "user"]
 MemoryDBServiceName = Literal["memorydb"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -76,14 +76,15 @@
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
@@ -104,31 +105,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -207,14 +211,15 @@
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
@@ -225,18 +230,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -267,14 +274,15 @@
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
@@ -293,16 +301,19 @@
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
@@ -382,18 +393,21 @@
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

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/paginator.py` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 class DescribeACLsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeACLs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeaclspaginator)
     """
 
     def paginate(
-        self, *, ACLName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ACLName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeACLsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeACLs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeaclspaginator)
         """
 
 
@@ -112,15 +112,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         ShowShardDetails: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeclusterspaginator)
         """
 
 
@@ -132,15 +132,15 @@
 
     def paginate(
         self,
         *,
         EngineVersion: str = ...,
         ParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeengineversionspaginator)
         """
 
 
@@ -154,45 +154,45 @@
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeeventspaginator)
         """
 
 
 class DescribeParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ParameterGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparametergroupspaginator)
         """
 
 
 class DescribeParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ParameterGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparameterspaginator)
         """
 
 
@@ -206,15 +206,15 @@
         self,
         *,
         ReservationId: str = ...,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describereservednodespaginator)
         """
 
 
@@ -227,15 +227,15 @@
     def paginate(
         self,
         *,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedNodesOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodesOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describereservednodesofferingspaginator)
         """
 
 
@@ -247,15 +247,15 @@
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeServiceUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeServiceUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeserviceupdatespaginator)
         """
 
 
@@ -268,30 +268,30 @@
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         SnapshotName: str = ...,
         Source: str = ...,
         ShowDetail: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describesnapshotspaginator)
         """
 
 
 class DescribeSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, SubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describesubnetgroupspaginator)
         """
 
 
@@ -302,13 +302,13 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeuserspaginator)
         """
```

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/paginator.pyi` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 class DescribeACLsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeACLs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeaclspaginator)
     """
 
     def paginate(
-        self, *, ACLName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ACLName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeACLsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeACLs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeaclspaginator)
         """
 
 class DescribeClustersPaginator(Paginator):
@@ -108,15 +108,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         ShowShardDetails: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeclusterspaginator)
         """
 
 class DescribeEngineVersionsPaginator(Paginator):
@@ -127,15 +127,15 @@
 
     def paginate(
         self,
         *,
         EngineVersion: str = ...,
         ParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeengineversionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -148,43 +148,43 @@
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeeventspaginator)
         """
 
 class DescribeParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ParameterGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparametergroupspaginator)
         """
 
 class DescribeParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ParameterGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeparameterspaginator)
         """
 
 class DescribeReservedNodesPaginator(Paginator):
@@ -197,15 +197,15 @@
         self,
         *,
         ReservationId: str = ...,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describereservednodespaginator)
         """
 
 class DescribeReservedNodesOfferingsPaginator(Paginator):
@@ -217,15 +217,15 @@
     def paginate(
         self,
         *,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedNodesOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodesOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describereservednodesofferingspaginator)
         """
 
 class DescribeServiceUpdatesPaginator(Paginator):
@@ -236,15 +236,15 @@
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeServiceUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeServiceUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeserviceupdatespaginator)
         """
 
 class DescribeSnapshotsPaginator(Paginator):
@@ -256,29 +256,29 @@
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         SnapshotName: str = ...,
         Source: str = ...,
         ShowDetail: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describesnapshotspaginator)
         """
 
 class DescribeSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, SubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describesubnetgroupspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -288,13 +288,13 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/paginators/#describeuserspaginator)
         """
```

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/type_defs.py` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AuthenticationTypeType,
     AZStatusType,
     DataTieringStatusType,
+    InputAuthenticationTypeType,
     ServiceUpdateStatusType,
     SourceTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -36,63 +37,74 @@
 __all__ = (
     "ACLPendingChangesTypeDef",
     "ACLsUpdateStatusTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AvailabilityZoneTypeDef",
     "ServiceUpdateRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedClusterTypeDef",
     "PendingModifiedServiceUpdateTypeDef",
     "EndpointTypeDef",
     "SecurityGroupMembershipTypeDef",
     "TagTypeDef",
     "ParameterGroupTypeDef",
     "DeleteACLRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
     "DescribeACLsRequestRequestTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
+    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
     "DescribeEngineVersionsRequestRequestTypeDef",
     "EngineVersionInfoTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "EventTypeDef",
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
+    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "ParameterTypeDef",
+    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
     "DescribeReservedNodesOfferingsRequestRequestTypeDef",
+    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesRequestRequestTypeDef",
+    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesRequestRequestTypeDef",
     "ServiceUpdateTypeDef",
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "FilterTypeDef",
     "FailoverShardRequestRequestTypeDef",
     "ListAllowedNodeTypeUpdatesRequestRequestTypeDef",
+    "ListAllowedNodeTypeUpdatesResponseTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RecurringChargeTypeDef",
     "ReplicaConfigurationRequestTypeDef",
     "ResetParameterGroupRequestRequestTypeDef",
     "SlotMigrationTypeDef",
+    "ResponseMetadataTypeDef",
     "ShardConfigurationRequestTypeDef",
     "ShardConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateACLRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "ACLTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserTypeDef",
     "SubnetTypeDef",
     "BatchUpdateClusterRequestRequestTypeDef",
-    "ListAllowedNodeTypeUpdatesResponseTypeDef",
     "NodeTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateACLRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
@@ -103,25 +115,14 @@
     "TagResourceResponseTypeDef",
     "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DeleteParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "ResetParameterGroupResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
-    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
-    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
-    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
-    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeEngineVersionsResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "DescribeServiceUpdatesResponseTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
@@ -179,15 +180,15 @@
     },
     total=False,
 )
 
 AuthenticationModeTypeDef = TypedDict(
     "AuthenticationModeTypeDef",
     {
-        "Type": Literal["password"],
+        "Type": InputAuthenticationTypeType,
         "Passwords": Sequence[str],
     },
     total=False,
 )
 
 AuthenticationTypeDef = TypedDict(
     "AuthenticationTypeDef",
@@ -210,25 +211,14 @@
     "ServiceUpdateRequestTypeDef",
     {
         "ServiceUpdateNameToApply": str,
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
 UnprocessedClusterTypeDef = TypedDict(
     "UnprocessedClusterTypeDef",
     {
         "ClusterName": str,
         "ErrorType": str,
         "ErrorMessage": str,
     },
@@ -334,45 +324,65 @@
 DeleteUserRequestRequestTypeDef = TypedDict(
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeACLsRequestDescribeACLsPaginateTypeDef = TypedDict(
+    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ACLName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeACLsRequestRequestTypeDef = TypedDict(
     "DescribeACLsRequestRequestTypeDef",
     {
         "ACLName": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "ClusterName": str,
+        "ShowShardDetails": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "ClusterName": str,
         "MaxResults": int,
         "NextToken": str,
         "ShowShardDetails": bool,
     },
     total=False,
 )
 
+DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
+    {
+        "EngineVersion": str,
+        "ParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEngineVersionsRequestRequestTypeDef = TypedDict(
     "DescribeEngineVersionsRequestRequestTypeDef",
     {
         "EngineVersion": str,
         "ParameterGroupFamily": str,
         "MaxResults": int,
         "NextToken": str,
@@ -387,14 +397,27 @@
         "EngineVersion": str,
         "EnginePatchVersion": str,
         "ParameterGroupFamily": str,
     },
     total=False,
 )
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -412,24 +435,55 @@
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
     },
     total=False,
 )
 
+DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeParameterGroupsRequestRequestTypeDef = TypedDict(
     "DescribeParameterGroupsRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeParametersRequestDescribeParametersPaginateTypeDef(
+    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
+    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -458,41 +512,77 @@
         "DataType": str,
         "AllowedValues": str,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
+DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedNodesOfferingId": str,
+        "NodeType": str,
+        "Duration": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodesOfferingsRequestRequestTypeDef = TypedDict(
     "DescribeReservedNodesOfferingsRequestRequestTypeDef",
     {
         "ReservedNodesOfferingId": str,
         "NodeType": str,
         "Duration": str,
         "OfferingType": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservationId": str,
+        "ReservedNodesOfferingId": str,
+        "NodeType": str,
+        "Duration": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodesRequestRequestTypeDef = TypedDict(
     "DescribeReservedNodesRequestRequestTypeDef",
     {
         "ReservationId": str,
         "ReservedNodesOfferingId": str,
         "NodeType": str,
         "Duration": str,
         "OfferingType": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ClusterNames": Sequence[str],
+        "Status": Sequence[ServiceUpdateStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeServiceUpdatesRequestRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesRequestRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ClusterNames": Sequence[str],
         "Status": Sequence[ServiceUpdateStatusType],
         "MaxResults": int,
@@ -512,27 +602,48 @@
         "Type": Literal["security-update"],
         "NodesUpdated": str,
         "AutoUpdateStartDate": datetime,
     },
     total=False,
 )
 
+DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    {
+        "ClusterName": str,
+        "SnapshotName": str,
+        "Source": str,
+        "ShowDetail": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "ClusterName": str,
         "SnapshotName": str,
         "Source": str,
         "NextToken": str,
         "MaxResults": int,
         "ShowDetail": bool,
     },
     total=False,
 )
 
+DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    {
+        "SubnetGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSubnetGroupsRequestRequestTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -558,21 +669,40 @@
 ListAllowedNodeTypeUpdatesRequestRequestTypeDef = TypedDict(
     "ListAllowedNodeTypeUpdatesRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
+ListAllowedNodeTypeUpdatesResponseTypeDef = TypedDict(
+    "ListAllowedNodeTypeUpdatesResponseTypeDef",
+    {
+        "ScaleUpNodeTypes": List[str],
+        "ScaleDownNodeTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ParameterNameValueTypeDef = TypedDict(
     "ParameterNameValueTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -622,14 +752,25 @@
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
 ShardConfigurationRequestTypeDef = TypedDict(
     "ShardConfigurationRequestTypeDef",
     {
         "ShardCount": int,
     },
     total=False,
 )
@@ -772,23 +913,14 @@
 class BatchUpdateClusterRequestRequestTypeDef(
     _RequiredBatchUpdateClusterRequestRequestTypeDef,
     _OptionalBatchUpdateClusterRequestRequestTypeDef,
 ):
     pass
 
 
-ListAllowedNodeTypeUpdatesResponseTypeDef = TypedDict(
-    "ListAllowedNodeTypeUpdatesResponseTypeDef",
-    {
-        "ScaleUpNodeTypes": List[str],
-        "ScaleDownNodeTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "Name": str,
         "Status": str,
         "AvailabilityZone": str,
         "CreateTime": datetime,
@@ -977,15 +1109,15 @@
     pass
 
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef",
     {
         "ReservedNodesOfferingId": str,
@@ -1017,240 +1149,109 @@
     },
 )
 
 TagResourceResponseTypeDef = TypedDict(
     "TagResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceResponseTypeDef = TypedDict(
     "UntagResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParameterGroupResponseTypeDef = TypedDict(
     "DeleteParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParameterGroupsResponseTypeDef = TypedDict(
     "DescribeParameterGroupsResponseTypeDef",
     {
         "NextToken": str,
         "ParameterGroups": List[ParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetParameterGroupResponseTypeDef = TypedDict(
     "ResetParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateParameterGroupResponseTypeDef = TypedDict(
     "UpdateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeACLsRequestDescribeACLsPaginateTypeDef = TypedDict(
-    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
-    {
-        "ACLName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "ClusterName": str,
-        "ShowShardDetails": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
-    {
-        "EngineVersion": str,
-        "ParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeParametersRequestDescribeParametersPaginateTypeDef(
-    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
-    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
-):
-    pass
-
-
-DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedNodesOfferingId": str,
-        "NodeType": str,
-        "Duration": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservationId": str,
-        "ReservedNodesOfferingId": str,
-        "NodeType": str,
-        "Duration": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ClusterNames": Sequence[str],
-        "Status": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    {
-        "ClusterName": str,
-        "SnapshotName": str,
-        "Source": str,
-        "ShowDetail": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    {
-        "SubnetGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 DescribeEngineVersionsResponseTypeDef = TypedDict(
     "DescribeEngineVersionsResponseTypeDef",
     {
         "NextToken": str,
         "EngineVersions": List[EngineVersionInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParametersResponseTypeDef = TypedDict(
     "DescribeParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServiceUpdatesResponseTypeDef = TypedDict(
     "DescribeServiceUpdatesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     {
         "UserName": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
@@ -1353,73 +1354,73 @@
     total=False,
 )
 
 CreateACLResponseTypeDef = TypedDict(
     "CreateACLResponseTypeDef",
     {
         "ACL": ACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteACLResponseTypeDef = TypedDict(
     "DeleteACLResponseTypeDef",
     {
         "ACL": ACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeACLsResponseTypeDef = TypedDict(
     "DescribeACLsResponseTypeDef",
     {
         "ACLs": List[ACLTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateACLResponseTypeDef = TypedDict(
     "UpdateACLResponseTypeDef",
     {
         "ACL": ACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteUserResponseTypeDef = TypedDict(
     "DeleteUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetGroupTypeDef = TypedDict(
     "SubnetGroupTypeDef",
     {
         "Name": str,
@@ -1444,32 +1445,32 @@
 )
 
 DescribeReservedNodesResponseTypeDef = TypedDict(
     "DescribeReservedNodesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseReservedNodesOfferingResponseTypeDef = TypedDict(
     "PurchaseReservedNodesOfferingResponseTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedNodesOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedNodesOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedNodesOfferings": List[ReservedNodesOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterPendingUpdatesTypeDef = TypedDict(
     "ClusterPendingUpdatesTypeDef",
     {
         "Resharding": ReshardingStatusTypeDef,
@@ -1500,40 +1501,40 @@
     total=False,
 )
 
 CreateSubnetGroupResponseTypeDef = TypedDict(
     "CreateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSubnetGroupResponseTypeDef = TypedDict(
     "DeleteSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeSubnetGroupsResponseTypeDef",
     {
         "NextToken": str,
         "SubnetGroups": List[SubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSubnetGroupResponseTypeDef = TypedDict(
     "UpdateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "Name": str,
@@ -1581,84 +1582,84 @@
 )
 
 BatchUpdateClusterResponseTypeDef = TypedDict(
     "BatchUpdateClusterResponseTypeDef",
     {
         "ProcessedClusters": List[ClusterTypeDef],
         "UnprocessedClusters": List[UnprocessedClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "NextToken": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailoverShardResponseTypeDef = TypedDict(
     "FailoverShardResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopySnapshotResponseTypeDef = TypedDict(
     "CopySnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotsResponseTypeDef = TypedDict(
     "DescribeSnapshotsResponseTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/type_defs.pyi` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AuthenticationTypeType,
     AZStatusType,
     DataTieringStatusType,
+    InputAuthenticationTypeType,
     ServiceUpdateStatusType,
     SourceTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -35,63 +36,74 @@
 __all__ = (
     "ACLPendingChangesTypeDef",
     "ACLsUpdateStatusTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AvailabilityZoneTypeDef",
     "ServiceUpdateRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedClusterTypeDef",
     "PendingModifiedServiceUpdateTypeDef",
     "EndpointTypeDef",
     "SecurityGroupMembershipTypeDef",
     "TagTypeDef",
     "ParameterGroupTypeDef",
     "DeleteACLRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
     "DescribeACLsRequestRequestTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
+    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
     "DescribeEngineVersionsRequestRequestTypeDef",
     "EngineVersionInfoTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "EventTypeDef",
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
+    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "ParameterTypeDef",
+    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
     "DescribeReservedNodesOfferingsRequestRequestTypeDef",
+    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesRequestRequestTypeDef",
+    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesRequestRequestTypeDef",
     "ServiceUpdateTypeDef",
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "FilterTypeDef",
     "FailoverShardRequestRequestTypeDef",
     "ListAllowedNodeTypeUpdatesRequestRequestTypeDef",
+    "ListAllowedNodeTypeUpdatesResponseTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RecurringChargeTypeDef",
     "ReplicaConfigurationRequestTypeDef",
     "ResetParameterGroupRequestRequestTypeDef",
     "SlotMigrationTypeDef",
+    "ResponseMetadataTypeDef",
     "ShardConfigurationRequestTypeDef",
     "ShardConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateACLRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "ACLTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserTypeDef",
     "SubnetTypeDef",
     "BatchUpdateClusterRequestRequestTypeDef",
-    "ListAllowedNodeTypeUpdatesResponseTypeDef",
     "NodeTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateACLRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
@@ -102,25 +114,14 @@
     "TagResourceResponseTypeDef",
     "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DeleteParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "ResetParameterGroupResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
-    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
-    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
-    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
-    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeEngineVersionsResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "DescribeServiceUpdatesResponseTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
@@ -178,15 +179,15 @@
     },
     total=False,
 )
 
 AuthenticationModeTypeDef = TypedDict(
     "AuthenticationModeTypeDef",
     {
-        "Type": Literal["password"],
+        "Type": InputAuthenticationTypeType,
         "Passwords": Sequence[str],
     },
     total=False,
 )
 
 AuthenticationTypeDef = TypedDict(
     "AuthenticationTypeDef",
@@ -209,25 +210,14 @@
     "ServiceUpdateRequestTypeDef",
     {
         "ServiceUpdateNameToApply": str,
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
 UnprocessedClusterTypeDef = TypedDict(
     "UnprocessedClusterTypeDef",
     {
         "ClusterName": str,
         "ErrorType": str,
         "ErrorMessage": str,
     },
@@ -331,45 +321,65 @@
 DeleteUserRequestRequestTypeDef = TypedDict(
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeACLsRequestDescribeACLsPaginateTypeDef = TypedDict(
+    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ACLName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeACLsRequestRequestTypeDef = TypedDict(
     "DescribeACLsRequestRequestTypeDef",
     {
         "ACLName": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "ClusterName": str,
+        "ShowShardDetails": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "ClusterName": str,
         "MaxResults": int,
         "NextToken": str,
         "ShowShardDetails": bool,
     },
     total=False,
 )
 
+DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
+    {
+        "EngineVersion": str,
+        "ParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEngineVersionsRequestRequestTypeDef = TypedDict(
     "DescribeEngineVersionsRequestRequestTypeDef",
     {
         "EngineVersion": str,
         "ParameterGroupFamily": str,
         "MaxResults": int,
         "NextToken": str,
@@ -384,14 +394,27 @@
         "EngineVersion": str,
         "EnginePatchVersion": str,
         "ParameterGroupFamily": str,
     },
     total=False,
 )
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -409,24 +432,53 @@
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
     },
     total=False,
 )
 
+DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeParameterGroupsRequestRequestTypeDef = TypedDict(
     "DescribeParameterGroupsRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeParametersRequestDescribeParametersPaginateTypeDef(
+    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
+    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -453,41 +505,77 @@
         "DataType": str,
         "AllowedValues": str,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
+DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedNodesOfferingId": str,
+        "NodeType": str,
+        "Duration": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodesOfferingsRequestRequestTypeDef = TypedDict(
     "DescribeReservedNodesOfferingsRequestRequestTypeDef",
     {
         "ReservedNodesOfferingId": str,
         "NodeType": str,
         "Duration": str,
         "OfferingType": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservationId": str,
+        "ReservedNodesOfferingId": str,
+        "NodeType": str,
+        "Duration": str,
+        "OfferingType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodesRequestRequestTypeDef = TypedDict(
     "DescribeReservedNodesRequestRequestTypeDef",
     {
         "ReservationId": str,
         "ReservedNodesOfferingId": str,
         "NodeType": str,
         "Duration": str,
         "OfferingType": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ClusterNames": Sequence[str],
+        "Status": Sequence[ServiceUpdateStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeServiceUpdatesRequestRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesRequestRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ClusterNames": Sequence[str],
         "Status": Sequence[ServiceUpdateStatusType],
         "MaxResults": int,
@@ -507,27 +595,48 @@
         "Type": Literal["security-update"],
         "NodesUpdated": str,
         "AutoUpdateStartDate": datetime,
     },
     total=False,
 )
 
+DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    {
+        "ClusterName": str,
+        "SnapshotName": str,
+        "Source": str,
+        "ShowDetail": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "ClusterName": str,
         "SnapshotName": str,
         "Source": str,
         "NextToken": str,
         "MaxResults": int,
         "ShowDetail": bool,
     },
     total=False,
 )
 
+DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    {
+        "SubnetGroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSubnetGroupsRequestRequestTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -553,21 +662,40 @@
 ListAllowedNodeTypeUpdatesRequestRequestTypeDef = TypedDict(
     "ListAllowedNodeTypeUpdatesRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
+ListAllowedNodeTypeUpdatesResponseTypeDef = TypedDict(
+    "ListAllowedNodeTypeUpdatesResponseTypeDef",
+    {
+        "ScaleUpNodeTypes": List[str],
+        "ScaleDownNodeTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ParameterNameValueTypeDef = TypedDict(
     "ParameterNameValueTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -615,14 +743,25 @@
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
 ShardConfigurationRequestTypeDef = TypedDict(
     "ShardConfigurationRequestTypeDef",
     {
         "ShardCount": int,
     },
     total=False,
 )
@@ -757,23 +896,14 @@
 
 class BatchUpdateClusterRequestRequestTypeDef(
     _RequiredBatchUpdateClusterRequestRequestTypeDef,
     _OptionalBatchUpdateClusterRequestRequestTypeDef,
 ):
     pass
 
-ListAllowedNodeTypeUpdatesResponseTypeDef = TypedDict(
-    "ListAllowedNodeTypeUpdatesResponseTypeDef",
-    {
-        "ScaleUpNodeTypes": List[str],
-        "ScaleDownNodeTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "Name": str,
         "Status": str,
         "AvailabilityZone": str,
         "CreateTime": datetime,
@@ -948,15 +1078,15 @@
 ):
     pass
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef",
     {
         "ReservedNodesOfferingId": str,
@@ -986,238 +1116,109 @@
     },
 )
 
 TagResourceResponseTypeDef = TypedDict(
     "TagResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceResponseTypeDef = TypedDict(
     "UntagResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParameterGroupResponseTypeDef = TypedDict(
     "DeleteParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParameterGroupsResponseTypeDef = TypedDict(
     "DescribeParameterGroupsResponseTypeDef",
     {
         "NextToken": str,
         "ParameterGroups": List[ParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetParameterGroupResponseTypeDef = TypedDict(
     "ResetParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateParameterGroupResponseTypeDef = TypedDict(
     "UpdateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeACLsRequestDescribeACLsPaginateTypeDef = TypedDict(
-    "DescribeACLsRequestDescribeACLsPaginateTypeDef",
-    {
-        "ACLName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "ClusterName": str,
-        "ShowShardDetails": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef",
-    {
-        "EngineVersion": str,
-        "ParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeParametersRequestDescribeParametersPaginateTypeDef(
-    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
-    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
-):
-    pass
-
-DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedNodesOfferingId": str,
-        "NodeType": str,
-        "Duration": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservationId": str,
-        "ReservedNodesOfferingId": str,
-        "NodeType": str,
-        "Duration": str,
-        "OfferingType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ClusterNames": Sequence[str],
-        "Status": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    {
-        "ClusterName": str,
-        "SnapshotName": str,
-        "Source": str,
-        "ShowDetail": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    {
-        "SubnetGroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 DescribeEngineVersionsResponseTypeDef = TypedDict(
     "DescribeEngineVersionsResponseTypeDef",
     {
         "NextToken": str,
         "EngineVersions": List[EngineVersionInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParametersResponseTypeDef = TypedDict(
     "DescribeParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServiceUpdatesResponseTypeDef = TypedDict(
     "DescribeServiceUpdatesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     {
         "UserName": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
@@ -1318,73 +1319,73 @@
     total=False,
 )
 
 CreateACLResponseTypeDef = TypedDict(
     "CreateACLResponseTypeDef",
     {
         "ACL": ACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteACLResponseTypeDef = TypedDict(
     "DeleteACLResponseTypeDef",
     {
         "ACL": ACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeACLsResponseTypeDef = TypedDict(
     "DescribeACLsResponseTypeDef",
     {
         "ACLs": List[ACLTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateACLResponseTypeDef = TypedDict(
     "UpdateACLResponseTypeDef",
     {
         "ACL": ACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteUserResponseTypeDef = TypedDict(
     "DeleteUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetGroupTypeDef = TypedDict(
     "SubnetGroupTypeDef",
     {
         "Name": str,
@@ -1409,32 +1410,32 @@
 )
 
 DescribeReservedNodesResponseTypeDef = TypedDict(
     "DescribeReservedNodesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseReservedNodesOfferingResponseTypeDef = TypedDict(
     "PurchaseReservedNodesOfferingResponseTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedNodesOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedNodesOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedNodesOfferings": List[ReservedNodesOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterPendingUpdatesTypeDef = TypedDict(
     "ClusterPendingUpdatesTypeDef",
     {
         "Resharding": ReshardingStatusTypeDef,
@@ -1465,40 +1466,40 @@
     total=False,
 )
 
 CreateSubnetGroupResponseTypeDef = TypedDict(
     "CreateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSubnetGroupResponseTypeDef = TypedDict(
     "DeleteSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeSubnetGroupsResponseTypeDef",
     {
         "NextToken": str,
         "SubnetGroups": List[SubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSubnetGroupResponseTypeDef = TypedDict(
     "UpdateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "Name": str,
@@ -1546,84 +1547,84 @@
 )
 
 BatchUpdateClusterResponseTypeDef = TypedDict(
     "BatchUpdateClusterResponseTypeDef",
     {
         "ProcessedClusters": List[ClusterTypeDef],
         "UnprocessedClusters": List[UnprocessedClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "NextToken": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailoverShardResponseTypeDef = TypedDict(
     "FailoverShardResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopySnapshotResponseTypeDef = TypedDict(
     "CopySnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotsResponseTypeDef = TypedDict(
     "DescribeSnapshotsResponseTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/PKG-INFO` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.26.38
-Summary: Type annotations for boto3.MemoryDB 1.26.38 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.MemoryDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,63 +382,74 @@
 from mypy_boto3_memorydb.type_defs import (
     ACLPendingChangesTypeDef,
     ACLsUpdateStatusTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AvailabilityZoneTypeDef,
     ServiceUpdateRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedClusterTypeDef,
     PendingModifiedServiceUpdateTypeDef,
     EndpointTypeDef,
     SecurityGroupMembershipTypeDef,
     TagTypeDef,
     ParameterGroupTypeDef,
     DeleteACLRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeACLsRequestDescribeACLsPaginateTypeDef,
     DescribeACLsRequestRequestTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
+    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
+    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
     DescribeReservedNodesOfferingsRequestRequestTypeDef,
+    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesRequestRequestTypeDef,
+    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
     ServiceUpdateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
+    ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
+    ResponseMetadataTypeDef,
     ShardConfigurationRequestTypeDef,
     ShardConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateACLRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     ACLTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     SubnetTypeDef,
     BatchUpdateClusterRequestRequestTypeDef,
-    ListAllowedNodeTypeUpdatesResponseTypeDef,
     NodeTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
@@ -449,25 +460,14 @@
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
-    DescribeACLsRequestDescribeACLsPaginateTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
-    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
-    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
@@ -517,42 +517,42 @@
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

### Comparing `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/SOURCES.txt` & `mypy-boto3-memorydb-1.27.0/mypy_boto3_memorydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.26.38/setup.py` & `mypy-boto3-memorydb-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-memorydb.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-memorydb",
-    version="1.26.38",
+    version="1.27.0",
     packages=["mypy_boto3_memorydb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MemoryDB 1.26.38 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.MemoryDB 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/",
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


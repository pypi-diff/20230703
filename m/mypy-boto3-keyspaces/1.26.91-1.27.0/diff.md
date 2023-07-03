# Comparing `tmp/mypy-boto3-keyspaces-1.26.91.tar.gz` & `tmp/mypy-boto3-keyspaces-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-keyspaces-1.26.91.tar", last modified: Tue Mar 14 19:48:00 2023, max compression
+gzip compressed data, was "mypy-boto3-keyspaces-1.27.0.tar", last modified: Mon Jul  3 19:50:58 2023, max compression
```

## Comparing `mypy-boto3-keyspaces-1.26.91.tar` & `mypy-boto3-keyspaces-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-03-14 19:47:50.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.803509 mypy-boto3-keyspaces-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-03 19:50:58.799509 mypy-boto3-keyspaces-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.787509 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-03 19:40:17.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-07-03 19:40:17.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.799509 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-03 19:50:58.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:58.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:58.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:58.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:58.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:58.000000 mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:58.803509 mypy-boto3-keyspaces-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:40:16.000000 mypy-boto3-keyspaces-1.27.0/setup.py
```

### Comparing `mypy-boto3-keyspaces-1.26.91/LICENSE` & `mypy-boto3-keyspaces-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-keyspaces-1.26.91/PKG-INFO` & `mypy-boto3-keyspaces-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.26.91
-Summary: Type annotations for boto3.Keyspaces 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.Keyspaces 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-keyspaces"></a>
 
 # mypy-boto3-keyspaces
 
 [![PyPI - mypy-boto3-keyspaces](https://img.shields.io/pypi/v/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,14 +314,15 @@
     ListTablesPaginatorName,
     ListTagsForResourcePaginatorName,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
     ThroughputModeType,
     TimeToLiveStatusType,
+    rsType,
     KeyspacesServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -341,47 +342,48 @@
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
+    ReplicationSpecificationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateKeyspaceResponseTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
+    CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     GetKeyspaceRequestRequestTypeDef,
+    GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
     KeyspaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListKeyspacesRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PartitionKeyTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreTableResponseTypeDef,
     StaticColumnTypeDef,
+    UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateKeyspaceResponseTypeDef,
-    CreateTableResponseTypeDef,
-    GetKeyspaceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RestoreTableResponseTypeDef,
-    UpdateTableResponseTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
-    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
     SchemaDefinitionTypeDef,
     CreateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
 )
 
 
@@ -392,42 +394,42 @@
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

### Comparing `mypy-boto3-keyspaces-1.26.91/README.md` & `mypy-boto3-keyspaces-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-keyspaces"></a>
 
 # mypy-boto3-keyspaces
 
 [![PyPI - mypy-boto3-keyspaces](https://img.shields.io/pypi/v/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,14 +282,15 @@
     ListTablesPaginatorName,
     ListTagsForResourcePaginatorName,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
     ThroughputModeType,
     TimeToLiveStatusType,
+    rsType,
     KeyspacesServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -309,47 +310,48 @@
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
+    ReplicationSpecificationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateKeyspaceResponseTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
+    CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     GetKeyspaceRequestRequestTypeDef,
+    GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
     KeyspaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListKeyspacesRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PartitionKeyTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreTableResponseTypeDef,
     StaticColumnTypeDef,
+    UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateKeyspaceResponseTypeDef,
-    CreateTableResponseTypeDef,
-    GetKeyspaceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RestoreTableResponseTypeDef,
-    UpdateTableResponseTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
-    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
     SchemaDefinitionTypeDef,
     CreateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
 )
 
 
@@ -360,42 +362,42 @@
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

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.py` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.pyi` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__main__.py` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Keyspaces 1.26.91\nVersion:         1.26.91\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.Keyspaces 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.91")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.py` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     EncryptionSpecificationTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableResponseTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PointInTimeRecoveryTypeDef,
+    ReplicationSpecificationTypeDef,
     RestoreTableResponseTypeDef,
     SchemaDefinitionTypeDef,
     TagTypeDef,
     TimeToLiveTypeDef,
     UpdateTableResponseTypeDef,
 )
 
@@ -98,15 +99,19 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#close)
         """
 
     def create_keyspace(
-        self, *, keyspaceName: str, tags: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        keyspaceName: str,
+        tags: Sequence[TagTypeDef] = ...,
+        replicationSpecification: ReplicationSpecificationTypeDef = ...
     ) -> CreateKeyspaceResponseTypeDef:
         """
         The `CreateKeyspace` operation adds a new keyspace to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_keyspace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#create_keyspace)
         """
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.pyi` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     EncryptionSpecificationTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableResponseTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PointInTimeRecoveryTypeDef,
+    ReplicationSpecificationTypeDef,
     RestoreTableResponseTypeDef,
     SchemaDefinitionTypeDef,
     TagTypeDef,
     TimeToLiveTypeDef,
     UpdateTableResponseTypeDef,
 )
 
@@ -91,15 +92,19 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#close)
         """
     def create_keyspace(
-        self, *, keyspaceName: str, tags: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        keyspaceName: str,
+        tags: Sequence[TagTypeDef] = ...,
+        replicationSpecification: ReplicationSpecificationTypeDef = ...
     ) -> CreateKeyspaceResponseTypeDef:
         """
         The `CreateKeyspace` operation adds a new keyspace to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_keyspace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#create_keyspace)
         """
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.py` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,33 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ClientSideTimestampsStatusType",
     "EncryptionTypeType",
     "ListKeyspacesPaginatorName",
     "ListTablesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "PointInTimeRecoveryStatusType",
     "SortOrderType",
     "TableStatusType",
     "ThroughputModeType",
     "TimeToLiveStatusType",
+    "rsType",
     "KeyspacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ClientSideTimestampsStatusType = Literal["ENABLED"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 ListKeyspacesPaginatorName = Literal["list_keyspaces"]
 ListTablesPaginatorName = Literal["list_tables"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 PointInTimeRecoveryStatusType = Literal["DISABLED", "ENABLED"]
 SortOrderType = Literal["ASC", "DESC"]
@@ -52,14 +51,15 @@
     "DELETING",
     "INACCESSIBLE_ENCRYPTION_CREDENTIALS",
     "RESTORING",
     "UPDATING",
 ]
 ThroughputModeType = Literal["PAY_PER_REQUEST", "PROVISIONED"]
 TimeToLiveStatusType = Literal["ENABLED"]
+rsType = Literal["MULTI_REGION", "SINGLE_REGION"]
 KeyspacesServiceName = Literal["keyspaces"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -68,14 +68,15 @@
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
@@ -115,14 +116,15 @@
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
@@ -220,14 +222,15 @@
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
@@ -263,14 +266,15 @@
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
@@ -289,16 +293,19 @@
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
@@ -382,15 +389,17 @@
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
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.pyi` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,35 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ClientSideTimestampsStatusType",
     "EncryptionTypeType",
     "ListKeyspacesPaginatorName",
     "ListTablesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "PointInTimeRecoveryStatusType",
     "SortOrderType",
     "TableStatusType",
     "ThroughputModeType",
     "TimeToLiveStatusType",
+    "rsType",
     "KeyspacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ClientSideTimestampsStatusType = Literal["ENABLED"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 ListKeyspacesPaginatorName = Literal["list_keyspaces"]
 ListTablesPaginatorName = Literal["list_tables"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 PointInTimeRecoveryStatusType = Literal["DISABLED", "ENABLED"]
 SortOrderType = Literal["ASC", "DESC"]
@@ -50,14 +53,15 @@
     "DELETING",
     "INACCESSIBLE_ENCRYPTION_CREDENTIALS",
     "RESTORING",
     "UPDATING",
 ]
 ThroughputModeType = Literal["PAY_PER_REQUEST", "PROVISIONED"]
 TimeToLiveStatusType = Literal["ENABLED"]
+rsType = Literal["MULTI_REGION", "SINGLE_REGION"]
 KeyspacesServiceName = Literal["keyspaces"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -66,14 +70,15 @@
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
@@ -113,14 +118,15 @@
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
@@ -218,14 +224,15 @@
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
@@ -261,14 +268,15 @@
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
@@ -287,16 +295,19 @@
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
@@ -380,15 +391,17 @@
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
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.py` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 class ListKeyspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeyspacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
         """
 
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, keyspaceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, keyspaceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.pyi` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,41 +47,41 @@
 class ListKeyspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeyspacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
         """
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, keyspaceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, keyspaceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.py` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .literals import (
     EncryptionTypeType,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
     ThroughputModeType,
+    rsType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -36,47 +37,48 @@
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
     "ClientSideTimestampsTypeDef",
     "ClusteringKeyTypeDef",
     "ColumnDefinitionTypeDef",
     "CommentTypeDef",
+    "ReplicationSpecificationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateKeyspaceResponseTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
     "TimeToLiveTypeDef",
+    "CreateTableResponseTypeDef",
     "DeleteKeyspaceRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "GetKeyspaceRequestRequestTypeDef",
+    "GetKeyspaceResponseTypeDef",
     "GetTableRequestRequestTypeDef",
     "PointInTimeRecoverySummaryTypeDef",
     "KeyspaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PartitionKeyTypeDef",
+    "ResponseMetadataTypeDef",
+    "RestoreTableResponseTypeDef",
     "StaticColumnTypeDef",
+    "UpdateTableResponseTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateKeyspaceResponseTypeDef",
-    "CreateTableResponseTypeDef",
-    "GetKeyspaceResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RestoreTableResponseTypeDef",
-    "UpdateTableResponseTypeDef",
     "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTablesResponseTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
@@ -150,30 +152,48 @@
 CommentTypeDef = TypedDict(
     "CommentTypeDef",
     {
         "message": str,
     },
 )
 
+_RequiredReplicationSpecificationTypeDef = TypedDict(
+    "_RequiredReplicationSpecificationTypeDef",
+    {
+        "replicationStrategy": rsType,
+    },
+)
+_OptionalReplicationSpecificationTypeDef = TypedDict(
+    "_OptionalReplicationSpecificationTypeDef",
+    {
+        "regionList": Sequence[str],
+    },
+    total=False,
+)
+
+
+class ReplicationSpecificationTypeDef(
+    _RequiredReplicationSpecificationTypeDef, _OptionalReplicationSpecificationTypeDef
+):
+    pass
+
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateKeyspaceResponseTypeDef = TypedDict(
+    "CreateKeyspaceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEncryptionSpecificationTypeDef = TypedDict(
     "_RequiredEncryptionSpecificationTypeDef",
     {
         "type": EncryptionTypeType,
@@ -204,14 +224,22 @@
 TimeToLiveTypeDef = TypedDict(
     "TimeToLiveTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
+CreateTableResponseTypeDef = TypedDict(
+    "CreateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteKeyspaceRequestRequestTypeDef = TypedDict(
     "DeleteKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
@@ -226,14 +254,25 @@
 GetKeyspaceRequestRequestTypeDef = TypedDict(
     "GetKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
+GetKeyspaceResponseTypeDef = TypedDict(
+    "GetKeyspaceResponseTypeDef",
+    {
+        "keyspaceName": str,
+        "resourceArn": str,
+        "replicationStrategy": rsType,
+        "replicationRegions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTableRequestRequestTypeDef = TypedDict(
     "GetTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
@@ -255,41 +294,74 @@
 
 class PointInTimeRecoverySummaryTypeDef(
     _RequiredPointInTimeRecoverySummaryTypeDef, _OptionalPointInTimeRecoverySummaryTypeDef
 ):
     pass
 
 
-KeyspaceSummaryTypeDef = TypedDict(
-    "KeyspaceSummaryTypeDef",
+_RequiredKeyspaceSummaryTypeDef = TypedDict(
+    "_RequiredKeyspaceSummaryTypeDef",
     {
         "keyspaceName": str,
         "resourceArn": str,
+        "replicationStrategy": rsType,
+    },
+)
+_OptionalKeyspaceSummaryTypeDef = TypedDict(
+    "_OptionalKeyspaceSummaryTypeDef",
+    {
+        "replicationRegions": List[str],
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+class KeyspaceSummaryTypeDef(_RequiredKeyspaceSummaryTypeDef, _OptionalKeyspaceSummaryTypeDef):
+    pass
+
+
+ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListKeyspacesRequestRequestTypeDef = TypedDict(
     "ListKeyspacesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "keyspaceName": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -313,14 +385,36 @@
     {
         "keyspaceName": str,
         "tableName": str,
         "resourceArn": str,
     },
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
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
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -336,112 +430,109 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
     },
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
+RestoreTableResponseTypeDef = TypedDict(
+    "RestoreTableResponseTypeDef",
+    {
+        "restoredTableARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
+UpdateTableResponseTypeDef = TypedDict(
+    "UpdateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateKeyspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalCreateKeyspaceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKeyspaceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
+        "replicationSpecification": ReplicationSpecificationTypeDef,
     },
     total=False,
 )
 
 
 class CreateKeyspaceRequestRequestTypeDef(
     _RequiredCreateKeyspaceRequestRequestTypeDef, _OptionalCreateKeyspaceRequestRequestTypeDef
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateKeyspaceResponseTypeDef = TypedDict(
-    "CreateKeyspaceResponseTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTableResponseTypeDef = TypedDict(
-    "CreateTableResponseTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKeyspaceResponseTypeDef = TypedDict(
-    "GetKeyspaceResponseTypeDef",
-    {
-        "keyspaceName": str,
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "nextToken": str,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RestoreTableResponseTypeDef = TypedDict(
-    "RestoreTableResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "restoredTableARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
-UpdateTableResponseTypeDef = TypedDict(
-    "UpdateTableResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredRestoreTableRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreTableRequestRequestTypeDef",
     {
         "sourceKeyspaceName": str,
@@ -498,76 +589,24 @@
 
 
 ListKeyspacesResponseTypeDef = TypedDict(
     "ListKeyspacesResponseTypeDef",
     {
         "nextToken": str,
         "keyspaces": List[KeyspaceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "keyspaceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "nextToken": str,
         "tables": List[TableSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSchemaDefinitionTypeDef = TypedDict(
     "_RequiredSchemaDefinitionTypeDef",
     {
         "allColumns": Sequence[ColumnDefinitionTypeDef],
@@ -630,10 +669,10 @@
         "capacitySpecification": CapacitySpecificationSummaryTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
         "comment": CommentTypeDef,
         "clientSideTimestamps": ClientSideTimestampsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.pyi` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .literals import (
     EncryptionTypeType,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
     ThroughputModeType,
+    rsType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -35,47 +36,48 @@
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
     "ClientSideTimestampsTypeDef",
     "ClusteringKeyTypeDef",
     "ColumnDefinitionTypeDef",
     "CommentTypeDef",
+    "ReplicationSpecificationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateKeyspaceResponseTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
     "TimeToLiveTypeDef",
+    "CreateTableResponseTypeDef",
     "DeleteKeyspaceRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "GetKeyspaceRequestRequestTypeDef",
+    "GetKeyspaceResponseTypeDef",
     "GetTableRequestRequestTypeDef",
     "PointInTimeRecoverySummaryTypeDef",
     "KeyspaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PartitionKeyTypeDef",
+    "ResponseMetadataTypeDef",
+    "RestoreTableResponseTypeDef",
     "StaticColumnTypeDef",
+    "UpdateTableResponseTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateKeyspaceResponseTypeDef",
-    "CreateTableResponseTypeDef",
-    "GetKeyspaceResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RestoreTableResponseTypeDef",
-    "UpdateTableResponseTypeDef",
     "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTablesResponseTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
@@ -145,30 +147,46 @@
 CommentTypeDef = TypedDict(
     "CommentTypeDef",
     {
         "message": str,
     },
 )
 
+_RequiredReplicationSpecificationTypeDef = TypedDict(
+    "_RequiredReplicationSpecificationTypeDef",
+    {
+        "replicationStrategy": rsType,
+    },
+)
+_OptionalReplicationSpecificationTypeDef = TypedDict(
+    "_OptionalReplicationSpecificationTypeDef",
+    {
+        "regionList": Sequence[str],
+    },
+    total=False,
+)
+
+class ReplicationSpecificationTypeDef(
+    _RequiredReplicationSpecificationTypeDef, _OptionalReplicationSpecificationTypeDef
+):
+    pass
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateKeyspaceResponseTypeDef = TypedDict(
+    "CreateKeyspaceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEncryptionSpecificationTypeDef = TypedDict(
     "_RequiredEncryptionSpecificationTypeDef",
     {
         "type": EncryptionTypeType,
@@ -197,14 +215,22 @@
 TimeToLiveTypeDef = TypedDict(
     "TimeToLiveTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
+CreateTableResponseTypeDef = TypedDict(
+    "CreateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteKeyspaceRequestRequestTypeDef = TypedDict(
     "DeleteKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
@@ -219,14 +245,25 @@
 GetKeyspaceRequestRequestTypeDef = TypedDict(
     "GetKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
+GetKeyspaceResponseTypeDef = TypedDict(
+    "GetKeyspaceResponseTypeDef",
+    {
+        "keyspaceName": str,
+        "resourceArn": str,
+        "replicationStrategy": rsType,
+        "replicationRegions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTableRequestRequestTypeDef = TypedDict(
     "GetTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
@@ -246,41 +283,70 @@
 )
 
 class PointInTimeRecoverySummaryTypeDef(
     _RequiredPointInTimeRecoverySummaryTypeDef, _OptionalPointInTimeRecoverySummaryTypeDef
 ):
     pass
 
-KeyspaceSummaryTypeDef = TypedDict(
-    "KeyspaceSummaryTypeDef",
+_RequiredKeyspaceSummaryTypeDef = TypedDict(
+    "_RequiredKeyspaceSummaryTypeDef",
     {
         "keyspaceName": str,
         "resourceArn": str,
+        "replicationStrategy": rsType,
+    },
+)
+_OptionalKeyspaceSummaryTypeDef = TypedDict(
+    "_OptionalKeyspaceSummaryTypeDef",
+    {
+        "replicationRegions": List[str],
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+class KeyspaceSummaryTypeDef(_RequiredKeyspaceSummaryTypeDef, _OptionalKeyspaceSummaryTypeDef):
+    pass
+
+ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListKeyspacesRequestRequestTypeDef = TypedDict(
     "ListKeyspacesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "keyspaceName": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
+):
+    pass
+
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -302,14 +368,34 @@
     {
         "keyspaceName": str,
         "tableName": str,
         "resourceArn": str,
     },
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
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
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -323,110 +409,107 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-PartitionKeyTypeDef = TypedDict(
-    "PartitionKeyTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-StaticColumnTypeDef = TypedDict(
-    "StaticColumnTypeDef",
+PartitionKeyTypeDef = TypedDict(
+    "PartitionKeyTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredCreateKeyspaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyspaceRequestRequestTypeDef",
-    {
-        "keyspaceName": str,
-    },
-)
-_OptionalCreateKeyspaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyspaceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class CreateKeyspaceRequestRequestTypeDef(
-    _RequiredCreateKeyspaceRequestRequestTypeDef, _OptionalCreateKeyspaceRequestRequestTypeDef
-):
-    pass
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+RestoreTableResponseTypeDef = TypedDict(
+    "RestoreTableResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "restoredTableARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StaticColumnTypeDef = TypedDict(
+    "StaticColumnTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "name": str,
     },
 )
 
-CreateKeyspaceResponseTypeDef = TypedDict(
-    "CreateKeyspaceResponseTypeDef",
+UpdateTableResponseTypeDef = TypedDict(
+    "UpdateTableResponseTypeDef",
     {
         "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTableResponseTypeDef = TypedDict(
-    "CreateTableResponseTypeDef",
+_RequiredCreateKeyspaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyspaceRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "keyspaceName": str,
     },
 )
-
-GetKeyspaceResponseTypeDef = TypedDict(
-    "GetKeyspaceResponseTypeDef",
+_OptionalCreateKeyspaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyspaceRequestRequestTypeDef",
     {
-        "keyspaceName": str,
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "replicationSpecification": ReplicationSpecificationTypeDef,
     },
+    total=False,
 )
 
+class CreateKeyspaceRequestRequestTypeDef(
+    _RequiredCreateKeyspaceRequestRequestTypeDef, _OptionalCreateKeyspaceRequestRequestTypeDef
+):
+    pass
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "nextToken": str,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RestoreTableResponseTypeDef = TypedDict(
-    "RestoreTableResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "restoredTableARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
-UpdateTableResponseTypeDef = TypedDict(
-    "UpdateTableResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredRestoreTableRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreTableRequestRequestTypeDef",
     {
         "sourceKeyspaceName": str,
@@ -479,72 +562,24 @@
     pass
 
 ListKeyspacesResponseTypeDef = TypedDict(
     "ListKeyspacesResponseTypeDef",
     {
         "nextToken": str,
         "keyspaces": List[KeyspaceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "keyspaceName": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "nextToken": str,
         "tables": List[TableSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSchemaDefinitionTypeDef = TypedDict(
     "_RequiredSchemaDefinitionTypeDef",
     {
         "allColumns": Sequence[ColumnDefinitionTypeDef],
@@ -603,10 +638,10 @@
         "capacitySpecification": CapacitySpecificationSummaryTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
         "comment": CommentTypeDef,
         "clientSideTimestamps": ClientSideTimestampsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/PKG-INFO` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.26.91
-Summary: Type annotations for boto3.Keyspaces 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.Keyspaces 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-keyspaces"></a>
 
 # mypy-boto3-keyspaces
 
 [![PyPI - mypy-boto3-keyspaces](https://img.shields.io/pypi/v/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,14 +314,15 @@
     ListTablesPaginatorName,
     ListTagsForResourcePaginatorName,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
     ThroughputModeType,
     TimeToLiveStatusType,
+    rsType,
     KeyspacesServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -341,47 +342,48 @@
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
     ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
+    ReplicationSpecificationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateKeyspaceResponseTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
+    CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     GetKeyspaceRequestRequestTypeDef,
+    GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
     KeyspaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListKeyspacesRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PartitionKeyTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreTableResponseTypeDef,
     StaticColumnTypeDef,
+    UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateKeyspaceResponseTypeDef,
-    CreateTableResponseTypeDef,
-    GetKeyspaceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RestoreTableResponseTypeDef,
-    UpdateTableResponseTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
-    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
     SchemaDefinitionTypeDef,
     CreateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
 )
 
 
@@ -392,42 +394,42 @@
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

### Comparing `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/SOURCES.txt` & `mypy-boto3-keyspaces-1.27.0/mypy_boto3_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.91/setup.py` & `mypy-boto3-keyspaces-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-keyspaces.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-keyspaces",
-    version="1.26.91",
+    version="1.27.0",
     packages=["mypy_boto3_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Keyspaces 1.26.91 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.Keyspaces 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/",
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


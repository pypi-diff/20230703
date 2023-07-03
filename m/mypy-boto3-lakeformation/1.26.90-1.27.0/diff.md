# Comparing `tmp/mypy-boto3-lakeformation-1.26.90.tar.gz` & `tmp/mypy-boto3-lakeformation-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.26.90.tar", last modified: Mon Mar 13 19:32:22 2023, max compression
+gzip compressed data, was "mypy-boto3-lakeformation-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-lakeformation-1.26.90.tar` & `mypy-boto3-lakeformation-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-lakeformation-1.26.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-03-13 19:32:22.895340 mypy-boto3-lakeformation-1.26.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36981 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36922 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-03-13 19:32:04.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-03-13 19:32:04.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47768 2023-03-13 19:32:05.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47685 2023-03-13 19:32:05.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-03-13 19:32:22.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-13 19:32:22.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 19:32:22.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 19:32:22.000000 mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:32:22.895340 mypy-boto3-lakeformation-1.26.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-13 19:32:03.000000 mypy-boto3-lakeformation-1.26.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.015549 mypy-boto3-lakeformation-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-03 19:51:01.011549 mypy-boto3-lakeformation-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.007549 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37031 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-03 19:40:34.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-03 19:40:34.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-03 19:40:34.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48249 2023-07-03 19:40:35.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48164 2023-07-03 19:40:34.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.011549 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-03 19:51:00.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:51:00.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:00.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:00.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:00.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:00.000000 mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.015549 mypy-boto3-lakeformation-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:40:33.000000 mypy-boto3-lakeformation-1.27.0/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.26.90/LICENSE` & `mypy-boto3-lakeformation-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lakeformation-1.26.90/PKG-INFO` & `mypy-boto3-lakeformation-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.26.90
-Summary: Type annotations for boto3.LakeFormation 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LakeFormation 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,23 +352,24 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
-    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
+    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
@@ -383,49 +384,50 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
+    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
+    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartQueryPlanningResponseTypeDef,
     StartTransactionRequestRequestTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    UpdateTableStorageOptimizerResponseTypeDef,
     ColumnLFTagTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
-    CommitTransactionResponseTypeDef,
-    GetLFTagResponseTypeDef,
-    GetQueryStateResponseTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
     ListLFTagsResponseTypeDef,
-    StartQueryPlanningResponseTypeDef,
-    StartTransactionResponseTypeDef,
-    UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     LFTagErrorTypeDef,
     PrincipalPermissionsTypeDef,
     TableWithColumnsResourceTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
@@ -433,16 +435,14 @@
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
@@ -491,42 +491,42 @@
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

### Comparing `mypy-boto3-lakeformation-1.26.90/README.md` & `mypy-boto3-lakeformation-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,23 +320,24 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
-    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
+    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
@@ -351,49 +352,50 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
+    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
+    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartQueryPlanningResponseTypeDef,
     StartTransactionRequestRequestTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    UpdateTableStorageOptimizerResponseTypeDef,
     ColumnLFTagTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
-    CommitTransactionResponseTypeDef,
-    GetLFTagResponseTypeDef,
-    GetQueryStateResponseTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
     ListLFTagsResponseTypeDef,
-    StartQueryPlanningResponseTypeDef,
-    StartTransactionResponseTypeDef,
-    UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     LFTagErrorTypeDef,
     PrincipalPermissionsTypeDef,
     TableWithColumnsResourceTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
@@ -401,16 +403,14 @@
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
@@ -459,42 +459,42 @@
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

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/__init__.py` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/__init__.pyi` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/client.py` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,15 +574,20 @@
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#put_data_lake_settings)
         """
 
     def register_resource(
-        self, *, ResourceArn: str, UseServiceLinkedRole: bool = ..., RoleArn: str = ...
+        self,
+        *,
+        ResourceArn: str,
+        UseServiceLinkedRole: bool = ...,
+        RoleArn: str = ...,
+        WithFederation: bool = ...
     ) -> Dict[str, Any]:
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#register_resource)
         """
@@ -634,15 +639,15 @@
         *,
         Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
-        This operation allows a search on `TABLE` resources by `LFTag` s.
+        This operation allows a search on `TABLE` resources by `LFTag`s.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_tables_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_tables_by_lf_tags)
         """
 
     def start_query_planning(
         self, *, QueryPlanningContext: QueryPlanningContextTypeDef, QueryString: str
@@ -683,15 +688,17 @@
         """
         Updates the list of possible values for the specified LF-tag key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_lf_tag)
         """
 
-    def update_resource(self, *, RoleArn: str, ResourceArn: str) -> Dict[str, Any]:
+    def update_resource(
+        self, *, RoleArn: str, ResourceArn: str, WithFederation: bool = ...
+    ) -> Dict[str, Any]:
         """
         Updates the data access role used for vending access to the given (registered)
         resource in Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_resource)
         """
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/client.pyi` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,20 @@
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#put_data_lake_settings)
         """
     def register_resource(
-        self, *, ResourceArn: str, UseServiceLinkedRole: bool = ..., RoleArn: str = ...
+        self,
+        *,
+        ResourceArn: str,
+        UseServiceLinkedRole: bool = ...,
+        RoleArn: str = ...,
+        WithFederation: bool = ...
     ) -> Dict[str, Any]:
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#register_resource)
         """
@@ -587,15 +592,15 @@
         *,
         Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
-        This operation allows a search on `TABLE` resources by `LFTag` s.
+        This operation allows a search on `TABLE` resources by `LFTag`s.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_tables_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_tables_by_lf_tags)
         """
     def start_query_planning(
         self, *, QueryPlanningContext: QueryPlanningContextTypeDef, QueryString: str
     ) -> StartQueryPlanningResponseTypeDef:
@@ -631,15 +636,17 @@
     ) -> Dict[str, Any]:
         """
         Updates the list of possible values for the specified LF-tag key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_lf_tag)
         """
-    def update_resource(self, *, RoleArn: str, ResourceArn: str) -> Dict[str, Any]:
+    def update_resource(
+        self, *, RoleArn: str, ResourceArn: str, WithFederation: bool = ...
+    ) -> Dict[str, Any]:
         """
         Updates the data access role used for vending access to the given (registered)
         resource in Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_resource)
         """
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/literals.py` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -293,14 +296,15 @@
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
@@ -319,16 +323,19 @@
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
@@ -412,15 +419,17 @@
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
@@ -457,19 +466,22 @@
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/literals.pyi` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
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
@@ -143,14 +144,15 @@
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
@@ -291,14 +294,15 @@
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
@@ -317,16 +321,19 @@
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
@@ -410,15 +417,17 @@
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
@@ -455,19 +464,22 @@
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/paginator.py` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,103 +47,96 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
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
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
-
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
-
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
-
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
-
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/paginator.pyi` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,96 +47,103 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
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
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
+
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
+
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
+
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
+
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/type_defs.py` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LFTagPairTypeDef",
-    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
+    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
@@ -67,49 +68,50 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
+    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
+    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
     "LFTagKeyResourceTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartQueryPlanningResponseTypeDef",
     "StartTransactionRequestRequestTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "UpdateTableStorageOptimizerResponseTypeDef",
     "ColumnLFTagTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    "CommitTransactionResponseTypeDef",
-    "GetLFTagResponseTypeDef",
-    "GetQueryStateResponseTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
     "ListLFTagsResponseTypeDef",
-    "StartQueryPlanningResponseTypeDef",
-    "StartTransactionResponseTypeDef",
-    "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     "LFTagErrorTypeDef",
     "PrincipalPermissionsTypeDef",
     "TableWithColumnsResourceTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
@@ -117,16 +119,14 @@
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
     "LFTagPolicyResourceTypeDef",
     "SearchDatabasesByLFTagsRequestRequestTypeDef",
     "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
@@ -183,25 +183,14 @@
 )
 
 
 class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
     pass
 
 
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
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -239,14 +228,25 @@
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
 
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
@@ -286,14 +286,22 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
+    {
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -461,14 +469,15 @@
 
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
+        "WithFederation": bool,
     },
     total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
@@ -582,21 +591,40 @@
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
 
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -641,33 +669,75 @@
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "QueryId": str,
+    },
+)
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -740,14 +810,24 @@
 )
 
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
 
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -800,14 +880,24 @@
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
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
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -845,33 +935,61 @@
     },
 )
 _OptionalRegisterResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterResourceRequestRequestTypeDef",
     {
         "UseServiceLinkedRole": bool,
         "RoleArn": str,
+        "WithFederation": bool,
     },
     total=False,
 )
 
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
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
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -887,21 +1005,35 @@
 
 class UpdateLFTagRequestRequestTypeDef(
     _RequiredUpdateLFTagRequestRequestTypeDef, _OptionalUpdateLFTagRequestRequestTypeDef
 ):
     pass
 
 
-UpdateResourceRequestRequestTypeDef = TypedDict(
-    "UpdateResourceRequestRequestTypeDef",
+_RequiredUpdateResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourceRequestRequestTypeDef",
     {
         "RoleArn": str,
         "ResourceArn": str,
     },
 )
+_OptionalUpdateResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourceRequestRequestTypeDef",
+    {
+        "WithFederation": bool,
+    },
+    total=False,
+)
+
+
+class UpdateResourceRequestRequestTypeDef(
+    _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableStorageOptimizerRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "StorageOptimizerConfig": Mapping[OptimizerTypeType, Mapping[str, str]],
@@ -919,121 +1051,37 @@
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
+    "UpdateTableStorageOptimizerResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairTypeDef],
     },
     total=False,
 )
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
-    "UpdateTableStorageOptimizerResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1168,41 +1216,41 @@
     pass
 
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1214,15 +1262,15 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1244,53 +1292,21 @@
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
-
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetWorkUnitsResponseTypeDef = TypedDict(
     "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
@@ -1342,15 +1358,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
     _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
@@ -1389,15 +1405,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
     _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
@@ -1406,15 +1422,15 @@
     pass
 
 
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1426,15 +1442,15 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
@@ -1453,15 +1469,15 @@
 
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
         "LFTagOnDatabase": List[LFTagPairTypeDef],
         "LFTagsOnTable": List[LFTagPairTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
         "Table": TableResourceTypeDef,
@@ -1472,23 +1488,23 @@
     total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": List[DataLakePrincipalTypeDef],
@@ -1510,24 +1526,24 @@
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilter": DataCellsFilterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilters": List[DataCellsFilterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
@@ -1535,15 +1551,15 @@
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1584,32 +1600,32 @@
 )
 
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchTablesByLFTagsResponseTypeDef = TypedDict(
     "SearchTablesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
@@ -1851,35 +1867,35 @@
 
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation/type_defs.pyi` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LFTagPairTypeDef",
-    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
+    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
@@ -66,49 +67,50 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
+    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
+    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
     "LFTagKeyResourceTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartQueryPlanningResponseTypeDef",
     "StartTransactionRequestRequestTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "UpdateTableStorageOptimizerResponseTypeDef",
     "ColumnLFTagTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    "CommitTransactionResponseTypeDef",
-    "GetLFTagResponseTypeDef",
-    "GetQueryStateResponseTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
     "ListLFTagsResponseTypeDef",
-    "StartQueryPlanningResponseTypeDef",
-    "StartTransactionResponseTypeDef",
-    "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     "LFTagErrorTypeDef",
     "PrincipalPermissionsTypeDef",
     "TableWithColumnsResourceTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
@@ -116,16 +118,14 @@
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
     "LFTagPolicyResourceTypeDef",
     "SearchDatabasesByLFTagsRequestRequestTypeDef",
     "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
@@ -180,25 +180,14 @@
     },
     total=False,
 )
 
 class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
     pass
 
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
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -232,14 +221,25 @@
 
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
@@ -279,14 +279,22 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
+    {
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -442,14 +450,15 @@
 
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
+        "WithFederation": bool,
     },
     total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
@@ -559,21 +568,40 @@
 )
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -616,33 +644,73 @@
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "QueryId": str,
+    },
+)
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -709,14 +777,24 @@
     },
     total=False,
 )
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -767,14 +845,24 @@
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
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
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -810,31 +898,59 @@
     },
 )
 _OptionalRegisterResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterResourceRequestRequestTypeDef",
     {
         "UseServiceLinkedRole": bool,
         "RoleArn": str,
+        "WithFederation": bool,
     },
     total=False,
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
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
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -848,21 +964,33 @@
 )
 
 class UpdateLFTagRequestRequestTypeDef(
     _RequiredUpdateLFTagRequestRequestTypeDef, _OptionalUpdateLFTagRequestRequestTypeDef
 ):
     pass
 
-UpdateResourceRequestRequestTypeDef = TypedDict(
-    "UpdateResourceRequestRequestTypeDef",
+_RequiredUpdateResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourceRequestRequestTypeDef",
     {
         "RoleArn": str,
         "ResourceArn": str,
     },
 )
+_OptionalUpdateResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourceRequestRequestTypeDef",
+    {
+        "WithFederation": bool,
+    },
+    total=False,
+)
+
+class UpdateResourceRequestRequestTypeDef(
+    _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
+):
+    pass
 
 _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableStorageOptimizerRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "StorageOptimizerConfig": Mapping[OptimizerTypeType, Mapping[str, str]],
@@ -878,121 +1006,37 @@
 
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
+UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
+    "UpdateTableStorageOptimizerResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairTypeDef],
     },
     total=False,
 )
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
-    "UpdateTableStorageOptimizerResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1119,41 +1163,41 @@
 ):
     pass
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1165,15 +1209,15 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1193,51 +1237,21 @@
 
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetWorkUnitsResponseTypeDef = TypedDict(
     "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
@@ -1285,15 +1299,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
     _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
@@ -1328,30 +1342,30 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
     _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
 ):
     pass
 
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1363,15 +1377,15 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
@@ -1390,15 +1404,15 @@
 
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
         "LFTagOnDatabase": List[LFTagPairTypeDef],
         "LFTagsOnTable": List[LFTagPairTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
         "Table": TableResourceTypeDef,
@@ -1409,23 +1423,23 @@
     total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": List[DataLakePrincipalTypeDef],
@@ -1447,24 +1461,24 @@
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilter": DataCellsFilterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilters": List[DataCellsFilterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
@@ -1472,15 +1486,15 @@
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1519,32 +1533,32 @@
 )
 
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchTablesByLFTagsResponseTypeDef = TypedDict(
     "SearchTablesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
@@ -1768,35 +1782,35 @@
     pass
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.26.90
-Summary: Type annotations for boto3.LakeFormation 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LakeFormation 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,23 +352,24 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
-    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
+    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
@@ -383,49 +384,50 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
+    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
+    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartQueryPlanningResponseTypeDef,
     StartTransactionRequestRequestTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    UpdateTableStorageOptimizerResponseTypeDef,
     ColumnLFTagTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
-    CommitTransactionResponseTypeDef,
-    GetLFTagResponseTypeDef,
-    GetQueryStateResponseTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
     ListLFTagsResponseTypeDef,
-    StartQueryPlanningResponseTypeDef,
-    StartTransactionResponseTypeDef,
-    UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     LFTagErrorTypeDef,
     PrincipalPermissionsTypeDef,
     TableWithColumnsResourceTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
@@ -433,16 +435,14 @@
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
@@ -491,42 +491,42 @@
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

### Comparing `mypy-boto3-lakeformation-1.26.90/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy-boto3-lakeformation-1.27.0/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.26.90/setup.py` & `mypy-boto3-lakeformation-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-lakeformation.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.26.90",
+    version="1.27.0",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LakeFormation 1.26.90 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.LakeFormation 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/",
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


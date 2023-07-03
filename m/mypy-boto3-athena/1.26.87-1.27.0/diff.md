# Comparing `tmp/mypy-boto3-athena-1.26.87.tar.gz` & `tmp/mypy-boto3-athena-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-athena-1.26.87.tar", last modified: Wed Mar  8 20:35:46 2023, max compression
+gzip compressed data, was "mypy-boto3-athena-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-athena-1.26.87.tar` & `mypy-boto3-athena-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.194592 mypy-boto3-athena-1.26.87/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41676 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41602 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57696 2023-03-08 20:34:16.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57613 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.798862 mypy-boto3-athena-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-07-03 19:50:24.798862 mypy-boto3-athena-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.798862 mypy-boto3-athena-1.27.0/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-03 19:32:50.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62804 2023-07-03 19:32:51.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62715 2023-07-03 19:32:50.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.798862 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-07-03 19:50:24.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:24.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:24.000000 mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.798862 mypy-boto3-athena-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:32:49.000000 mypy-boto3-athena-1.27.0/setup.py
```

### Comparing `mypy-boto3-athena-1.26.87/LICENSE` & `mypy-boto3-athena-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-athena-1.26.87/PKG-INFO` & `mypy-boto3-athena-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.26.87
-Summary: Type annotations for boto3.Athena 1.26.87 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Athena 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-athena"></a>
 
 # mypy-boto3-athena
 
 [![PyPI - mypy-boto3-athena](https://img.shields.io/pypi/v/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,14 +317,16 @@
 
 `mypy_boto3_athena.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_athena.literals import (
     CalculationExecutionStateType,
+    CapacityAllocationStatusType,
+    CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
     ExecutorStateType,
     ExecutorTypeType,
     GetQueryResultsPaginatorName,
     ListDataCatalogsPaginatorName,
@@ -361,124 +363,143 @@
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
+    CancelCapacityReservationInputRequestTypeDef,
+    CapacityAllocationTypeDef,
+    CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
+    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
+    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
+    DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
     EngineConfigurationTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
+    GetCapacityAssignmentConfigurationInputRequestTypeDef,
+    GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
+    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
+    ListCapacityReservationsInputRequestTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
+    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
+    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
+    ResponseMetadataTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
+    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
+    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
-    CreateNamedQueryOutputTypeDef,
-    CreateNotebookOutputTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
-    ImportNotebookOutputTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
-    ListNamedQueriesOutputTypeDef,
-    ListQueryExecutionsOutputTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
-    StopCalculationExecutionResponseTypeDef,
-    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
+    CapacityReservationTypeDef,
+    CapacityAssignmentConfigurationTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
+    CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
@@ -490,29 +511,25 @@
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
+    GetCapacityReservationOutputTypeDef,
+    ListCapacityReservationsOutputTypeDef,
+    GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -537,42 +554,42 @@
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

### Comparing `mypy-boto3-athena-1.26.87/README.md` & `mypy-boto3-athena-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-athena"></a>
 
 # mypy-boto3-athena
 
 [![PyPI - mypy-boto3-athena](https://img.shields.io/pypi/v/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,14 +285,16 @@
 
 `mypy_boto3_athena.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_athena.literals import (
     CalculationExecutionStateType,
+    CapacityAllocationStatusType,
+    CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
     ExecutorStateType,
     ExecutorTypeType,
     GetQueryResultsPaginatorName,
     ListDataCatalogsPaginatorName,
@@ -329,124 +331,143 @@
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
+    CancelCapacityReservationInputRequestTypeDef,
+    CapacityAllocationTypeDef,
+    CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
+    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
+    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
+    DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
     EngineConfigurationTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
+    GetCapacityAssignmentConfigurationInputRequestTypeDef,
+    GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
+    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
+    ListCapacityReservationsInputRequestTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
+    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
+    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
+    ResponseMetadataTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
+    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
+    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
-    CreateNamedQueryOutputTypeDef,
-    CreateNotebookOutputTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
-    ImportNotebookOutputTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
-    ListNamedQueriesOutputTypeDef,
-    ListQueryExecutionsOutputTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
-    StopCalculationExecutionResponseTypeDef,
-    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
+    CapacityReservationTypeDef,
+    CapacityAssignmentConfigurationTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
+    CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
@@ -458,29 +479,25 @@
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
+    GetCapacityReservationOutputTypeDef,
+    ListCapacityReservationsOutputTypeDef,
+    GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -505,42 +522,42 @@
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

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.26.87\nVersion:         1.26.87\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.Athena 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.87")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,23 +35,26 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
+    CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
     EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
+    GetCapacityAssignmentConfigurationOutputTypeDef,
+    GetCapacityReservationOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetNamedQueryOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetQueryResultsOutputTypeDef,
@@ -59,14 +62,15 @@
     GetSessionResponseTypeDef,
     GetSessionStatusResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     GetWorkGroupOutputTypeDef,
     ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesOutputTypeDef,
     ListCalculationExecutionsResponseTypeDef,
+    ListCapacityReservationsOutputTypeDef,
     ListDatabasesOutputTypeDef,
     ListDataCatalogsOutputTypeDef,
     ListEngineVersionsOutputTypeDef,
     ListExecutorsResponseTypeDef,
     ListNamedQueriesOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookSessionsResponseTypeDef,
@@ -170,22 +174,41 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#can_paginate)
         """
 
+    def cancel_capacity_reservation(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Cancels the capacity reservation with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.cancel_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#cancel_capacity_reservation)
+        """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#close)
         """
 
+    def create_capacity_reservation(
+        self, *, TargetDpus: int, Name: str, Tags: Sequence[TagTypeDef] = ...
+    ) -> Dict[str, Any]:
+        """
+        Creates a capacity reservation with the specified name and number of requested
+        data processing units.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_capacity_reservation)
+        """
+
     def create_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
         Parameters: Mapping[str, str] = ...,
@@ -256,14 +279,22 @@
         """
         Creates a workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_work_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_work_group)
         """
 
+    def delete_capacity_reservation(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes a cancelled capacity reservation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_capacity_reservation)
+        """
+
     def delete_data_catalog(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes a data catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_data_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_data_catalog)
         """
@@ -336,16 +367,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution)
         """
 
     def get_calculation_execution_code(
         self, *, CalculationExecutionId: str
     ) -> GetCalculationExecutionCodeResponseTypeDef:
         """
-        Retrieves a pre-signed URL to a copy of the code that was executed for the
-        calculation.
+        Retrieves the unencrypted code that was executed for the calculation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_code)
         """
 
     def get_calculation_execution_status(
         self, *, CalculationExecutionId: str
@@ -353,14 +383,33 @@
         """
         Gets the status of a current calculation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_status)
         """
 
+    def get_capacity_assignment_configuration(
+        self, *, CapacityReservationName: str
+    ) -> GetCapacityAssignmentConfigurationOutputTypeDef:
+        """
+        Gets the capacity assignment configuration for a capacity reservation, if one
+        exists.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_capacity_assignment_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_capacity_assignment_configuration)
+        """
+
+    def get_capacity_reservation(self, *, Name: str) -> GetCapacityReservationOutputTypeDef:
+        """
+        Returns information about the capacity reservation with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_capacity_reservation)
+        """
+
     def get_data_catalog(self, *, Name: str) -> GetDataCatalogOutputTypeDef:
         """
         Returns the specified data catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_data_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_data_catalog)
         """
@@ -483,15 +532,15 @@
         """
 
     def list_application_dpu_sizes(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListApplicationDPUSizesOutputTypeDef:
         """
         Returns the supported DPU sizes for the supported application runtimes (for
-        example, `Jupyter 1.0` ).
+        example, `Athena notebook version 1`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_application_dpu_sizes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_application_dpu_sizes)
         """
 
     def list_calculation_executions(
         self,
@@ -505,14 +554,24 @@
         Lists the calculations that have been submitted to a session in descending
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_calculation_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_calculation_executions)
         """
 
+    def list_capacity_reservations(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListCapacityReservationsOutputTypeDef:
+        """
+        Lists the capacity reservations for the current account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_capacity_reservations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_capacity_reservations)
+        """
+
     def list_data_catalogs(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCatalogsOutputTypeDef:
         """
         Lists the data catalogs in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_data_catalogs)
@@ -545,15 +604,15 @@
         *,
         SessionId: str,
         ExecutorStateFilter: ExecutorStateType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListExecutorsResponseTypeDef:
         """
-        Lists, in descending order, the executors that have been submitted to a session.
+        Lists, in descending order, the executors that joined a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_executors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_executors)
         """
 
     def list_named_queries(
         self, *, NextToken: str = ..., MaxResults: int = ..., WorkGroup: str = ...
@@ -582,15 +641,15 @@
         """
 
     def list_notebook_sessions(
         self, *, NotebookId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListNotebookSessionsResponseTypeDef:
         """
         Lists, in descending order, the sessions that have been created in a notebook
-        that are in an active state like `CREATING` , `CREATED` , `IDLE` or `BUSY`.
+        that are in an active state like `CREATING`, `CREATED`, `IDLE` or `BUSY`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_sessions)
         """
 
     def list_prepared_statements(
         self, *, WorkGroup: str, NextToken: str = ..., MaxResults: int = ...
@@ -618,16 +677,16 @@
         *,
         WorkGroup: str,
         StateFilter: SessionStateType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListSessionsResponseTypeDef:
         """
-        Lists the sessions in a workgroup that are in an active state like `CREATING` ,
-        `CREATED` , `IDLE` , or `BUSY`.
+        Lists the sessions in a workgroup that are in an active state like `CREATING`,
+        `CREATED`, `IDLE`, or `BUSY`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_sessions)
         """
 
     def list_table_metadata(
         self,
@@ -645,15 +704,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_table_metadata)
         """
 
     def list_tags_for_resource(
         self, *, ResourceARN: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
-        Lists the tags associated with an Athena workgroup or data catalog resource.
+        Lists the tags associated with an Athena resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_tags_for_resource)
         """
 
     def list_work_groups(
         self, *, NextToken: str = ..., MaxResults: int = ...
@@ -661,14 +720,28 @@
         """
         Lists available workgroups for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
 
+    def put_capacity_assignment_configuration(
+        self,
+        *,
+        CapacityReservationName: str,
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Puts a new capacity assignment configuration for a specified capacity
+        reservation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
+        """
+
     def start_calculation_execution(
         self,
         *,
         SessionId: str,
         Description: str = ...,
         CalculationConfiguration: CalculationConfigurationTypeDef = ...,
         CodeBlock: str = ...,
@@ -748,20 +821,29 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.terminate_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#terminate_session)
         """
 
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes one or more tags from a data catalog or workgroup resource.
+        Removes one or more tags from an Athena resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#untag_resource)
         """
 
+    def update_capacity_reservation(self, *, TargetDpus: int, Name: str) -> Dict[str, Any]:
+        """
+        Updates the number of requested data processing units for the capacity
+        reservation with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_capacity_reservation)
+        """
+
     def update_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
         Parameters: Mapping[str, str] = ...
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -35,23 +35,26 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
+    CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
     EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
+    GetCapacityAssignmentConfigurationOutputTypeDef,
+    GetCapacityReservationOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetNamedQueryOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetQueryResultsOutputTypeDef,
@@ -59,14 +62,15 @@
     GetSessionResponseTypeDef,
     GetSessionStatusResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     GetWorkGroupOutputTypeDef,
     ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesOutputTypeDef,
     ListCalculationExecutionsResponseTypeDef,
+    ListCapacityReservationsOutputTypeDef,
     ListDatabasesOutputTypeDef,
     ListDataCatalogsOutputTypeDef,
     ListEngineVersionsOutputTypeDef,
     ListExecutorsResponseTypeDef,
     ListNamedQueriesOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookSessionsResponseTypeDef,
@@ -161,21 +165,38 @@
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#can_paginate)
         """
+    def cancel_capacity_reservation(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Cancels the capacity reservation with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.cancel_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#cancel_capacity_reservation)
+        """
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#close)
         """
+    def create_capacity_reservation(
+        self, *, TargetDpus: int, Name: str, Tags: Sequence[TagTypeDef] = ...
+    ) -> Dict[str, Any]:
+        """
+        Creates a capacity reservation with the specified name and number of requested
+        data processing units.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_capacity_reservation)
+        """
     def create_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
         Parameters: Mapping[str, str] = ...,
@@ -240,14 +261,21 @@
     ) -> Dict[str, Any]:
         """
         Creates a workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_work_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_work_group)
         """
+    def delete_capacity_reservation(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes a cancelled capacity reservation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_capacity_reservation)
+        """
     def delete_data_catalog(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes a data catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_data_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_data_catalog)
         """
@@ -312,29 +340,45 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution)
         """
     def get_calculation_execution_code(
         self, *, CalculationExecutionId: str
     ) -> GetCalculationExecutionCodeResponseTypeDef:
         """
-        Retrieves a pre-signed URL to a copy of the code that was executed for the
-        calculation.
+        Retrieves the unencrypted code that was executed for the calculation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_code)
         """
     def get_calculation_execution_status(
         self, *, CalculationExecutionId: str
     ) -> GetCalculationExecutionStatusResponseTypeDef:
         """
         Gets the status of a current calculation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_status)
         """
+    def get_capacity_assignment_configuration(
+        self, *, CapacityReservationName: str
+    ) -> GetCapacityAssignmentConfigurationOutputTypeDef:
+        """
+        Gets the capacity assignment configuration for a capacity reservation, if one
+        exists.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_capacity_assignment_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_capacity_assignment_configuration)
+        """
+    def get_capacity_reservation(self, *, Name: str) -> GetCapacityReservationOutputTypeDef:
+        """
+        Returns information about the capacity reservation with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_capacity_reservation)
+        """
     def get_data_catalog(self, *, Name: str) -> GetDataCatalogOutputTypeDef:
         """
         Returns the specified data catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_data_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_data_catalog)
         """
@@ -444,15 +488,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#import_notebook)
         """
     def list_application_dpu_sizes(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListApplicationDPUSizesOutputTypeDef:
         """
         Returns the supported DPU sizes for the supported application runtimes (for
-        example, `Jupyter 1.0` ).
+        example, `Athena notebook version 1`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_application_dpu_sizes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_application_dpu_sizes)
         """
     def list_calculation_executions(
         self,
         *,
@@ -464,14 +508,23 @@
         """
         Lists the calculations that have been submitted to a session in descending
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_calculation_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_calculation_executions)
         """
+    def list_capacity_reservations(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListCapacityReservationsOutputTypeDef:
+        """
+        Lists the capacity reservations for the current account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_capacity_reservations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_capacity_reservations)
+        """
     def list_data_catalogs(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCatalogsOutputTypeDef:
         """
         Lists the data catalogs in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_data_catalogs)
@@ -501,15 +554,15 @@
         *,
         SessionId: str,
         ExecutorStateFilter: ExecutorStateType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListExecutorsResponseTypeDef:
         """
-        Lists, in descending order, the executors that have been submitted to a session.
+        Lists, in descending order, the executors that joined a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_executors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_executors)
         """
     def list_named_queries(
         self, *, NextToken: str = ..., MaxResults: int = ..., WorkGroup: str = ...
     ) -> ListNamedQueriesOutputTypeDef:
@@ -535,15 +588,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_metadata)
         """
     def list_notebook_sessions(
         self, *, NotebookId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListNotebookSessionsResponseTypeDef:
         """
         Lists, in descending order, the sessions that have been created in a notebook
-        that are in an active state like `CREATING` , `CREATED` , `IDLE` or `BUSY`.
+        that are in an active state like `CREATING`, `CREATED`, `IDLE` or `BUSY`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_sessions)
         """
     def list_prepared_statements(
         self, *, WorkGroup: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPreparedStatementsOutputTypeDef:
@@ -568,16 +621,16 @@
         *,
         WorkGroup: str,
         StateFilter: SessionStateType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListSessionsResponseTypeDef:
         """
-        Lists the sessions in a workgroup that are in an active state like `CREATING` ,
-        `CREATED` , `IDLE` , or `BUSY`.
+        Lists the sessions in a workgroup that are in an active state like `CREATING`,
+        `CREATED`, `IDLE`, or `BUSY`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_sessions)
         """
     def list_table_metadata(
         self,
         *,
@@ -593,28 +646,41 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_table_metadata)
         """
     def list_tags_for_resource(
         self, *, ResourceARN: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
-        Lists the tags associated with an Athena workgroup or data catalog resource.
+        Lists the tags associated with an Athena resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_tags_for_resource)
         """
     def list_work_groups(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkGroupsOutputTypeDef:
         """
         Lists available workgroups for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
+    def put_capacity_assignment_configuration(
+        self,
+        *,
+        CapacityReservationName: str,
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Puts a new capacity assignment configuration for a specified capacity
+        reservation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
+        """
     def start_calculation_execution(
         self,
         *,
         SessionId: str,
         Description: str = ...,
         CalculationConfiguration: CalculationConfigurationTypeDef = ...,
         CodeBlock: str = ...,
@@ -687,19 +753,27 @@
         Terminates an active session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.terminate_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#terminate_session)
         """
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes one or more tags from a data catalog or workgroup resource.
+        Removes one or more tags from an Athena resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#untag_resource)
         """
+    def update_capacity_reservation(self, *, TargetDpus: int, Name: str) -> Dict[str, Any]:
+        """
+        Updates the number of requested data processing units for the capacity
+        reservation with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_capacity_reservation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_capacity_reservation)
+        """
     def update_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
         Parameters: Mapping[str, str] = ...
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CalculationExecutionStateType",
+    "CapacityAllocationStatusType",
+    "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
     "ExecutorStateType",
     "ExecutorTypeType",
     "GetQueryResultsPaginatorName",
     "ListDataCatalogsPaginatorName",
@@ -42,18 +43,21 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
+CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
+CapacityReservationStatusType = Literal[
+    "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
+]
 ColumnNullableType = Literal["NOT_NULL", "NULLABLE", "UNKNOWN"]
 DataCatalogTypeType = Literal["GLUE", "HIVE", "LAMBDA"]
 EncryptionOptionType = Literal["CSE_KMS", "SSE_KMS", "SSE_S3"]
 ExecutorStateType = Literal[
     "CREATED", "CREATING", "FAILED", "REGISTERED", "TERMINATED", "TERMINATING"
 ]
 ExecutorTypeType = Literal["COORDINATOR", "GATEWAY", "WORKER"]
@@ -84,14 +88,15 @@
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
@@ -131,14 +136,15 @@
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
@@ -236,14 +242,15 @@
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
@@ -279,14 +286,15 @@
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
@@ -305,16 +313,19 @@
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
@@ -398,15 +409,17 @@
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
@@ -450,14 +463,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
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

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "CalculationExecutionStateType",
+    "CapacityAllocationStatusType",
+    "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
     "ExecutorStateType",
     "ExecutorTypeType",
     "GetQueryResultsPaginatorName",
     "ListDataCatalogsPaginatorName",
@@ -41,17 +44,22 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
+CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
+CapacityReservationStatusType = Literal[
+    "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
+]
 ColumnNullableType = Literal["NOT_NULL", "NULLABLE", "UNKNOWN"]
 DataCatalogTypeType = Literal["GLUE", "HIVE", "LAMBDA"]
 EncryptionOptionType = Literal["CSE_KMS", "SSE_KMS", "SSE_S3"]
 ExecutorStateType = Literal[
     "CREATED", "CREATING", "FAILED", "REGISTERED", "TERMINATED", "TERMINATING"
 ]
 ExecutorTypeType = Literal["COORDINATOR", "GATEWAY", "WORKER"]
@@ -82,14 +90,15 @@
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
@@ -129,14 +138,15 @@
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
@@ -234,14 +244,15 @@
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
@@ -277,14 +288,15 @@
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
@@ -303,16 +315,19 @@
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
@@ -396,15 +411,17 @@
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
@@ -448,14 +465,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
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

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,126 +52,117 @@
     "ListDatabasesPaginator",
     "ListNamedQueriesPaginator",
     "ListQueryExecutionsPaginator",
     "ListTableMetadataPaginator",
     "ListTagsForResourcePaginator",
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
 class GetQueryResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
     """
 
     def paginate(
-        self, *, QueryExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueryExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetQueryResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
         """
 
-
 class ListDataCatalogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataCatalogsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
         """
 
-
 class ListDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
     """
 
     def paginate(
-        self, *, CatalogName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CatalogName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
         """
 
-
 class ListNamedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNamedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
         """
 
-
 class ListQueryExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueryExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
         """
 
-
 class ListTableMetadataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtablemetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtablemetadatapaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,117 +52,126 @@
     "ListDatabasesPaginator",
     "ListNamedQueriesPaginator",
     "ListQueryExecutionsPaginator",
     "ListTableMetadataPaginator",
     "ListTagsForResourcePaginator",
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
 class GetQueryResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
     """
 
     def paginate(
-        self, *, QueryExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueryExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetQueryResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
         """
 
+
 class ListDataCatalogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataCatalogsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
         """
 
+
 class ListDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
     """
 
     def paginate(
-        self, *, CatalogName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CatalogName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
         """
 
+
 class ListNamedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNamedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
         """
 
+
 class ListQueryExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueryExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
         """
 
+
 class ListTableMetadataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtablemetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtablemetadatapaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     CalculationExecutionStateType,
+    CapacityAllocationStatusType,
+    CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
     ExecutorStateType,
     ExecutorTypeType,
     QueryExecutionStateType,
     SessionStateType,
@@ -40,124 +42,143 @@
 
 __all__ = (
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
+    "CancelCapacityReservationInputRequestTypeDef",
+    "CapacityAllocationTypeDef",
+    "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
+    "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
+    "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
+    "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetCalculationExecutionRequestRequestTypeDef",
     "GetCalculationExecutionStatusRequestRequestTypeDef",
+    "GetCapacityAssignmentConfigurationInputRequestTypeDef",
+    "GetCapacityReservationInputRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
     "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "SessionStatisticsTypeDef",
     "SessionStatusTypeDef",
     "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
     "ImportNotebookInputRequestTypeDef",
+    "ImportNotebookOutputTypeDef",
     "ListApplicationDPUSizesInputRequestTypeDef",
     "ListCalculationExecutionsRequestRequestTypeDef",
+    "ListCapacityReservationsInputRequestTypeDef",
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
     "ListExecutorsRequestRequestTypeDef",
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
+    "ListNamedQueriesOutputTypeDef",
     "ListNotebookSessionsRequestRequestTypeDef",
     "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
+    "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
+    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
+    "ResponseMetadataTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
+    "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
+    "TerminateSessionResponseTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateCapacityReservationInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
     "UpdateNotebookInputRequestTypeDef",
     "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
     "QueryExecutionStatusTypeDef",
-    "CreateNamedQueryOutputTypeDef",
-    "CreateNotebookOutputTypeDef",
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
-    "ImportNotebookOutputTypeDef",
-    "ListApplicationDPUSizesOutputTypeDef",
-    "ListNamedQueriesOutputTypeDef",
-    "ListQueryExecutionsOutputTypeDef",
-    "StartCalculationExecutionResponseTypeDef",
-    "StartQueryExecutionOutputTypeDef",
-    "StartSessionResponseTypeDef",
-    "StopCalculationExecutionResponseTypeDef",
-    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
+    "CapacityReservationTypeDef",
+    "CapacityAssignmentConfigurationTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
+    "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
@@ -169,29 +190,25 @@
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
-    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
+    "GetCapacityReservationOutputTypeDef",
+    "ListCapacityReservationsOutputTypeDef",
+    "GetCapacityAssignmentConfigurationOutputTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -261,25 +278,14 @@
 )
 
 
 class NamedQueryTypeDef(_RequiredNamedQueryTypeDef, _OptionalNamedQueryTypeDef):
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
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -368,14 +374,52 @@
         "CompletionDateTime": datetime,
         "State": CalculationExecutionStateType,
         "StateChangeReason": str,
     },
     total=False,
 )
 
+CancelCapacityReservationInputRequestTypeDef = TypedDict(
+    "CancelCapacityReservationInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
+_RequiredCapacityAllocationTypeDef = TypedDict(
+    "_RequiredCapacityAllocationTypeDef",
+    {
+        "Status": CapacityAllocationStatusType,
+        "RequestTime": datetime,
+    },
+)
+_OptionalCapacityAllocationTypeDef = TypedDict(
+    "_OptionalCapacityAllocationTypeDef",
+    {
+        "StatusMessage": str,
+        "RequestCompletionTime": datetime,
+    },
+    total=False,
+)
+
+
+class CapacityAllocationTypeDef(
+    _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
+):
+    pass
+
+
+CapacityAssignmentTypeDef = TypedDict(
+    "CapacityAssignmentTypeDef",
+    {
+        "WorkGroupNames": List[str],
+    },
+    total=False,
+)
+
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Name": str,
         "Type": str,
     },
 )
@@ -449,14 +493,22 @@
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
 
+CreateNamedQueryOutputTypeDef = TypedDict(
+    "CreateNamedQueryOutputTypeDef",
+    {
+        "NamedQueryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateNotebookInputRequestTypeDef = TypedDict(
     "_RequiredCreateNotebookInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Name": str,
     },
 )
@@ -471,14 +523,22 @@
 
 class CreateNotebookInputRequestTypeDef(
     _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
 ):
     pass
 
 
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -502,14 +562,24 @@
 CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -567,14 +637,21 @@
     "DatumTypeDef",
     {
         "VarCharValue": str,
     },
     total=False,
 )
 
+DeleteCapacityReservationInputRequestTypeDef = TypedDict(
+    "DeleteCapacityReservationInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 DeleteDataCatalogInputRequestTypeDef = TypedDict(
     "DeleteDataCatalogInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -650,14 +727,15 @@
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
         "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
     },
     total=False,
 )
 
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
@@ -728,28 +806,50 @@
 GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCalculationExecutionRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
 GetCalculationExecutionStatusRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionStatusRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
+GetCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "GetCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+    },
+)
+
+GetCapacityReservationInputRequestTypeDef = TypedDict(
+    "GetCapacityReservationInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 GetDataCatalogInputRequestTypeDef = TypedDict(
     "GetDataCatalogInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -786,24 +886,36 @@
 GetQueryExecutionInputRequestTypeDef = TypedDict(
     "GetQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "QueryExecutionId": str,
+    },
+)
+_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
+    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetQueryResultsInputRequestTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputRequestTypeDef = TypedDict(
@@ -900,14 +1012,22 @@
 
 class ImportNotebookInputRequestTypeDef(
     _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
 ):
     pass
 
 
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
     "ListApplicationDPUSizesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -933,23 +1053,62 @@
 class ListCalculationExecutionsRequestRequestTypeDef(
     _RequiredListCalculationExecutionsRequestRequestTypeDef,
     _OptionalListCalculationExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListCapacityReservationsInputRequestTypeDef = TypedDict(
+    "ListCapacityReservationsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "CatalogName": str,
+    },
+)
+_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDatabasesInputListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDatabasesInputRequestTypeDef = TypedDict(
     "_RequiredListDatabasesInputRequestTypeDef",
     {
         "CatalogName": str,
     },
 )
 _OptionalListDatabasesInputRequestTypeDef = TypedDict(
@@ -996,24 +1155,42 @@
 
 class ListExecutorsRequestRequestTypeDef(
     _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
 ):
     pass
 
 
+ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+ListNamedQueriesOutputTypeDef = TypedDict(
+    "ListNamedQueriesOutputTypeDef",
+    {
+        "NamedQueryIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListNotebookSessionsRequestRequestTypeDef",
     {
         "NotebookId": str,
     },
 )
 _OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
@@ -1070,24 +1247,42 @@
     {
         "StatementName": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueryExecutionsInputRequestTypeDef = TypedDict(
     "ListQueryExecutionsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+ListQueryExecutionsOutputTypeDef = TypedDict(
+    "ListQueryExecutionsOutputTypeDef",
+    {
+        "QueryExecutionIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionsRequestRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListSessionsRequestRequestTypeDef = TypedDict(
@@ -1103,14 +1298,38 @@
 
 class ListSessionsRequestRequestTypeDef(
     _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "CatalogName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "Expression": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTableMetadataInputListTableMetadataPaginateTypeDef(
+    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
+    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -1127,14 +1346,36 @@
 
 class ListTableMetadataInputRequestTypeDef(
     _RequiredListTableMetadataInputRequestTypeDef, _OptionalListTableMetadataInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1158,14 +1399,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1224,14 +1475,25 @@
         "ExecutionTime": int,
         "QueryStagePlan": "QueryStagePlanNodeTypeDef",
         "SubStages": List[Dict[str, Any]],
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
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1245,43 +1507,93 @@
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
 
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartQueryExecutionOutputTypeDef = TypedDict(
+    "StartQueryExecutionOutputTypeDef",
+    {
+        "QueryExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopCalculationExecutionRequestRequestTypeDef = TypedDict(
     "StopCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateCapacityReservationInputRequestTypeDef = TypedDict(
+    "UpdateCapacityReservationInputRequestTypeDef",
+    {
+        "TargetDpus": int,
+        "Name": str,
+    },
+)
+
 _RequiredUpdateDataCatalogInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDataCatalogInputRequestTypeDef",
     {
         "Name": str,
         "Type": DataCatalogTypeType,
     },
 )
@@ -1391,168 +1703,66 @@
 class UpdatePreparedStatementInputRequestTypeDef(
     _RequiredUpdatePreparedStatementInputRequestTypeDef,
     _OptionalUpdatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
 
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 QueryExecutionStatusTypeDef = TypedDict(
     "QueryExecutionStatusTypeDef",
     {
         "State": QueryExecutionStateType,
         "StateChangeReason": str,
         "SubmissionDateTime": datetime,
         "CompletionDateTime": datetime,
         "AthenaError": AthenaErrorTypeDef,
     },
     total=False,
 )
 
-CreateNamedQueryOutputTypeDef = TypedDict(
-    "CreateNamedQueryOutputTypeDef",
-    {
-        "NamedQueryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNotebookOutputTypeDef = TypedDict(
-    "CreateNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    {
-        "NotebookUrl": str,
-        "AuthToken": str,
-        "AuthTokenExpirationTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCalculationExecutionCodeResponseTypeDef = TypedDict(
-    "GetCalculationExecutionCodeResponseTypeDef",
-    {
-        "CodeBlock": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportNotebookOutputTypeDef = TypedDict(
-    "ImportNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationDPUSizesOutputTypeDef = TypedDict(
-    "ListApplicationDPUSizesOutputTypeDef",
-    {
-        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListNamedQueriesOutputTypeDef = TypedDict(
-    "ListNamedQueriesOutputTypeDef",
-    {
-        "NamedQueryIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueryExecutionsOutputTypeDef = TypedDict(
-    "ListQueryExecutionsOutputTypeDef",
-    {
-        "QueryExecutionIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartCalculationExecutionResponseTypeDef = TypedDict(
-    "StartCalculationExecutionResponseTypeDef",
-    {
-        "CalculationExecutionId": str,
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryExecutionOutputTypeDef = TypedDict(
-    "StartQueryExecutionOutputTypeDef",
-    {
-        "QueryExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "State": SessionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopCalculationExecutionResponseTypeDef = TypedDict(
-    "StopCalculationExecutionResponseTypeDef",
-    {
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "State": SessionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPreparedStatementOutputTypeDef = TypedDict(
     "GetPreparedStatementOutputTypeDef",
     {
         "PreparedStatement": PreparedStatementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetPreparedStatementOutputTypeDef = TypedDict(
     "BatchGetPreparedStatementOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCalculationExecutionRequestRequestTypeDef",
     {
         "SessionId": str,
@@ -1593,24 +1803,67 @@
         "CalculationExecutionId": str,
         "SessionId": str,
         "Description": str,
         "WorkingDirectory": str,
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
         "Result": CalculationResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCalculationExecutionStatusResponseTypeDef = TypedDict(
     "GetCalculationExecutionStatusResponseTypeDef",
     {
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCapacityReservationTypeDef = TypedDict(
+    "_RequiredCapacityReservationTypeDef",
+    {
+        "Name": str,
+        "Status": CapacityReservationStatusType,
+        "TargetDpus": int,
+        "AllocatedDpus": int,
+        "CreationTime": datetime,
+    },
+)
+_OptionalCapacityReservationTypeDef = TypedDict(
+    "_OptionalCapacityReservationTypeDef",
+    {
+        "LastAllocation": CapacityAllocationTypeDef,
+        "LastSuccessfulAllocationTime": datetime,
+    },
+    total=False,
+)
+
+
+class CapacityReservationTypeDef(
+    _RequiredCapacityReservationTypeDef, _OptionalCapacityReservationTypeDef
+):
+    pass
+
+
+CapacityAssignmentConfigurationTypeDef = TypedDict(
+    "CapacityAssignmentConfigurationTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": List[CapacityAssignmentTypeDef],
+    },
+    total=False,
+)
+
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
     },
 )
 
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
@@ -1638,14 +1891,37 @@
 )
 
 
 class TableMetadataTypeDef(_RequiredTableMetadataTypeDef, _OptionalTableMetadataTypeDef):
     pass
 
 
+_RequiredCreateCapacityReservationInputRequestTypeDef = TypedDict(
+    "_RequiredCreateCapacityReservationInputRequestTypeDef",
+    {
+        "TargetDpus": int,
+        "Name": str,
+    },
+)
+_OptionalCreateCapacityReservationInputRequestTypeDef = TypedDict(
+    "_OptionalCreateCapacityReservationInputRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateCapacityReservationInputRequestTypeDef(
+    _RequiredCreateCapacityReservationInputRequestTypeDef,
+    _OptionalCreateCapacityReservationInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateDataCatalogInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataCatalogInputRequestTypeDef",
     {
         "Name": str,
         "Type": DataCatalogTypeType,
     },
 )
@@ -1667,15 +1943,15 @@
 
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1684,40 +1960,40 @@
 )
 
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
@@ -1788,15 +2064,15 @@
 
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
@@ -1810,41 +2086,41 @@
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
         "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNotebookMetadataOutputTypeDef = TypedDict(
     "GetNotebookMetadataOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
         "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -1864,136 +2140,20 @@
 class ListNotebookMetadataInputRequestTypeDef(
     _RequiredListNotebookMetadataInputRequestTypeDef,
     _OptionalListNotebookMetadataInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "QueryExecutionId": str,
-    },
-)
-_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
-    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-):
-    pass
-
-
-ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "CatalogName": str,
-    },
-)
-_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatabasesInputListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
-):
-    pass
-
-
-ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "CatalogName": str,
-        "DatabaseName": str,
-    },
-)
-_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "Expression": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTableMetadataInputListTableMetadataPaginateTypeDef(
-    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
-    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 GetSessionStatusResponseTypeDef = TypedDict(
     "GetSessionStatusResponseTypeDef",
     {
         "SessionId": str,
         "Status": SessionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
@@ -2006,24 +2166,24 @@
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
@@ -2057,32 +2217,57 @@
 )
 
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCapacityReservationOutputTypeDef = TypedDict(
+    "GetCapacityReservationOutputTypeDef",
+    {
+        "CapacityReservation": CapacityReservationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCapacityReservationsOutputTypeDef = TypedDict(
+    "ListCapacityReservationsOutputTypeDef",
+    {
+        "NextToken": str,
+        "CapacityReservations": List[CapacityReservationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
+    "GetCapacityAssignmentConfigurationOutputTypeDef",
+    {
+        "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": List[RowTypeDef],
@@ -2099,14 +2284,15 @@
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
         "AdditionalConfiguration": str,
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
+        "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
 WorkGroupConfigurationUpdatesTypeDef = TypedDict(
     "WorkGroupConfigurationUpdatesTypeDef",
     {
@@ -2117,14 +2303,15 @@
         "RemoveBytesScannedCutoffPerQuery": bool,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
         "RemoveCustomerContentEncryptionConfiguration": bool,
         "AdditionalConfiguration": str,
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
+        "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
@@ -2133,41 +2320,41 @@
         "WorkGroup": str,
         "EngineVersion": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
@@ -2214,15 +2401,15 @@
 
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
@@ -2291,26 +2478,26 @@
 
 
 BatchGetQueryExecutionOutputTypeDef = TypedDict(
     "BatchGetQueryExecutionOutputTypeDef",
     {
         "QueryExecutions": List[QueryExecutionTypeDef],
         "UnprocessedQueryExecutionIds": List[UnprocessedQueryExecutionIdTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryExecutionOutputTypeDef = TypedDict(
     "GetQueryExecutionOutputTypeDef",
     {
         "QueryExecution": QueryExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkGroupOutputTypeDef = TypedDict(
     "GetWorkGroupOutputTypeDef",
     {
         "WorkGroup": WorkGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     CalculationExecutionStateType,
+    CapacityAllocationStatusType,
+    CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
     ExecutorStateType,
     ExecutorTypeType,
     QueryExecutionStateType,
     SessionStateType,
@@ -39,124 +41,143 @@
 
 __all__ = (
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
+    "CancelCapacityReservationInputRequestTypeDef",
+    "CapacityAllocationTypeDef",
+    "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
+    "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
+    "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
+    "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetCalculationExecutionRequestRequestTypeDef",
     "GetCalculationExecutionStatusRequestRequestTypeDef",
+    "GetCapacityAssignmentConfigurationInputRequestTypeDef",
+    "GetCapacityReservationInputRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
     "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "SessionStatisticsTypeDef",
     "SessionStatusTypeDef",
     "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
     "ImportNotebookInputRequestTypeDef",
+    "ImportNotebookOutputTypeDef",
     "ListApplicationDPUSizesInputRequestTypeDef",
     "ListCalculationExecutionsRequestRequestTypeDef",
+    "ListCapacityReservationsInputRequestTypeDef",
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
     "ListExecutorsRequestRequestTypeDef",
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
+    "ListNamedQueriesOutputTypeDef",
     "ListNotebookSessionsRequestRequestTypeDef",
     "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
+    "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
+    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
+    "ResponseMetadataTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
+    "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
+    "TerminateSessionResponseTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateCapacityReservationInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
     "UpdateNotebookInputRequestTypeDef",
     "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
     "QueryExecutionStatusTypeDef",
-    "CreateNamedQueryOutputTypeDef",
-    "CreateNotebookOutputTypeDef",
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
-    "ImportNotebookOutputTypeDef",
-    "ListApplicationDPUSizesOutputTypeDef",
-    "ListNamedQueriesOutputTypeDef",
-    "ListQueryExecutionsOutputTypeDef",
-    "StartCalculationExecutionResponseTypeDef",
-    "StartQueryExecutionOutputTypeDef",
-    "StartSessionResponseTypeDef",
-    "StopCalculationExecutionResponseTypeDef",
-    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
+    "CapacityReservationTypeDef",
+    "CapacityAssignmentConfigurationTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
+    "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
@@ -168,29 +189,25 @@
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
-    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
+    "GetCapacityReservationOutputTypeDef",
+    "ListCapacityReservationsOutputTypeDef",
+    "GetCapacityAssignmentConfigurationOutputTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -258,25 +275,14 @@
     },
     total=False,
 )
 
 class NamedQueryTypeDef(_RequiredNamedQueryTypeDef, _OptionalNamedQueryTypeDef):
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
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -365,14 +371,50 @@
         "CompletionDateTime": datetime,
         "State": CalculationExecutionStateType,
         "StateChangeReason": str,
     },
     total=False,
 )
 
+CancelCapacityReservationInputRequestTypeDef = TypedDict(
+    "CancelCapacityReservationInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
+_RequiredCapacityAllocationTypeDef = TypedDict(
+    "_RequiredCapacityAllocationTypeDef",
+    {
+        "Status": CapacityAllocationStatusType,
+        "RequestTime": datetime,
+    },
+)
+_OptionalCapacityAllocationTypeDef = TypedDict(
+    "_OptionalCapacityAllocationTypeDef",
+    {
+        "StatusMessage": str,
+        "RequestCompletionTime": datetime,
+    },
+    total=False,
+)
+
+class CapacityAllocationTypeDef(
+    _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
+):
+    pass
+
+CapacityAssignmentTypeDef = TypedDict(
+    "CapacityAssignmentTypeDef",
+    {
+        "WorkGroupNames": List[str],
+    },
+    total=False,
+)
+
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Name": str,
         "Type": str,
     },
 )
@@ -440,14 +482,22 @@
 )
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
+CreateNamedQueryOutputTypeDef = TypedDict(
+    "CreateNamedQueryOutputTypeDef",
+    {
+        "NamedQueryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateNotebookInputRequestTypeDef = TypedDict(
     "_RequiredCreateNotebookInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Name": str,
     },
 )
@@ -460,14 +510,22 @@
 )
 
 class CreateNotebookInputRequestTypeDef(
     _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
 ):
     pass
 
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -489,14 +547,24 @@
 CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -550,14 +618,21 @@
     "DatumTypeDef",
     {
         "VarCharValue": str,
     },
     total=False,
 )
 
+DeleteCapacityReservationInputRequestTypeDef = TypedDict(
+    "DeleteCapacityReservationInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 DeleteDataCatalogInputRequestTypeDef = TypedDict(
     "DeleteDataCatalogInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -629,14 +704,15 @@
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
         "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
     },
     total=False,
 )
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
@@ -703,28 +779,50 @@
 GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCalculationExecutionRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
 GetCalculationExecutionStatusRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionStatusRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
+GetCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "GetCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+    },
+)
+
+GetCapacityReservationInputRequestTypeDef = TypedDict(
+    "GetCapacityReservationInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 GetDataCatalogInputRequestTypeDef = TypedDict(
     "GetDataCatalogInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -761,24 +859,34 @@
 GetQueryExecutionInputRequestTypeDef = TypedDict(
     "GetQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "QueryExecutionId": str,
+    },
+)
+_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
+    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetQueryResultsInputRequestTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputRequestTypeDef = TypedDict(
@@ -871,14 +979,22 @@
 )
 
 class ImportNotebookInputRequestTypeDef(
     _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
 ):
     pass
 
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
     "ListApplicationDPUSizesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -902,23 +1018,60 @@
 
 class ListCalculationExecutionsRequestRequestTypeDef(
     _RequiredListCalculationExecutionsRequestRequestTypeDef,
     _OptionalListCalculationExecutionsRequestRequestTypeDef,
 ):
     pass
 
+ListCapacityReservationsInputRequestTypeDef = TypedDict(
+    "ListCapacityReservationsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "CatalogName": str,
+    },
+)
+_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDatabasesInputListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDatabasesInputRequestTypeDef = TypedDict(
     "_RequiredListDatabasesInputRequestTypeDef",
     {
         "CatalogName": str,
     },
 )
 _OptionalListDatabasesInputRequestTypeDef = TypedDict(
@@ -961,24 +1114,42 @@
 )
 
 class ListExecutorsRequestRequestTypeDef(
     _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
 ):
     pass
 
+ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+ListNamedQueriesOutputTypeDef = TypedDict(
+    "ListNamedQueriesOutputTypeDef",
+    {
+        "NamedQueryIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListNotebookSessionsRequestRequestTypeDef",
     {
         "NotebookId": str,
     },
 )
 _OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
@@ -1031,24 +1202,42 @@
     {
         "StatementName": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueryExecutionsInputRequestTypeDef = TypedDict(
     "ListQueryExecutionsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+ListQueryExecutionsOutputTypeDef = TypedDict(
+    "ListQueryExecutionsOutputTypeDef",
+    {
+        "QueryExecutionIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionsRequestRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListSessionsRequestRequestTypeDef = TypedDict(
@@ -1062,14 +1251,36 @@
 )
 
 class ListSessionsRequestRequestTypeDef(
     _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "CatalogName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "Expression": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTableMetadataInputListTableMetadataPaginateTypeDef(
+    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
+    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
+):
+    pass
+
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -1084,14 +1295,34 @@
 )
 
 class ListTableMetadataInputRequestTypeDef(
     _RequiredListTableMetadataInputRequestTypeDef, _OptionalListTableMetadataInputRequestTypeDef
 ):
     pass
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1113,14 +1344,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1179,14 +1420,25 @@
         "ExecutionTime": int,
         "QueryStagePlan": "QueryStagePlanNodeTypeDef",
         "SubStages": List[Dict[str, Any]],
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
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1198,43 +1450,93 @@
 )
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartQueryExecutionOutputTypeDef = TypedDict(
+    "StartQueryExecutionOutputTypeDef",
+    {
+        "QueryExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopCalculationExecutionRequestRequestTypeDef = TypedDict(
     "StopCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateCapacityReservationInputRequestTypeDef = TypedDict(
+    "UpdateCapacityReservationInputRequestTypeDef",
+    {
+        "TargetDpus": int,
+        "Name": str,
+    },
+)
+
 _RequiredUpdateDataCatalogInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDataCatalogInputRequestTypeDef",
     {
         "Name": str,
         "Type": DataCatalogTypeType,
     },
 )
@@ -1334,168 +1636,66 @@
 
 class UpdatePreparedStatementInputRequestTypeDef(
     _RequiredUpdatePreparedStatementInputRequestTypeDef,
     _OptionalUpdatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 QueryExecutionStatusTypeDef = TypedDict(
     "QueryExecutionStatusTypeDef",
     {
         "State": QueryExecutionStateType,
         "StateChangeReason": str,
         "SubmissionDateTime": datetime,
         "CompletionDateTime": datetime,
         "AthenaError": AthenaErrorTypeDef,
     },
     total=False,
 )
 
-CreateNamedQueryOutputTypeDef = TypedDict(
-    "CreateNamedQueryOutputTypeDef",
-    {
-        "NamedQueryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNotebookOutputTypeDef = TypedDict(
-    "CreateNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    {
-        "NotebookUrl": str,
-        "AuthToken": str,
-        "AuthTokenExpirationTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCalculationExecutionCodeResponseTypeDef = TypedDict(
-    "GetCalculationExecutionCodeResponseTypeDef",
-    {
-        "CodeBlock": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportNotebookOutputTypeDef = TypedDict(
-    "ImportNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationDPUSizesOutputTypeDef = TypedDict(
-    "ListApplicationDPUSizesOutputTypeDef",
-    {
-        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListNamedQueriesOutputTypeDef = TypedDict(
-    "ListNamedQueriesOutputTypeDef",
-    {
-        "NamedQueryIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueryExecutionsOutputTypeDef = TypedDict(
-    "ListQueryExecutionsOutputTypeDef",
-    {
-        "QueryExecutionIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartCalculationExecutionResponseTypeDef = TypedDict(
-    "StartCalculationExecutionResponseTypeDef",
-    {
-        "CalculationExecutionId": str,
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryExecutionOutputTypeDef = TypedDict(
-    "StartQueryExecutionOutputTypeDef",
-    {
-        "QueryExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "State": SessionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopCalculationExecutionResponseTypeDef = TypedDict(
-    "StopCalculationExecutionResponseTypeDef",
-    {
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "State": SessionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPreparedStatementOutputTypeDef = TypedDict(
     "GetPreparedStatementOutputTypeDef",
     {
         "PreparedStatement": PreparedStatementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetPreparedStatementOutputTypeDef = TypedDict(
     "BatchGetPreparedStatementOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCalculationExecutionRequestRequestTypeDef",
     {
         "SessionId": str,
@@ -1534,24 +1734,65 @@
         "CalculationExecutionId": str,
         "SessionId": str,
         "Description": str,
         "WorkingDirectory": str,
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
         "Result": CalculationResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCalculationExecutionStatusResponseTypeDef = TypedDict(
     "GetCalculationExecutionStatusResponseTypeDef",
     {
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCapacityReservationTypeDef = TypedDict(
+    "_RequiredCapacityReservationTypeDef",
+    {
+        "Name": str,
+        "Status": CapacityReservationStatusType,
+        "TargetDpus": int,
+        "AllocatedDpus": int,
+        "CreationTime": datetime,
+    },
+)
+_OptionalCapacityReservationTypeDef = TypedDict(
+    "_OptionalCapacityReservationTypeDef",
+    {
+        "LastAllocation": CapacityAllocationTypeDef,
+        "LastSuccessfulAllocationTime": datetime,
+    },
+    total=False,
+)
+
+class CapacityReservationTypeDef(
+    _RequiredCapacityReservationTypeDef, _OptionalCapacityReservationTypeDef
+):
+    pass
+
+CapacityAssignmentConfigurationTypeDef = TypedDict(
+    "CapacityAssignmentConfigurationTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": List[CapacityAssignmentTypeDef],
+    },
+    total=False,
+)
+
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
     },
 )
 
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
@@ -1577,14 +1818,35 @@
     },
     total=False,
 )
 
 class TableMetadataTypeDef(_RequiredTableMetadataTypeDef, _OptionalTableMetadataTypeDef):
     pass
 
+_RequiredCreateCapacityReservationInputRequestTypeDef = TypedDict(
+    "_RequiredCreateCapacityReservationInputRequestTypeDef",
+    {
+        "TargetDpus": int,
+        "Name": str,
+    },
+)
+_OptionalCreateCapacityReservationInputRequestTypeDef = TypedDict(
+    "_OptionalCreateCapacityReservationInputRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateCapacityReservationInputRequestTypeDef(
+    _RequiredCreateCapacityReservationInputRequestTypeDef,
+    _OptionalCreateCapacityReservationInputRequestTypeDef,
+):
+    pass
+
 _RequiredCreateDataCatalogInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataCatalogInputRequestTypeDef",
     {
         "Name": str,
         "Type": DataCatalogTypeType,
     },
 )
@@ -1604,15 +1866,15 @@
     pass
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1621,40 +1883,40 @@
 )
 
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
@@ -1723,15 +1985,15 @@
     pass
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
@@ -1745,41 +2007,41 @@
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
         "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNotebookMetadataOutputTypeDef = TypedDict(
     "GetNotebookMetadataOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
         "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -1797,128 +2059,20 @@
 
 class ListNotebookMetadataInputRequestTypeDef(
     _RequiredListNotebookMetadataInputRequestTypeDef,
     _OptionalListNotebookMetadataInputRequestTypeDef,
 ):
     pass
 
-_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "QueryExecutionId": str,
-    },
-)
-_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
-    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-):
-    pass
-
-ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "CatalogName": str,
-    },
-)
-_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatabasesInputListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
-):
-    pass
-
-ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "CatalogName": str,
-        "DatabaseName": str,
-    },
-)
-_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "Expression": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTableMetadataInputListTableMetadataPaginateTypeDef(
-    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
-    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
-):
-    pass
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 GetSessionStatusResponseTypeDef = TypedDict(
     "GetSessionStatusResponseTypeDef",
     {
         "SessionId": str,
         "Status": SessionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
@@ -1931,24 +2085,24 @@
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
@@ -1982,32 +2136,57 @@
 )
 
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCapacityReservationOutputTypeDef = TypedDict(
+    "GetCapacityReservationOutputTypeDef",
+    {
+        "CapacityReservation": CapacityReservationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCapacityReservationsOutputTypeDef = TypedDict(
+    "ListCapacityReservationsOutputTypeDef",
+    {
+        "NextToken": str,
+        "CapacityReservations": List[CapacityReservationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
+    "GetCapacityAssignmentConfigurationOutputTypeDef",
+    {
+        "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": List[RowTypeDef],
@@ -2024,14 +2203,15 @@
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
         "AdditionalConfiguration": str,
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
+        "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
 WorkGroupConfigurationUpdatesTypeDef = TypedDict(
     "WorkGroupConfigurationUpdatesTypeDef",
     {
@@ -2042,14 +2222,15 @@
         "RemoveBytesScannedCutoffPerQuery": bool,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
         "RemoveCustomerContentEncryptionConfiguration": bool,
         "AdditionalConfiguration": str,
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
+        "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
@@ -2058,41 +2239,41 @@
         "WorkGroup": str,
         "EngineVersion": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
@@ -2137,15 +2318,15 @@
 
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
@@ -2208,26 +2389,26 @@
     pass
 
 BatchGetQueryExecutionOutputTypeDef = TypedDict(
     "BatchGetQueryExecutionOutputTypeDef",
     {
         "QueryExecutions": List[QueryExecutionTypeDef],
         "UnprocessedQueryExecutionIds": List[UnprocessedQueryExecutionIdTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryExecutionOutputTypeDef = TypedDict(
     "GetQueryExecutionOutputTypeDef",
     {
         "QueryExecution": QueryExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkGroupOutputTypeDef = TypedDict(
     "GetWorkGroupOutputTypeDef",
     {
         "WorkGroup": WorkGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.26.87
-Summary: Type annotations for boto3.Athena 1.26.87 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Athena 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-athena"></a>
 
 # mypy-boto3-athena
 
 [![PyPI - mypy-boto3-athena](https://img.shields.io/pypi/v/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,14 +317,16 @@
 
 `mypy_boto3_athena.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_athena.literals import (
     CalculationExecutionStateType,
+    CapacityAllocationStatusType,
+    CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
     ExecutorStateType,
     ExecutorTypeType,
     GetQueryResultsPaginatorName,
     ListDataCatalogsPaginatorName,
@@ -361,124 +363,143 @@
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
+    CancelCapacityReservationInputRequestTypeDef,
+    CapacityAllocationTypeDef,
+    CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
+    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
+    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
+    DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
     EngineConfigurationTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
+    GetCapacityAssignmentConfigurationInputRequestTypeDef,
+    GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
+    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
+    ListCapacityReservationsInputRequestTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
+    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
+    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
+    ResponseMetadataTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
+    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
+    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
-    CreateNamedQueryOutputTypeDef,
-    CreateNotebookOutputTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
-    ImportNotebookOutputTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
-    ListNamedQueriesOutputTypeDef,
-    ListQueryExecutionsOutputTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
-    StopCalculationExecutionResponseTypeDef,
-    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
+    CapacityReservationTypeDef,
+    CapacityAssignmentConfigurationTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
+    CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
@@ -490,29 +511,25 @@
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
+    GetCapacityReservationOutputTypeDef,
+    ListCapacityReservationsOutputTypeDef,
+    GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -537,42 +554,42 @@
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

### Comparing `mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.27.0/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.87/setup.py` & `mypy-boto3-athena-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-athena.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.26.87",
+    version="1.27.0",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Athena 1.26.87 service generated with mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.Athena 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/",
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


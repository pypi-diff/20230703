# Comparing `tmp/mypy-boto3-cleanrooms-1.26.96.tar.gz` & `tmp/mypy-boto3-cleanrooms-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.26.96.tar", last modified: Tue Mar 21 19:19:40 2023, max compression
+gzip compressed data, was "mypy-boto3-cleanrooms-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-cleanrooms-1.26.96.tar` & `mypy-boto3-cleanrooms-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17430 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29891 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29840 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-03-21 19:18:33.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41217 2023-03-21 19:18:33.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41164 2023-03-21 19:18:33.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.162939 mypy-boto3-cleanrooms-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-07-03 19:50:29.162939 mypy-boto3-cleanrooms-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.150939 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-07-03 19:33:34.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29837 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-03 19:33:34.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-03 19:33:34.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-03 19:33:34.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-03 19:33:34.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-03 19:33:35.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41640 2023-07-03 19:33:34.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.162939 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-07-03 19:50:28.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:29.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:28.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:28.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:28.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:28.000000 mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.162939 mypy-boto3-cleanrooms-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:33:33.000000 mypy-boto3-cleanrooms-1.27.0/setup.py
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/LICENSE` & `mypy-boto3-cleanrooms-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cleanrooms-1.26.96/PKG-INFO` & `mypy-boto3-cleanrooms-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.26.96
-Summary: Type annotations for boto3.CleanRoomsService 1.26.96 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.CleanRoomsService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cleanrooms"></a>
 
 # mypy-boto3-cleanrooms
 
 [![PyPI - mypy-boto3-cleanrooms](https://img.shields.io/pypi/v/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
     AggregateFunctionNameType,
     AggregationTypeType,
     AnalysisMethodType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     JoinRequiredOptionType,
     ListCollaborationsPaginatorName,
     ListConfiguredTableAssociationsPaginatorName,
     ListConfiguredTablesPaginatorName,
     ListMembersPaginatorName,
     ListMembershipsPaginatorName,
     ListProtectedQueriesPaginatorName,
@@ -370,15 +371,14 @@
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
     AggregateColumnTypeDef,
     AggregationConstraintTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
     DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
     MemberSpecificationTypeDef,
@@ -396,61 +396,62 @@
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     GlueTableReferenceTypeDef,
-    PaginatorConfigTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
     ListCollaborationsInputRequestTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     TableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
@@ -492,42 +493,42 @@
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

### Comparing `mypy-boto3-cleanrooms-1.26.96/README.md` & `mypy-boto3-cleanrooms-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cleanrooms"></a>
 
 # mypy-boto3-cleanrooms
 
 [![PyPI - mypy-boto3-cleanrooms](https://img.shields.io/pypi/v/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,14 +294,15 @@
     AggregateFunctionNameType,
     AggregationTypeType,
     AnalysisMethodType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     JoinRequiredOptionType,
     ListCollaborationsPaginatorName,
     ListConfiguredTableAssociationsPaginatorName,
     ListConfiguredTablesPaginatorName,
     ListMembersPaginatorName,
     ListMembershipsPaginatorName,
     ListProtectedQueriesPaginatorName,
@@ -338,15 +339,14 @@
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
     AggregateColumnTypeDef,
     AggregationConstraintTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
     DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
     MemberSpecificationTypeDef,
@@ -364,61 +364,62 @@
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     GlueTableReferenceTypeDef,
-    PaginatorConfigTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
     ListCollaborationsInputRequestTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     TableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
@@ -460,42 +461,42 @@
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

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.py` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.pyi` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__main__.py` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsService 1.26.96\nVersion:         1.26.96\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.CleanRoomsService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.96")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.py` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
         resultConfiguration: ProtectedQueryResultConfigurationTypeDef
     ) -> StartProtectedQueryOutputTypeDef:
         """
-        Creates a protected query that is started by AWS Clean Rooms.
+        Creates a protected query that is started by Clean Rooms .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#start_protected_query)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.pyi` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
         resultConfiguration: ProtectedQueryResultConfigurationTypeDef
     ) -> StartProtectedQueryOutputTypeDef:
         """
-        Creates a protected query that is started by AWS Clean Rooms.
+        Creates a protected query that is started by Clean Rooms .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#start_protected_query)
         """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource.
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.py` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
     "FilterableMemberStatusType",
+    "JoinOperatorType",
     "JoinRequiredOptionType",
     "ListCollaborationsPaginatorName",
     "ListConfiguredTableAssociationsPaginatorName",
     "ListConfiguredTablesPaginatorName",
     "ListMembersPaginatorName",
     "ListMembershipsPaginatorName",
     "ListProtectedQueriesPaginatorName",
@@ -56,14 +57,15 @@
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
+JoinOperatorType = Literal["AND", "OR"]
 JoinRequiredOptionType = Literal["QUERY_RUNNER"]
 ListCollaborationsPaginatorName = Literal["list_collaborations"]
 ListConfiguredTableAssociationsPaginatorName = Literal["list_configured_table_associations"]
 ListConfiguredTablesPaginatorName = Literal["list_configured_tables"]
 ListMembersPaginatorName = Literal["list_members"]
 ListMembershipsPaginatorName = Literal["list_memberships"]
 ListProtectedQueriesPaginatorName = Literal["list_protected_queries"]
@@ -106,14 +108,15 @@
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
@@ -153,14 +156,15 @@
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
@@ -258,14 +262,15 @@
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
@@ -301,14 +306,15 @@
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
@@ -327,16 +333,19 @@
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
@@ -420,15 +429,17 @@
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

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.pyi` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
     "FilterableMemberStatusType",
+    "JoinOperatorType",
     "JoinRequiredOptionType",
     "ListCollaborationsPaginatorName",
     "ListConfiguredTableAssociationsPaginatorName",
     "ListConfiguredTablesPaginatorName",
     "ListMembersPaginatorName",
     "ListMembershipsPaginatorName",
     "ListProtectedQueriesPaginatorName",
@@ -54,14 +55,15 @@
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
+JoinOperatorType = Literal["AND", "OR"]
 JoinRequiredOptionType = Literal["QUERY_RUNNER"]
 ListCollaborationsPaginatorName = Literal["list_collaborations"]
 ListConfiguredTableAssociationsPaginatorName = Literal["list_configured_table_associations"]
 ListConfiguredTablesPaginatorName = Literal["list_configured_tables"]
 ListMembersPaginatorName = Literal["list_members"]
 ListMembershipsPaginatorName = Literal["list_memberships"]
 ListProtectedQueriesPaginatorName = Literal["list_protected_queries"]
@@ -104,14 +106,15 @@
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
@@ -151,14 +154,15 @@
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
@@ -256,14 +260,15 @@
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
@@ -299,14 +304,15 @@
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
@@ -325,16 +331,19 @@
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
@@ -418,15 +427,17 @@
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

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.py` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -49,143 +49,136 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
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
 class ListCollaborationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
-
 class ListConfiguredTableAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
-        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, membershipIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
-
 class ListConfiguredTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
-
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, collaborationIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
         """
 
-
 class ListMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
-        self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        status: MembershipStatusType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
         """
 
-
 class ListProtectedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
-
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.pyi` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,133 +49,146 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
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
 class ListCollaborationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
+
 class ListConfiguredTableAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
-        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, membershipIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
+
 class ListConfiguredTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
+
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, collaborationIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
         """
 
+
 class ListMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
-        self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        status: MembershipStatusType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
         """
 
+
 class ListProtectedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
+
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.py` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
     MembershipStatusType,
     MemberStatusType,
     ProtectedQueryStatusType,
     ResultFormatType,
     ScalarFunctionsType,
@@ -42,15 +43,14 @@
 
 __all__ = (
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
     "MemberSpecificationTypeDef",
@@ -68,61 +68,62 @@
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "GlueTableReferenceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     "ListCollaborationsInputRequestTypeDef",
+    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
+    "ListMembersInputListMembersPaginateTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
+    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
     "TableReferenceTypeDef",
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
-    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    "ListMembersInputListMembersPaginateTypeDef",
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
@@ -169,21 +170,33 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
-AnalysisRuleListTypeDef = TypedDict(
-    "AnalysisRuleListTypeDef",
+_RequiredAnalysisRuleListTypeDef = TypedDict(
+    "_RequiredAnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
+_OptionalAnalysisRuleListTypeDef = TypedDict(
+    "_OptionalAnalysisRuleListTypeDef",
+    {
+        "allowedJoinOperators": Sequence[JoinOperatorType],
+    },
+    total=False,
+)
+
+
+class AnalysisRuleListTypeDef(_RequiredAnalysisRuleListTypeDef, _OptionalAnalysisRuleListTypeDef):
+    pass
+
 
 BatchGetSchemaErrorTypeDef = TypedDict(
     "BatchGetSchemaErrorTypeDef",
     {
         "name": str,
         "code": str,
         "message": str,
@@ -194,25 +207,14 @@
     "BatchGetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "names": Sequence[str],
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
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -499,34 +501,55 @@
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "memberStatus": FilterableMemberStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
     total=False,
 )
 
+_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
+    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
     "_RequiredListConfiguredTableAssociationsInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
@@ -542,23 +565,53 @@
 class ListConfiguredTableAssociationsInputRequestTypeDef(
     _RequiredListConfiguredTableAssociationsInputRequestTypeDef,
     _OptionalListConfiguredTableAssociationsInputRequestTypeDef,
 ):
     pass
 
 
+ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConfiguredTablesInputRequestTypeDef = TypedDict(
     "ListConfiguredTablesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersInputListMembersPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersInputListMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListMembersInputListMembersPaginateTypeDef(
+    _RequiredListMembersInputListMembersPaginateTypeDef,
+    _OptionalListMembersInputListMembersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListMembersInputRequestTypeDef = TypedDict(
     "_RequiredListMembersInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListMembersInputRequestTypeDef = TypedDict(
@@ -598,14 +651,23 @@
 )
 
 
 class MemberSummaryTypeDef(_RequiredMemberSummaryTypeDef, _OptionalMemberSummaryTypeDef):
     pass
 
 
+ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    {
+        "status": MembershipStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMembershipsInputRequestTypeDef = TypedDict(
     "ListMembershipsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": MembershipStatusType,
     },
@@ -625,14 +687,37 @@
         "createTime": datetime,
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
     },
 )
 
+_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "status": ProtectedQueryStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
+    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListProtectedQueriesInputRequestTypeDef = TypedDict(
     "_RequiredListProtectedQueriesInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListProtectedQueriesInputRequestTypeDef = TypedDict(
@@ -660,14 +745,37 @@
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
         "status": ProtectedQueryStatusType,
     },
 )
 
+_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "schemaType": Literal["TABLE"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSchemasInputListSchemasPaginateTypeDef(
+    _RequiredListSchemasInputListSchemasPaginateTypeDef,
+    _OptionalListSchemasInputListSchemasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSchemasInputRequestTypeDef = TypedDict(
     "_RequiredListSchemasInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListSchemasInputRequestTypeDef = TypedDict(
@@ -716,14 +824,32 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
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
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
@@ -759,24 +885,36 @@
 )
 
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
     },
+    total=False,
 )
 
 ProtectedQueryStatisticsTypeDef = TypedDict(
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -898,39 +1036,32 @@
         "outputConstraints": Sequence[AggregationConstraintTypeDef],
     },
 )
 _OptionalAnalysisRuleAggregationTypeDef = TypedDict(
     "_OptionalAnalysisRuleAggregationTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
+        "allowedJoinOperators": Sequence[JoinOperatorType],
     },
     total=False,
 )
 
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCollaborationTypeDef = TypedDict(
     "_RequiredCollaborationTypeDef",
     {
         "id": str,
@@ -990,48 +1121,48 @@
 
 
 ListConfiguredTableAssociationsOutputTypeDef = TypedDict(
     "ListConfiguredTableAssociationsOutputTypeDef",
     {
         "configuredTableAssociationSummaries": List[ConfiguredTableAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "CreateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConfiguredTableAssociationOutputTypeDef = TypedDict(
     "GetConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfiguredTablesOutputTypeDef = TypedDict(
     "ListConfiguredTablesOutputTypeDef",
     {
         "configuredTableSummaries": List[ConfiguredTableSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredCreateCollaborationInputRequestTypeDef",
     {
         "members": Sequence[MemberSpecificationTypeDef],
@@ -1058,191 +1189,75 @@
     pass
 
 
 CreateMembershipOutputTypeDef = TypedDict(
     "CreateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMembershipOutputTypeDef = TypedDict(
     "GetMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMembershipOutputTypeDef = TypedDict(
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableReferenceTypeDef = TypedDict(
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
-ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
-    {
-        "memberStatus": FilterableMemberStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
-    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-):
-    pass
-
-
-ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersInputListMembersPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersInputListMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListMembersInputListMembersPaginateTypeDef(
-    _RequiredListMembersInputListMembersPaginateTypeDef,
-    _OptionalListMembersInputListMembersPaginateTypeDef,
-):
-    pass
-
-
-ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    {
-        "status": MembershipStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "status": ProtectedQueryStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
-    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "schemaType": Literal["TABLE"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSchemasInputListSchemasPaginateTypeDef(
-    _RequiredListSchemasInputListSchemasPaginateTypeDef,
-    _OptionalListSchemasInputListSchemasPaginateTypeDef,
-):
-    pass
-
-
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "nextToken": str,
         "memberSummaries": List[MemberSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMembershipsOutputTypeDef = TypedDict(
     "ListMembershipsOutputTypeDef",
     {
         "nextToken": str,
         "membershipSummaries": List[MembershipSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtectedQueriesOutputTypeDef = TypedDict(
     "ListProtectedQueriesOutputTypeDef",
     {
         "nextToken": str,
         "protectedQueries": List[ProtectedQuerySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasOutputTypeDef = TypedDict(
     "ListSchemasOutputTypeDef",
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
@@ -1276,48 +1291,48 @@
     total=False,
 )
 
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCollaborationOutputTypeDef = TypedDict(
     "GetCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCollaborationOutputTypeDef = TypedDict(
     "UpdateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetSchemaOutputTypeDef = TypedDict(
     "BatchGetSchemaOutputTypeDef",
     {
         "schemas": List[SchemaTypeDef],
         "errors": List[BatchGetSchemaErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaOutputTypeDef = TypedDict(
     "GetSchemaOutputTypeDef",
     {
         "schema": SchemaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
@@ -1400,31 +1415,31 @@
     total=False,
 )
 
 CreateConfiguredTableOutputTypeDef = TypedDict(
     "CreateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConfiguredTableOutputTypeDef = TypedDict(
     "GetConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfiguredTableOutputTypeDef = TypedDict(
     "UpdateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartProtectedQueryInputRequestTypeDef = TypedDict(
     "StartProtectedQueryInputRequestTypeDef",
     {
         "type": Literal["SQL"],
@@ -1503,58 +1518,58 @@
     },
 )
 
 GetProtectedQueryOutputTypeDef = TypedDict(
     "GetProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartProtectedQueryOutputTypeDef = TypedDict(
     "StartProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProtectedQueryOutputTypeDef = TypedDict(
     "UpdateProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaAnalysisRuleOutputTypeDef = TypedDict(
     "GetSchemaAnalysisRuleOutputTypeDef",
     {
         "analysisRule": AnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.pyi` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
     MembershipStatusType,
     MemberStatusType,
     ProtectedQueryStatusType,
     ResultFormatType,
     ScalarFunctionsType,
@@ -41,15 +42,14 @@
 
 __all__ = (
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
     "MemberSpecificationTypeDef",
@@ -67,61 +67,62 @@
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "GlueTableReferenceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     "ListCollaborationsInputRequestTypeDef",
+    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
+    "ListMembersInputListMembersPaginateTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
+    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
     "TableReferenceTypeDef",
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
-    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    "ListMembersInputListMembersPaginateTypeDef",
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
@@ -168,21 +169,31 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
-AnalysisRuleListTypeDef = TypedDict(
-    "AnalysisRuleListTypeDef",
+_RequiredAnalysisRuleListTypeDef = TypedDict(
+    "_RequiredAnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
+_OptionalAnalysisRuleListTypeDef = TypedDict(
+    "_OptionalAnalysisRuleListTypeDef",
+    {
+        "allowedJoinOperators": Sequence[JoinOperatorType],
+    },
+    total=False,
+)
+
+class AnalysisRuleListTypeDef(_RequiredAnalysisRuleListTypeDef, _OptionalAnalysisRuleListTypeDef):
+    pass
 
 BatchGetSchemaErrorTypeDef = TypedDict(
     "BatchGetSchemaErrorTypeDef",
     {
         "name": str,
         "code": str,
         "message": str,
@@ -193,25 +204,14 @@
     "BatchGetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "names": Sequence[str],
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
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -490,34 +490,53 @@
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "memberStatus": FilterableMemberStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
     total=False,
 )
 
+_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
+    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
     "_RequiredListConfiguredTableAssociationsInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
@@ -531,23 +550,51 @@
 
 class ListConfiguredTableAssociationsInputRequestTypeDef(
     _RequiredListConfiguredTableAssociationsInputRequestTypeDef,
     _OptionalListConfiguredTableAssociationsInputRequestTypeDef,
 ):
     pass
 
+ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConfiguredTablesInputRequestTypeDef = TypedDict(
     "ListConfiguredTablesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersInputListMembersPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersInputListMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListMembersInputListMembersPaginateTypeDef(
+    _RequiredListMembersInputListMembersPaginateTypeDef,
+    _OptionalListMembersInputListMembersPaginateTypeDef,
+):
+    pass
+
 _RequiredListMembersInputRequestTypeDef = TypedDict(
     "_RequiredListMembersInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListMembersInputRequestTypeDef = TypedDict(
@@ -583,14 +630,23 @@
     },
     total=False,
 )
 
 class MemberSummaryTypeDef(_RequiredMemberSummaryTypeDef, _OptionalMemberSummaryTypeDef):
     pass
 
+ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    {
+        "status": MembershipStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMembershipsInputRequestTypeDef = TypedDict(
     "ListMembershipsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": MembershipStatusType,
     },
@@ -610,14 +666,35 @@
         "createTime": datetime,
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
     },
 )
 
+_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "status": ProtectedQueryStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
+    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+):
+    pass
+
 _RequiredListProtectedQueriesInputRequestTypeDef = TypedDict(
     "_RequiredListProtectedQueriesInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListProtectedQueriesInputRequestTypeDef = TypedDict(
@@ -643,14 +720,35 @@
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
         "status": ProtectedQueryStatusType,
     },
 )
 
+_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "schemaType": Literal["TABLE"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSchemasInputListSchemasPaginateTypeDef(
+    _RequiredListSchemasInputListSchemasPaginateTypeDef,
+    _OptionalListSchemasInputListSchemasPaginateTypeDef,
+):
+    pass
+
 _RequiredListSchemasInputRequestTypeDef = TypedDict(
     "_RequiredListSchemasInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListSchemasInputRequestTypeDef = TypedDict(
@@ -695,14 +793,32 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
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
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
@@ -736,24 +852,36 @@
 )
 
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
     },
+    total=False,
 )
 
 ProtectedQueryStatisticsTypeDef = TypedDict(
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -867,37 +995,30 @@
         "outputConstraints": Sequence[AggregationConstraintTypeDef],
     },
 )
 _OptionalAnalysisRuleAggregationTypeDef = TypedDict(
     "_OptionalAnalysisRuleAggregationTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
+        "allowedJoinOperators": Sequence[JoinOperatorType],
     },
     total=False,
 )
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCollaborationTypeDef = TypedDict(
     "_RequiredCollaborationTypeDef",
     {
         "id": str,
@@ -953,48 +1074,48 @@
     pass
 
 ListConfiguredTableAssociationsOutputTypeDef = TypedDict(
     "ListConfiguredTableAssociationsOutputTypeDef",
     {
         "configuredTableAssociationSummaries": List[ConfiguredTableAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "CreateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConfiguredTableAssociationOutputTypeDef = TypedDict(
     "GetConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfiguredTablesOutputTypeDef = TypedDict(
     "ListConfiguredTablesOutputTypeDef",
     {
         "configuredTableSummaries": List[ConfiguredTableSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredCreateCollaborationInputRequestTypeDef",
     {
         "members": Sequence[MemberSpecificationTypeDef],
@@ -1019,183 +1140,75 @@
 ):
     pass
 
 CreateMembershipOutputTypeDef = TypedDict(
     "CreateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMembershipOutputTypeDef = TypedDict(
     "GetMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMembershipOutputTypeDef = TypedDict(
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableReferenceTypeDef = TypedDict(
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
-ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
-    {
-        "memberStatus": FilterableMemberStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
-    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-):
-    pass
-
-ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersInputListMembersPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersInputListMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListMembersInputListMembersPaginateTypeDef(
-    _RequiredListMembersInputListMembersPaginateTypeDef,
-    _OptionalListMembersInputListMembersPaginateTypeDef,
-):
-    pass
-
-ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    {
-        "status": MembershipStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "status": ProtectedQueryStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
-    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-):
-    pass
-
-_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "schemaType": Literal["TABLE"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSchemasInputListSchemasPaginateTypeDef(
-    _RequiredListSchemasInputListSchemasPaginateTypeDef,
-    _OptionalListSchemasInputListSchemasPaginateTypeDef,
-):
-    pass
-
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "nextToken": str,
         "memberSummaries": List[MemberSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMembershipsOutputTypeDef = TypedDict(
     "ListMembershipsOutputTypeDef",
     {
         "nextToken": str,
         "membershipSummaries": List[MembershipSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtectedQueriesOutputTypeDef = TypedDict(
     "ListProtectedQueriesOutputTypeDef",
     {
         "nextToken": str,
         "protectedQueries": List[ProtectedQuerySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasOutputTypeDef = TypedDict(
     "ListSchemasOutputTypeDef",
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
@@ -1229,48 +1242,48 @@
     total=False,
 )
 
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCollaborationOutputTypeDef = TypedDict(
     "GetCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCollaborationOutputTypeDef = TypedDict(
     "UpdateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetSchemaOutputTypeDef = TypedDict(
     "BatchGetSchemaOutputTypeDef",
     {
         "schemas": List[SchemaTypeDef],
         "errors": List[BatchGetSchemaErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaOutputTypeDef = TypedDict(
     "GetSchemaOutputTypeDef",
     {
         "schema": SchemaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
@@ -1349,31 +1362,31 @@
     total=False,
 )
 
 CreateConfiguredTableOutputTypeDef = TypedDict(
     "CreateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConfiguredTableOutputTypeDef = TypedDict(
     "GetConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfiguredTableOutputTypeDef = TypedDict(
     "UpdateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartProtectedQueryInputRequestTypeDef = TypedDict(
     "StartProtectedQueryInputRequestTypeDef",
     {
         "type": Literal["SQL"],
@@ -1450,58 +1463,58 @@
     },
 )
 
 GetProtectedQueryOutputTypeDef = TypedDict(
     "GetProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartProtectedQueryOutputTypeDef = TypedDict(
     "StartProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProtectedQueryOutputTypeDef = TypedDict(
     "UpdateProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaAnalysisRuleOutputTypeDef = TypedDict(
     "GetSchemaAnalysisRuleOutputTypeDef",
     {
         "analysisRule": AnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/PKG-INFO` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.26.96
-Summary: Type annotations for boto3.CleanRoomsService 1.26.96 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.CleanRoomsService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cleanrooms"></a>
 
 # mypy-boto3-cleanrooms
 
 [![PyPI - mypy-boto3-cleanrooms](https://img.shields.io/pypi/v/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
     AggregateFunctionNameType,
     AggregationTypeType,
     AnalysisMethodType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     JoinRequiredOptionType,
     ListCollaborationsPaginatorName,
     ListConfiguredTableAssociationsPaginatorName,
     ListConfiguredTablesPaginatorName,
     ListMembersPaginatorName,
     ListMembershipsPaginatorName,
     ListProtectedQueriesPaginatorName,
@@ -370,15 +371,14 @@
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
     AggregateColumnTypeDef,
     AggregationConstraintTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
     DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
     MemberSpecificationTypeDef,
@@ -396,61 +396,62 @@
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     GlueTableReferenceTypeDef,
-    PaginatorConfigTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
     ListCollaborationsInputRequestTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     TableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
@@ -492,42 +493,42 @@
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

### Comparing `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/SOURCES.txt` & `mypy-boto3-cleanrooms-1.27.0/mypy_boto3_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.96/setup.py` & `mypy-boto3-cleanrooms-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-cleanrooms.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cleanrooms",
-    version="1.26.96",
+    version="1.27.0",
     packages=["mypy_boto3_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CleanRoomsService 1.26.96 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.CleanRoomsService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/",
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


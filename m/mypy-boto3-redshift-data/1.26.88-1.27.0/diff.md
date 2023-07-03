# Comparing `tmp/mypy-boto3-redshift-data-1.26.88.tar.gz` & `tmp/mypy-boto3-redshift-data-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-data-1.26.88.tar", last modified: Thu Mar  9 20:38:41 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-data-1.27.0.tar", last modified: Mon Jul  3 19:51:18 2023, max compression
```

## Comparing `mypy-boto3-redshift-data-1.26.88.tar` & `mypy-boto3-redshift-data-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-09 20:37:53.000000 mypy-boto3-redshift-data-1.26.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:18.827862 mypy-boto3-redshift-data-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-03 19:51:18.827862 mypy-boto3-redshift-data-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:18.823862 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:18.827862 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-03 19:51:18.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:51:18.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:18.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:18.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:18.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:18.000000 mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:18.827862 mypy-boto3-redshift-data-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-03 19:46:06.000000 mypy-boto3-redshift-data-1.27.0/setup.py
```

### Comparing `mypy-boto3-redshift-data-1.26.88/LICENSE` & `mypy-boto3-redshift-data-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-redshift-data-1.26.88/PKG-INFO` & `mypy-boto3-redshift-data-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.26.88
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-redshift-data"></a>
 
 # mypy-boto3-redshift-data
 
 [![PyPI - mypy-boto3-redshift-data](https://img.shields.io/pypi/v/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,44 +341,44 @@
 
 `mypy_boto3_redshift_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
     CancelStatementRequestRequestTypeDef,
+    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
     SqlParameterTypeDef,
     SubStatementDataTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
     DescribeTableRequestRequestTypeDef,
+    ExecuteStatementOutputTypeDef,
     FieldTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
+    ListSchemasResponseTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    CancelStatementResponseTypeDef,
-    ExecuteStatementOutputTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     DescribeTableResponseTypeDef,
     ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
@@ -388,42 +388,42 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.88/README.md` & `mypy-boto3-redshift-data-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-redshift-data"></a>
 
 # mypy-boto3-redshift-data
 
 [![PyPI - mypy-boto3-redshift-data](https://img.shields.io/pypi/v/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,44 +309,44 @@
 
 `mypy_boto3_redshift_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
     CancelStatementRequestRequestTypeDef,
+    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
     SqlParameterTypeDef,
     SubStatementDataTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
     DescribeTableRequestRequestTypeDef,
+    ExecuteStatementOutputTypeDef,
     FieldTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
+    ListSchemasResponseTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    CancelStatementResponseTypeDef,
-    ExecuteStatementOutputTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     DescribeTableResponseTypeDef,
     ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
@@ -356,42 +356,42 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.py` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.pyi` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__main__.py` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftDataAPIService 1.26.88\nVersion:        "
-        " 1.26.88\nBuilder version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.RedshiftDataAPIService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.88")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.py` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.pyi` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.py` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -104,14 +105,15 @@
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
@@ -209,14 +211,15 @@
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
@@ -252,14 +255,15 @@
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
@@ -278,16 +282,19 @@
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
@@ -371,15 +378,17 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.pyi` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -102,14 +103,15 @@
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
@@ -207,14 +209,15 @@
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
@@ -250,14 +253,15 @@
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
@@ -276,16 +280,19 @@
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
@@ -369,15 +376,17 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.py` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,30 +77,30 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#describetablepaginator)
         """
 
 
 class GetStatementResultPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
     """
 
     def paginate(
-        self, *, Id: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetStatementResultResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
         """
 
 
@@ -114,15 +114,15 @@
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listdatabasespaginator)
         """
 
 
@@ -138,15 +138,15 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listschemaspaginator)
         """
 
 
@@ -158,15 +158,15 @@
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#liststatementspaginator)
         """
 
 
@@ -183,13 +183,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.pyi` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,29 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#describetablepaginator)
         """
 
 class GetStatementResultPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
     """
 
     def paginate(
-        self, *, Id: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetStatementResultResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
         """
 
 class ListDatabasesPaginator(Paginator):
@@ -109,15 +109,15 @@
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listdatabasespaginator)
         """
 
 class ListSchemasPaginator(Paginator):
@@ -132,15 +132,15 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listschemaspaginator)
         """
 
 class ListStatementsPaginator(Paginator):
@@ -151,15 +151,15 @@
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#liststatementspaginator)
         """
 
 class ListTablesPaginator(Paginator):
@@ -175,13 +175,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.py` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,44 +21,44 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
     "CancelStatementRequestRequestTypeDef",
+    "CancelStatementResponseTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
     "SqlParameterTypeDef",
     "SubStatementDataTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeTableRequestDescribeTablePaginateTypeDef",
     "DescribeTableRequestRequestTypeDef",
+    "ExecuteStatementOutputTypeDef",
     "FieldTypeDef",
+    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "GetStatementResultRequestRequestTypeDef",
+    "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListDatabasesRequestRequestTypeDef",
+    "ListDatabasesResponseTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
+    "ListSchemasResponseTypeDef",
+    "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListStatementsRequestRequestTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
-    "CancelStatementResponseTypeDef",
-    "ExecuteStatementOutputTypeDef",
-    "ListDatabasesResponseTypeDef",
-    "ListSchemasResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeTableResponseTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
-    "DescribeTableRequestDescribeTablePaginateTypeDef",
-    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
-    "ListDatabasesRequestListDatabasesPaginateTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -85,32 +85,43 @@
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelStatementRequestRequestTypeDef = TypedDict(
     "CancelStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+CancelStatementResponseTypeDef = TypedDict(
+    "CancelStatementResponseTypeDef",
+    {
+        "Status": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "columnDefault": str,
         "isCaseSensitive": bool,
         "isCurrency": bool,
         "isSigned": bool,
@@ -166,24 +177,43 @@
 )
 
 
 class SubStatementDataTypeDef(_RequiredSubStatementDataTypeDef, _OptionalSubStatementDataTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Database": str,
+    },
+)
+_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "Schema": str,
+        "SecretArn": str,
+        "Table": str,
+        "WorkgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeTableRequestDescribeTablePaginateTypeDef(
+    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
+    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeTableRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTableRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalDescribeTableRequestRequestTypeDef = TypedDict(
@@ -205,27 +235,63 @@
 
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
 
+ExecuteStatementOutputTypeDef = TypedDict(
+    "ExecuteStatementOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
         "booleanValue": bool,
         "doubleValue": float,
         "isNull": bool,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
 )
 
+_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetStatementResultRequestGetStatementResultPaginateTypeDef(
+    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
+    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetStatementResultRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementResultRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStatementResultRequestRequestTypeDef = TypedDict(
@@ -240,14 +306,40 @@
 class GetStatementResultRequestRequestTypeDef(
     _RequiredGetStatementResultRequestRequestTypeDef,
     _OptionalGetStatementResultRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDatabasesRequestListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatabasesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListDatabasesRequestRequestTypeDef = TypedDict(
@@ -266,14 +358,51 @@
 
 class ListDatabasesRequestRequestTypeDef(
     _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
 ):
     pass
 
 
+ListDatabasesResponseTypeDef = TypedDict(
+    "ListDatabasesResponseTypeDef",
+    {
+        "Databases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -294,26 +423,75 @@
 
 class ListSchemasRequestRequestTypeDef(
     _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
 ):
     pass
 
 
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
+    {
+        "NextToken": str,
+        "Schemas": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    {
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStatementsRequestRequestTypeDef = TypedDict(
     "ListStatementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RoleLevel": bool,
         "StatementName": str,
         "Status": StatusStringType,
     },
     total=False,
 )
 
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "TablePattern": str,
+        "WorkgroupName": str,
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
         "Database": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -345,75 +523,42 @@
         "name": str,
         "schema": str,
         "type": str,
     },
     total=False,
 )
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelStatementResponseTypeDef = TypedDict(
-    "CancelStatementResponseTypeDef",
-    {
-        "Status": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExecuteStatementOutputTypeDef = TypedDict(
-    "ExecuteStatementOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatabasesResponseTypeDef = TypedDict(
-    "ListDatabasesResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Databases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NextToken": str,
-        "Schemas": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "ColumnList": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "TableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Database": str,
@@ -487,184 +632,39 @@
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
         "SubStatements": List[SubStatementDataTypeDef],
         "UpdatedAt": datetime,
         "WorkgroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "Schema": str,
-        "SecretArn": str,
-        "Table": str,
-        "WorkgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeTableRequestDescribeTablePaginateTypeDef(
-    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
-    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetStatementResultRequestGetStatementResultPaginateTypeDef(
-    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
-    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatabasesRequestListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-
-ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    {
-        "RoleLevel": bool,
-        "StatementName": str,
-        "Status": StatusStringType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "TablePattern": str,
-        "WorkgroupName": str,
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
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "NextToken": str,
         "Tables": List[TableMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "NextToken": str,
         "Statements": List[StatementDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.pyi` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -20,44 +20,44 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
     "CancelStatementRequestRequestTypeDef",
+    "CancelStatementResponseTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
     "SqlParameterTypeDef",
     "SubStatementDataTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeTableRequestDescribeTablePaginateTypeDef",
     "DescribeTableRequestRequestTypeDef",
+    "ExecuteStatementOutputTypeDef",
     "FieldTypeDef",
+    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "GetStatementResultRequestRequestTypeDef",
+    "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListDatabasesRequestRequestTypeDef",
+    "ListDatabasesResponseTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
+    "ListSchemasResponseTypeDef",
+    "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListStatementsRequestRequestTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
-    "CancelStatementResponseTypeDef",
-    "ExecuteStatementOutputTypeDef",
-    "ListDatabasesResponseTypeDef",
-    "ListSchemasResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeTableResponseTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
-    "DescribeTableRequestDescribeTablePaginateTypeDef",
-    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
-    "ListDatabasesRequestListDatabasesPaginateTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -82,32 +82,43 @@
 
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelStatementRequestRequestTypeDef = TypedDict(
     "CancelStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+CancelStatementResponseTypeDef = TypedDict(
+    "CancelStatementResponseTypeDef",
+    {
+        "Status": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "columnDefault": str,
         "isCaseSensitive": bool,
         "isCurrency": bool,
         "isSigned": bool,
@@ -161,24 +172,41 @@
     },
     total=False,
 )
 
 class SubStatementDataTypeDef(_RequiredSubStatementDataTypeDef, _OptionalSubStatementDataTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Database": str,
+    },
+)
+_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "Schema": str,
+        "SecretArn": str,
+        "Table": str,
+        "WorkgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeTableRequestDescribeTablePaginateTypeDef(
+    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
+    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeTableRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTableRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalDescribeTableRequestRequestTypeDef = TypedDict(
@@ -198,27 +226,61 @@
 )
 
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
+ExecuteStatementOutputTypeDef = TypedDict(
+    "ExecuteStatementOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
         "booleanValue": bool,
         "doubleValue": float,
         "isNull": bool,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
 )
 
+_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetStatementResultRequestGetStatementResultPaginateTypeDef(
+    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
+    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
+):
+    pass
+
 _RequiredGetStatementResultRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementResultRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStatementResultRequestRequestTypeDef = TypedDict(
@@ -231,14 +293,38 @@
 
 class GetStatementResultRequestRequestTypeDef(
     _RequiredGetStatementResultRequestRequestTypeDef,
     _OptionalGetStatementResultRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDatabasesRequestListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatabasesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListDatabasesRequestRequestTypeDef = TypedDict(
@@ -255,14 +341,49 @@
 )
 
 class ListDatabasesRequestRequestTypeDef(
     _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
 ):
     pass
 
+ListDatabasesResponseTypeDef = TypedDict(
+    "ListDatabasesResponseTypeDef",
+    {
+        "Databases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -281,26 +402,73 @@
 )
 
 class ListSchemasRequestRequestTypeDef(
     _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
 ):
     pass
 
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
+    {
+        "NextToken": str,
+        "Schemas": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    {
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStatementsRequestRequestTypeDef = TypedDict(
     "ListStatementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RoleLevel": bool,
         "StatementName": str,
         "Status": StatusStringType,
     },
     total=False,
 )
 
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "TablePattern": str,
+        "WorkgroupName": str,
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
         "Database": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -330,75 +498,42 @@
         "name": str,
         "schema": str,
         "type": str,
     },
     total=False,
 )
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelStatementResponseTypeDef = TypedDict(
-    "CancelStatementResponseTypeDef",
-    {
-        "Status": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExecuteStatementOutputTypeDef = TypedDict(
-    "ExecuteStatementOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatabasesResponseTypeDef = TypedDict(
-    "ListDatabasesResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Databases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NextToken": str,
-        "Schemas": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "ColumnList": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "TableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Database": str,
@@ -468,174 +603,39 @@
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
         "SubStatements": List[SubStatementDataTypeDef],
         "UpdatedAt": datetime,
         "WorkgroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "Database": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "Schema": str,
-        "SecretArn": str,
-        "Table": str,
-        "WorkgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeTableRequestDescribeTablePaginateTypeDef(
-    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
-    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
-):
-    pass
-
-_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetStatementResultRequestGetStatementResultPaginateTypeDef(
-    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
-    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
-):
-    pass
-
-_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatabasesRequestListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
-):
-    pass
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    {
-        "RoleLevel": bool,
-        "StatementName": str,
-        "Status": StatusStringType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "TablePattern": str,
-        "WorkgroupName": str,
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
 
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "NextToken": str,
         "Tables": List[TableMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "NextToken": str,
         "Statements": List[StatementDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/PKG-INFO` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.26.88
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-redshift-data"></a>
 
 # mypy-boto3-redshift-data
 
 [![PyPI - mypy-boto3-redshift-data](https://img.shields.io/pypi/v/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,44 +341,44 @@
 
 `mypy_boto3_redshift_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
     CancelStatementRequestRequestTypeDef,
+    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
     SqlParameterTypeDef,
     SubStatementDataTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
     DescribeTableRequestRequestTypeDef,
+    ExecuteStatementOutputTypeDef,
     FieldTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
+    ListSchemasResponseTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    CancelStatementResponseTypeDef,
-    ExecuteStatementOutputTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     DescribeTableResponseTypeDef,
     ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
@@ -388,42 +388,42 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/SOURCES.txt` & `mypy-boto3-redshift-data-1.27.0/mypy_boto3_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.88/setup.py` & `mypy-boto3-redshift-data-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-redshift-data.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-data",
-    version="1.26.88",
+    version="1.27.0",
     packages=["mypy_boto3_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftDataAPIService 1.26.88 service generated with"
-        " mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.RedshiftDataAPIService 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/",
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


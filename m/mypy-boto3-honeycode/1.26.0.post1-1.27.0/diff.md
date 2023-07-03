# Comparing `tmp/mypy-boto3-honeycode-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-honeycode-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-honeycode-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:30 2022, max compression
+gzip compressed data, was "mypy-boto3-honeycode-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-honeycode-1.26.0.post1.tar` & `mypy-boto3-honeycode-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.676826 mypy-boto3-honeycode-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15235 2022-11-01 21:43:30.676826 mypy-boto3-honeycode-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13786 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.676826 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15516 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15490 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8458 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8456 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5166 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5160 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    20800 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20765 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.676826 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15235 2022-11-01 21:43:30.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-01 21:43:30.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:30.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:30.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:30.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-01 21:43:30.000000 mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:30.676826 mypy-boto3-honeycode-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-01 21:35:35.000000 mypy-boto3-honeycode-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.767365 mypy-boto3-honeycode-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-03 19:50:50.759365 mypy-boto3-honeycode-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.759365 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-03 19:38:53.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-03 19:38:53.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-03 19:38:53.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 19:38:53.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20834 2023-07-03 19:38:53.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-07-03 19:38:53.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.759365 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-03 19:50:50.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:50.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:50.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:50.000000 mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.767365 mypy-boto3-honeycode-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:38:52.000000 mypy-boto3-honeycode-1.27.0/setup.py
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/LICENSE` & `mypy-boto3-honeycode-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-honeycode-1.26.0.post1/PKG-INFO` & `mypy-boto3-honeycode-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Honeycode 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Honeycode 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
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
 
 <a id="mypy-boto3-honeycode"></a>
 
 # mypy-boto3-honeycode
 
 [![PyPI - mypy-boto3-honeycode](https://img.shields.io/pypi/v/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-honeycode?color=blue)](https://pypistats.org/packages/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,58 +336,58 @@
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    PaginatorConfigTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
     DestinationOptionsTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
     ImportDataSourceTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
@@ -406,42 +407,42 @@
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

### Comparing `mypy-boto3-honeycode-1.26.0.post1/README.md` & `mypy-boto3-honeycode-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-honeycode"></a>
 
 # mypy-boto3-honeycode
 
 [![PyPI - mypy-boto3-honeycode](https://img.shields.io/pypi/v/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-honeycode?color=blue)](https://pypistats.org/packages/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,58 +304,58 @@
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    PaginatorConfigTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
     DestinationOptionsTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
     ImportDataSourceTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
@@ -375,42 +375,42 @@
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

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/__init__.py` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/__init__.pyi` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/__main__.py` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Honeycode 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.Honeycode 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/client.py` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/client.pyi` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/literals.py` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,23 +90,25 @@
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
@@ -116,30 +118,35 @@
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
@@ -165,14 +172,15 @@
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
@@ -217,51 +225,57 @@
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
@@ -274,14 +288,15 @@
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
@@ -293,28 +308,35 @@
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
@@ -323,14 +345,15 @@
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
@@ -341,55 +364,64 @@
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
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/literals.pyi` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,23 +88,25 @@
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
@@ -114,30 +116,35 @@
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
@@ -163,14 +170,15 @@
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
@@ -215,51 +223,57 @@
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
@@ -272,14 +286,15 @@
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
@@ -291,28 +306,35 @@
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
@@ -321,14 +343,15 @@
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
@@ -339,55 +362,64 @@
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
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/paginator.py` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class ListTableColumnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, tableId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workbookId: str, tableId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableColumnsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
         """
 
 
@@ -79,30 +79,30 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablerowspaginator)
         """
 
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workbookId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
         """
 
 
@@ -114,13 +114,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/paginator.pyi` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 class ListTableColumnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, tableId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workbookId: str, tableId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableColumnsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
         """
 
 class ListTableRowsPaginator(Paginator):
@@ -75,29 +75,29 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablerowspaginator)
         """
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workbookId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
         """
 
 class QueryTableRowsPaginator(Paginator):
@@ -108,13 +108,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/type_defs.py` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,58 +31,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FailedBatchItemTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
-    "PaginatorConfigTypeDef",
+    "InvokeScreenAutomationResultTypeDef",
+    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
+    "ListTableRowsRequestListTableRowsPaginateTypeDef",
     "ListTableRowsRequestRequestTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartTableDataImportJobResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchCreateTableRowsResultTypeDef",
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
-    "InvokeScreenAutomationResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
     "DestinationOptionsTypeDef",
+    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
     "ImportDataSourceTypeDef",
-    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    "ListTableRowsRequestListTableRowsPaginateTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
-    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
@@ -98,25 +98,14 @@
     "FailedBatchItemTypeDef",
     {
         "id": str,
         "errorMessage": str,
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
 _RequiredBatchDeleteTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowIds": Sequence[str],
     },
@@ -263,24 +252,45 @@
     {
         "email": str,
         "userArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+InvokeScreenAutomationResultTypeDef = TypedDict(
+    "InvokeScreenAutomationResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "workbookCursor": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
+    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTableColumnsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableColumnsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -305,14 +315,38 @@
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
     total=False,
 )
 
+_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "rowIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTableRowsRequestListTableRowsPaginateTypeDef(
+    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
+    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -329,14 +363,36 @@
 
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "workbookId": str,
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
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -367,14 +423,52 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
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
+StartTableDataImportJobResultTypeDef = TypedDict(
+    "StartTableDataImportJobResultTypeDef",
+    {
+        "jobId": str,
+        "jobStatus": TableDataImportJobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -389,68 +483,43 @@
 
 BatchCreateTableRowsResultTypeDef = TypedDict(
     "BatchCreateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "createdRows": Dict[str, str],
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteTableRowsResultTypeDef = TypedDict(
     "BatchDeleteTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateTableRowsResultTypeDef = TypedDict(
     "BatchUpdateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvokeScreenAutomationResultTypeDef = TypedDict(
-    "InvokeScreenAutomationResultTypeDef",
-    {
-        "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTableDataImportJobResultTypeDef = TypedDict(
-    "StartTableDataImportJobResultTypeDef",
-    {
-        "jobId": str,
-        "jobStatus": TableDataImportJobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpsertTableRowsResultTypeDef = TypedDict(
     "BatchUpsertTableRowsResultTypeDef",
     {
         "rows": Dict[str, UpsertRowsResultTypeDef],
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRowDataTypeDef = TypedDict(
     "CreateRowDataTypeDef",
     {
         "batchItemId": str,
@@ -497,14 +566,38 @@
     "DestinationOptionsTypeDef",
     {
         "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
+_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+        "filterFormula": FilterTypeDef,
+    },
+)
+_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
+    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -589,124 +682,31 @@
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
-_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
-    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "rowIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTableRowsRequestListTableRowsPaginateTypeDef(
-    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
-    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "workbookId": str,
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
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-        "filterFormula": FilterTypeDef,
-    },
-)
-_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
-    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-):
-    pass
-
-
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTablesResultTypeDef = TypedDict(
     "ListTablesResultTypeDef",
     {
         "tables": List[TableTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchCreateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -758,26 +758,26 @@
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryTableRowsResultTypeDef = TypedDict(
     "QueryTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
@@ -820,15 +820,15 @@
 
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -853,10 +853,10 @@
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode/type_defs.pyi` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,58 +30,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FailedBatchItemTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
-    "PaginatorConfigTypeDef",
+    "InvokeScreenAutomationResultTypeDef",
+    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
+    "ListTableRowsRequestListTableRowsPaginateTypeDef",
     "ListTableRowsRequestRequestTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartTableDataImportJobResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchCreateTableRowsResultTypeDef",
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
-    "InvokeScreenAutomationResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
     "DestinationOptionsTypeDef",
+    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
     "ImportDataSourceTypeDef",
-    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    "ListTableRowsRequestListTableRowsPaginateTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
-    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
@@ -97,25 +97,14 @@
     "FailedBatchItemTypeDef",
     {
         "id": str,
         "errorMessage": str,
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
 _RequiredBatchDeleteTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowIds": Sequence[str],
     },
@@ -256,24 +245,43 @@
     {
         "email": str,
         "userArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+InvokeScreenAutomationResultTypeDef = TypedDict(
+    "InvokeScreenAutomationResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "workbookCursor": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
+    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTableColumnsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableColumnsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -296,14 +304,36 @@
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
     total=False,
 )
 
+_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "rowIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTableRowsRequestListTableRowsPaginateTypeDef(
+    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
+    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -318,14 +348,34 @@
 )
 
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "workbookId": str,
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
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -354,14 +404,52 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
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
+StartTableDataImportJobResultTypeDef = TypedDict(
+    "StartTableDataImportJobResultTypeDef",
+    {
+        "jobId": str,
+        "jobStatus": TableDataImportJobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -376,68 +464,43 @@
 
 BatchCreateTableRowsResultTypeDef = TypedDict(
     "BatchCreateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "createdRows": Dict[str, str],
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteTableRowsResultTypeDef = TypedDict(
     "BatchDeleteTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateTableRowsResultTypeDef = TypedDict(
     "BatchUpdateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvokeScreenAutomationResultTypeDef = TypedDict(
-    "InvokeScreenAutomationResultTypeDef",
-    {
-        "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTableDataImportJobResultTypeDef = TypedDict(
-    "StartTableDataImportJobResultTypeDef",
-    {
-        "jobId": str,
-        "jobStatus": TableDataImportJobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpsertTableRowsResultTypeDef = TypedDict(
     "BatchUpsertTableRowsResultTypeDef",
     {
         "rows": Dict[str, UpsertRowsResultTypeDef],
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRowDataTypeDef = TypedDict(
     "CreateRowDataTypeDef",
     {
         "batchItemId": str,
@@ -482,14 +545,36 @@
     "DestinationOptionsTypeDef",
     {
         "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
+_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+        "filterFormula": FilterTypeDef,
+    },
+)
+_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
+    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+):
+    pass
+
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -568,116 +653,31 @@
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
-_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
-    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
-):
-    pass
-
-_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "rowIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTableRowsRequestListTableRowsPaginateTypeDef(
-    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
-    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
-):
-    pass
-
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "workbookId": str,
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
-_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-        "filterFormula": FilterTypeDef,
-    },
-)
-_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
-    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-):
-    pass
-
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTablesResultTypeDef = TypedDict(
     "ListTablesResultTypeDef",
     {
         "tables": List[TableTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchCreateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -725,26 +725,26 @@
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryTableRowsResultTypeDef = TypedDict(
     "QueryTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
@@ -785,15 +785,15 @@
 
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -818,10 +818,10 @@
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/PKG-INFO` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Honeycode 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Honeycode 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
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
 
 <a id="mypy-boto3-honeycode"></a>
 
 # mypy-boto3-honeycode
 
 [![PyPI - mypy-boto3-honeycode](https://img.shields.io/pypi/v/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-honeycode?color=blue)](https://pypistats.org/packages/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,58 +336,58 @@
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    PaginatorConfigTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
     DestinationOptionsTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
     ImportDataSourceTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
@@ -406,42 +407,42 @@
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

### Comparing `mypy-boto3-honeycode-1.26.0.post1/mypy_boto3_honeycode.egg-info/SOURCES.txt` & `mypy-boto3-honeycode-1.27.0/mypy_boto3_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.26.0.post1/setup.py` & `mypy-boto3-honeycode-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-honeycode.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-honeycode",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Honeycode 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Honeycode 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 honeycode type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_honeycode": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_honeycode": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/",
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


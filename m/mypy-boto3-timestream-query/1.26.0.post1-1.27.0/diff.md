# Comparing `tmp/mypy-boto3-timestream-query-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-timestream-query-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:05 2022, max compression
+gzip compressed data, was "mypy-boto3-timestream-query-1.27.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
```

## Comparing `mypy-boto3-timestream-query-1.26.0.post1.tar` & `mypy-boto3-timestream-query-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:05.416854 mypy-boto3-timestream-query-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15390 2022-11-01 21:44:05.412854 mypy-boto3-timestream-query-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13914 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:05.412854 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13166 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13143 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8171 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4181 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4176 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    19433 2022-11-01 21:42:10.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19402 2022-11-01 21:42:09.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:42:07.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:05.412854 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15390 2022-11-01 21:44:05.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-01 21:44:05.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:05.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:05.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:05.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-01 21:44:05.000000 mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:05.416854 mypy-boto3-timestream-query-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-11-01 21:42:06.000000 mypy-boto3-timestream-query-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/LICENSE` & `mypy-boto3-timestream-query-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/PKG-INFO` & `mypy-boto3-timestream-query-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.TimestreamQuery 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.TimestreamQuery 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
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
 
 <a id="mypy-boto3-timestream-query"></a>
 
 # mypy-boto3-timestream-query
 
 [![PyPI - mypy-boto3-timestream-query](https://img.shields.io/pypi/v/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,54 +339,54 @@
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelQueryResponseTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
+    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
-    PaginatorConfigTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
+    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
+    ResponseMetadataTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
-    CreateScheduledQueryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/README.md` & `mypy-boto3-timestream-query-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-timestream-query"></a>
 
 # mypy-boto3-timestream-query
 
 [![PyPI - mypy-boto3-timestream-query](https://img.shields.io/pypi/v/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,54 +307,54 @@
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelQueryResponseTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
+    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
-    PaginatorConfigTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
+    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
+    ResponseMetadataTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
-    CreateScheduledQueryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/__init__.py` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/__init__.pyi` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/__main__.py` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.TimestreamQuery 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/client.py` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/client.pyi` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/literals.py` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,25 @@
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
@@ -102,30 +104,35 @@
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
@@ -151,14 +158,15 @@
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
@@ -203,51 +211,57 @@
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
@@ -260,14 +274,15 @@
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
@@ -279,28 +294,35 @@
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
@@ -309,14 +331,15 @@
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
@@ -327,55 +350,64 @@
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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/literals.pyi` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -74,23 +74,25 @@
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
@@ -100,30 +102,35 @@
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
@@ -149,14 +156,15 @@
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
@@ -201,51 +209,57 @@
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
@@ -258,14 +272,15 @@
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
@@ -277,28 +292,35 @@
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
@@ -307,14 +329,15 @@
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
@@ -325,55 +348,64 @@
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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/paginator.py` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,65 +32,60 @@
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QueryResponseTypeDef,
 )
 
 __all__ = ("ListScheduledQueriesPaginator", "ListTagsForResourcePaginator", "QueryPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListScheduledQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScheduledQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
         """
 
-
 class QueryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#querypaginator)
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/paginator.pyi` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,60 +32,65 @@
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QueryResponseTypeDef,
 )
 
 __all__ = ("ListScheduledQueriesPaginator", "ListTagsForResourcePaginator", "QueryPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListScheduledQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScheduledQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
         """
 
+
 class QueryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#querypaginator)
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/type_defs.py` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,54 +32,54 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelQueryResponseTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
+    "CreateScheduledQueryResponseTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
     "DimensionMappingTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ExecutionStatsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "SnsConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
+    "QueryRequestQueryPaginateTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
-    "CreateScheduledQueryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "QueryRequestQueryPaginateTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
@@ -95,22 +95,19 @@
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CancellationMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Type": Dict[str, Any],
@@ -140,26 +137,34 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateScheduledQueryResponseTypeDef = TypedDict(
+    "CreateScheduledQueryResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List["DatumTypeDef"],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": "DatumTypeDef",
+        "Value": Dict[str, Any],
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
@@ -185,14 +190,21 @@
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ConfigurationTypeDef = TypedDict(
@@ -249,33 +261,53 @@
         "BytesMetered": int,
         "RecordsIngested": int,
         "QueryResultRows": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListScheduledQueriesRequestRequestTypeDef = TypedDict(
     "ListScheduledQueriesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
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
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -320,14 +352,24 @@
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
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
 ParameterMappingTypeDef = TypedDict(
     "ParameterMappingTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
     },
 )
@@ -361,14 +403,36 @@
         "DatabaseName": str,
         "TableName": str,
         "Aliased": bool,
     },
     total=False,
 )
 
+_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryRequestQueryPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryRequestQueryPaginateTypeDef",
+    {
+        "ClientToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class QueryRequestQueryPaginateTypeDef(
+    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
+):
+    pass
+
+
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -394,14 +458,25 @@
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
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
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
     total=False,
@@ -430,43 +505,20 @@
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
-    {
-        "CancellationMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScheduledQueryResponseTypeDef = TypedDict(
-    "CreateScheduledQueryResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -486,15 +538,15 @@
     total=False,
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -505,66 +557,14 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
-ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
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
-
-_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryRequestQueryPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryRequestQueryPaginateTypeDef",
-    {
-        "ClientToken": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryRequestQueryPaginateTypeDef(
-    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
-):
-    pass
-
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -615,27 +615,27 @@
 
 PrepareQueryResponseTypeDef = TypedDict(
     "PrepareQueryResponseTypeDef",
     {
         "QueryString": str,
         "Columns": List[SelectColumnTypeDef],
         "Parameters": List[ParameterMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": TimestreamDestinationTypeDef,
@@ -716,15 +716,15 @@
 )
 
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
         "Name": str,
@@ -788,10 +788,10 @@
     pass
 
 
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query/type_defs.pyi` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,54 +31,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelQueryResponseTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
+    "CreateScheduledQueryResponseTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
     "DimensionMappingTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ExecutionStatsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "SnsConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
+    "QueryRequestQueryPaginateTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
-    "CreateScheduledQueryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "QueryRequestQueryPaginateTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
@@ -94,22 +94,19 @@
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CancellationMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Type": Dict[str, Any],
@@ -137,26 +134,34 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateScheduledQueryResponseTypeDef = TypedDict(
+    "CreateScheduledQueryResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List["DatumTypeDef"],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": "DatumTypeDef",
+        "Value": Dict[str, Any],
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
@@ -182,14 +187,21 @@
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ConfigurationTypeDef = TypedDict(
@@ -242,33 +254,51 @@
         "BytesMetered": int,
         "RecordsIngested": int,
         "QueryResultRows": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListScheduledQueriesRequestRequestTypeDef = TypedDict(
     "ListScheduledQueriesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
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
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -309,14 +339,24 @@
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
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
 ParameterMappingTypeDef = TypedDict(
     "ParameterMappingTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
     },
 )
@@ -348,14 +388,34 @@
         "DatabaseName": str,
         "TableName": str,
         "Aliased": bool,
     },
     total=False,
 )
 
+_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryRequestQueryPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryRequestQueryPaginateTypeDef",
+    {
+        "ClientToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class QueryRequestQueryPaginateTypeDef(
+    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
+):
+    pass
+
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -379,14 +439,25 @@
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
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
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
     total=False,
@@ -415,43 +486,20 @@
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
-    {
-        "CancellationMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScheduledQueryResponseTypeDef = TypedDict(
-    "CreateScheduledQueryResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -471,15 +519,15 @@
     total=False,
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -490,62 +538,14 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
-ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
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
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryRequestQueryPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryRequestQueryPaginateTypeDef",
-    {
-        "ClientToken": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class QueryRequestQueryPaginateTypeDef(
-    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
-):
-    pass
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -592,27 +592,27 @@
 
 PrepareQueryResponseTypeDef = TypedDict(
     "PrepareQueryResponseTypeDef",
     {
         "QueryString": str,
         "Columns": List[SelectColumnTypeDef],
         "Parameters": List[ParameterMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": TimestreamDestinationTypeDef,
@@ -689,15 +689,15 @@
 )
 
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
         "Name": str,
@@ -757,10 +757,10 @@
 ):
     pass
 
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.TimestreamQuery 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.TimestreamQuery 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
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
 
 <a id="mypy-boto3-timestream-query"></a>
 
 # mypy-boto3-timestream-query
 
 [![PyPI - mypy-boto3-timestream-query](https://img.shields.io/pypi/v/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,54 +339,54 @@
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelQueryResponseTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
+    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
-    PaginatorConfigTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
+    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
+    ResponseMetadataTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
-    CreateScheduledQueryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
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

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.26.0.post1/setup.py` & `mypy-boto3-timestream-query-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-timestream-query.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamQuery 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.TimestreamQuery 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 timestream-query type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_timestream_query": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_timestream_query": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/",
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


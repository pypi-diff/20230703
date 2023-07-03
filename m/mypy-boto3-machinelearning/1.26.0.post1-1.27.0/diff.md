# Comparing `tmp/mypy-boto3-machinelearning-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-machinelearning-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-machinelearning-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:41 2022, max compression
+gzip compressed data, was "mypy-boto3-machinelearning-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-machinelearning-1.26.0.post1.tar` & `mypy-boto3-machinelearning-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:41.432833 mypy-boto3-machinelearning-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18219 2022-11-01 21:43:41.428833 mypy-boto3-machinelearning-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16746 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:41.424833 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26169 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    26126 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9577 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9575 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6677 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    31635 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    31610 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6049 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6045 2022-11-01 21:37:36.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:41.428833 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18219 2022-11-01 21:43:41.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-01 21:43:41.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:41.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:41.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:41.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-01 21:43:41.000000 mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:41.432833 mypy-boto3-machinelearning-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-11-01 21:37:35.000000 mypy-boto3-machinelearning-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.951602 mypy-boto3-machinelearning-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-03 19:51:03.951602 mypy-boto3-machinelearning-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.947602 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-03 19:41:28.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31699 2023-07-03 19:41:29.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-03 19:41:28.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.951602 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-03 19:51:03.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-03 19:51:03.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:03.000000 mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.951602 mypy-boto3-machinelearning-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-03 19:41:26.000000 mypy-boto3-machinelearning-1.27.0/setup.py
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/LICENSE` & `mypy-boto3-machinelearning-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/PKG-INFO` & `mypy-boto3-machinelearning-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-machinelearning
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MachineLearning 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MachineLearning 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/
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
 
 <a id="mypy-boto3-machinelearning"></a>
 
 # mypy-boto3-machinelearning
 
 [![PyPI - mypy-boto3-machinelearning](https://img.shields.io/pypi/v/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-machinelearning?color=blue)](https://pypistats.org/packages/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,83 +385,83 @@
 
 `mypy_boto3_machinelearning.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_machinelearning.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AddTagsOutputTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
+    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
+    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
+    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
+    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
+    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
+    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
+    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
+    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
+    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
+    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
+    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    AddTagsOutputTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
-    CreateEvaluationOutputTypeDef,
-    CreateMLModelOutputTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
-    DeleteDataSourceOutputTypeDef,
-    DeleteEvaluationOutputTypeDef,
-    DeleteMLModelOutputTypeDef,
-    DeleteTagsOutputTypeDef,
     DescribeTagsOutputTypeDef,
-    GetBatchPredictionOutputTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
-    UpdateDataSourceOutputTypeDef,
-    UpdateEvaluationOutputTypeDef,
-    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
@@ -481,42 +482,42 @@
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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/README.md` & `mypy-boto3-machinelearning-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-machinelearning"></a>
 
 # mypy-boto3-machinelearning
 
 [![PyPI - mypy-boto3-machinelearning](https://img.shields.io/pypi/v/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-machinelearning?color=blue)](https://pypistats.org/packages/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,83 +353,83 @@
 
 `mypy_boto3_machinelearning.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_machinelearning.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AddTagsOutputTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
+    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
+    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
+    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
+    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
+    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
+    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
+    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
+    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
+    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
+    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
+    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    AddTagsOutputTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
-    CreateEvaluationOutputTypeDef,
-    CreateMLModelOutputTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
-    DeleteDataSourceOutputTypeDef,
-    DeleteEvaluationOutputTypeDef,
-    DeleteMLModelOutputTypeDef,
-    DeleteTagsOutputTypeDef,
     DescribeTagsOutputTypeDef,
-    GetBatchPredictionOutputTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
-    UpdateDataSourceOutputTypeDef,
-    UpdateEvaluationOutputTypeDef,
-    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
@@ -450,42 +450,42 @@
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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/__init__.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/__init__.pyi` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/__main__.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MachineLearning 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.MachineLearning 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/client.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,47 +252,47 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#create_realtime_endpoint)
         """
 
     def delete_batch_prediction(
         self, *, BatchPredictionId: str
     ) -> DeleteBatchPredictionOutputTypeDef:
         """
-        Assigns the DELETED status to a `BatchPrediction` , rendering it unusable.
+        Assigns the DELETED status to a `BatchPrediction`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_batch_prediction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_batch_prediction)
         """
 
     def delete_data_source(self, *, DataSourceId: str) -> DeleteDataSourceOutputTypeDef:
         """
-        Assigns the DELETED status to a `DataSource` , rendering it unusable.
+        Assigns the DELETED status to a `DataSource`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_data_source)
         """
 
     def delete_evaluation(self, *, EvaluationId: str) -> DeleteEvaluationOutputTypeDef:
         """
-        Assigns the `DELETED` status to an `Evaluation` , rendering it unusable.
+        Assigns the `DELETED` status to an `Evaluation`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_evaluation)
         """
 
     def delete_ml_model(self, *, MLModelId: str) -> DeleteMLModelOutputTypeDef:
         """
-        Assigns the `DELETED` status to an `MLModel` , rendering it unusable.
+        Assigns the `DELETED` status to an `MLModel`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_ml_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_ml_model)
         """
 
     def delete_realtime_endpoint(self, *, MLModelId: str) -> DeleteRealtimeEndpointOutputTypeDef:
         """
-        Deletes a real time endpoint of an `MLModel` .
+        Deletes a real time endpoint of an `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_realtime_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_realtime_endpoint)
         """
 
     def delete_tags(
         self, *, TagKeys: Sequence[str], ResourceId: str, ResourceType: TaggableResourceTypeType
@@ -428,83 +428,83 @@
         """
 
     def get_data_source(
         self, *, DataSourceId: str, Verbose: bool = ...
     ) -> GetDataSourceOutputTypeDef:
         """
         Returns a `DataSource` that includes metadata and data file information, as well
-        as the current status of the `DataSource` .
+        as the current status of the `DataSource`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.get_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_data_source)
         """
 
     def get_evaluation(self, *, EvaluationId: str) -> GetEvaluationOutputTypeDef:
         """
         Returns an `Evaluation` that includes metadata as well as the current status of
-        the `Evaluation` .
+        the `Evaluation`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.get_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_evaluation)
         """
 
     def get_ml_model(self, *, MLModelId: str, Verbose: bool = ...) -> GetMLModelOutputTypeDef:
         """
         Returns an `MLModel` that includes detailed metadata, data source information,
-        and the current status of the `MLModel` .
+        and the current status of the `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.get_ml_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_ml_model)
         """
 
     def predict(
         self, *, MLModelId: str, Record: Mapping[str, str], PredictEndpoint: str
     ) -> PredictOutputTypeDef:
         """
-        Generates a prediction for the observation using the specified `ML Model` .
+        Generates a prediction for the observation using the specified `ML Model`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.predict)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#predict)
         """
 
     def update_batch_prediction(
         self, *, BatchPredictionId: str, BatchPredictionName: str
     ) -> UpdateBatchPredictionOutputTypeDef:
         """
-        Updates the `BatchPredictionName` of a `BatchPrediction` .
+        Updates the `BatchPredictionName` of a `BatchPrediction`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_batch_prediction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_batch_prediction)
         """
 
     def update_data_source(
         self, *, DataSourceId: str, DataSourceName: str
     ) -> UpdateDataSourceOutputTypeDef:
         """
-        Updates the `DataSourceName` of a `DataSource` .
+        Updates the `DataSourceName` of a `DataSource`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_data_source)
         """
 
     def update_evaluation(
         self, *, EvaluationId: str, EvaluationName: str
     ) -> UpdateEvaluationOutputTypeDef:
         """
-        Updates the `EvaluationName` of an `Evaluation` .
+        Updates the `EvaluationName` of an `Evaluation`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_evaluation)
         """
 
     def update_ml_model(
         self, *, MLModelId: str, MLModelName: str = ..., ScoreThreshold: float = ...
     ) -> UpdateMLModelOutputTypeDef:
         """
-        Updates the `MLModelName` and the `ScoreThreshold` of an `MLModel` .
+        Updates the `MLModelName` and the `ScoreThreshold` of an `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_ml_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_ml_model)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/client.pyi` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -237,43 +237,43 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_realtime_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#create_realtime_endpoint)
         """
     def delete_batch_prediction(
         self, *, BatchPredictionId: str
     ) -> DeleteBatchPredictionOutputTypeDef:
         """
-        Assigns the DELETED status to a `BatchPrediction` , rendering it unusable.
+        Assigns the DELETED status to a `BatchPrediction`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_batch_prediction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_batch_prediction)
         """
     def delete_data_source(self, *, DataSourceId: str) -> DeleteDataSourceOutputTypeDef:
         """
-        Assigns the DELETED status to a `DataSource` , rendering it unusable.
+        Assigns the DELETED status to a `DataSource`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_data_source)
         """
     def delete_evaluation(self, *, EvaluationId: str) -> DeleteEvaluationOutputTypeDef:
         """
-        Assigns the `DELETED` status to an `Evaluation` , rendering it unusable.
+        Assigns the `DELETED` status to an `Evaluation`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_evaluation)
         """
     def delete_ml_model(self, *, MLModelId: str) -> DeleteMLModelOutputTypeDef:
         """
-        Assigns the `DELETED` status to an `MLModel` , rendering it unusable.
+        Assigns the `DELETED` status to an `MLModel`, rendering it unusable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_ml_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_ml_model)
         """
     def delete_realtime_endpoint(self, *, MLModelId: str) -> DeleteRealtimeEndpointOutputTypeDef:
         """
-        Deletes a real time endpoint of an `MLModel` .
+        Deletes a real time endpoint of an `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.delete_realtime_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#delete_realtime_endpoint)
         """
     def delete_tags(
         self, *, TagKeys: Sequence[str], ResourceId: str, ResourceType: TaggableResourceTypeType
     ) -> DeleteTagsOutputTypeDef:
@@ -400,76 +400,76 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_batch_prediction)
         """
     def get_data_source(
         self, *, DataSourceId: str, Verbose: bool = ...
     ) -> GetDataSourceOutputTypeDef:
         """
         Returns a `DataSource` that includes metadata and data file information, as well
-        as the current status of the `DataSource` .
+        as the current status of the `DataSource`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.get_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_data_source)
         """
     def get_evaluation(self, *, EvaluationId: str) -> GetEvaluationOutputTypeDef:
         """
         Returns an `Evaluation` that includes metadata as well as the current status of
-        the `Evaluation` .
+        the `Evaluation`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.get_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_evaluation)
         """
     def get_ml_model(self, *, MLModelId: str, Verbose: bool = ...) -> GetMLModelOutputTypeDef:
         """
         Returns an `MLModel` that includes detailed metadata, data source information,
-        and the current status of the `MLModel` .
+        and the current status of the `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.get_ml_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#get_ml_model)
         """
     def predict(
         self, *, MLModelId: str, Record: Mapping[str, str], PredictEndpoint: str
     ) -> PredictOutputTypeDef:
         """
-        Generates a prediction for the observation using the specified `ML Model` .
+        Generates a prediction for the observation using the specified `ML Model`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.predict)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#predict)
         """
     def update_batch_prediction(
         self, *, BatchPredictionId: str, BatchPredictionName: str
     ) -> UpdateBatchPredictionOutputTypeDef:
         """
-        Updates the `BatchPredictionName` of a `BatchPrediction` .
+        Updates the `BatchPredictionName` of a `BatchPrediction`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_batch_prediction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_batch_prediction)
         """
     def update_data_source(
         self, *, DataSourceId: str, DataSourceName: str
     ) -> UpdateDataSourceOutputTypeDef:
         """
-        Updates the `DataSourceName` of a `DataSource` .
+        Updates the `DataSourceName` of a `DataSource`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_data_source)
         """
     def update_evaluation(
         self, *, EvaluationId: str, EvaluationName: str
     ) -> UpdateEvaluationOutputTypeDef:
         """
-        Updates the `EvaluationName` of an `Evaluation` .
+        Updates the `EvaluationName` of an `Evaluation`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_evaluation)
         """
     def update_ml_model(
         self, *, MLModelId: str, MLModelName: str = ..., ScoreThreshold: float = ...
     ) -> UpdateMLModelOutputTypeDef:
         """
-        Updates the `MLModelName` and the `ScoreThreshold` of an `MLModel` .
+        Updates the `MLModelName` and the `ScoreThreshold` of an `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.update_ml_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/client/#update_ml_model)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_batch_predictions"]
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/literals.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,23 +110,25 @@
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
@@ -136,30 +138,35 @@
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
@@ -185,14 +192,15 @@
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
@@ -237,51 +245,57 @@
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
@@ -294,14 +308,15 @@
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
@@ -313,28 +328,35 @@
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
@@ -343,14 +365,15 @@
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
@@ -361,55 +384,64 @@
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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/literals.pyi` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -108,23 +108,25 @@
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
@@ -134,30 +136,35 @@
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
@@ -183,14 +190,15 @@
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
@@ -235,51 +243,57 @@
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
@@ -292,14 +306,15 @@
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
@@ -311,28 +326,35 @@
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
@@ -341,14 +363,15 @@
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
@@ -359,55 +382,64 @@
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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/paginator.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 
@@ -102,15 +102,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 
@@ -128,15 +128,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 
@@ -154,13 +154,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/paginator.pyi` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 class DescribeDataSourcesPaginator(Paginator):
@@ -98,15 +98,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 class DescribeEvaluationsPaginator(Paginator):
@@ -123,15 +123,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 class DescribeMLModelsPaginator(Paginator):
@@ -148,13 +148,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/type_defs.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,83 +36,83 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddTagsOutputTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
+    "CreateBatchPredictionOutputTypeDef",
+    "CreateDataSourceFromRDSOutputTypeDef",
+    "CreateDataSourceFromRedshiftOutputTypeDef",
     "S3DataSpecTypeDef",
+    "CreateDataSourceFromS3OutputTypeDef",
     "CreateEvaluationInputRequestTypeDef",
+    "CreateEvaluationOutputTypeDef",
     "CreateMLModelInputRequestTypeDef",
+    "CreateMLModelOutputTypeDef",
     "CreateRealtimeEndpointInputRequestTypeDef",
     "RealtimeEndpointInfoTypeDef",
     "DeleteBatchPredictionInputRequestTypeDef",
+    "DeleteBatchPredictionOutputTypeDef",
     "DeleteDataSourceInputRequestTypeDef",
+    "DeleteDataSourceOutputTypeDef",
     "DeleteEvaluationInputRequestTypeDef",
+    "DeleteEvaluationOutputTypeDef",
     "DeleteMLModelInputRequestTypeDef",
+    "DeleteMLModelOutputTypeDef",
     "DeleteRealtimeEndpointInputRequestTypeDef",
     "DeleteTagsInputRequestTypeDef",
+    "DeleteTagsOutputTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
     "DescribeBatchPredictionsInputRequestTypeDef",
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
+    "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
+    "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
+    "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
+    "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
+    "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
-    "AddTagsOutputTypeDef",
-    "CreateBatchPredictionOutputTypeDef",
-    "CreateDataSourceFromRDSOutputTypeDef",
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    "CreateDataSourceFromS3OutputTypeDef",
-    "CreateEvaluationOutputTypeDef",
-    "CreateMLModelOutputTypeDef",
-    "DeleteBatchPredictionOutputTypeDef",
-    "DeleteDataSourceOutputTypeDef",
-    "DeleteEvaluationOutputTypeDef",
-    "DeleteMLModelOutputTypeDef",
-    "DeleteTagsOutputTypeDef",
     "DescribeTagsOutputTypeDef",
-    "GetBatchPredictionOutputTypeDef",
-    "UpdateBatchPredictionOutputTypeDef",
-    "UpdateDataSourceOutputTypeDef",
-    "UpdateEvaluationOutputTypeDef",
-    "UpdateMLModelOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -130,22 +130,20 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddTagsOutputTypeDef = TypedDict(
+    "AddTagsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPredictionTypeDef = TypedDict(
     "BatchPredictionTypeDef",
     {
         "BatchPredictionId": str,
@@ -189,14 +187,38 @@
 class CreateBatchPredictionInputRequestTypeDef(
     _RequiredCreateBatchPredictionInputRequestTypeDef,
     _OptionalCreateBatchPredictionInputRequestTypeDef,
 ):
     pass
 
 
+CreateBatchPredictionOutputTypeDef = TypedDict(
+    "CreateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSourceFromRDSOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRDSOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredS3DataSpecTypeDef = TypedDict(
     "_RequiredS3DataSpecTypeDef",
     {
         "DataLocationS3": str,
     },
 )
 _OptionalS3DataSpecTypeDef = TypedDict(
@@ -210,14 +232,22 @@
 )
 
 
 class S3DataSpecTypeDef(_RequiredS3DataSpecTypeDef, _OptionalS3DataSpecTypeDef):
     pass
 
 
+CreateDataSourceFromS3OutputTypeDef = TypedDict(
+    "CreateDataSourceFromS3OutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateEvaluationInputRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
     },
@@ -233,14 +263,22 @@
 
 class CreateEvaluationInputRequestTypeDef(
     _RequiredCreateEvaluationInputRequestTypeDef, _OptionalCreateEvaluationInputRequestTypeDef
 ):
     pass
 
 
+CreateEvaluationOutputTypeDef = TypedDict(
+    "CreateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredCreateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
         "MLModelType": MLModelTypeType,
         "TrainingDataSourceId": str,
     },
@@ -259,14 +297,22 @@
 
 class CreateMLModelInputRequestTypeDef(
     _RequiredCreateMLModelInputRequestTypeDef, _OptionalCreateMLModelInputRequestTypeDef
 ):
     pass
 
 
+CreateMLModelOutputTypeDef = TypedDict(
+    "CreateMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateRealtimeEndpointInputRequestTypeDef = TypedDict(
     "CreateRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -284,35 +330,67 @@
 DeleteBatchPredictionInputRequestTypeDef = TypedDict(
     "DeleteBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
+DeleteBatchPredictionOutputTypeDef = TypedDict(
+    "DeleteBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDataSourceInputRequestTypeDef = TypedDict(
     "DeleteDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 
+DeleteDataSourceOutputTypeDef = TypedDict(
+    "DeleteDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEvaluationInputRequestTypeDef = TypedDict(
     "DeleteEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
+DeleteEvaluationOutputTypeDef = TypedDict(
+    "DeleteEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMLModelInputRequestTypeDef = TypedDict(
     "DeleteMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
+DeleteMLModelOutputTypeDef = TypedDict(
+    "DeleteMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRealtimeEndpointInputRequestTypeDef = TypedDict(
     "DeleteRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -321,29 +399,45 @@
     {
         "TagKeys": Sequence[str],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
+DeleteTagsOutputTypeDef = TypedDict(
+    "DeleteTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FilterVariable": BatchPredictionFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeBatchPredictionsInputRequestTypeDef = TypedDict(
     "DescribeBatchPredictionsInputRequestTypeDef",
     {
@@ -358,14 +452,31 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    {
+        "FilterVariable": DataSourceFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSourcesInputRequestTypeDef = TypedDict(
     "DescribeDataSourcesInputRequestTypeDef",
     {
         "FilterVariable": DataSourceFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -376,14 +487,31 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    {
+        "FilterVariable": EvaluationFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEvaluationsInputRequestTypeDef = TypedDict(
     "DescribeEvaluationsInputRequestTypeDef",
     {
         "FilterVariable": EvaluationFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -394,14 +522,31 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
+    {
+        "FilterVariable": MLModelFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMLModelsInputRequestTypeDef = TypedDict(
     "DescribeMLModelsInputRequestTypeDef",
     {
         "FilterVariable": MLModelFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -435,14 +580,38 @@
 GetBatchPredictionInputRequestTypeDef = TypedDict(
     "GetBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
+GetBatchPredictionOutputTypeDef = TypedDict(
+    "GetBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "MLModelId": str,
+        "BatchPredictionDataSourceId": str,
+        "InputDataLocationS3": str,
+        "CreatedByIamUser": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Name": str,
+        "Status": EntityStatusType,
+        "OutputUri": str,
+        "LogUri": str,
+        "Message": str,
+        "ComputeTime": int,
+        "FinishedAt": datetime,
+        "StartedAt": datetime,
+        "TotalRecordCount": int,
+        "InvalidRecordCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDataSourceInputRequestTypeDef = TypedDict(
     "_RequiredGetDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalGetDataSourceInputRequestTypeDef = TypedDict(
@@ -484,14 +653,24 @@
 
 class GetMLModelInputRequestTypeDef(
     _RequiredGetMLModelInputRequestTypeDef, _OptionalGetMLModelInputRequestTypeDef
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
 PredictInputRequestTypeDef = TypedDict(
     "PredictInputRequestTypeDef",
     {
         "MLModelId": str,
         "Record": Mapping[str, str],
         "PredictEndpoint": str,
     },
@@ -536,38 +715,73 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
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
 UpdateBatchPredictionInputRequestTypeDef = TypedDict(
     "UpdateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
         "BatchPredictionName": str,
     },
 )
 
+UpdateBatchPredictionOutputTypeDef = TypedDict(
+    "UpdateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateDataSourceInputRequestTypeDef = TypedDict(
     "UpdateDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSourceName": str,
     },
 )
 
+UpdateDataSourceOutputTypeDef = TypedDict(
+    "UpdateDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateEvaluationInputRequestTypeDef = TypedDict(
     "UpdateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "EvaluationName": str,
     },
 )
 
+UpdateEvaluationOutputTypeDef = TypedDict(
+    "UpdateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 _OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
@@ -582,193 +796,47 @@
 
 class UpdateMLModelInputRequestTypeDef(
     _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
 ):
     pass
 
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-    },
-)
-
-AddTagsOutputTypeDef = TypedDict(
-    "AddTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBatchPredictionOutputTypeDef = TypedDict(
-    "CreateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceFromRDSOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRDSOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceFromS3OutputTypeDef = TypedDict(
-    "CreateDataSourceFromS3OutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEvaluationOutputTypeDef = TypedDict(
-    "CreateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMLModelOutputTypeDef = TypedDict(
-    "CreateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBatchPredictionOutputTypeDef = TypedDict(
-    "DeleteBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDataSourceOutputTypeDef = TypedDict(
-    "DeleteDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEvaluationOutputTypeDef = TypedDict(
-    "DeleteEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMLModelOutputTypeDef = TypedDict(
-    "DeleteMLModelOutputTypeDef",
+UpdateMLModelOutputTypeDef = TypedDict(
+    "UpdateMLModelOutputTypeDef",
     {
         "MLModelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTagsOutputTypeDef = TypedDict(
-    "DeleteTagsOutputTypeDef",
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
     {
+        "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBatchPredictionOutputTypeDef = TypedDict(
-    "GetBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "MLModelId": str,
-        "BatchPredictionDataSourceId": str,
-        "InputDataLocationS3": str,
-        "CreatedByIamUser": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Name": str,
-        "Status": EntityStatusType,
-        "OutputUri": str,
-        "LogUri": str,
-        "Message": str,
-        "ComputeTime": int,
-        "FinishedAt": datetime,
-        "StartedAt": datetime,
-        "TotalRecordCount": int,
-        "InvalidRecordCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBatchPredictionOutputTypeDef = TypedDict(
-    "UpdateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDataSourceOutputTypeDef = TypedDict(
-    "UpdateDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEvaluationOutputTypeDef = TypedDict(
-    "UpdateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMLModelOutputTypeDef = TypedDict(
-    "UpdateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceFromS3InputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromS3InputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -793,24 +861,24 @@
 
 
 CreateRealtimeEndpointOutputTypeDef = TypedDict(
     "CreateRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRealtimeEndpointOutputTypeDef = TypedDict(
     "DeleteRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMLModelOutputTypeDef = TypedDict(
     "GetMLModelOutputTypeDef",
     {
         "MLModelId": str,
@@ -830,15 +898,15 @@
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "Recipe": str,
         "Schema": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MLModelTypeDef = TypedDict(
     "MLModelTypeDef",
     {
         "MLModelId": str,
@@ -936,82 +1004,14 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
-    {
-        "FilterVariable": BatchPredictionFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    {
-        "FilterVariable": DataSourceFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    {
-        "FilterVariable": EvaluationFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
-    {
-        "FilterVariable": MLModelFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
         "InputDataLocationS3": str,
@@ -1043,23 +1043,23 @@
         "Status": EntityStatusType,
         "PerformanceMetrics": PerformanceMetricsTypeDef,
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PredictOutputTypeDef = TypedDict(
     "PredictOutputTypeDef",
     {
         "Prediction": PredictionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRDSDataSpecTypeDef = TypedDict(
     "_RequiredRDSDataSpecTypeDef",
     {
         "DatabaseInformation": RDSDatabaseTypeDef,
@@ -1135,24 +1135,24 @@
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
     "DescribeMLModelsOutputTypeDef",
     {
         "Results": List[MLModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEvaluationsOutputTypeDef = TypedDict(
     "DescribeEvaluationsOutputTypeDef",
     {
         "Results": List[EvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceFromRDSInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRDSInputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -1246,19 +1246,19 @@
         "RDSMetadata": RDSMetadataTypeDef,
         "RoleARN": str,
         "ComputeStatistics": bool,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "DataSourceSchema": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSourcesOutputTypeDef = TypedDict(
     "DescribeDataSourcesOutputTypeDef",
     {
         "Results": List[DataSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/type_defs.pyi` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,83 +35,83 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddTagsOutputTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
+    "CreateBatchPredictionOutputTypeDef",
+    "CreateDataSourceFromRDSOutputTypeDef",
+    "CreateDataSourceFromRedshiftOutputTypeDef",
     "S3DataSpecTypeDef",
+    "CreateDataSourceFromS3OutputTypeDef",
     "CreateEvaluationInputRequestTypeDef",
+    "CreateEvaluationOutputTypeDef",
     "CreateMLModelInputRequestTypeDef",
+    "CreateMLModelOutputTypeDef",
     "CreateRealtimeEndpointInputRequestTypeDef",
     "RealtimeEndpointInfoTypeDef",
     "DeleteBatchPredictionInputRequestTypeDef",
+    "DeleteBatchPredictionOutputTypeDef",
     "DeleteDataSourceInputRequestTypeDef",
+    "DeleteDataSourceOutputTypeDef",
     "DeleteEvaluationInputRequestTypeDef",
+    "DeleteEvaluationOutputTypeDef",
     "DeleteMLModelInputRequestTypeDef",
+    "DeleteMLModelOutputTypeDef",
     "DeleteRealtimeEndpointInputRequestTypeDef",
     "DeleteTagsInputRequestTypeDef",
+    "DeleteTagsOutputTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
     "DescribeBatchPredictionsInputRequestTypeDef",
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
+    "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
+    "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
+    "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
+    "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
+    "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
-    "AddTagsOutputTypeDef",
-    "CreateBatchPredictionOutputTypeDef",
-    "CreateDataSourceFromRDSOutputTypeDef",
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    "CreateDataSourceFromS3OutputTypeDef",
-    "CreateEvaluationOutputTypeDef",
-    "CreateMLModelOutputTypeDef",
-    "DeleteBatchPredictionOutputTypeDef",
-    "DeleteDataSourceOutputTypeDef",
-    "DeleteEvaluationOutputTypeDef",
-    "DeleteMLModelOutputTypeDef",
-    "DeleteTagsOutputTypeDef",
     "DescribeTagsOutputTypeDef",
-    "GetBatchPredictionOutputTypeDef",
-    "UpdateBatchPredictionOutputTypeDef",
-    "UpdateDataSourceOutputTypeDef",
-    "UpdateEvaluationOutputTypeDef",
-    "UpdateMLModelOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -129,22 +129,20 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddTagsOutputTypeDef = TypedDict(
+    "AddTagsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPredictionTypeDef = TypedDict(
     "BatchPredictionTypeDef",
     {
         "BatchPredictionId": str,
@@ -186,14 +184,38 @@
 
 class CreateBatchPredictionInputRequestTypeDef(
     _RequiredCreateBatchPredictionInputRequestTypeDef,
     _OptionalCreateBatchPredictionInputRequestTypeDef,
 ):
     pass
 
+CreateBatchPredictionOutputTypeDef = TypedDict(
+    "CreateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSourceFromRDSOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRDSOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredS3DataSpecTypeDef = TypedDict(
     "_RequiredS3DataSpecTypeDef",
     {
         "DataLocationS3": str,
     },
 )
 _OptionalS3DataSpecTypeDef = TypedDict(
@@ -205,14 +227,22 @@
     },
     total=False,
 )
 
 class S3DataSpecTypeDef(_RequiredS3DataSpecTypeDef, _OptionalS3DataSpecTypeDef):
     pass
 
+CreateDataSourceFromS3OutputTypeDef = TypedDict(
+    "CreateDataSourceFromS3OutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateEvaluationInputRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
     },
@@ -226,14 +256,22 @@
 )
 
 class CreateEvaluationInputRequestTypeDef(
     _RequiredCreateEvaluationInputRequestTypeDef, _OptionalCreateEvaluationInputRequestTypeDef
 ):
     pass
 
+CreateEvaluationOutputTypeDef = TypedDict(
+    "CreateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredCreateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
         "MLModelType": MLModelTypeType,
         "TrainingDataSourceId": str,
     },
@@ -250,14 +288,22 @@
 )
 
 class CreateMLModelInputRequestTypeDef(
     _RequiredCreateMLModelInputRequestTypeDef, _OptionalCreateMLModelInputRequestTypeDef
 ):
     pass
 
+CreateMLModelOutputTypeDef = TypedDict(
+    "CreateMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateRealtimeEndpointInputRequestTypeDef = TypedDict(
     "CreateRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -275,35 +321,67 @@
 DeleteBatchPredictionInputRequestTypeDef = TypedDict(
     "DeleteBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
+DeleteBatchPredictionOutputTypeDef = TypedDict(
+    "DeleteBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDataSourceInputRequestTypeDef = TypedDict(
     "DeleteDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 
+DeleteDataSourceOutputTypeDef = TypedDict(
+    "DeleteDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEvaluationInputRequestTypeDef = TypedDict(
     "DeleteEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
+DeleteEvaluationOutputTypeDef = TypedDict(
+    "DeleteEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMLModelInputRequestTypeDef = TypedDict(
     "DeleteMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
+DeleteMLModelOutputTypeDef = TypedDict(
+    "DeleteMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRealtimeEndpointInputRequestTypeDef = TypedDict(
     "DeleteRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -312,29 +390,45 @@
     {
         "TagKeys": Sequence[str],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
+DeleteTagsOutputTypeDef = TypedDict(
+    "DeleteTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FilterVariable": BatchPredictionFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeBatchPredictionsInputRequestTypeDef = TypedDict(
     "DescribeBatchPredictionsInputRequestTypeDef",
     {
@@ -349,14 +443,31 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    {
+        "FilterVariable": DataSourceFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSourcesInputRequestTypeDef = TypedDict(
     "DescribeDataSourcesInputRequestTypeDef",
     {
         "FilterVariable": DataSourceFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -367,14 +478,31 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    {
+        "FilterVariable": EvaluationFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEvaluationsInputRequestTypeDef = TypedDict(
     "DescribeEvaluationsInputRequestTypeDef",
     {
         "FilterVariable": EvaluationFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -385,14 +513,31 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
+    {
+        "FilterVariable": MLModelFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMLModelsInputRequestTypeDef = TypedDict(
     "DescribeMLModelsInputRequestTypeDef",
     {
         "FilterVariable": MLModelFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -426,14 +571,38 @@
 GetBatchPredictionInputRequestTypeDef = TypedDict(
     "GetBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
+GetBatchPredictionOutputTypeDef = TypedDict(
+    "GetBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "MLModelId": str,
+        "BatchPredictionDataSourceId": str,
+        "InputDataLocationS3": str,
+        "CreatedByIamUser": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Name": str,
+        "Status": EntityStatusType,
+        "OutputUri": str,
+        "LogUri": str,
+        "Message": str,
+        "ComputeTime": int,
+        "FinishedAt": datetime,
+        "StartedAt": datetime,
+        "TotalRecordCount": int,
+        "InvalidRecordCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDataSourceInputRequestTypeDef = TypedDict(
     "_RequiredGetDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalGetDataSourceInputRequestTypeDef = TypedDict(
@@ -471,14 +640,24 @@
 )
 
 class GetMLModelInputRequestTypeDef(
     _RequiredGetMLModelInputRequestTypeDef, _OptionalGetMLModelInputRequestTypeDef
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
 PredictInputRequestTypeDef = TypedDict(
     "PredictInputRequestTypeDef",
     {
         "MLModelId": str,
         "Record": Mapping[str, str],
         "PredictEndpoint": str,
     },
@@ -523,38 +702,73 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
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
 UpdateBatchPredictionInputRequestTypeDef = TypedDict(
     "UpdateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
         "BatchPredictionName": str,
     },
 )
 
+UpdateBatchPredictionOutputTypeDef = TypedDict(
+    "UpdateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateDataSourceInputRequestTypeDef = TypedDict(
     "UpdateDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSourceName": str,
     },
 )
 
+UpdateDataSourceOutputTypeDef = TypedDict(
+    "UpdateDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateEvaluationInputRequestTypeDef = TypedDict(
     "UpdateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "EvaluationName": str,
     },
 )
 
+UpdateEvaluationOutputTypeDef = TypedDict(
+    "UpdateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 _OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
@@ -567,193 +781,47 @@
 )
 
 class UpdateMLModelInputRequestTypeDef(
     _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
 ):
     pass
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-    },
-)
-
-AddTagsOutputTypeDef = TypedDict(
-    "AddTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBatchPredictionOutputTypeDef = TypedDict(
-    "CreateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceFromRDSOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRDSOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceFromS3OutputTypeDef = TypedDict(
-    "CreateDataSourceFromS3OutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEvaluationOutputTypeDef = TypedDict(
-    "CreateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMLModelOutputTypeDef = TypedDict(
-    "CreateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBatchPredictionOutputTypeDef = TypedDict(
-    "DeleteBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDataSourceOutputTypeDef = TypedDict(
-    "DeleteDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEvaluationOutputTypeDef = TypedDict(
-    "DeleteEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMLModelOutputTypeDef = TypedDict(
-    "DeleteMLModelOutputTypeDef",
+UpdateMLModelOutputTypeDef = TypedDict(
+    "UpdateMLModelOutputTypeDef",
     {
         "MLModelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTagsOutputTypeDef = TypedDict(
-    "DeleteTagsOutputTypeDef",
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
     {
+        "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBatchPredictionOutputTypeDef = TypedDict(
-    "GetBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "MLModelId": str,
-        "BatchPredictionDataSourceId": str,
-        "InputDataLocationS3": str,
-        "CreatedByIamUser": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Name": str,
-        "Status": EntityStatusType,
-        "OutputUri": str,
-        "LogUri": str,
-        "Message": str,
-        "ComputeTime": int,
-        "FinishedAt": datetime,
-        "StartedAt": datetime,
-        "TotalRecordCount": int,
-        "InvalidRecordCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBatchPredictionOutputTypeDef = TypedDict(
-    "UpdateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDataSourceOutputTypeDef = TypedDict(
-    "UpdateDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEvaluationOutputTypeDef = TypedDict(
-    "UpdateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMLModelOutputTypeDef = TypedDict(
-    "UpdateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceFromS3InputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromS3InputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -776,24 +844,24 @@
     pass
 
 CreateRealtimeEndpointOutputTypeDef = TypedDict(
     "CreateRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRealtimeEndpointOutputTypeDef = TypedDict(
     "DeleteRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMLModelOutputTypeDef = TypedDict(
     "GetMLModelOutputTypeDef",
     {
         "MLModelId": str,
@@ -813,15 +881,15 @@
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "Recipe": str,
         "Schema": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MLModelTypeDef = TypedDict(
     "MLModelTypeDef",
     {
         "MLModelId": str,
@@ -919,82 +987,14 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
-    {
-        "FilterVariable": BatchPredictionFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    {
-        "FilterVariable": DataSourceFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    {
-        "FilterVariable": EvaluationFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
-    {
-        "FilterVariable": MLModelFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
         "InputDataLocationS3": str,
@@ -1026,23 +1026,23 @@
         "Status": EntityStatusType,
         "PerformanceMetrics": PerformanceMetricsTypeDef,
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PredictOutputTypeDef = TypedDict(
     "PredictOutputTypeDef",
     {
         "Prediction": PredictionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRDSDataSpecTypeDef = TypedDict(
     "_RequiredRDSDataSpecTypeDef",
     {
         "DatabaseInformation": RDSDatabaseTypeDef,
@@ -1114,24 +1114,24 @@
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
     "DescribeMLModelsOutputTypeDef",
     {
         "Results": List[MLModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEvaluationsOutputTypeDef = TypedDict(
     "DescribeEvaluationsOutputTypeDef",
     {
         "Results": List[EvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceFromRDSInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRDSInputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -1221,19 +1221,19 @@
         "RDSMetadata": RDSMetadataTypeDef,
         "RoleARN": str,
         "ComputeStatistics": bool,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "DataSourceSchema": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSourcesOutputTypeDef = TypedDict(
     "DescribeDataSourcesOutputTypeDef",
     {
         "Results": List[DataSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/waiter.py` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning/waiter.pyi` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/PKG-INFO` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-machinelearning
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MachineLearning 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MachineLearning 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/
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
 
 <a id="mypy-boto3-machinelearning"></a>
 
 # mypy-boto3-machinelearning
 
 [![PyPI - mypy-boto3-machinelearning](https://img.shields.io/pypi/v/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-machinelearning?color=blue)](https://pypistats.org/packages/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,83 +385,83 @@
 
 `mypy_boto3_machinelearning.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_machinelearning.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AddTagsOutputTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
+    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
+    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
+    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
+    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
+    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
+    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
+    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
+    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
+    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
+    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
+    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    AddTagsOutputTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
-    CreateEvaluationOutputTypeDef,
-    CreateMLModelOutputTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
-    DeleteDataSourceOutputTypeDef,
-    DeleteEvaluationOutputTypeDef,
-    DeleteMLModelOutputTypeDef,
-    DeleteTagsOutputTypeDef,
     DescribeTagsOutputTypeDef,
-    GetBatchPredictionOutputTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
-    UpdateDataSourceOutputTypeDef,
-    UpdateEvaluationOutputTypeDef,
-    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
@@ -481,42 +482,42 @@
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

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/mypy_boto3_machinelearning.egg-info/SOURCES.txt` & `mypy-boto3-machinelearning-1.27.0/mypy_boto3_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.26.0.post1/setup.py` & `mypy-boto3-machinelearning-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-machinelearning.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-machinelearning",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MachineLearning 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.MachineLearning 1.27.0 service generated with"
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
     keywords="boto3 machinelearning type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_machinelearning": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_machinelearning": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/",
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


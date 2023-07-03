# Comparing `tmp/mypy-boto3-iotanalytics-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iotanalytics-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotanalytics-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:33 2022, max compression
+gzip compressed data, was "mypy-boto3-iotanalytics-1.27.0.tar", last modified: Mon Jul  3 19:50:54 2023, max compression
```

## Comparing `mypy-boto3-iotanalytics-1.26.0.post1.tar` & `mypy-boto3-iotanalytics-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:33.168828 mypy-boto3-iotanalytics-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18575 2022-11-01 21:43:33.160828 mypy-boto3-iotanalytics-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17114 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:33.156828 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26324 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    26278 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8396 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8394 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6260 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    46181 2022-11-01 21:36:08.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    46110 2022-11-01 21:36:08.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:33.156828 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18575 2022-11-01 21:43:32.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-01 21:43:33.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:32.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:32.000000 mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:33.168828 mypy-boto3-iotanalytics-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:36:06.000000 mypy-boto3-iotanalytics-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.519432 mypy-boto3-iotanalytics-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-07-03 19:50:54.519432 mypy-boto3-iotanalytics-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.515432 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-03 19:39:35.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46164 2023-07-03 19:39:35.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.519432 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-07-03 19:50:54.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:54.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:54.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:54.000000 mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:54.519432 mypy-boto3-iotanalytics-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:39:34.000000 mypy-boto3-iotanalytics-1.27.0/setup.py
```

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/LICENSE` & `mypy-boto3-iotanalytics-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/PKG-INFO` & `mypy-boto3-iotanalytics-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTAnalytics 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTAnalytics 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
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
 
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,27 +347,28 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
-    ResponseMetadataTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
     RetentionPeriodTypeDef,
     ColumnTypeDef,
     ResourceConfigurationTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
+    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
+    CreatePipelineResponseTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
@@ -387,40 +389,44 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
     LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
     DeviceShadowEnrichActivityTypeDef,
+    EmptyResponseMetadataTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
+    PaginatorConfigTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    CreateDatasetContentResponseTypeDef,
-    CreatePipelineResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -435,19 +441,14 @@
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     VariableTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
     ChannelSummaryTypeDef,
     ChannelTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
@@ -493,42 +494,42 @@
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

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/README.md` & `mypy-boto3-iotanalytics-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,27 +315,28 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
-    ResponseMetadataTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
     RetentionPeriodTypeDef,
     ColumnTypeDef,
     ResourceConfigurationTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
+    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
+    CreatePipelineResponseTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
@@ -356,40 +357,44 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
     LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
     DeviceShadowEnrichActivityTypeDef,
+    EmptyResponseMetadataTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
+    PaginatorConfigTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    CreateDatasetContentResponseTypeDef,
-    CreatePipelineResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -404,19 +409,14 @@
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     VariableTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
     ChannelSummaryTypeDef,
     ChannelTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
@@ -462,42 +462,42 @@
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

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/__init__.py` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/__init__.pyi` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/client.py` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/client.pyi` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/literals.py` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,23 +68,25 @@
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
@@ -94,30 +96,35 @@
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
@@ -143,14 +150,15 @@
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
@@ -195,51 +203,57 @@
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
@@ -252,14 +266,15 @@
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
@@ -271,28 +286,35 @@
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
@@ -301,14 +323,15 @@
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
@@ -319,55 +342,64 @@
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

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/literals.pyi` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -66,23 +66,25 @@
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
@@ -92,30 +94,35 @@
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
@@ -141,14 +148,15 @@
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
@@ -193,51 +201,57 @@
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
@@ -250,14 +264,15 @@
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
@@ -269,28 +284,35 @@
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
@@ -299,14 +321,15 @@
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
@@ -317,55 +340,64 @@
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

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/paginator.py` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
         """
 
 
@@ -83,58 +83,58 @@
 
     def paginate(
         self,
         *,
         datasetName: str,
         scheduledOnOrAfter: Union[datetime, str] = ...,
         scheduledBefore: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
         """
 
 
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
         """
 
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/paginator.pyi` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listchannelspaginator)
         """
 
 class ListDatasetContentsPaginator(Paginator):
@@ -79,55 +79,55 @@
 
     def paginate(
         self,
         *,
         datasetName: str,
         scheduledOnOrAfter: Union[datetime, str] = ...,
         scheduledBefore: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatasetspaginator)
         """
 
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listdatastorespaginator)
         """
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/paginators/#listpipelinespaginator)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/type_defs.py` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,27 +38,28 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "MessageTypeDef",
-    "ResponseMetadataTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
     "RetentionPeriodTypeDef",
     "ColumnTypeDef",
     "ResourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
+    "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
+    "CreatePipelineResponseTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
@@ -79,40 +80,44 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
     "LoggingOptionsTypeDef",
     "DescribePipelineRequestRequestTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
     "GlueConfigurationTypeDef",
     "LambdaActivityTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "SampleChannelDataRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageRequestRequestTypeDef",
-    "BatchPutMessageResponseTypeDef",
-    "CreateDatasetContentResponseTypeDef",
-    "CreatePipelineResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
+    "SampleChannelDataRequestRequestTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "BatchPutMessageResponseTypeDef",
+    "BatchPutMessageRequestRequestTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
     "ChannelStorageSummaryTypeDef",
     "ChannelStorageTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
@@ -127,19 +132,14 @@
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     "DatastorePartitionTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "VariableTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
     "ChannelSummaryTypeDef",
     "ChannelTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
@@ -213,25 +213,14 @@
     "MessageTypeDef",
     {
         "messageId": str,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
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
 CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
@@ -356,23 +345,40 @@
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
 
+CreateDatasetContentResponseTypeDef = TypedDict(
+    "CreateDatasetContentResponseTypeDef",
+    {
+        "versionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
 )
 
+CreatePipelineResponseTypeDef = TypedDict(
+    "CreatePipelineResponseTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -700,14 +706,21 @@
 
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -770,33 +783,55 @@
 )
 
 
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "scheduledOnOrAfter": Union[datetime, str],
+        "scheduledBefore": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
+    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetContentsRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
@@ -814,32 +849,56 @@
 class ListDatasetContentsRequestRequestTypeDef(
     _RequiredListDatasetContentsRequestRequestTypeDef,
     _OptionalListDatasetContentsRequestRequestTypeDef,
 ):
     pass
 
 
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -876,14 +935,24 @@
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
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
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -930,14 +999,34 @@
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
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
+RunPipelineActivityResponseTypeDef = TypedDict(
+    "RunPipelineActivityResponseTypeDef",
+    {
+        "payloads": List[bytes],
+        "logResult": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
     "_RequiredSampleChannelDataRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
@@ -953,84 +1042,51 @@
 
 class SampleChannelDataRequestRequestTypeDef(
     _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
 ):
     pass
 
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
-    {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
-    },
-)
-
-BatchPutMessageResponseTypeDef = TypedDict(
-    "BatchPutMessageResponseTypeDef",
-    {
-        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetContentResponseTypeDef = TypedDict(
-    "CreateDatasetContentResponseTypeDef",
-    {
-        "versionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePipelineResponseTypeDef = TypedDict(
-    "CreatePipelineResponseTypeDef",
+SampleChannelDataResponseTypeDef = TypedDict(
+    "SampleChannelDataResponseTypeDef",
     {
-        "pipelineName": str,
-        "pipelineArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "payloads": List[bytes],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+StartPipelineReprocessingResponseTypeDef = TypedDict(
+    "StartPipelineReprocessingResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "reprocessingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RunPipelineActivityResponseTypeDef = TypedDict(
-    "RunPipelineActivityResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "payloads": List[bytes],
-        "logResult": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-SampleChannelDataResponseTypeDef = TypedDict(
-    "SampleChannelDataResponseTypeDef",
+BatchPutMessageResponseTypeDef = TypedDict(
+    "BatchPutMessageResponseTypeDef",
     {
-        "payloads": List[bytes],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartPipelineReprocessingResponseTypeDef = TypedDict(
-    "StartPipelineReprocessingResponseTypeDef",
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
     {
-        "reprocessingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "channelName": str,
+        "messages": Sequence[MessageTypeDef],
     },
 )
 
 _RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
@@ -1090,35 +1146,35 @@
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
@@ -1126,15 +1182,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1156,15 +1212,15 @@
 
 GetDatasetContentResponseTypeDef = TypedDict(
     "GetDatasetContentResponseTypeDef",
     {
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
@@ -1213,15 +1269,15 @@
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
@@ -1247,70 +1303,14 @@
 
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
-    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-):
-    pass
-
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1439,15 +1439,15 @@
 )
 
 ListDatasetContentsResponseTypeDef = TypedDict(
     "ListDatasetContentsResponseTypeDef",
     {
         "datasetContentSummaries": List[DatasetContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
@@ -1612,33 +1612,33 @@
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
@@ -1648,15 +1648,15 @@
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
@@ -1702,15 +1702,15 @@
     total=False,
 )
 
 DescribePipelineResponseTypeDef = TypedDict(
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
@@ -1776,15 +1776,15 @@
 
 
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
@@ -1856,18 +1856,18 @@
 
 
 DescribeDatastoreResponseTypeDef = TypedDict(
     "DescribeDatastoreResponseTypeDef",
     {
         "datastore": DatastoreTypeDef,
         "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics/type_defs.pyi` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,28 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "MessageTypeDef",
-    "ResponseMetadataTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
     "RetentionPeriodTypeDef",
     "ColumnTypeDef",
     "ResourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
+    "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
+    "CreatePipelineResponseTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
@@ -78,40 +79,44 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
     "LoggingOptionsTypeDef",
     "DescribePipelineRequestRequestTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
     "GlueConfigurationTypeDef",
     "LambdaActivityTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "SampleChannelDataRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageRequestRequestTypeDef",
-    "BatchPutMessageResponseTypeDef",
-    "CreateDatasetContentResponseTypeDef",
-    "CreatePipelineResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
+    "SampleChannelDataRequestRequestTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "BatchPutMessageResponseTypeDef",
+    "BatchPutMessageRequestRequestTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
     "ChannelStorageSummaryTypeDef",
     "ChannelStorageTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
@@ -126,19 +131,14 @@
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     "DatastorePartitionTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "VariableTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
     "ChannelSummaryTypeDef",
     "ChannelTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
@@ -210,25 +210,14 @@
     "MessageTypeDef",
     {
         "messageId": str,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
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
 CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
@@ -347,23 +336,40 @@
 
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
+CreateDatasetContentResponseTypeDef = TypedDict(
+    "CreateDatasetContentResponseTypeDef",
+    {
+        "versionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
 )
 
+CreatePipelineResponseTypeDef = TypedDict(
+    "CreatePipelineResponseTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -675,14 +681,21 @@
 )
 
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -739,33 +752,53 @@
     },
     total=False,
 )
 
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "scheduledOnOrAfter": Union[datetime, str],
+        "scheduledBefore": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
+    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetContentsRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
@@ -781,32 +814,56 @@
 
 class ListDatasetContentsRequestRequestTypeDef(
     _RequiredListDatasetContentsRequestRequestTypeDef,
     _OptionalListDatasetContentsRequestRequestTypeDef,
 ):
     pass
 
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -841,14 +898,24 @@
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
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
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -891,14 +958,34 @@
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
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
+RunPipelineActivityResponseTypeDef = TypedDict(
+    "RunPipelineActivityResponseTypeDef",
+    {
+        "payloads": List[bytes],
+        "logResult": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
     "_RequiredSampleChannelDataRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
@@ -912,84 +999,51 @@
 )
 
 class SampleChannelDataRequestRequestTypeDef(
     _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
 ):
     pass
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
-    {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
-    },
-)
-
-BatchPutMessageResponseTypeDef = TypedDict(
-    "BatchPutMessageResponseTypeDef",
-    {
-        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetContentResponseTypeDef = TypedDict(
-    "CreateDatasetContentResponseTypeDef",
-    {
-        "versionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePipelineResponseTypeDef = TypedDict(
-    "CreatePipelineResponseTypeDef",
+SampleChannelDataResponseTypeDef = TypedDict(
+    "SampleChannelDataResponseTypeDef",
     {
-        "pipelineName": str,
-        "pipelineArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "payloads": List[bytes],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+StartPipelineReprocessingResponseTypeDef = TypedDict(
+    "StartPipelineReprocessingResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "reprocessingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RunPipelineActivityResponseTypeDef = TypedDict(
-    "RunPipelineActivityResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "payloads": List[bytes],
-        "logResult": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-SampleChannelDataResponseTypeDef = TypedDict(
-    "SampleChannelDataResponseTypeDef",
+BatchPutMessageResponseTypeDef = TypedDict(
+    "BatchPutMessageResponseTypeDef",
     {
-        "payloads": List[bytes],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartPipelineReprocessingResponseTypeDef = TypedDict(
-    "StartPipelineReprocessingResponseTypeDef",
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
     {
-        "reprocessingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "channelName": str,
+        "messages": Sequence[MessageTypeDef],
     },
 )
 
 _RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
@@ -1047,35 +1101,35 @@
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
@@ -1083,15 +1137,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1113,15 +1167,15 @@
 
 GetDatasetContentResponseTypeDef = TypedDict(
     "GetDatasetContentResponseTypeDef",
     {
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
@@ -1170,15 +1224,15 @@
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
@@ -1202,68 +1256,14 @@
 )
 
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
-    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-):
-    pass
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1386,15 +1386,15 @@
 )
 
 ListDatasetContentsResponseTypeDef = TypedDict(
     "ListDatasetContentsResponseTypeDef",
     {
         "datasetContentSummaries": List[DatasetContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
@@ -1551,33 +1551,33 @@
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
@@ -1587,15 +1587,15 @@
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
@@ -1639,15 +1639,15 @@
     total=False,
 )
 
 DescribePipelineResponseTypeDef = TypedDict(
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
@@ -1709,15 +1709,15 @@
     pass
 
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
@@ -1785,18 +1785,18 @@
     pass
 
 DescribeDatastoreResponseTypeDef = TypedDict(
     "DescribeDatastoreResponseTypeDef",
     {
         "datastore": DatastoreTypeDef,
         "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/PKG-INFO` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTAnalytics 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTAnalytics 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
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
 
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,27 +347,28 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
-    ResponseMetadataTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
     RetentionPeriodTypeDef,
     ColumnTypeDef,
     ResourceConfigurationTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
+    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
+    CreatePipelineResponseTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
@@ -387,40 +389,44 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
     LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
     DeviceShadowEnrichActivityTypeDef,
+    EmptyResponseMetadataTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
+    PaginatorConfigTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    CreateDatasetContentResponseTypeDef,
-    CreatePipelineResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
     ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -435,19 +441,14 @@
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     VariableTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
     ChannelSummaryTypeDef,
     ChannelTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
@@ -493,42 +494,42 @@
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

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/mypy_boto3_iotanalytics.egg-info/SOURCES.txt` & `mypy-boto3-iotanalytics-1.27.0/mypy_boto3_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.26.0.post1/setup.py` & `mypy-boto3-iotanalytics-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iotanalytics.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotanalytics",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTAnalytics 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.IoTAnalytics 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iotanalytics": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iotanalytics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/",
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


# Comparing `tmp/mypy-boto3-kinesis-1.26.61.tar.gz` & `tmp/mypy-boto3-kinesis-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-1.26.61.tar", last modified: Tue Jan 31 20:49:57 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-1.27.0.tar", last modified: Mon Jul  3 19:50:58 2023, max compression
```

## Comparing `mypy-boto3-kinesis-1.26.61.tar` & `mypy-boto3-kinesis-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.142170 mypy-boto3-kinesis-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-01-31 20:49:57.130169 mypy-boto3-kinesis-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.126170 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31826 2023-01-31 20:48:48.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31765 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-31 20:48:47.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.130169 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-01-31 20:49:56.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-31 20:49:56.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-31 20:49:56.000000 mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:57.142170 mypy-boto3-kinesis-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-31 20:48:46.000000 mypy-boto3-kinesis-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.955511 mypy-boto3-kinesis-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-07-03 19:50:58.955511 mypy-boto3-kinesis-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.955511 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-07-03 19:40:20.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-03 19:40:19.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.955511 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-07-03 19:50:58.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 19:50:58.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:58.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:58.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:58.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:58.000000 mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:58.955511 mypy-boto3-kinesis-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:40:17.000000 mypy-boto3-kinesis-1.27.0/setup.py
```

### Comparing `mypy-boto3-kinesis-1.26.61/LICENSE` & `mypy-boto3-kinesis-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kinesis-1.26.61/PKG-INFO` & `mypy-boto3-kinesis-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.26.61
-Summary: Type annotations for boto3.Kinesis 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Kinesis 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kinesis"></a>
 
 # mypy-boto3-kinesis
 
 [![PyPI - mypy-boto3-kinesis](https://img.shields.io/pypi/v/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,69 +371,69 @@
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeStreamInputDescribeStreamPaginateTypeDef,
     DescribeStreamInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
+    EnhancedMonitoringOutputTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
     GetShardIteratorInputRequestTypeDef,
+    GetShardIteratorOutputTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
     ShardFilterTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamConsumersInputRequestTypeDef,
+    ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutRecordInputRequestTypeDef,
+    PutRecordOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
+    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
     UpdateShardCountInputRequestTypeDef,
+    UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
-    CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnhancedMonitoringOutputTypeDef,
-    GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
-    PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
-    UpdateShardCountOutputTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
+    CreateStreamInputRequestTypeDef,
+    StreamSummaryTypeDef,
+    UpdateStreamModeInputRequestTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
     StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
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

### Comparing `mypy-boto3-kinesis-1.26.61/README.md` & `mypy-boto3-kinesis-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kinesis"></a>
 
 # mypy-boto3-kinesis
 
 [![PyPI - mypy-boto3-kinesis](https://img.shields.io/pypi/v/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,69 +339,69 @@
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeStreamInputDescribeStreamPaginateTypeDef,
     DescribeStreamInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
+    EnhancedMonitoringOutputTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
     GetShardIteratorInputRequestTypeDef,
+    GetShardIteratorOutputTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
     ShardFilterTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamConsumersInputRequestTypeDef,
+    ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutRecordInputRequestTypeDef,
+    PutRecordOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
+    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
     UpdateShardCountInputRequestTypeDef,
+    UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
-    CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnhancedMonitoringOutputTypeDef,
-    GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
-    PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
-    UpdateShardCountOutputTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
+    CreateStreamInputRequestTypeDef,
+    StreamSummaryTypeDef,
+    UpdateStreamModeInputRequestTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
     StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
@@ -427,42 +427,42 @@
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

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/__init__.py` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/__init__.pyi` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/client.py` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/client.pyi` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/literals.py` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
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
@@ -134,14 +135,15 @@
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
@@ -238,14 +241,15 @@
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
@@ -281,14 +285,15 @@
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
@@ -307,16 +312,19 @@
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
@@ -396,18 +404,21 @@
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

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/literals.pyi` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -132,14 +133,15 @@
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
@@ -218,14 +220,15 @@
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
@@ -236,14 +239,15 @@
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
@@ -279,14 +283,15 @@
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
@@ -305,16 +310,19 @@
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
@@ -394,18 +402,21 @@
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

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/paginator.py` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStreamOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#describestreampaginator)
         """
 
 
@@ -86,15 +86,15 @@
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
         StreamCreationTimestamp: Union[datetime, str] = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#listshardspaginator)
         """
 
 
@@ -105,28 +105,31 @@
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
         StreamCreationTimestamp: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
         """
 
 
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self, *, ExclusiveStartStreamName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ExclusiveStartStreamName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/paginator.pyi` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStreamOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#describestreampaginator)
         """
 
 class ListShardsPaginator(Paginator):
@@ -82,15 +82,15 @@
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
         StreamCreationTimestamp: Union[datetime, str] = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#listshardspaginator)
         """
 
 class ListStreamConsumersPaginator(Paginator):
@@ -100,27 +100,30 @@
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
         StreamCreationTimestamp: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamconsumerspaginator)
         """
 
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self, *, ExclusiveStartStreamName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ExclusiveStartStreamName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/type_defs.py` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,69 +42,69 @@
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
     "DecreaseStreamRetentionPeriodInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "DeregisterStreamConsumerInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeStreamSummaryInputRequestTypeDef",
     "DisableEnhancedMonitoringInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableEnhancedMonitoringInputRequestTypeDef",
     "EnhancedMetricsTypeDef",
+    "EnhancedMonitoringOutputTypeDef",
     "GetRecordsInputRequestTypeDef",
     "RecordTypeDef",
     "GetShardIteratorInputRequestTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "IncreaseStreamRetentionPeriodInputRequestTypeDef",
     "InternalFailureExceptionTypeDef",
     "KMSAccessDeniedExceptionTypeDef",
     "KMSDisabledExceptionTypeDef",
     "KMSInvalidStateExceptionTypeDef",
     "KMSNotFoundExceptionTypeDef",
     "KMSOptInRequiredTypeDef",
     "KMSThrottlingExceptionTypeDef",
     "ShardFilterTypeDef",
+    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     "ListStreamConsumersInputRequestTypeDef",
+    "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "TagTypeDef",
     "MergeShardsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutRecordInputRequestTypeDef",
+    "PutRecordOutputTypeDef",
     "PutRecordsRequestEntryTypeDef",
     "PutRecordsResultEntryTypeDef",
     "RegisterStreamConsumerInputRequestTypeDef",
     "RemoveTagsFromStreamInputRequestTypeDef",
     "ResourceInUseExceptionTypeDef",
     "ResourceNotFoundExceptionTypeDef",
+    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
     "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
     "UpdateShardCountInputRequestTypeDef",
+    "UpdateShardCountOutputTypeDef",
     "ChildShardTypeDef",
-    "CreateStreamInputRequestTypeDef",
-    "StreamSummaryTypeDef",
-    "UpdateStreamModeInputRequestTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnhancedMonitoringOutputTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
-    "PutRecordOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
-    "UpdateShardCountOutputTypeDef",
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
-    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    "ListStreamsInputListStreamsPaginateTypeDef",
+    "CreateStreamInputRequestTypeDef",
+    "StreamSummaryTypeDef",
+    "UpdateStreamModeInputRequestTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
     "StreamDescriptionSummaryTypeDef",
     "ListShardsInputListShardsPaginateTypeDef",
     "ListShardsInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "PutRecordsInputRequestTypeDef",
@@ -219,41 +219,41 @@
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ShardLimit": int,
+        "OpenShardCount": int,
+        "OnDemandStreamCount": int,
+        "OnDemandStreamCountLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStreamConsumerInputRequestTypeDef = TypedDict(
     "DescribeStreamConsumerInputRequestTypeDef",
     {
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeStreamInputRequestTypeDef = TypedDict(
     "DescribeStreamInputRequestTypeDef",
     {
@@ -302,14 +302,21 @@
 class DisableEnhancedMonitoringInputRequestTypeDef(
     _RequiredDisableEnhancedMonitoringInputRequestTypeDef,
     _OptionalDisableEnhancedMonitoringInputRequestTypeDef,
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
     "_RequiredEnableEnhancedMonitoringInputRequestTypeDef",
     {
         "ShardLevelMetrics": Sequence[MetricsNameType],
     },
 )
 _OptionalEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
@@ -333,14 +340,25 @@
     "EnhancedMetricsTypeDef",
     {
         "ShardLevelMetrics": List[MetricsNameType],
     },
     total=False,
 )
 
+EnhancedMonitoringOutputTypeDef = TypedDict(
+    "EnhancedMonitoringOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardLevelMetrics": List[MetricsNameType],
+        "DesiredShardLevelMetrics": List[MetricsNameType],
+        "StreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -402,14 +420,22 @@
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
     "_RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef",
     {
         "RetentionPeriodHours": int,
     },
 )
 _OptionalIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
@@ -501,14 +527,37 @@
 )
 
 
 class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
     pass
 
 
+_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamCreationTimestamp": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
+    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
     "_RequiredListStreamConsumersInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
@@ -524,14 +573,23 @@
 
 class ListStreamConsumersInputRequestTypeDef(
     _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
 ):
     pass
 
 
+ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsInputListStreamsPaginateTypeDef",
+    {
+        "ExclusiveStartStreamName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "Limit": int,
         "ExclusiveStartStreamName": str,
         "NextToken": str,
     },
@@ -587,14 +645,24 @@
 
 class MergeShardsInputRequestTypeDef(
     _RequiredMergeShardsInputRequestTypeDef, _OptionalMergeShardsInputRequestTypeDef
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
 _RequiredPutRecordInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordInputRequestTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -612,14 +680,24 @@
 
 class PutRecordInputRequestTypeDef(
     _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
 ):
     pass
 
 
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "ShardId": str,
+        "SequenceNumber": str,
+        "EncryptionType": EncryptionTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutRecordsRequestEntryTypeDef = TypedDict(
     "_RequiredPutRecordsRequestEntryTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -692,14 +770,25 @@
     "ResourceNotFoundExceptionTypeDef",
     {
         "message": str,
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
 _RequiredSequenceNumberRangeTypeDef = TypedDict(
     "_RequiredSequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
     },
 )
 _OptionalSequenceNumberRangeTypeDef = TypedDict(
@@ -827,23 +916,59 @@
 
 class UpdateShardCountInputRequestTypeDef(
     _RequiredUpdateShardCountInputRequestTypeDef, _OptionalUpdateShardCountInputRequestTypeDef
 ):
     pass
 
 
+UpdateShardCountOutputTypeDef = TypedDict(
+    "UpdateShardCountOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardCount": int,
+        "TargetShardCount": int,
+        "StreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChildShardTypeDef = TypedDict(
     "ChildShardTypeDef",
     {
         "ShardId": str,
         "ParentShards": List[str],
         "HashKeyRange": HashKeyRangeTypeDef,
     },
 )
 
+DescribeStreamConsumerOutputTypeDef = TypedDict(
+    "DescribeStreamConsumerOutputTypeDef",
+    {
+        "ConsumerDescription": ConsumerDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStreamConsumersOutputTypeDef = TypedDict(
+    "ListStreamConsumersOutputTypeDef",
+    {
+        "Consumers": List[ConsumerTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterStreamConsumerOutputTypeDef = TypedDict(
+    "RegisterStreamConsumerOutputTypeDef",
+    {
+        "Consumer": ConsumerTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
     },
 )
 _OptionalCreateStreamInputRequestTypeDef = TypedDict(
@@ -888,139 +1013,14 @@
     "UpdateStreamModeInputRequestTypeDef",
     {
         "StreamARN": str,
         "StreamModeDetails": StreamModeDetailsTypeDef,
     },
 )
 
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "ShardLimit": int,
-        "OpenShardCount": int,
-        "OnDemandStreamCount": int,
-        "OnDemandStreamCountLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStreamConsumerOutputTypeDef = TypedDict(
-    "DescribeStreamConsumerOutputTypeDef",
-    {
-        "ConsumerDescription": ConsumerDescriptionTypeDef,
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
-EnhancedMonitoringOutputTypeDef = TypedDict(
-    "EnhancedMonitoringOutputTypeDef",
-    {
-        "StreamName": str,
-        "CurrentShardLevelMetrics": List[MetricsNameType],
-        "DesiredShardLevelMetrics": List[MetricsNameType],
-        "StreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStreamConsumersOutputTypeDef = TypedDict(
-    "ListStreamConsumersOutputTypeDef",
-    {
-        "Consumers": List[ConsumerTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
-    {
-        "ShardId": str,
-        "SequenceNumber": str,
-        "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterStreamConsumerOutputTypeDef = TypedDict(
-    "RegisterStreamConsumerOutputTypeDef",
-    {
-        "Consumer": ConsumerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateShardCountOutputTypeDef = TypedDict(
-    "UpdateShardCountOutputTypeDef",
-    {
-        "StreamName": str,
-        "CurrentShardCount": int,
-        "TargetShardCount": int,
-        "StreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamCreationTimestamp": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
-    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-):
-    pass
-
-
-ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsInputListStreamsPaginateTypeDef",
-    {
-        "ExclusiveStartStreamName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeStreamInputStreamExistsWaitTypeDef = TypedDict(
     "DescribeStreamInputStreamExistsWaitTypeDef",
     {
         "StreamName": str,
         "Limit": int,
         "ExclusiveStartShardId": str,
         "StreamARN": str,
@@ -1075,15 +1075,15 @@
     "ListShardsInputListShardsPaginateTypeDef",
     {
         "StreamName": str,
         "ExclusiveStartShardId": str,
         "StreamCreationTimestamp": Union[datetime, str],
         "ShardFilter": ShardFilterTypeDef,
         "StreamARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListShardsInputRequestTypeDef = TypedDict(
     "ListShardsInputRequestTypeDef",
     {
@@ -1099,15 +1099,15 @@
 )
 
 ListTagsForStreamOutputTypeDef = TypedDict(
     "ListTagsForStreamOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "HasMoreTags": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutRecordsInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordsInputRequestTypeDef",
     {
         "Records": Sequence[PutRecordsRequestEntryTypeDef],
@@ -1131,15 +1131,15 @@
 
 PutRecordsOutputTypeDef = TypedDict(
     "PutRecordsOutputTypeDef",
     {
         "FailedRecordCount": int,
         "Records": List[PutRecordsResultEntryTypeDef],
         "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredShardTypeDef = TypedDict(
     "_RequiredShardTypeDef",
     {
         "ShardId": str,
@@ -1173,15 +1173,15 @@
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubscribeToShardEventTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -1207,32 +1207,32 @@
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamNames": List[str],
         "HasMoreStreams": bool,
         "NextToken": str,
         "StreamSummaries": List[StreamSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStreamSummaryOutputTypeDef = TypedDict(
     "DescribeStreamSummaryOutputTypeDef",
     {
         "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamDescriptionTypeDef = TypedDict(
     "_RequiredStreamDescriptionTypeDef",
     {
         "StreamName": str,
@@ -1291,18 +1291,18 @@
     pass
 
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscribeToShardOutputTypeDef = TypedDict(
     "SubscribeToShardOutputTypeDef",
     {
         "EventStream": SubscribeToShardEventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/type_defs.pyi` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -41,69 +41,69 @@
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
     "DecreaseStreamRetentionPeriodInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "DeregisterStreamConsumerInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeStreamSummaryInputRequestTypeDef",
     "DisableEnhancedMonitoringInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableEnhancedMonitoringInputRequestTypeDef",
     "EnhancedMetricsTypeDef",
+    "EnhancedMonitoringOutputTypeDef",
     "GetRecordsInputRequestTypeDef",
     "RecordTypeDef",
     "GetShardIteratorInputRequestTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "IncreaseStreamRetentionPeriodInputRequestTypeDef",
     "InternalFailureExceptionTypeDef",
     "KMSAccessDeniedExceptionTypeDef",
     "KMSDisabledExceptionTypeDef",
     "KMSInvalidStateExceptionTypeDef",
     "KMSNotFoundExceptionTypeDef",
     "KMSOptInRequiredTypeDef",
     "KMSThrottlingExceptionTypeDef",
     "ShardFilterTypeDef",
+    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
     "ListStreamConsumersInputRequestTypeDef",
+    "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "TagTypeDef",
     "MergeShardsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutRecordInputRequestTypeDef",
+    "PutRecordOutputTypeDef",
     "PutRecordsRequestEntryTypeDef",
     "PutRecordsResultEntryTypeDef",
     "RegisterStreamConsumerInputRequestTypeDef",
     "RemoveTagsFromStreamInputRequestTypeDef",
     "ResourceInUseExceptionTypeDef",
     "ResourceNotFoundExceptionTypeDef",
+    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
     "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
     "UpdateShardCountInputRequestTypeDef",
+    "UpdateShardCountOutputTypeDef",
     "ChildShardTypeDef",
-    "CreateStreamInputRequestTypeDef",
-    "StreamSummaryTypeDef",
-    "UpdateStreamModeInputRequestTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnhancedMonitoringOutputTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
-    "PutRecordOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
-    "UpdateShardCountOutputTypeDef",
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
-    "ListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    "ListStreamsInputListStreamsPaginateTypeDef",
+    "CreateStreamInputRequestTypeDef",
+    "StreamSummaryTypeDef",
+    "UpdateStreamModeInputRequestTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
     "StreamDescriptionSummaryTypeDef",
     "ListShardsInputListShardsPaginateTypeDef",
     "ListShardsInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "PutRecordsInputRequestTypeDef",
@@ -214,41 +214,41 @@
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ShardLimit": int,
+        "OpenShardCount": int,
+        "OnDemandStreamCount": int,
+        "OnDemandStreamCountLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStreamConsumerInputRequestTypeDef = TypedDict(
     "DescribeStreamConsumerInputRequestTypeDef",
     {
         "StreamARN": str,
         "ConsumerName": str,
         "ConsumerARN": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
+    "DescribeStreamInputDescribeStreamPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeStreamInputRequestTypeDef = TypedDict(
     "DescribeStreamInputRequestTypeDef",
     {
@@ -295,14 +295,21 @@
 
 class DisableEnhancedMonitoringInputRequestTypeDef(
     _RequiredDisableEnhancedMonitoringInputRequestTypeDef,
     _OptionalDisableEnhancedMonitoringInputRequestTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
     "_RequiredEnableEnhancedMonitoringInputRequestTypeDef",
     {
         "ShardLevelMetrics": Sequence[MetricsNameType],
     },
 )
 _OptionalEnableEnhancedMonitoringInputRequestTypeDef = TypedDict(
@@ -324,14 +331,25 @@
     "EnhancedMetricsTypeDef",
     {
         "ShardLevelMetrics": List[MetricsNameType],
     },
     total=False,
 )
 
+EnhancedMonitoringOutputTypeDef = TypedDict(
+    "EnhancedMonitoringOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardLevelMetrics": List[MetricsNameType],
+        "DesiredShardLevelMetrics": List[MetricsNameType],
+        "StreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -387,14 +405,22 @@
 )
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
     "_RequiredIncreaseStreamRetentionPeriodInputRequestTypeDef",
     {
         "RetentionPeriodHours": int,
     },
 )
 _OptionalIncreaseStreamRetentionPeriodInputRequestTypeDef = TypedDict(
@@ -482,14 +508,35 @@
     },
     total=False,
 )
 
 class ShardFilterTypeDef(_RequiredShardFilterTypeDef, _OptionalShardFilterTypeDef):
     pass
 
+_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamARN": str,
+    },
+)
+_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
+    {
+        "StreamCreationTimestamp": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
+    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
+):
+    pass
+
 _RequiredListStreamConsumersInputRequestTypeDef = TypedDict(
     "_RequiredListStreamConsumersInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalListStreamConsumersInputRequestTypeDef = TypedDict(
@@ -503,14 +550,23 @@
 )
 
 class ListStreamConsumersInputRequestTypeDef(
     _RequiredListStreamConsumersInputRequestTypeDef, _OptionalListStreamConsumersInputRequestTypeDef
 ):
     pass
 
+ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsInputListStreamsPaginateTypeDef",
+    {
+        "ExclusiveStartStreamName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
         "Limit": int,
         "ExclusiveStartStreamName": str,
         "NextToken": str,
     },
@@ -562,14 +618,24 @@
 )
 
 class MergeShardsInputRequestTypeDef(
     _RequiredMergeShardsInputRequestTypeDef, _OptionalMergeShardsInputRequestTypeDef
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
 _RequiredPutRecordInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordInputRequestTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -585,14 +651,24 @@
 )
 
 class PutRecordInputRequestTypeDef(
     _RequiredPutRecordInputRequestTypeDef, _OptionalPutRecordInputRequestTypeDef
 ):
     pass
 
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "ShardId": str,
+        "SequenceNumber": str,
+        "EncryptionType": EncryptionTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutRecordsRequestEntryTypeDef = TypedDict(
     "_RequiredPutRecordsRequestEntryTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "PartitionKey": str,
     },
 )
@@ -661,14 +737,25 @@
     "ResourceNotFoundExceptionTypeDef",
     {
         "message": str,
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
 _RequiredSequenceNumberRangeTypeDef = TypedDict(
     "_RequiredSequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
     },
 )
 _OptionalSequenceNumberRangeTypeDef = TypedDict(
@@ -784,23 +871,59 @@
 )
 
 class UpdateShardCountInputRequestTypeDef(
     _RequiredUpdateShardCountInputRequestTypeDef, _OptionalUpdateShardCountInputRequestTypeDef
 ):
     pass
 
+UpdateShardCountOutputTypeDef = TypedDict(
+    "UpdateShardCountOutputTypeDef",
+    {
+        "StreamName": str,
+        "CurrentShardCount": int,
+        "TargetShardCount": int,
+        "StreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChildShardTypeDef = TypedDict(
     "ChildShardTypeDef",
     {
         "ShardId": str,
         "ParentShards": List[str],
         "HashKeyRange": HashKeyRangeTypeDef,
     },
 )
 
+DescribeStreamConsumerOutputTypeDef = TypedDict(
+    "DescribeStreamConsumerOutputTypeDef",
+    {
+        "ConsumerDescription": ConsumerDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStreamConsumersOutputTypeDef = TypedDict(
+    "ListStreamConsumersOutputTypeDef",
+    {
+        "Consumers": List[ConsumerTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterStreamConsumerOutputTypeDef = TypedDict(
+    "RegisterStreamConsumerOutputTypeDef",
+    {
+        "Consumer": ConsumerTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
     },
 )
 _OptionalCreateStreamInputRequestTypeDef = TypedDict(
@@ -841,137 +964,14 @@
     "UpdateStreamModeInputRequestTypeDef",
     {
         "StreamARN": str,
         "StreamModeDetails": StreamModeDetailsTypeDef,
     },
 )
 
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "ShardLimit": int,
-        "OpenShardCount": int,
-        "OnDemandStreamCount": int,
-        "OnDemandStreamCountLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStreamConsumerOutputTypeDef = TypedDict(
-    "DescribeStreamConsumerOutputTypeDef",
-    {
-        "ConsumerDescription": ConsumerDescriptionTypeDef,
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
-EnhancedMonitoringOutputTypeDef = TypedDict(
-    "EnhancedMonitoringOutputTypeDef",
-    {
-        "StreamName": str,
-        "CurrentShardLevelMetrics": List[MetricsNameType],
-        "DesiredShardLevelMetrics": List[MetricsNameType],
-        "StreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStreamConsumersOutputTypeDef = TypedDict(
-    "ListStreamConsumersOutputTypeDef",
-    {
-        "Consumers": List[ConsumerTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
-    {
-        "ShardId": str,
-        "SequenceNumber": str,
-        "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterStreamConsumerOutputTypeDef = TypedDict(
-    "RegisterStreamConsumerOutputTypeDef",
-    {
-        "Consumer": ConsumerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateShardCountOutputTypeDef = TypedDict(
-    "UpdateShardCountOutputTypeDef",
-    {
-        "StreamName": str,
-        "CurrentShardCount": int,
-        "TargetShardCount": int,
-        "StreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStreamInputDescribeStreamPaginateTypeDef = TypedDict(
-    "DescribeStreamInputDescribeStreamPaginateTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamARN": str,
-    },
-)
-_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef",
-    {
-        "StreamCreationTimestamp": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStreamConsumersInputListStreamConsumersPaginateTypeDef(
-    _RequiredListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    _OptionalListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-):
-    pass
-
-ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsInputListStreamsPaginateTypeDef",
-    {
-        "ExclusiveStartStreamName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeStreamInputStreamExistsWaitTypeDef = TypedDict(
     "DescribeStreamInputStreamExistsWaitTypeDef",
     {
         "StreamName": str,
         "Limit": int,
         "ExclusiveStartShardId": str,
         "StreamARN": str,
@@ -1024,15 +1024,15 @@
     "ListShardsInputListShardsPaginateTypeDef",
     {
         "StreamName": str,
         "ExclusiveStartShardId": str,
         "StreamCreationTimestamp": Union[datetime, str],
         "ShardFilter": ShardFilterTypeDef,
         "StreamARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListShardsInputRequestTypeDef = TypedDict(
     "ListShardsInputRequestTypeDef",
     {
@@ -1048,15 +1048,15 @@
 )
 
 ListTagsForStreamOutputTypeDef = TypedDict(
     "ListTagsForStreamOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "HasMoreTags": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutRecordsInputRequestTypeDef = TypedDict(
     "_RequiredPutRecordsInputRequestTypeDef",
     {
         "Records": Sequence[PutRecordsRequestEntryTypeDef],
@@ -1078,15 +1078,15 @@
 
 PutRecordsOutputTypeDef = TypedDict(
     "PutRecordsOutputTypeDef",
     {
         "FailedRecordCount": int,
         "Records": List[PutRecordsResultEntryTypeDef],
         "EncryptionType": EncryptionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredShardTypeDef = TypedDict(
     "_RequiredShardTypeDef",
     {
         "ShardId": str,
@@ -1118,15 +1118,15 @@
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubscribeToShardEventTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -1150,32 +1150,32 @@
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamNames": List[str],
         "HasMoreStreams": bool,
         "NextToken": str,
         "StreamSummaries": List[StreamSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStreamSummaryOutputTypeDef = TypedDict(
     "DescribeStreamSummaryOutputTypeDef",
     {
         "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamDescriptionTypeDef = TypedDict(
     "_RequiredStreamDescriptionTypeDef",
     {
         "StreamName": str,
@@ -1230,18 +1230,18 @@
 ):
     pass
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscribeToShardOutputTypeDef = TypedDict(
     "SubscribeToShardOutputTypeDef",
     {
         "EventStream": SubscribeToShardEventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/waiter.py` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis/waiter.pyi` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/PKG-INFO` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.26.61
-Summary: Type annotations for boto3.Kinesis 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Kinesis 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kinesis"></a>
 
 # mypy-boto3-kinesis
 
 [![PyPI - mypy-boto3-kinesis](https://img.shields.io/pypi/v/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,69 +371,69 @@
     HashKeyRangeTypeDef,
     ConsumerDescriptionTypeDef,
     ConsumerTypeDef,
     StreamModeDetailsTypeDef,
     DecreaseStreamRetentionPeriodInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     DeregisterStreamConsumerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeStreamInputDescribeStreamPaginateTypeDef,
     DescribeStreamInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeStreamSummaryInputRequestTypeDef,
     DisableEnhancedMonitoringInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableEnhancedMonitoringInputRequestTypeDef,
     EnhancedMetricsTypeDef,
+    EnhancedMonitoringOutputTypeDef,
     GetRecordsInputRequestTypeDef,
     RecordTypeDef,
     GetShardIteratorInputRequestTypeDef,
+    GetShardIteratorOutputTypeDef,
     IncreaseStreamRetentionPeriodInputRequestTypeDef,
     InternalFailureExceptionTypeDef,
     KMSAccessDeniedExceptionTypeDef,
     KMSDisabledExceptionTypeDef,
     KMSInvalidStateExceptionTypeDef,
     KMSNotFoundExceptionTypeDef,
     KMSOptInRequiredTypeDef,
     KMSThrottlingExceptionTypeDef,
     ShardFilterTypeDef,
+    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
     ListStreamConsumersInputRequestTypeDef,
+    ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     TagTypeDef,
     MergeShardsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutRecordInputRequestTypeDef,
+    PutRecordOutputTypeDef,
     PutRecordsRequestEntryTypeDef,
     PutRecordsResultEntryTypeDef,
     RegisterStreamConsumerInputRequestTypeDef,
     RemoveTagsFromStreamInputRequestTypeDef,
     ResourceInUseExceptionTypeDef,
     ResourceNotFoundExceptionTypeDef,
+    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
     UpdateShardCountInputRequestTypeDef,
+    UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
-    CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeStreamConsumerOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnhancedMonitoringOutputTypeDef,
-    GetShardIteratorOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
-    PutRecordOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
-    UpdateShardCountOutputTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
+    CreateStreamInputRequestTypeDef,
+    StreamSummaryTypeDef,
+    UpdateStreamModeInputRequestTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
     StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
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

### Comparing `mypy-boto3-kinesis-1.26.61/mypy_boto3_kinesis.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-1.27.0/mypy_boto3_kinesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.26.61/setup.py` & `mypy-boto3-kinesis-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-kinesis.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis",
-    version="1.26.61",
+    version="1.27.0",
     packages=["mypy_boto3_kinesis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kinesis 1.26.61 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Kinesis 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/",
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


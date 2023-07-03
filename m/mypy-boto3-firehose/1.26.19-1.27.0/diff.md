# Comparing `tmp/mypy-boto3-firehose-1.26.19.tar.gz` & `tmp/mypy-boto3-firehose-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-firehose-1.26.19.tar", last modified: Tue Nov 29 20:35:12 2022, max compression
+gzip compressed data, was "mypy-boto3-firehose-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
```

## Comparing `mypy-boto3-firehose-1.26.19.tar` & `mypy-boto3-firehose-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.129234 mypy-boto3-firehose-1.26.19/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    16192 2022-11-29 20:35:12.121234 mypy-boto3-firehose-1.26.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14751 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.113234 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      912 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12873 2022-11-29 20:34:48.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    12855 2022-11-29 20:34:48.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10741 2022-11-29 20:34:48.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10739 2022-11-29 20:34:48.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    44828 2022-11-29 20:34:49.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    44779 2022-11-29 20:34:48.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16192 2022-11-29 20:35:11.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      632 2022-11-29 20:35:11.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 20:35:11.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-11-29 20:35:11.000000 mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 20:35:12.129234 mypy-boto3-firehose-1.26.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2022-11-29 20:34:47.000000 mypy-boto3-firehose-1.26.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.023261 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45008 2023-07-03 19:37:48.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44959 2023-07-03 19:37:48.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/setup.py
```

### Comparing `mypy-boto3-firehose-1.26.19/LICENSE` & `mypy-boto3-firehose-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-firehose-1.26.19/PKG-INFO` & `mypy-boto3-firehose-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.26.19
-Summary: Type annotations for boto3.Firehose 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.Firehose 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
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
 
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,15 +331,15 @@
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
     BufferingHintsTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
     RetryOptionsTypeDef,
@@ -348,30 +349,30 @@
     HttpEndpointBufferingHintsTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
     OrcSerDeTypeDef,
     ParquetSerDeTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
+    PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
+    ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
-    TagDeliveryStreamInputRequestTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamOutputTypeDef,
-    PutRecordOutputTypeDef,
+    TagDeliveryStreamInputRequestTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
     DeserializerTypeDef,
     DynamicPartitioningConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
     SerializerTypeDef,
@@ -422,42 +423,42 @@
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

### Comparing `mypy-boto3-firehose-1.26.19/README.md` & `mypy-boto3-firehose-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,15 +299,15 @@
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
     BufferingHintsTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
     RetryOptionsTypeDef,
@@ -317,30 +317,30 @@
     HttpEndpointBufferingHintsTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
     OrcSerDeTypeDef,
     ParquetSerDeTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
+    PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
+    ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
-    TagDeliveryStreamInputRequestTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamOutputTypeDef,
-    PutRecordOutputTypeDef,
+    TagDeliveryStreamInputRequestTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
     DeserializerTypeDef,
     DynamicPartitioningConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
     SerializerTypeDef,
@@ -391,42 +391,42 @@
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

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/client.py` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/client.pyi` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/literals.py` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
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
@@ -151,30 +152,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -200,14 +205,15 @@
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
@@ -252,14 +258,15 @@
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
@@ -270,34 +277,38 @@
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
@@ -310,14 +321,15 @@
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
@@ -336,24 +348,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -381,14 +397,16 @@
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
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -422,18 +440,21 @@
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
@@ -458,21 +479,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/literals.pyi` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -121,14 +121,15 @@
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
@@ -149,30 +150,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -198,14 +203,15 @@
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
@@ -250,14 +256,15 @@
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
@@ -268,34 +275,38 @@
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
@@ -308,14 +319,15 @@
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
@@ -334,24 +346,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -379,14 +395,16 @@
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
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -420,18 +438,21 @@
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
@@ -456,21 +477,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/type_defs.py` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
     "BufferingHintsTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDeliveryStreamOutputTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
     "RetryOptionsTypeDef",
@@ -80,30 +80,30 @@
     "HttpEndpointBufferingHintsTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
+    "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
     "OrcSerDeTypeDef",
     "ParquetSerDeTypeDef",
     "ProcessorParameterTypeDef",
     "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
+    "PutRecordOutputTypeDef",
     "RedshiftRetryOptionsTypeDef",
+    "ResponseMetadataTypeDef",
     "SplunkRetryOptionsTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
-    "TagDeliveryStreamInputRequestTypeDef",
-    "CreateDeliveryStreamOutputTypeDef",
-    "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamOutputTypeDef",
-    "PutRecordOutputTypeDef",
+    "TagDeliveryStreamInputRequestTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
     "DeserializerTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
     "SerializerTypeDef",
@@ -283,22 +283,19 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDeliveryStreamOutputTypeDef = TypedDict(
+    "CreateDeliveryStreamOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DeliveryStreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SchemaConfigurationTypeDef = TypedDict(
     "SchemaConfigurationTypeDef",
     {
         "RoleARN": str,
@@ -486,14 +483,23 @@
         "Limit": int,
         "DeliveryStreamType": DeliveryStreamTypeType,
         "ExclusiveStartDeliveryStreamName": str,
     },
     total=False,
 )
 
+ListDeliveryStreamsOutputTypeDef = TypedDict(
+    "ListDeliveryStreamsOutputTypeDef",
+    {
+        "DeliveryStreamNames": List[str],
+        "HasMoreDeliveryStreams": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -564,22 +570,42 @@
         "RecordId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "RecordId": str,
+        "Encrypted": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RedshiftRetryOptionsTypeDef = TypedDict(
     "RedshiftRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
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
 SplunkRetryOptionsTypeDef = TypedDict(
     "SplunkRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
@@ -604,67 +630,43 @@
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "_OptionalStartDeliveryStreamEncryptionInputRequestTypeDef",
     {
-        "DeliveryStreamEncryptionConfigurationInput": DeliveryStreamEncryptionConfigurationInputTypeDef,
+        "DeliveryStreamEncryptionConfigurationInput": (
+            DeliveryStreamEncryptionConfigurationInputTypeDef
+        ),
     },
     total=False,
 )
 
 
 class StartDeliveryStreamEncryptionInputRequestTypeDef(
     _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef,
     _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
 
-TagDeliveryStreamInputRequestTypeDef = TypedDict(
-    "TagDeliveryStreamInputRequestTypeDef",
-    {
-        "DeliveryStreamName": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateDeliveryStreamOutputTypeDef = TypedDict(
-    "CreateDeliveryStreamOutputTypeDef",
-    {
-        "DeliveryStreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeliveryStreamsOutputTypeDef = TypedDict(
-    "ListDeliveryStreamsOutputTypeDef",
-    {
-        "DeliveryStreamNames": List[str],
-        "HasMoreDeliveryStreams": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
     "ListTagsForDeliveryStreamOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "HasMoreTags": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
+TagDeliveryStreamInputRequestTypeDef = TypedDict(
+    "TagDeliveryStreamInputRequestTypeDef",
     {
-        "RecordId": str,
-        "Encrypted": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DeliveryStreamName": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 DeliveryStreamEncryptionConfigurationTypeDef = TypedDict(
     "DeliveryStreamEncryptionConfigurationTypeDef",
     {
         "KeyARN": str,
@@ -765,15 +767,15 @@
 
 PutRecordBatchOutputTypeDef = TypedDict(
     "PutRecordBatchOutputTypeDef",
     {
         "FailedPutCount": int,
         "Encrypted": bool,
         "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputFormatConfigurationTypeDef = TypedDict(
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
@@ -1374,24 +1376,30 @@
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_OptionalCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamType": DeliveryStreamTypeType,
         "KinesisStreamSourceConfiguration": KinesisStreamSourceConfigurationTypeDef,
-        "DeliveryStreamEncryptionConfigurationInput": DeliveryStreamEncryptionConfigurationInputTypeDef,
+        "DeliveryStreamEncryptionConfigurationInput": (
+            DeliveryStreamEncryptionConfigurationInputTypeDef
+        ),
         "S3DestinationConfiguration": S3DestinationConfigurationTypeDef,
         "ExtendedS3DestinationConfiguration": ExtendedS3DestinationConfigurationTypeDef,
         "RedshiftDestinationConfiguration": RedshiftDestinationConfigurationTypeDef,
         "ElasticsearchDestinationConfiguration": ElasticsearchDestinationConfigurationTypeDef,
-        "AmazonopensearchserviceDestinationConfiguration": AmazonopensearchserviceDestinationConfigurationTypeDef,
+        "AmazonopensearchserviceDestinationConfiguration": (
+            AmazonopensearchserviceDestinationConfigurationTypeDef
+        ),
         "SplunkDestinationConfiguration": SplunkDestinationConfigurationTypeDef,
         "HttpEndpointDestinationConfiguration": HttpEndpointDestinationConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
-        "AmazonOpenSearchServerlessDestinationConfiguration": AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
+        "AmazonOpenSearchServerlessDestinationConfiguration": (
+            AmazonOpenSearchServerlessDestinationConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
@@ -1409,18 +1417,22 @@
 _OptionalDestinationDescriptionTypeDef = TypedDict(
     "_OptionalDestinationDescriptionTypeDef",
     {
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
         "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
         "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
-        "AmazonopensearchserviceDestinationDescription": AmazonopensearchserviceDestinationDescriptionTypeDef,
+        "AmazonopensearchserviceDestinationDescription": (
+            AmazonopensearchserviceDestinationDescriptionTypeDef
+        ),
         "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
         "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
-        "AmazonOpenSearchServerlessDestinationDescription": AmazonOpenSearchServerlessDestinationDescriptionTypeDef,
+        "AmazonOpenSearchServerlessDestinationDescription": (
+            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
+        ),
     },
     total=False,
 )
 
 
 class DestinationDescriptionTypeDef(
     _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
@@ -1442,15 +1454,17 @@
         "S3DestinationUpdate": S3DestinationUpdateTypeDef,
         "ExtendedS3DestinationUpdate": ExtendedS3DestinationUpdateTypeDef,
         "RedshiftDestinationUpdate": RedshiftDestinationUpdateTypeDef,
         "ElasticsearchDestinationUpdate": ElasticsearchDestinationUpdateTypeDef,
         "AmazonopensearchserviceDestinationUpdate": AmazonopensearchserviceDestinationUpdateTypeDef,
         "SplunkDestinationUpdate": SplunkDestinationUpdateTypeDef,
         "HttpEndpointDestinationUpdate": HttpEndpointDestinationUpdateTypeDef,
-        "AmazonOpenSearchServerlessDestinationUpdate": AmazonOpenSearchServerlessDestinationUpdateTypeDef,
+        "AmazonOpenSearchServerlessDestinationUpdate": (
+            AmazonOpenSearchServerlessDestinationUpdateTypeDef
+        ),
     },
     total=False,
 )
 
 
 class UpdateDestinationInputRequestTypeDef(
     _RequiredUpdateDestinationInputRequestTypeDef, _OptionalUpdateDestinationInputRequestTypeDef
@@ -1489,10 +1503,10 @@
     pass
 
 
 DescribeDeliveryStreamOutputTypeDef = TypedDict(
     "DescribeDeliveryStreamOutputTypeDef",
     {
         "DeliveryStreamDescription": DeliveryStreamDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose/type_defs.pyi` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
     "BufferingHintsTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDeliveryStreamOutputTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
     "RetryOptionsTypeDef",
@@ -79,30 +79,30 @@
     "HttpEndpointBufferingHintsTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
+    "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
     "OrcSerDeTypeDef",
     "ParquetSerDeTypeDef",
     "ProcessorParameterTypeDef",
     "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
+    "PutRecordOutputTypeDef",
     "RedshiftRetryOptionsTypeDef",
+    "ResponseMetadataTypeDef",
     "SplunkRetryOptionsTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
-    "TagDeliveryStreamInputRequestTypeDef",
-    "CreateDeliveryStreamOutputTypeDef",
-    "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamOutputTypeDef",
-    "PutRecordOutputTypeDef",
+    "TagDeliveryStreamInputRequestTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
     "DeserializerTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
     "SerializerTypeDef",
@@ -276,22 +276,19 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDeliveryStreamOutputTypeDef = TypedDict(
+    "CreateDeliveryStreamOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DeliveryStreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SchemaConfigurationTypeDef = TypedDict(
     "SchemaConfigurationTypeDef",
     {
         "RoleARN": str,
@@ -473,14 +470,23 @@
         "Limit": int,
         "DeliveryStreamType": DeliveryStreamTypeType,
         "ExclusiveStartDeliveryStreamName": str,
     },
     total=False,
 )
 
+ListDeliveryStreamsOutputTypeDef = TypedDict(
+    "ListDeliveryStreamsOutputTypeDef",
+    {
+        "DeliveryStreamNames": List[str],
+        "HasMoreDeliveryStreams": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalListTagsForDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -549,22 +555,42 @@
         "RecordId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+PutRecordOutputTypeDef = TypedDict(
+    "PutRecordOutputTypeDef",
+    {
+        "RecordId": str,
+        "Encrypted": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RedshiftRetryOptionsTypeDef = TypedDict(
     "RedshiftRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
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
 SplunkRetryOptionsTypeDef = TypedDict(
     "SplunkRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
@@ -589,65 +615,41 @@
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "_OptionalStartDeliveryStreamEncryptionInputRequestTypeDef",
     {
-        "DeliveryStreamEncryptionConfigurationInput": DeliveryStreamEncryptionConfigurationInputTypeDef,
+        "DeliveryStreamEncryptionConfigurationInput": (
+            DeliveryStreamEncryptionConfigurationInputTypeDef
+        ),
     },
     total=False,
 )
 
 class StartDeliveryStreamEncryptionInputRequestTypeDef(
     _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef,
     _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
-TagDeliveryStreamInputRequestTypeDef = TypedDict(
-    "TagDeliveryStreamInputRequestTypeDef",
-    {
-        "DeliveryStreamName": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateDeliveryStreamOutputTypeDef = TypedDict(
-    "CreateDeliveryStreamOutputTypeDef",
-    {
-        "DeliveryStreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeliveryStreamsOutputTypeDef = TypedDict(
-    "ListDeliveryStreamsOutputTypeDef",
-    {
-        "DeliveryStreamNames": List[str],
-        "HasMoreDeliveryStreams": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
     "ListTagsForDeliveryStreamOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "HasMoreTags": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutRecordOutputTypeDef = TypedDict(
-    "PutRecordOutputTypeDef",
+TagDeliveryStreamInputRequestTypeDef = TypedDict(
+    "TagDeliveryStreamInputRequestTypeDef",
     {
-        "RecordId": str,
-        "Encrypted": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DeliveryStreamName": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 DeliveryStreamEncryptionConfigurationTypeDef = TypedDict(
     "DeliveryStreamEncryptionConfigurationTypeDef",
     {
         "KeyARN": str,
@@ -746,15 +748,15 @@
 
 PutRecordBatchOutputTypeDef = TypedDict(
     "PutRecordBatchOutputTypeDef",
     {
         "FailedPutCount": int,
         "Encrypted": bool,
         "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputFormatConfigurationTypeDef = TypedDict(
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
@@ -1333,24 +1335,30 @@
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_OptionalCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamType": DeliveryStreamTypeType,
         "KinesisStreamSourceConfiguration": KinesisStreamSourceConfigurationTypeDef,
-        "DeliveryStreamEncryptionConfigurationInput": DeliveryStreamEncryptionConfigurationInputTypeDef,
+        "DeliveryStreamEncryptionConfigurationInput": (
+            DeliveryStreamEncryptionConfigurationInputTypeDef
+        ),
         "S3DestinationConfiguration": S3DestinationConfigurationTypeDef,
         "ExtendedS3DestinationConfiguration": ExtendedS3DestinationConfigurationTypeDef,
         "RedshiftDestinationConfiguration": RedshiftDestinationConfigurationTypeDef,
         "ElasticsearchDestinationConfiguration": ElasticsearchDestinationConfigurationTypeDef,
-        "AmazonopensearchserviceDestinationConfiguration": AmazonopensearchserviceDestinationConfigurationTypeDef,
+        "AmazonopensearchserviceDestinationConfiguration": (
+            AmazonopensearchserviceDestinationConfigurationTypeDef
+        ),
         "SplunkDestinationConfiguration": SplunkDestinationConfigurationTypeDef,
         "HttpEndpointDestinationConfiguration": HttpEndpointDestinationConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
-        "AmazonOpenSearchServerlessDestinationConfiguration": AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
+        "AmazonOpenSearchServerlessDestinationConfiguration": (
+            AmazonOpenSearchServerlessDestinationConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
@@ -1366,18 +1374,22 @@
 _OptionalDestinationDescriptionTypeDef = TypedDict(
     "_OptionalDestinationDescriptionTypeDef",
     {
         "S3DestinationDescription": S3DestinationDescriptionTypeDef,
         "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
         "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
         "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
-        "AmazonopensearchserviceDestinationDescription": AmazonopensearchserviceDestinationDescriptionTypeDef,
+        "AmazonopensearchserviceDestinationDescription": (
+            AmazonopensearchserviceDestinationDescriptionTypeDef
+        ),
         "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
         "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
-        "AmazonOpenSearchServerlessDestinationDescription": AmazonOpenSearchServerlessDestinationDescriptionTypeDef,
+        "AmazonOpenSearchServerlessDestinationDescription": (
+            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
+        ),
     },
     total=False,
 )
 
 class DestinationDescriptionTypeDef(
     _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
 ):
@@ -1397,15 +1409,17 @@
         "S3DestinationUpdate": S3DestinationUpdateTypeDef,
         "ExtendedS3DestinationUpdate": ExtendedS3DestinationUpdateTypeDef,
         "RedshiftDestinationUpdate": RedshiftDestinationUpdateTypeDef,
         "ElasticsearchDestinationUpdate": ElasticsearchDestinationUpdateTypeDef,
         "AmazonopensearchserviceDestinationUpdate": AmazonopensearchserviceDestinationUpdateTypeDef,
         "SplunkDestinationUpdate": SplunkDestinationUpdateTypeDef,
         "HttpEndpointDestinationUpdate": HttpEndpointDestinationUpdateTypeDef,
-        "AmazonOpenSearchServerlessDestinationUpdate": AmazonOpenSearchServerlessDestinationUpdateTypeDef,
+        "AmazonOpenSearchServerlessDestinationUpdate": (
+            AmazonOpenSearchServerlessDestinationUpdateTypeDef
+        ),
     },
     total=False,
 )
 
 class UpdateDestinationInputRequestTypeDef(
     _RequiredUpdateDestinationInputRequestTypeDef, _OptionalUpdateDestinationInputRequestTypeDef
 ):
@@ -1440,10 +1454,10 @@
 ):
     pass
 
 DescribeDeliveryStreamOutputTypeDef = TypedDict(
     "DescribeDeliveryStreamOutputTypeDef",
     {
         "DeliveryStreamDescription": DeliveryStreamDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/PKG-INFO` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.26.19
-Summary: Type annotations for boto3.Firehose 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.Firehose 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
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
 
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,15 +331,15 @@
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
     BufferingHintsTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
     RetryOptionsTypeDef,
@@ -348,30 +349,30 @@
     HttpEndpointBufferingHintsTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
     OrcSerDeTypeDef,
     ParquetSerDeTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
+    PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
+    ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
-    TagDeliveryStreamInputRequestTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamOutputTypeDef,
-    PutRecordOutputTypeDef,
+    TagDeliveryStreamInputRequestTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
     DeserializerTypeDef,
     DynamicPartitioningConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
     SerializerTypeDef,
@@ -422,42 +423,42 @@
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

### Comparing `mypy-boto3-firehose-1.26.19/mypy_boto3_firehose.egg-info/SOURCES.txt` & `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.26.19/setup.py` & `mypy-boto3-firehose-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-firehose.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-firehose",
-    version="1.26.19",
+    version="1.27.0",
     packages=["mypy_boto3_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Firehose 1.26.19 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.Firehose 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 firehose type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_firehose": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_firehose": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/",
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


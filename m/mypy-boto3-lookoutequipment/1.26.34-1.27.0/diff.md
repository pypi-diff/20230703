# Comparing `tmp/mypy-boto3-lookoutequipment-1.26.34.tar.gz` & `tmp/mypy-boto3-lookoutequipment-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutequipment-1.26.34.tar", last modified: Tue Dec 20 20:26:41 2022, max compression
+gzip compressed data, was "mypy-boto3-lookoutequipment-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-lookoutequipment-1.26.34.tar` & `mypy-boto3-lookoutequipment-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.050595 mypy-boto3-lookoutequipment-1.26.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2022-12-20 20:26:41.046595 mypy-boto3-lookoutequipment-1.26.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2022-12-20 20:25:56.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25676 2022-12-20 20:25:56.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2022-12-20 20:25:56.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2022-12-20 20:25:56.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35906 2022-12-20 20:25:56.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35865 2022-12-20 20:25:56.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2022-12-20 20:26:40.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-20 20:26:40.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 20:26:40.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-20 20:26:40.000000 mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 20:26:41.050595 mypy-boto3-lookoutequipment-1.26.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2022-12-20 20:25:55.000000 mypy-boto3-lookoutequipment-1.26.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.671597 mypy-boto3-lookoutequipment-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-07-03 19:51:03.671597 mypy-boto3-lookoutequipment-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.667597 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-07-03 19:41:19.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35915 2023-07-03 19:41:19.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.671597 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-07-03 19:51:03.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-03 19:51:03.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:03.000000 mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.671597 mypy-boto3-lookoutequipment-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 19:41:18.000000 mypy-boto3-lookoutequipment-1.27.0/setup.py
```

### Comparing `mypy-boto3-lookoutequipment-1.26.34/LICENSE` & `mypy-boto3-lookoutequipment-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lookoutequipment-1.26.34/PKG-INFO` & `mypy-boto3-lookoutequipment-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutequipment
-Version: 1.26.34
-Summary: Type annotations for boto3.LookoutEquipment 1.26.34 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LookoutEquipment 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lookoutequipment"></a>
 
 # mypy-boto3-lookoutequipment
 
 [![PyPI - mypy-boto3-lookoutequipment](https://img.shields.io/pypi/v/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutequipment?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,33 +312,40 @@
 
 ```python
 from mypy_boto3_lookoutequipment.type_defs import (
     CategoricalValuesTypeDef,
     CountPercentTypeDef,
     DatasetSchemaTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateInferenceSchedulerResponseTypeDef,
+    CreateLabelGroupResponseTypeDef,
     CreateLabelRequestRequestTypeDef,
+    CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
+    CreateModelResponseTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
     DeleteLabelGroupRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DescribeDataIngestionJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeInferenceSchedulerRequestRequestTypeDef,
     DescribeLabelGroupRequestRequestTypeDef,
+    DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
+    DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
     IngestionS3InputConfigurationTypeDef,
@@ -357,33 +364,26 @@
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
+    ResponseMetadataTypeDef,
+    StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
+    StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
+    StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateInferenceSchedulerResponseTypeDef,
-    CreateLabelGroupResponseTypeDef,
-    CreateLabelResponseTypeDef,
-    CreateModelResponseTypeDef,
-    DescribeLabelGroupResponseTypeDef,
-    DescribeLabelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartDataIngestionJobResponseTypeDef,
-    StartInferenceSchedulerResponseTypeDef,
-    StopInferenceSchedulerResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
     InferenceInputConfigurationTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
     IngestionInputConfigurationTypeDef,
@@ -417,42 +417,42 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.26.34/README.md` & `mypy-boto3-lookoutequipment-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lookoutequipment"></a>
 
 # mypy-boto3-lookoutequipment
 
 [![PyPI - mypy-boto3-lookoutequipment](https://img.shields.io/pypi/v/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutequipment?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,33 +280,40 @@
 
 ```python
 from mypy_boto3_lookoutequipment.type_defs import (
     CategoricalValuesTypeDef,
     CountPercentTypeDef,
     DatasetSchemaTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateInferenceSchedulerResponseTypeDef,
+    CreateLabelGroupResponseTypeDef,
     CreateLabelRequestRequestTypeDef,
+    CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
+    CreateModelResponseTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
     DeleteLabelGroupRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DescribeDataIngestionJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeInferenceSchedulerRequestRequestTypeDef,
     DescribeLabelGroupRequestRequestTypeDef,
+    DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
+    DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
     IngestionS3InputConfigurationTypeDef,
@@ -325,33 +332,26 @@
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
+    ResponseMetadataTypeDef,
+    StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
+    StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
+    StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateInferenceSchedulerResponseTypeDef,
-    CreateLabelGroupResponseTypeDef,
-    CreateLabelResponseTypeDef,
-    CreateModelResponseTypeDef,
-    DescribeLabelGroupResponseTypeDef,
-    DescribeLabelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartDataIngestionJobResponseTypeDef,
-    StartInferenceSchedulerResponseTypeDef,
-    StopInferenceSchedulerResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
     InferenceInputConfigurationTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
     IngestionInputConfigurationTypeDef,
@@ -385,42 +385,42 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/__main__.py` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutEquipment 1.26.34\nVersion:         1.26.34\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.LookoutEquipment 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.34")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/client.py` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/client.pyi` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/literals.py` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
@@ -91,31 +92,34 @@
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
@@ -194,14 +198,15 @@
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
@@ -212,18 +217,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -233,14 +240,15 @@
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
@@ -253,14 +261,15 @@
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
@@ -279,16 +288,19 @@
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
@@ -368,18 +380,21 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/literals.pyi` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
@@ -89,31 +90,34 @@
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
@@ -192,14 +196,15 @@
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
@@ -210,18 +215,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -231,14 +238,15 @@
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
@@ -251,14 +259,15 @@
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
@@ -277,16 +286,19 @@
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
@@ -366,18 +378,21 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/type_defs.py` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,33 +36,40 @@
 
 
 __all__ = (
     "CategoricalValuesTypeDef",
     "CountPercentTypeDef",
     "DatasetSchemaTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateInferenceSchedulerResponseTypeDef",
+    "CreateLabelGroupResponseTypeDef",
     "CreateLabelRequestRequestTypeDef",
+    "CreateLabelResponseTypeDef",
     "DataPreProcessingConfigurationTypeDef",
+    "CreateModelResponseTypeDef",
     "DuplicateTimestampsTypeDef",
     "InvalidSensorDataTypeDef",
     "MissingSensorDataTypeDef",
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
     "DeleteLabelGroupRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DescribeDataIngestionJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeInferenceSchedulerRequestRequestTypeDef",
     "DescribeLabelGroupRequestRequestTypeDef",
+    "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelRequestRequestTypeDef",
+    "DescribeLabelResponseTypeDef",
     "DescribeModelRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
     "IngestionS3InputConfigurationTypeDef",
@@ -81,33 +88,26 @@
     "ListLabelsRequestRequestTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
+    "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
+    "StopInferenceSchedulerResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateInferenceSchedulerResponseTypeDef",
-    "CreateLabelGroupResponseTypeDef",
-    "CreateLabelResponseTypeDef",
-    "CreateModelResponseTypeDef",
-    "DescribeLabelGroupResponseTypeDef",
-    "DescribeLabelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartDataIngestionJobResponseTypeDef",
-    "StartInferenceSchedulerResponseTypeDef",
-    "StopInferenceSchedulerResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
     "InferenceInputConfigurationTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
     "IngestionInputConfigurationTypeDef",
@@ -174,22 +174,40 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Status": DatasetStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateInferenceSchedulerResponseTypeDef = TypedDict(
+    "CreateInferenceSchedulerResponseTypeDef",
+    {
+        "InferenceSchedulerArn": str,
+        "InferenceSchedulerName": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLabelGroupResponseTypeDef = TypedDict(
+    "CreateLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
@@ -212,22 +230,39 @@
 
 class CreateLabelRequestRequestTypeDef(
     _RequiredCreateLabelRequestRequestTypeDef, _OptionalCreateLabelRequestRequestTypeDef
 ):
     pass
 
 
+CreateLabelResponseTypeDef = TypedDict(
+    "CreateLabelResponseTypeDef",
+    {
+        "LabelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataPreProcessingConfigurationTypeDef = TypedDict(
     "DataPreProcessingConfigurationTypeDef",
     {
         "TargetSamplingRate": TargetSamplingRateType,
     },
     total=False,
 )
 
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "Status": ModelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DuplicateTimestampsTypeDef = TypedDict(
     "DuplicateTimestampsTypeDef",
     {
         "TotalNumberOfDuplicateTimestamps": int,
     },
 )
 
@@ -325,29 +360,65 @@
 DescribeLabelGroupRequestRequestTypeDef = TypedDict(
     "DescribeLabelGroupRequestRequestTypeDef",
     {
         "LabelGroupName": str,
     },
 )
 
+DescribeLabelGroupResponseTypeDef = TypedDict(
+    "DescribeLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "FaultCodes": List[str],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLabelRequestRequestTypeDef = TypedDict(
     "DescribeLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
         "LabelId": str,
     },
 )
 
+DescribeLabelResponseTypeDef = TypedDict(
+    "DescribeLabelResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "LabelId": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "Rating": LabelRatingType,
+        "FaultCode": str,
+        "Notes": str,
+        "Equipment": str,
+        "CreatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeModelRequestRequestTypeDef = TypedDict(
     "DescribeModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InferenceEventSummaryTypeDef = TypedDict(
     "InferenceEventSummaryTypeDef",
     {
         "InferenceSchedulerArn": str,
         "InferenceSchedulerName": str,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
@@ -735,28 +806,72 @@
 MultipleOperatingModesTypeDef = TypedDict(
     "MultipleOperatingModesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
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
+StartDataIngestionJobResponseTypeDef = TypedDict(
+    "StartDataIngestionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "Status": IngestionJobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StartInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
+StartInferenceSchedulerResponseTypeDef = TypedDict(
+    "StartInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StopInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
+StopInferenceSchedulerResponseTypeDef = TypedDict(
+    "StopInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -825,160 +940,45 @@
 
 class CreateLabelGroupRequestRequestTypeDef(
     _RequiredCreateLabelGroupRequestRequestTypeDef, _OptionalCreateLabelGroupRequestRequestTypeDef
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Status": DatasetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateInferenceSchedulerResponseTypeDef = TypedDict(
-    "CreateInferenceSchedulerResponseTypeDef",
-    {
-        "InferenceSchedulerArn": str,
-        "InferenceSchedulerName": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLabelGroupResponseTypeDef = TypedDict(
-    "CreateLabelGroupResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLabelResponseTypeDef = TypedDict(
-    "CreateLabelResponseTypeDef",
-    {
-        "LabelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "Status": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLabelGroupResponseTypeDef = TypedDict(
-    "DescribeLabelGroupResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "FaultCodes": List[str],
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLabelResponseTypeDef = TypedDict(
-    "DescribeLabelResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "LabelId": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "Rating": LabelRatingType,
-        "FaultCode": str,
-        "Notes": str,
-        "Equipment": str,
-        "CreatedAt": datetime,
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
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDataIngestionJobResponseTypeDef = TypedDict(
-    "StartDataIngestionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "Status": IngestionJobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartInferenceSchedulerResponseTypeDef = TypedDict(
-    "StartInferenceSchedulerResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopInferenceSchedulerResponseTypeDef = TypedDict(
-    "StopInferenceSchedulerResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "NextToken": str,
         "DatasetSummaries": List[DatasetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInferenceEventsResponseTypeDef = TypedDict(
     "ListInferenceEventsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceEventSummaries": List[InferenceEventSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIngestedFilesSummaryTypeDef = TypedDict(
     "_RequiredIngestedFilesSummaryTypeDef",
     {
         "TotalNumberOfFiles": int,
@@ -1032,15 +1032,15 @@
 
 
 ListInferenceSchedulersResponseTypeDef = TypedDict(
     "ListInferenceSchedulersResponseTypeDef",
     {
         "NextToken": str,
         "InferenceSchedulerSummaries": List[InferenceSchedulerSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IngestionInputConfigurationTypeDef = TypedDict(
     "IngestionInputConfigurationTypeDef",
     {
         "S3InputConfiguration": IngestionS3InputConfigurationTypeDef,
@@ -1056,24 +1056,24 @@
 )
 
 ListLabelGroupsResponseTypeDef = TypedDict(
     "ListLabelGroupsResponseTypeDef",
     {
         "NextToken": str,
         "LabelGroupSummaries": List[LabelGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLabelsResponseTypeDef = TypedDict(
     "ListLabelsResponseTypeDef",
     {
         "NextToken": str,
         "LabelSummaries": List[LabelSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LabelsInputConfigurationTypeDef = TypedDict(
     "LabelsInputConfigurationTypeDef",
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
@@ -1083,15 +1083,15 @@
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SensorStatisticsSummaryTypeDef = TypedDict(
     "SensorStatisticsSummaryTypeDef",
     {
         "ComponentName": str,
@@ -1154,15 +1154,15 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "DataInputConfiguration": InferenceInputConfigurationTypeDef,
         "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
         "RoleArn": str,
         "ServerSideKmsKeyId": str,
         "LatestInferenceResult": LatestInferenceResultType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferenceExecutionSummaryTypeDef = TypedDict(
     "InferenceExecutionSummaryTypeDef",
     {
         "ModelName": str,
@@ -1293,42 +1293,42 @@
         "TrainingExecutionEndTime": datetime,
         "FailedReason": str,
         "ModelMetrics": str,
         "LastUpdatedTime": datetime,
         "CreatedAt": datetime,
         "ServerSideKmsKeyId": str,
         "OffCondition": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInferenceExecutionsResponseTypeDef = TypedDict(
     "ListInferenceExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceExecutionSummaries": List[InferenceExecutionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataIngestionJobsResponseTypeDef = TypedDict(
     "ListDataIngestionJobsResponseTypeDef",
     {
         "NextToken": str,
         "DataIngestionJobSummaries": List[DataIngestionJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataIngestionJobResponseTypeDef = TypedDict(
     "DescribeDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
@@ -1340,15 +1340,15 @@
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
         "IngestedDataSize": int,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetName": str,
@@ -1360,10 +1360,10 @@
         "ServerSideKmsKeyId": str,
         "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment/type_defs.pyi` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,33 +35,40 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "CategoricalValuesTypeDef",
     "CountPercentTypeDef",
     "DatasetSchemaTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateInferenceSchedulerResponseTypeDef",
+    "CreateLabelGroupResponseTypeDef",
     "CreateLabelRequestRequestTypeDef",
+    "CreateLabelResponseTypeDef",
     "DataPreProcessingConfigurationTypeDef",
+    "CreateModelResponseTypeDef",
     "DuplicateTimestampsTypeDef",
     "InvalidSensorDataTypeDef",
     "MissingSensorDataTypeDef",
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
     "DeleteLabelGroupRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DescribeDataIngestionJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeInferenceSchedulerRequestRequestTypeDef",
     "DescribeLabelGroupRequestRequestTypeDef",
+    "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelRequestRequestTypeDef",
+    "DescribeLabelResponseTypeDef",
     "DescribeModelRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
     "IngestionS3InputConfigurationTypeDef",
@@ -80,33 +87,26 @@
     "ListLabelsRequestRequestTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
+    "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
+    "StopInferenceSchedulerResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateInferenceSchedulerResponseTypeDef",
-    "CreateLabelGroupResponseTypeDef",
-    "CreateLabelResponseTypeDef",
-    "CreateModelResponseTypeDef",
-    "DescribeLabelGroupResponseTypeDef",
-    "DescribeLabelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartDataIngestionJobResponseTypeDef",
-    "StartInferenceSchedulerResponseTypeDef",
-    "StopInferenceSchedulerResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
     "InferenceInputConfigurationTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
     "IngestionInputConfigurationTypeDef",
@@ -171,22 +171,40 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Status": DatasetStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateInferenceSchedulerResponseTypeDef = TypedDict(
+    "CreateInferenceSchedulerResponseTypeDef",
+    {
+        "InferenceSchedulerArn": str,
+        "InferenceSchedulerName": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLabelGroupResponseTypeDef = TypedDict(
+    "CreateLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
@@ -207,22 +225,39 @@
 )
 
 class CreateLabelRequestRequestTypeDef(
     _RequiredCreateLabelRequestRequestTypeDef, _OptionalCreateLabelRequestRequestTypeDef
 ):
     pass
 
+CreateLabelResponseTypeDef = TypedDict(
+    "CreateLabelResponseTypeDef",
+    {
+        "LabelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataPreProcessingConfigurationTypeDef = TypedDict(
     "DataPreProcessingConfigurationTypeDef",
     {
         "TargetSamplingRate": TargetSamplingRateType,
     },
     total=False,
 )
 
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "Status": ModelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DuplicateTimestampsTypeDef = TypedDict(
     "DuplicateTimestampsTypeDef",
     {
         "TotalNumberOfDuplicateTimestamps": int,
     },
 )
 
@@ -320,29 +355,65 @@
 DescribeLabelGroupRequestRequestTypeDef = TypedDict(
     "DescribeLabelGroupRequestRequestTypeDef",
     {
         "LabelGroupName": str,
     },
 )
 
+DescribeLabelGroupResponseTypeDef = TypedDict(
+    "DescribeLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "FaultCodes": List[str],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLabelRequestRequestTypeDef = TypedDict(
     "DescribeLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
         "LabelId": str,
     },
 )
 
+DescribeLabelResponseTypeDef = TypedDict(
+    "DescribeLabelResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "LabelId": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "Rating": LabelRatingType,
+        "FaultCode": str,
+        "Notes": str,
+        "Equipment": str,
+        "CreatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeModelRequestRequestTypeDef = TypedDict(
     "DescribeModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InferenceEventSummaryTypeDef = TypedDict(
     "InferenceEventSummaryTypeDef",
     {
         "InferenceSchedulerArn": str,
         "InferenceSchedulerName": str,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
@@ -710,28 +781,72 @@
 MultipleOperatingModesTypeDef = TypedDict(
     "MultipleOperatingModesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
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
+StartDataIngestionJobResponseTypeDef = TypedDict(
+    "StartDataIngestionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "Status": IngestionJobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StartInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
+StartInferenceSchedulerResponseTypeDef = TypedDict(
+    "StartInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StopInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
+StopInferenceSchedulerResponseTypeDef = TypedDict(
+    "StopInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -794,160 +909,45 @@
 )
 
 class CreateLabelGroupRequestRequestTypeDef(
     _RequiredCreateLabelGroupRequestRequestTypeDef, _OptionalCreateLabelGroupRequestRequestTypeDef
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Status": DatasetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateInferenceSchedulerResponseTypeDef = TypedDict(
-    "CreateInferenceSchedulerResponseTypeDef",
-    {
-        "InferenceSchedulerArn": str,
-        "InferenceSchedulerName": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLabelGroupResponseTypeDef = TypedDict(
-    "CreateLabelGroupResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLabelResponseTypeDef = TypedDict(
-    "CreateLabelResponseTypeDef",
-    {
-        "LabelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "Status": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLabelGroupResponseTypeDef = TypedDict(
-    "DescribeLabelGroupResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "FaultCodes": List[str],
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLabelResponseTypeDef = TypedDict(
-    "DescribeLabelResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "LabelId": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "Rating": LabelRatingType,
-        "FaultCode": str,
-        "Notes": str,
-        "Equipment": str,
-        "CreatedAt": datetime,
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
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDataIngestionJobResponseTypeDef = TypedDict(
-    "StartDataIngestionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "Status": IngestionJobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartInferenceSchedulerResponseTypeDef = TypedDict(
-    "StartInferenceSchedulerResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopInferenceSchedulerResponseTypeDef = TypedDict(
-    "StopInferenceSchedulerResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "NextToken": str,
         "DatasetSummaries": List[DatasetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInferenceEventsResponseTypeDef = TypedDict(
     "ListInferenceEventsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceEventSummaries": List[InferenceEventSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIngestedFilesSummaryTypeDef = TypedDict(
     "_RequiredIngestedFilesSummaryTypeDef",
     {
         "TotalNumberOfFiles": int,
@@ -997,15 +997,15 @@
     pass
 
 ListInferenceSchedulersResponseTypeDef = TypedDict(
     "ListInferenceSchedulersResponseTypeDef",
     {
         "NextToken": str,
         "InferenceSchedulerSummaries": List[InferenceSchedulerSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IngestionInputConfigurationTypeDef = TypedDict(
     "IngestionInputConfigurationTypeDef",
     {
         "S3InputConfiguration": IngestionS3InputConfigurationTypeDef,
@@ -1021,24 +1021,24 @@
 )
 
 ListLabelGroupsResponseTypeDef = TypedDict(
     "ListLabelGroupsResponseTypeDef",
     {
         "NextToken": str,
         "LabelGroupSummaries": List[LabelGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLabelsResponseTypeDef = TypedDict(
     "ListLabelsResponseTypeDef",
     {
         "NextToken": str,
         "LabelSummaries": List[LabelSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LabelsInputConfigurationTypeDef = TypedDict(
     "LabelsInputConfigurationTypeDef",
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
@@ -1048,15 +1048,15 @@
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SensorStatisticsSummaryTypeDef = TypedDict(
     "SensorStatisticsSummaryTypeDef",
     {
         "ComponentName": str,
@@ -1117,15 +1117,15 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "DataInputConfiguration": InferenceInputConfigurationTypeDef,
         "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
         "RoleArn": str,
         "ServerSideKmsKeyId": str,
         "LatestInferenceResult": LatestInferenceResultType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferenceExecutionSummaryTypeDef = TypedDict(
     "InferenceExecutionSummaryTypeDef",
     {
         "ModelName": str,
@@ -1252,42 +1252,42 @@
         "TrainingExecutionEndTime": datetime,
         "FailedReason": str,
         "ModelMetrics": str,
         "LastUpdatedTime": datetime,
         "CreatedAt": datetime,
         "ServerSideKmsKeyId": str,
         "OffCondition": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInferenceExecutionsResponseTypeDef = TypedDict(
     "ListInferenceExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceExecutionSummaries": List[InferenceExecutionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataIngestionJobsResponseTypeDef = TypedDict(
     "ListDataIngestionJobsResponseTypeDef",
     {
         "NextToken": str,
         "DataIngestionJobSummaries": List[DataIngestionJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataIngestionJobResponseTypeDef = TypedDict(
     "DescribeDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
@@ -1299,15 +1299,15 @@
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
         "IngestedDataSize": int,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetName": str,
@@ -1319,10 +1319,10 @@
         "ServerSideKmsKeyId": str,
         "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/PKG-INFO` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutequipment
-Version: 1.26.34
-Summary: Type annotations for boto3.LookoutEquipment 1.26.34 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LookoutEquipment 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lookoutequipment"></a>
 
 # mypy-boto3-lookoutequipment
 
 [![PyPI - mypy-boto3-lookoutequipment](https://img.shields.io/pypi/v/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutequipment?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,33 +312,40 @@
 
 ```python
 from mypy_boto3_lookoutequipment.type_defs import (
     CategoricalValuesTypeDef,
     CountPercentTypeDef,
     DatasetSchemaTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateInferenceSchedulerResponseTypeDef,
+    CreateLabelGroupResponseTypeDef,
     CreateLabelRequestRequestTypeDef,
+    CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
+    CreateModelResponseTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
     DeleteLabelGroupRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DescribeDataIngestionJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeInferenceSchedulerRequestRequestTypeDef,
     DescribeLabelGroupRequestRequestTypeDef,
+    DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
+    DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
     IngestionS3InputConfigurationTypeDef,
@@ -357,33 +364,26 @@
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
+    ResponseMetadataTypeDef,
+    StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
+    StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
+    StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateInferenceSchedulerResponseTypeDef,
-    CreateLabelGroupResponseTypeDef,
-    CreateLabelResponseTypeDef,
-    CreateModelResponseTypeDef,
-    DescribeLabelGroupResponseTypeDef,
-    DescribeLabelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartDataIngestionJobResponseTypeDef,
-    StartInferenceSchedulerResponseTypeDef,
-    StopInferenceSchedulerResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
     InferenceInputConfigurationTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
     IngestionInputConfigurationTypeDef,
@@ -417,42 +417,42 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.26.34/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt` & `mypy-boto3-lookoutequipment-1.27.0/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.26.34/setup.py` & `mypy-boto3-lookoutequipment-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-lookoutequipment.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutequipment",
-    version="1.26.34",
+    version="1.27.0",
     packages=["mypy_boto3_lookoutequipment"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutEquipment 1.26.34 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.LookoutEquipment 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/",
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


# Comparing `tmp/mypy-boto3-frauddetector-1.26.72.tar.gz` & `tmp/mypy-boto3-frauddetector-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-frauddetector-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
+gzip compressed data, was "mypy-boto3-frauddetector-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
```

## Comparing `mypy-boto3-frauddetector-1.26.72.tar` & `mypy-boto3-frauddetector-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-02-15 22:27:08.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46164 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-02-15 22:27:08.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-02-15 22:27:08.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59063 2023-02-15 22:27:10.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58996 2023-02-15 22:27:09.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.887277 mypy-boto3-frauddetector-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-07-03 19:50:47.887277 mypy-boto3-frauddetector-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17364 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.887277 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46336 2023-07-03 19:37:59.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-03 19:38:00.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-03 19:37:59.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59398 2023-07-03 19:38:01.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59331 2023-07-03 19:38:00.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.887277 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-07-03 19:50:47.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 19:50:47.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:47.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:50:47.000000 mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.887277 mypy-boto3-frauddetector-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:37:58.000000 mypy-boto3-frauddetector-1.27.0/setup.py
```

### Comparing `mypy-boto3-frauddetector-1.26.72/LICENSE` & `mypy-boto3-frauddetector-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-frauddetector-1.26.72/PKG-INFO` & `mypy-boto3-frauddetector-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.26.72
-Summary: Type annotations for boto3.FraudDetector 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.FraudDetector 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-frauddetector"></a>
 
 # mypy-boto3-frauddetector
 
 [![PyPI - mypy-boto3-frauddetector](https://img.shields.io/pypi/v/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,35 +320,37 @@
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
     AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
+    CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
+    CreateModelVersionResultTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
+    DeleteEventsByEventTypeResultTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
@@ -356,37 +358,40 @@
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
+    EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
     ExternalModelSummaryTypeDef,
     ModelInputConfigurationTypeDef,
     ModelOutputConfigurationTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
+    GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
     GetListElementsRequestRequestTypeDef,
+    GetListElementsResultTypeDef,
     GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
@@ -398,47 +403,42 @@
     ListTagsForResourceRequestRequestTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
     UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
+    UpdateModelVersionResultTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
+    GetListsMetadataResultTypeDef,
+    BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
-    PutEventTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
-    BatchCreateVariableResultTypeDef,
-    CreateDetectorVersionResultTypeDef,
-    CreateModelVersionResultTypeDef,
-    DeleteEventsByEventTypeResultTypeDef,
-    GetDeleteEventsByEventTypeStatusResultTypeDef,
-    GetListElementsResultTypeDef,
-    GetListsMetadataResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
     CreateRuleResultTypeDef,
@@ -450,14 +450,15 @@
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
+    PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
     PutExternalModelRequestRequestTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
@@ -500,42 +501,42 @@
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

### Comparing `mypy-boto3-frauddetector-1.26.72/README.md` & `mypy-boto3-frauddetector-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-frauddetector"></a>
 
 # mypy-boto3-frauddetector
 
 [![PyPI - mypy-boto3-frauddetector](https://img.shields.io/pypi/v/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,35 +288,37 @@
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
     AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
+    CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
+    CreateModelVersionResultTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
+    DeleteEventsByEventTypeResultTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
@@ -324,37 +326,40 @@
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
+    EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
     ExternalModelSummaryTypeDef,
     ModelInputConfigurationTypeDef,
     ModelOutputConfigurationTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
+    GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
     GetListElementsRequestRequestTypeDef,
+    GetListElementsResultTypeDef,
     GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
@@ -366,47 +371,42 @@
     ListTagsForResourceRequestRequestTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
     UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
+    UpdateModelVersionResultTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
+    GetListsMetadataResultTypeDef,
+    BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
-    PutEventTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
-    BatchCreateVariableResultTypeDef,
-    CreateDetectorVersionResultTypeDef,
-    CreateModelVersionResultTypeDef,
-    DeleteEventsByEventTypeResultTypeDef,
-    GetDeleteEventsByEventTypeStatusResultTypeDef,
-    GetListElementsResultTypeDef,
-    GetListsMetadataResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
     CreateRuleResultTypeDef,
@@ -418,14 +418,15 @@
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
+    PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
     PutExternalModelRequestRequestTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
@@ -468,42 +469,42 @@
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

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__main__.py` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FraudDetector 1.26.72\nVersion:         1.26.72\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.FraudDetector 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.72")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.py` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     CreateDetectorVersionResultTypeDef,
     CreateModelVersionResultTypeDef,
     CreateRuleResultTypeDef,
     DeleteEventsByEventTypeResultTypeDef,
     DescribeDetectorResultTypeDef,
     DescribeModelVersionsResultTypeDef,
     EntityTypeDef,
+    EventOrchestrationTypeDef,
     ExternalEventsDetailTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorsResultTypeDef,
     GetDetectorVersionResultTypeDef,
@@ -79,37 +80,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FraudDetectorClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class FraudDetectorClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/)
     """
 
     meta: ClientMeta
@@ -118,65 +115,58 @@
     def exceptions(self) -> Exceptions:
         """
         FraudDetectorClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#exceptions)
         """
-
     def batch_create_variable(
         self, *, variableEntries: Sequence[VariableEntryTypeDef], tags: Sequence[TagTypeDef] = ...
     ) -> BatchCreateVariableResultTypeDef:
         """
         Creates a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_create_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#batch_create_variable)
         """
-
     def batch_get_variable(self, *, names: Sequence[str]) -> BatchGetVariableResultTypeDef:
         """
         Gets a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_get_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#batch_get_variable)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#can_paginate)
         """
-
     def cancel_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels an in-progress batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#cancel_batch_import_job)
         """
-
     def cancel_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels the specified batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_prediction_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#cancel_batch_prediction_job)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#close)
         """
-
     def create_batch_import_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -185,15 +175,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_batch_import_job)
         """
-
     def create_batch_prediction_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -204,15 +193,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_prediction_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_batch_prediction_job)
         """
-
     def create_detector_version(
         self,
         *,
         detectorId: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         externalModelEndpoints: Sequence[str] = ...,
@@ -222,15 +210,14 @@
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_detector_version)
         """
-
     def create_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         variableType: str = ...,
         description: str = ...,
@@ -238,15 +225,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_list)
         """
-
     def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
@@ -254,15 +240,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a model using the specified model type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_model)
         """
-
     def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
         trainingDataSchema: TrainingDataSchemaTypeDef,
@@ -272,15 +257,14 @@
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_model_version)
         """
-
     def create_rule(
         self,
         *,
         ruleId: str,
         detectorId: str,
         expression: str,
         language: Literal["DETECTORPL"],
@@ -290,15 +274,14 @@
     ) -> CreateRuleResultTypeDef:
         """
         Creates a rule for use with the specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_rule)
         """
-
     def create_variable(
         self,
         *,
         name: str,
         dataType: DataTypeType,
         dataSource: DataSourceType,
         defaultValue: str,
@@ -308,159 +291,141 @@
     ) -> Dict[str, Any]:
         """
         Creates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_variable)
         """
-
     def delete_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes the specified batch import job ID record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_batch_import_job)
         """
-
     def delete_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_prediction_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_batch_prediction_job)
         """
-
     def delete_detector(self, *, detectorId: str) -> Dict[str, Any]:
         """
         Deletes the detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_detector)
         """
-
     def delete_detector_version(self, *, detectorId: str, detectorVersionId: str) -> Dict[str, Any]:
         """
         Deletes the detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_detector_version)
         """
-
     def delete_entity_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_entity_type)
         """
-
     def delete_event(
         self, *, eventId: str, eventTypeName: str, deleteAuditHistory: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_event)
         """
-
     def delete_event_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_event_type)
         """
-
     def delete_events_by_event_type(
         self, *, eventTypeName: str
     ) -> DeleteEventsByEventTypeResultTypeDef:
         """
         Deletes all events of a particular event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_events_by_event_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_events_by_event_type)
         """
-
     def delete_external_model(self, *, modelEndpoint: str) -> Dict[str, Any]:
         """
         Removes a SageMaker model from Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_external_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_external_model)
         """
-
     def delete_label(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_label)
         """
-
     def delete_list(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes the list, provided it is not used in a rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_list)
         """
-
     def delete_model(self, *, modelId: str, modelType: ModelTypeEnumType) -> Dict[str, Any]:
         """
         Deletes a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_model)
         """
-
     def delete_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> Dict[str, Any]:
         """
         Deletes a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_model_version)
         """
-
     def delete_outcome(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_outcome)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_outcome)
         """
-
     def delete_rule(self, *, rule: RuleTypeDef) -> Dict[str, Any]:
         """
         Deletes the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_rule)
         """
-
     def delete_variable(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_variable)
         """
-
     def describe_detector(
         self, *, detectorId: str, nextToken: str = ..., maxResults: int = ...
     ) -> DescribeDetectorResultTypeDef:
         """
         Gets all versions for a specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#describe_detector)
         """
-
     def describe_model_versions(
         self,
         *,
         modelId: str = ...,
         modelVersionNumber: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
@@ -469,97 +434,88 @@
         """
         Gets all of the model versions for the specified model type or for the specified
         model type and model ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_model_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#describe_model_versions)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#generate_presigned_url)
         """
-
     def get_batch_import_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchImportJobsResultTypeDef:
         """
         Gets all batch import jobs or a specific job of the specified ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_batch_import_jobs)
         """
-
     def get_batch_prediction_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchPredictionJobsResultTypeDef:
         """
         Gets all batch prediction jobs or a specific job if you specify a job ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_prediction_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_batch_prediction_jobs)
         """
-
     def get_delete_events_by_event_type_status(
         self, *, eventTypeName: str
     ) -> GetDeleteEventsByEventTypeStatusResultTypeDef:
         """
         Retrieves the status of a `DeleteEventsByEventType` action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_delete_events_by_event_type_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_delete_events_by_event_type_status)
         """
-
     def get_detector_version(
         self, *, detectorId: str, detectorVersionId: str
     ) -> GetDetectorVersionResultTypeDef:
         """
         Gets a particular detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_detector_version)
         """
-
     def get_detectors(
         self, *, detectorId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetDetectorsResultTypeDef:
         """
         Gets all detectors or a single detector if a `detectorId` is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_detectors)
         """
-
     def get_entity_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEntityTypesResultTypeDef:
         """
         Gets all entity types or a specific entity type if a name is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_entity_types)
         """
-
     def get_event(self, *, eventId: str, eventTypeName: str) -> GetEventResultTypeDef:
         """
         Retrieves details of events stored with Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event)
         """
-
     def get_event_prediction(
         self,
         *,
         detectorId: str,
         eventId: str,
         eventTypeName: str,
         entities: Sequence[EntityTypeDef],
@@ -570,15 +526,14 @@
     ) -> GetEventPredictionResultTypeDef:
         """
         Evaluates an event against a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event_prediction)
         """
-
     def get_event_prediction_metadata(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         detectorId: str,
         detectorVersionId: str,
@@ -588,111 +543,101 @@
         Gets details of the past fraud predictions for the specified event ID, event
         type, detector ID, and detector version ID that was generated in the specified
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event_prediction_metadata)
         """
-
     def get_event_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEventTypesResultTypeDef:
         """
         Gets all event types or a specific event type if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event_types)
         """
-
     def get_external_models(
         self, *, modelEndpoint: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetExternalModelsResultTypeDef:
         """
         Gets the details for one or more Amazon SageMaker models that have been imported
         into the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_external_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_external_models)
         """
-
     def get_kms_encryption_key(self) -> GetKMSEncryptionKeyResultTypeDef:
         """
         Gets the encryption key if a KMS key has been specified to be used to encrypt
         content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_kms_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_kms_encryption_key)
         """
-
     def get_labels(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetLabelsResultTypeDef:
         """
         Gets all labels or a specific label if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_labels)
         """
-
     def get_list_elements(
         self, *, name: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetListElementsResultTypeDef:
         """
         Gets all the elements in the specified list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_list_elements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_list_elements)
         """
-
     def get_lists_metadata(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetListsMetadataResultTypeDef:
         """
         Gets the metadata of either all the lists under the account or the specified
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_lists_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_lists_metadata)
         """
-
     def get_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> GetModelVersionResultTypeDef:
         """
         Gets the details of the specified model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_model_version)
         """
-
     def get_models(
         self,
         *,
         modelId: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetModelsResultTypeDef:
         """
         Gets one or more models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_models)
         """
-
     def get_outcomes(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetOutcomesResultTypeDef:
         """
         Gets one or more outcomes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_outcomes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_outcomes)
         """
-
     def get_rules(
         self,
         *,
         detectorId: str,
         ruleId: str = ...,
         ruleVersion: str = ...,
         nextToken: str = ...,
@@ -701,25 +646,23 @@
         """
         Get all rules for a detector (paginated) if `ruleId` and `ruleVersion` are not
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_rules)
         """
-
     def get_variables(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetVariablesResultTypeDef:
         """
         Gets all of the variables or the specific variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_variables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_variables)
         """
-
     def list_event_predictions(
         self,
         *,
         eventId: FilterConditionTypeDef = ...,
         eventType: FilterConditionTypeDef = ...,
         detectorId: FilterConditionTypeDef = ...,
         detectorVersionId: FilterConditionTypeDef = ...,
@@ -729,68 +672,64 @@
     ) -> ListEventPredictionsResultTypeDef:
         """
         Gets a list of past predictions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_event_predictions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#list_event_predictions)
         """
-
     def list_tags_for_resource(
         self, *, resourceARN: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListTagsForResourceResultTypeDef:
         """
         Lists all tags associated with the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#list_tags_for_resource)
         """
-
     def put_detector(
         self,
         *,
         detectorId: str,
         eventTypeName: str,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_detector)
         """
-
     def put_entity_type(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_entity_type)
         """
-
     def put_event_type(
         self,
         *,
         name: str,
         eventVariables: Sequence[str],
         entityTypes: Sequence[str],
         description: str = ...,
         labels: Sequence[str] = ...,
         eventIngestion: EventIngestionType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
+        eventOrchestration: EventOrchestrationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_event_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_event_type)
         """
-
     def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
@@ -800,43 +739,39 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_external_model)
         """
-
     def put_kms_encryption_key(self, *, kmsEncryptionKeyArn: str) -> Dict[str, Any]:
         """
         Specifies the KMS key to be used to encrypt content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_kms_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_kms_encryption_key)
         """
-
     def put_label(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_label)
         """
-
     def put_outcome(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_outcome)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_outcome)
         """
-
     def send_event(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
@@ -847,31 +782,28 @@
         """
         Stores events in Amazon Fraud Detector without generating fraud predictions for
         those events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.send_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#send_event)
         """
-
     def tag_resource(self, *, resourceARN: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Assigns tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#untag_resource)
         """
-
     def update_detector_version(
         self,
         *,
         detectorId: str,
         detectorVersionId: str,
         externalModelEndpoints: Sequence[str],
         rules: Sequence[RuleTypeDef],
@@ -881,45 +813,41 @@
     ) -> Dict[str, Any]:
         """
         Updates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_detector_version)
         """
-
     def update_detector_version_metadata(
         self, *, detectorId: str, detectorVersionId: str, description: str
     ) -> Dict[str, Any]:
         """
         Updates the detector version's description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_detector_version_metadata)
         """
-
     def update_detector_version_status(
         self, *, detectorId: str, detectorVersionId: str, status: DetectorVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the detector version’s status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_detector_version_status)
         """
-
     def update_event_label(
         self, *, eventId: str, eventTypeName: str, assignedLabel: str, labelTimestamp: str
     ) -> Dict[str, Any]:
         """
         Updates the specified event with a new label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_event_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_event_label)
         """
-
     def update_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         description: str = ...,
         updateMode: ListUpdateModeType = ...,
@@ -927,25 +855,23 @@
     ) -> Dict[str, Any]:
         """
         Updates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_list)
         """
-
     def update_model(
         self, *, modelId: str, modelType: ModelTypeEnumType, description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates model description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_model)
         """
-
     def update_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         majorVersionNumber: str,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
@@ -954,38 +880,35 @@
     ) -> UpdateModelVersionResultTypeDef:
         """
         Updates a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_model_version)
         """
-
     def update_model_version_status(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         modelVersionNumber: str,
         status: ModelVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the status of a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_model_version_status)
         """
-
     def update_rule_metadata(self, *, rule: RuleTypeDef, description: str) -> Dict[str, Any]:
         """
         Updates a rule's metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_rule_metadata)
         """
-
     def update_rule_version(
         self,
         *,
         rule: RuleTypeDef,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
@@ -994,15 +917,14 @@
     ) -> UpdateRuleVersionResultTypeDef:
         """
         Updates a rule version resulting in a new rule version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_rule_version)
         """
-
     def update_variable(
         self, *, name: str, defaultValue: str = ..., description: str = ..., variableType: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_variable)
```

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.pyi` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     CreateDetectorVersionResultTypeDef,
     CreateModelVersionResultTypeDef,
     CreateRuleResultTypeDef,
     DeleteEventsByEventTypeResultTypeDef,
     DescribeDetectorResultTypeDef,
     DescribeModelVersionsResultTypeDef,
     EntityTypeDef,
+    EventOrchestrationTypeDef,
     ExternalEventsDetailTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorsResultTypeDef,
     GetDetectorVersionResultTypeDef,
@@ -79,33 +80,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("FraudDetectorClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class FraudDetectorClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/)
     """
 
     meta: ClientMeta
@@ -114,58 +119,65 @@
     def exceptions(self) -> Exceptions:
         """
         FraudDetectorClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#exceptions)
         """
+
     def batch_create_variable(
         self, *, variableEntries: Sequence[VariableEntryTypeDef], tags: Sequence[TagTypeDef] = ...
     ) -> BatchCreateVariableResultTypeDef:
         """
         Creates a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_create_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#batch_create_variable)
         """
+
     def batch_get_variable(self, *, names: Sequence[str]) -> BatchGetVariableResultTypeDef:
         """
         Gets a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_get_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#batch_get_variable)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#can_paginate)
         """
+
     def cancel_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels an in-progress batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#cancel_batch_import_job)
         """
+
     def cancel_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels the specified batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_prediction_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#cancel_batch_prediction_job)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#close)
         """
+
     def create_batch_import_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -174,14 +186,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_batch_import_job)
         """
+
     def create_batch_prediction_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -192,14 +205,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_prediction_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_batch_prediction_job)
         """
+
     def create_detector_version(
         self,
         *,
         detectorId: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         externalModelEndpoints: Sequence[str] = ...,
@@ -209,14 +223,15 @@
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_detector_version)
         """
+
     def create_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         variableType: str = ...,
         description: str = ...,
@@ -224,14 +239,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_list)
         """
+
     def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
@@ -239,14 +255,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a model using the specified model type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_model)
         """
+
     def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
         trainingDataSchema: TrainingDataSchemaTypeDef,
@@ -256,14 +273,15 @@
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_model_version)
         """
+
     def create_rule(
         self,
         *,
         ruleId: str,
         detectorId: str,
         expression: str,
         language: Literal["DETECTORPL"],
@@ -273,14 +291,15 @@
     ) -> CreateRuleResultTypeDef:
         """
         Creates a rule for use with the specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_rule)
         """
+
     def create_variable(
         self,
         *,
         name: str,
         dataType: DataTypeType,
         dataSource: DataSourceType,
         defaultValue: str,
@@ -290,141 +309,159 @@
     ) -> Dict[str, Any]:
         """
         Creates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_variable)
         """
+
     def delete_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes the specified batch import job ID record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_batch_import_job)
         """
+
     def delete_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_prediction_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_batch_prediction_job)
         """
+
     def delete_detector(self, *, detectorId: str) -> Dict[str, Any]:
         """
         Deletes the detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_detector)
         """
+
     def delete_detector_version(self, *, detectorId: str, detectorVersionId: str) -> Dict[str, Any]:
         """
         Deletes the detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_detector_version)
         """
+
     def delete_entity_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_entity_type)
         """
+
     def delete_event(
         self, *, eventId: str, eventTypeName: str, deleteAuditHistory: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_event)
         """
+
     def delete_event_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_event_type)
         """
+
     def delete_events_by_event_type(
         self, *, eventTypeName: str
     ) -> DeleteEventsByEventTypeResultTypeDef:
         """
         Deletes all events of a particular event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_events_by_event_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_events_by_event_type)
         """
+
     def delete_external_model(self, *, modelEndpoint: str) -> Dict[str, Any]:
         """
         Removes a SageMaker model from Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_external_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_external_model)
         """
+
     def delete_label(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_label)
         """
+
     def delete_list(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes the list, provided it is not used in a rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_list)
         """
+
     def delete_model(self, *, modelId: str, modelType: ModelTypeEnumType) -> Dict[str, Any]:
         """
         Deletes a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_model)
         """
+
     def delete_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> Dict[str, Any]:
         """
         Deletes a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_model_version)
         """
+
     def delete_outcome(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_outcome)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_outcome)
         """
+
     def delete_rule(self, *, rule: RuleTypeDef) -> Dict[str, Any]:
         """
         Deletes the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_rule)
         """
+
     def delete_variable(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_variable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_variable)
         """
+
     def describe_detector(
         self, *, detectorId: str, nextToken: str = ..., maxResults: int = ...
     ) -> DescribeDetectorResultTypeDef:
         """
         Gets all versions for a specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#describe_detector)
         """
+
     def describe_model_versions(
         self,
         *,
         modelId: str = ...,
         modelVersionNumber: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
@@ -433,88 +470,97 @@
         """
         Gets all of the model versions for the specified model type or for the specified
         model type and model ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_model_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#describe_model_versions)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#generate_presigned_url)
         """
+
     def get_batch_import_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchImportJobsResultTypeDef:
         """
         Gets all batch import jobs or a specific job of the specified ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_batch_import_jobs)
         """
+
     def get_batch_prediction_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchPredictionJobsResultTypeDef:
         """
         Gets all batch prediction jobs or a specific job if you specify a job ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_prediction_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_batch_prediction_jobs)
         """
+
     def get_delete_events_by_event_type_status(
         self, *, eventTypeName: str
     ) -> GetDeleteEventsByEventTypeStatusResultTypeDef:
         """
         Retrieves the status of a `DeleteEventsByEventType` action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_delete_events_by_event_type_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_delete_events_by_event_type_status)
         """
+
     def get_detector_version(
         self, *, detectorId: str, detectorVersionId: str
     ) -> GetDetectorVersionResultTypeDef:
         """
         Gets a particular detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_detector_version)
         """
+
     def get_detectors(
         self, *, detectorId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetDetectorsResultTypeDef:
         """
         Gets all detectors or a single detector if a `detectorId` is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_detectors)
         """
+
     def get_entity_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEntityTypesResultTypeDef:
         """
         Gets all entity types or a specific entity type if a name is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_entity_types)
         """
+
     def get_event(self, *, eventId: str, eventTypeName: str) -> GetEventResultTypeDef:
         """
         Retrieves details of events stored with Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event)
         """
+
     def get_event_prediction(
         self,
         *,
         detectorId: str,
         eventId: str,
         eventTypeName: str,
         entities: Sequence[EntityTypeDef],
@@ -525,14 +571,15 @@
     ) -> GetEventPredictionResultTypeDef:
         """
         Evaluates an event against a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event_prediction)
         """
+
     def get_event_prediction_metadata(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         detectorId: str,
         detectorVersionId: str,
@@ -542,101 +589,111 @@
         Gets details of the past fraud predictions for the specified event ID, event
         type, detector ID, and detector version ID that was generated in the specified
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event_prediction_metadata)
         """
+
     def get_event_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEventTypesResultTypeDef:
         """
         Gets all event types or a specific event type if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_event_types)
         """
+
     def get_external_models(
         self, *, modelEndpoint: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetExternalModelsResultTypeDef:
         """
         Gets the details for one or more Amazon SageMaker models that have been imported
         into the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_external_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_external_models)
         """
+
     def get_kms_encryption_key(self) -> GetKMSEncryptionKeyResultTypeDef:
         """
         Gets the encryption key if a KMS key has been specified to be used to encrypt
         content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_kms_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_kms_encryption_key)
         """
+
     def get_labels(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetLabelsResultTypeDef:
         """
         Gets all labels or a specific label if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_labels)
         """
+
     def get_list_elements(
         self, *, name: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetListElementsResultTypeDef:
         """
         Gets all the elements in the specified list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_list_elements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_list_elements)
         """
+
     def get_lists_metadata(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetListsMetadataResultTypeDef:
         """
         Gets the metadata of either all the lists under the account or the specified
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_lists_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_lists_metadata)
         """
+
     def get_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> GetModelVersionResultTypeDef:
         """
         Gets the details of the specified model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_model_version)
         """
+
     def get_models(
         self,
         *,
         modelId: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetModelsResultTypeDef:
         """
         Gets one or more models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_models)
         """
+
     def get_outcomes(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetOutcomesResultTypeDef:
         """
         Gets one or more outcomes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_outcomes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_outcomes)
         """
+
     def get_rules(
         self,
         *,
         detectorId: str,
         ruleId: str = ...,
         ruleVersion: str = ...,
         nextToken: str = ...,
@@ -645,23 +702,25 @@
         """
         Get all rules for a detector (paginated) if `ruleId` and `ruleVersion` are not
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_rules)
         """
+
     def get_variables(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetVariablesResultTypeDef:
         """
         Gets all of the variables or the specific variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_variables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_variables)
         """
+
     def list_event_predictions(
         self,
         *,
         eventId: FilterConditionTypeDef = ...,
         eventType: FilterConditionTypeDef = ...,
         detectorId: FilterConditionTypeDef = ...,
         detectorVersionId: FilterConditionTypeDef = ...,
@@ -671,63 +730,69 @@
     ) -> ListEventPredictionsResultTypeDef:
         """
         Gets a list of past predictions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_event_predictions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#list_event_predictions)
         """
+
     def list_tags_for_resource(
         self, *, resourceARN: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListTagsForResourceResultTypeDef:
         """
         Lists all tags associated with the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#list_tags_for_resource)
         """
+
     def put_detector(
         self,
         *,
         detectorId: str,
         eventTypeName: str,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_detector)
         """
+
     def put_entity_type(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_entity_type)
         """
+
     def put_event_type(
         self,
         *,
         name: str,
         eventVariables: Sequence[str],
         entityTypes: Sequence[str],
         description: str = ...,
         labels: Sequence[str] = ...,
         eventIngestion: EventIngestionType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
+        eventOrchestration: EventOrchestrationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_event_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_event_type)
         """
+
     def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
@@ -737,39 +802,43 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_external_model)
         """
+
     def put_kms_encryption_key(self, *, kmsEncryptionKeyArn: str) -> Dict[str, Any]:
         """
         Specifies the KMS key to be used to encrypt content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_kms_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_kms_encryption_key)
         """
+
     def put_label(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_label)
         """
+
     def put_outcome(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_outcome)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#put_outcome)
         """
+
     def send_event(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
@@ -780,28 +849,31 @@
         """
         Stores events in Amazon Fraud Detector without generating fraud predictions for
         those events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.send_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#send_event)
         """
+
     def tag_resource(self, *, resourceARN: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Assigns tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#untag_resource)
         """
+
     def update_detector_version(
         self,
         *,
         detectorId: str,
         detectorVersionId: str,
         externalModelEndpoints: Sequence[str],
         rules: Sequence[RuleTypeDef],
@@ -811,41 +883,45 @@
     ) -> Dict[str, Any]:
         """
         Updates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_detector_version)
         """
+
     def update_detector_version_metadata(
         self, *, detectorId: str, detectorVersionId: str, description: str
     ) -> Dict[str, Any]:
         """
         Updates the detector version's description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_detector_version_metadata)
         """
+
     def update_detector_version_status(
         self, *, detectorId: str, detectorVersionId: str, status: DetectorVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the detector version’s status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_detector_version_status)
         """
+
     def update_event_label(
         self, *, eventId: str, eventTypeName: str, assignedLabel: str, labelTimestamp: str
     ) -> Dict[str, Any]:
         """
         Updates the specified event with a new label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_event_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_event_label)
         """
+
     def update_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         description: str = ...,
         updateMode: ListUpdateModeType = ...,
@@ -853,23 +929,25 @@
     ) -> Dict[str, Any]:
         """
         Updates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_list)
         """
+
     def update_model(
         self, *, modelId: str, modelType: ModelTypeEnumType, description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates model description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_model)
         """
+
     def update_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         majorVersionNumber: str,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
@@ -878,35 +956,38 @@
     ) -> UpdateModelVersionResultTypeDef:
         """
         Updates a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_model_version)
         """
+
     def update_model_version_status(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         modelVersionNumber: str,
         status: ModelVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the status of a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_model_version_status)
         """
+
     def update_rule_metadata(self, *, rule: RuleTypeDef, description: str) -> Dict[str, Any]:
         """
         Updates a rule's metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_rule_metadata)
         """
+
     def update_rule_version(
         self,
         *,
         rule: RuleTypeDef,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
@@ -915,14 +996,15 @@
     ) -> UpdateRuleVersionResultTypeDef:
         """
         Updates a rule version resulting in a new rule version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_rule_version)
         """
+
     def update_variable(
         self, *, name: str, defaultValue: str = ..., description: str = ..., variableType: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_variable)
```

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.py` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "CANCEL_IN_PROGRESS",
     "COMPLETE",
     "FAILED",
     "IN_PROGRESS",
     "IN_PROGRESS_INITIALIZING",
 ]
 DataSourceType = Literal["EVENT", "EXTERNAL_MODEL_SCORE", "MODEL_SCORE"]
-DataTypeType = Literal["BOOLEAN", "FLOAT", "INTEGER", "STRING"]
+DataTypeType = Literal["BOOLEAN", "DATETIME", "FLOAT", "INTEGER", "STRING"]
 DetectorVersionStatusType = Literal["ACTIVE", "DRAFT", "INACTIVE"]
 EventIngestionType = Literal["DISABLED", "ENABLED"]
 LanguageType = Literal["DETECTORPL"]
 ListUpdateModeType = Literal["APPEND", "REMOVE", "REPLACE"]
 ModelEndpointStatusType = Literal["ASSOCIATED", "DISSOCIATED"]
 ModelInputDataFormatType = Literal["APPLICATION_JSON", "TEXT_CSV"]
 ModelOutputDataFormatType = Literal["APPLICATION_JSONLINES", "TEXT_CSV"]
@@ -80,14 +80,15 @@
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
@@ -127,14 +128,15 @@
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
@@ -213,14 +215,15 @@
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
@@ -231,14 +234,15 @@
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
@@ -274,14 +278,15 @@
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
@@ -300,16 +305,19 @@
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
@@ -389,18 +397,21 @@
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

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.pyi` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "CANCEL_IN_PROGRESS",
     "COMPLETE",
     "FAILED",
     "IN_PROGRESS",
     "IN_PROGRESS_INITIALIZING",
 ]
 DataSourceType = Literal["EVENT", "EXTERNAL_MODEL_SCORE", "MODEL_SCORE"]
-DataTypeType = Literal["BOOLEAN", "FLOAT", "INTEGER", "STRING"]
+DataTypeType = Literal["BOOLEAN", "DATETIME", "FLOAT", "INTEGER", "STRING"]
 DetectorVersionStatusType = Literal["ACTIVE", "DRAFT", "INACTIVE"]
 EventIngestionType = Literal["DISABLED", "ENABLED"]
 LanguageType = Literal["DETECTORPL"]
 ListUpdateModeType = Literal["APPEND", "REMOVE", "REPLACE"]
 ModelEndpointStatusType = Literal["ASSOCIATED", "DISSOCIATED"]
 ModelInputDataFormatType = Literal["APPLICATION_JSON", "TEXT_CSV"]
 ModelOutputDataFormatType = Literal["APPLICATION_JSONLINES", "TEXT_CSV"]
@@ -78,14 +78,15 @@
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
@@ -125,14 +126,15 @@
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
@@ -211,14 +213,15 @@
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
@@ -229,14 +232,15 @@
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
@@ -272,14 +276,15 @@
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
@@ -298,16 +303,19 @@
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
@@ -387,18 +395,21 @@
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

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.py` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,35 +48,37 @@
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
     "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
     "TagTypeDef",
     "VariableEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
     "BatchImportTypeDef",
     "BatchPredictionTypeDef",
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
+    "CreateDetectorVersionResultTypeDef",
     "ExternalEventsDetailTypeDef",
+    "CreateModelVersionResultTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
     "DeleteBatchImportJobRequestRequestTypeDef",
     "DeleteBatchPredictionJobRequestRequestTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
     "DeleteEventRequestRequestTypeDef",
     "DeleteEventTypeRequestRequestTypeDef",
     "DeleteEventsByEventTypeRequestRequestTypeDef",
+    "DeleteEventsByEventTypeResultTypeDef",
     "DeleteExternalModelRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteListRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
@@ -84,37 +86,40 @@
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
     "DetectorTypeDef",
     "EntityTypeDef",
     "EntityTypeTypeDef",
     "EvaluatedExternalModelTypeDef",
     "EvaluatedRuleTypeDef",
+    "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
     "ExternalModelSummaryTypeDef",
     "ModelInputConfigurationTypeDef",
     "ModelOutputConfigurationTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
     "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
     "GetListElementsRequestRequestTypeDef",
+    "GetListElementsResultTypeDef",
     "GetListsMetadataRequestRequestTypeDef",
     "GetModelVersionRequestRequestTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
@@ -126,47 +131,42 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
     "UpdateDetectorVersionStatusRequestRequestTypeDef",
     "UpdateEventLabelRequestRequestTypeDef",
     "UpdateListRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
+    "UpdateModelVersionResultTypeDef",
     "UpdateModelVersionStatusRequestRequestTypeDef",
     "UpdateVariableRequestRequestTypeDef",
     "ATITrainingMetricsValueTypeDef",
     "AggregatedVariablesImportanceMetricsTypeDef",
+    "GetListsMetadataResultTypeDef",
+    "BatchCreateVariableResultTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
     "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
-    "PutEventTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
     "PutOutcomeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
-    "BatchCreateVariableResultTypeDef",
-    "CreateDetectorVersionResultTypeDef",
-    "CreateModelVersionResultTypeDef",
-    "DeleteEventsByEventTypeResultTypeDef",
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
-    "GetListElementsResultTypeDef",
-    "GetListsMetadataResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
     "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
     "CreateRuleResultTypeDef",
@@ -178,14 +178,15 @@
     "UpdateRuleVersionResultTypeDef",
     "DataValidationMetricsTypeDef",
     "DescribeDetectorResultTypeDef",
     "GetDetectorsResultTypeDef",
     "EventTypeDef",
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
+    "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
     "PutExternalModelRequestRequestTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
@@ -307,25 +308,14 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
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
 BatchGetVariableErrorTypeDef = TypedDict(
     "BatchGetVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -437,22 +427,43 @@
     {
         "detectorId": str,
         "ruleId": str,
         "ruleVersion": str,
     },
 )
 
+CreateDetectorVersionResultTypeDef = TypedDict(
+    "CreateDetectorVersionResultTypeDef",
+    {
+        "detectorId": str,
+        "detectorVersionId": str,
+        "status": DetectorVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExternalEventsDetailTypeDef = TypedDict(
     "ExternalEventsDetailTypeDef",
     {
         "dataLocation": str,
         "dataAccessRoleArn": str,
     },
 )
 
+CreateModelVersionResultTypeDef = TypedDict(
+    "CreateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FieldValidationMessageTypeDef = TypedDict(
     "FieldValidationMessageTypeDef",
     {
         "fieldName": str,
         "identifier": str,
         "title": str,
         "content": str,
@@ -539,14 +550,23 @@
 DeleteEventsByEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventsByEventTypeRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
+DeleteEventsByEventTypeResultTypeDef = TypedDict(
+    "DeleteEventsByEventTypeResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteExternalModelRequestRequestTypeDef = TypedDict(
     "DeleteExternalModelRequestRequestTypeDef",
     {
         "modelEndpoint": str,
     },
 )
 
@@ -694,14 +714,21 @@
         "outcomes": List[str],
         "evaluated": bool,
         "matched": bool,
     },
     total=False,
 )
 
+EventOrchestrationTypeDef = TypedDict(
+    "EventOrchestrationTypeDef",
+    {
+        "eventBridgeEnabled": bool,
+    },
+)
+
 EventPredictionSummaryTypeDef = TypedDict(
     "EventPredictionSummaryTypeDef",
     {
         "eventId": str,
         "eventTypeName": str,
         "eventTimestamp": str,
         "predictionTimestamp": str,
@@ -819,14 +846,23 @@
 GetDeleteEventsByEventTypeStatusRequestRequestTypeDef = TypedDict(
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
+GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": AsyncJobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDetectorVersionRequestRequestTypeDef = TypedDict(
     "GetDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
     },
 )
@@ -956,14 +992,23 @@
 
 class GetListElementsRequestRequestTypeDef(
     _RequiredGetListElementsRequestRequestTypeDef, _OptionalGetListElementsRequestRequestTypeDef
 ):
     pass
 
 
+GetListElementsResultTypeDef = TypedDict(
+    "GetListElementsResultTypeDef",
+    {
+        "elements": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetListsMetadataRequestRequestTypeDef = TypedDict(
     "GetListsMetadataRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1177,14 +1222,25 @@
 PutKMSEncryptionKeyRequestRequestTypeDef = TypedDict(
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     {
         "kmsEncryptionKeyArn": str,
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
 TFIMetricDataPointTypeDef = TypedDict(
     "TFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1270,14 +1326,25 @@
 
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
 
+UpdateModelVersionResultTypeDef = TypedDict(
+    "UpdateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateModelVersionStatusRequestRequestTypeDef = TypedDict(
     "UpdateModelVersionStatusRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": ModelVersionStatusType,
@@ -1320,14 +1387,31 @@
     "AggregatedVariablesImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[AggregatedLogOddsMetricTypeDef],
     },
     total=False,
 )
 
+GetListsMetadataResultTypeDef = TypedDict(
+    "GetListsMetadataResultTypeDef",
+    {
+        "lists": List[AllowDenyListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchCreateVariableResultTypeDef = TypedDict(
+    "BatchCreateVariableResultTypeDef",
+    {
+        "errors": List[BatchCreateVariableErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBatchImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchImportJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1474,14 +1558,23 @@
 
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1519,40 +1612,14 @@
 
 class PutEntityTypeRequestRequestTypeDef(
     _RequiredPutEntityTypeRequestRequestTypeDef, _OptionalPutEntityTypeRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventTypeRequestRequestTypeDef",
-    {
-        "name": str,
-        "eventVariables": Sequence[str],
-        "entityTypes": Sequence[str],
-    },
-)
-_OptionalPutEventTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventTypeRequestRequestTypeDef",
-    {
-        "description": str,
-        "labels": Sequence[str],
-        "eventIngestion": EventIngestionType,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutEventTypeRequestRequestTypeDef(
-    _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredPutLabelRequestRequestTypeDef = TypedDict(
     "_RequiredPutLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutLabelRequestRequestTypeDef = TypedDict(
@@ -1619,132 +1686,47 @@
 class BatchCreateVariableRequestRequestTypeDef(
     _RequiredBatchCreateVariableRequestRequestTypeDef,
     _OptionalBatchCreateVariableRequestRequestTypeDef,
 ):
     pass
 
 
-BatchCreateVariableResultTypeDef = TypedDict(
-    "BatchCreateVariableResultTypeDef",
-    {
-        "errors": List[BatchCreateVariableErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDetectorVersionResultTypeDef = TypedDict(
-    "CreateDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "status": DetectorVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateModelVersionResultTypeDef = TypedDict(
-    "CreateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEventsByEventTypeResultTypeDef = TypedDict(
-    "DeleteEventsByEventTypeResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": AsyncJobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetListElementsResultTypeDef = TypedDict(
-    "GetListElementsResultTypeDef",
-    {
-        "elements": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetListsMetadataResultTypeDef = TypedDict(
-    "GetListsMetadataResultTypeDef",
-    {
-        "lists": List[AllowDenyListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateModelVersionResultTypeDef = TypedDict(
-    "UpdateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetVariableResultTypeDef = TypedDict(
     "BatchGetVariableResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "errors": List[BatchGetVariableErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVariablesResultTypeDef = TypedDict(
     "GetVariablesResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBatchImportJobsResultTypeDef = TypedDict(
     "GetBatchImportJobsResultTypeDef",
     {
         "batchImports": List[BatchImportTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBatchPredictionJobsResultTypeDef = TypedDict(
     "GetBatchPredictionJobsResultTypeDef",
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelScoresTypeDef = TypedDict(
     "ModelScoresTypeDef",
     {
         "modelVersion": ModelVersionTypeDef,
@@ -1780,15 +1762,15 @@
     pass
 
 
 CreateRuleResultTypeDef = TypedDict(
     "CreateRuleResultTypeDef",
     {
         "rule": RuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
@@ -1805,15 +1787,15 @@
         "modelVersions": List[ModelVersionTypeDef],
         "rules": List[RuleTypeDef],
         "status": DetectorVersionStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "ruleExecutionMode": RuleExecutionModeType,
         "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
@@ -1873,15 +1855,15 @@
     pass
 
 
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
         "rule": RuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataValidationMetricsTypeDef = TypedDict(
     "DataValidationMetricsTypeDef",
     {
         "fileLevelMessages": List[FileValidationMessageTypeDef],
@@ -1893,24 +1875,24 @@
 DescribeDetectorResultTypeDef = TypedDict(
     "DescribeDetectorResultTypeDef",
     {
         "detectorId": str,
         "detectorVersionSummaries": List[DetectorVersionSummaryTypeDef],
         "nextToken": str,
         "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDetectorsResultTypeDef = TypedDict(
     "GetDetectorsResultTypeDef",
     {
         "detectors": List[DetectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "eventId": str,
@@ -1951,24 +1933,51 @@
 
 
 GetEntityTypesResultTypeDef = TypedDict(
     "GetEntityTypesResultTypeDef",
     {
         "entityTypes": List[EntityTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventTypeRequestRequestTypeDef",
+    {
+        "name": str,
+        "eventVariables": Sequence[str],
+        "entityTypes": Sequence[str],
     },
 )
+_OptionalPutEventTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "labels": Sequence[str],
+        "eventIngestion": EventIngestionType,
+        "tags": Sequence[TagTypeDef],
+        "eventOrchestration": EventOrchestrationTypeDef,
+    },
+    total=False,
+)
+
+
+class PutEventTypeRequestRequestTypeDef(
+    _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
+):
+    pass
+
 
 ListEventPredictionsResultTypeDef = TypedDict(
     "ListEventPredictionsResultTypeDef",
     {
         "eventPredictionSummaries": List[EventPredictionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeTypeDef = TypedDict(
     "EventTypeTypeDef",
     {
         "name": str,
@@ -1977,14 +1986,15 @@
         "labels": List[str],
         "entityTypes": List[str],
         "eventIngestion": EventIngestionType,
         "ingestedEventStatistics": IngestedEventStatisticsTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
+        "eventOrchestration": EventOrchestrationTypeDef,
     },
     total=False,
 )
 
 ExternalModelOutputsTypeDef = TypedDict(
     "ExternalModelOutputsTypeDef",
     {
@@ -2064,51 +2074,51 @@
     pass
 
 
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLabelsResultTypeDef = TypedDict(
     "GetLabelsResultTypeDef",
     {
         "labels": List[LabelTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetModelsResultTypeDef = TypedDict(
     "GetModelsResultTypeDef",
     {
         "nextToken": str,
         "models": List[ModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOutcomesResultTypeDef = TypedDict(
     "GetOutcomesResultTypeDef",
     {
         "outcomes": List[OutcomeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRulesResultTypeDef = TypedDict(
     "GetRulesResultTypeDef",
     {
         "ruleDetails": List[RuleDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
@@ -2194,43 +2204,43 @@
     total=False,
 )
 
 GetEventResultTypeDef = TypedDict(
     "GetEventResultTypeDef",
     {
         "event": EventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventTypesResultTypeDef = TypedDict(
     "GetEventTypesResultTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventPredictionResultTypeDef = TypedDict(
     "GetEventPredictionResultTypeDef",
     {
         "modelScores": List[ModelScoresTypeDef],
         "ruleResults": List[RuleResultTypeDef],
         "externalModelOutputs": List[ExternalModelOutputsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExternalModelsResultTypeDef = TypedDict(
     "GetExternalModelsResultTypeDef",
     {
         "externalModels": List[ExternalModelTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
@@ -2291,15 +2301,15 @@
         "modelVersionNumber": str,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "status": str,
         "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
@@ -2383,15 +2393,15 @@
         "eventVariables": List[EventVariableSummaryTypeDef],
         "rules": List[EvaluatedRuleTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "outcomes": List[str],
         "evaluatedModelVersions": List[EvaluatedModelVersionTypeDef],
         "evaluatedExternalModels": List[EvaluatedExternalModelTypeDef],
         "predictionTimestamp": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelVersionDetailTypeDef = TypedDict(
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
@@ -2412,10 +2422,10 @@
 )
 
 DescribeModelVersionsResultTypeDef = TypedDict(
     "DescribeModelVersionsResultTypeDef",
     {
         "modelVersionDetails": List[ModelVersionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.pyi` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,35 +47,37 @@
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
     "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
     "TagTypeDef",
     "VariableEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
     "BatchImportTypeDef",
     "BatchPredictionTypeDef",
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
+    "CreateDetectorVersionResultTypeDef",
     "ExternalEventsDetailTypeDef",
+    "CreateModelVersionResultTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
     "DeleteBatchImportJobRequestRequestTypeDef",
     "DeleteBatchPredictionJobRequestRequestTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
     "DeleteEventRequestRequestTypeDef",
     "DeleteEventTypeRequestRequestTypeDef",
     "DeleteEventsByEventTypeRequestRequestTypeDef",
+    "DeleteEventsByEventTypeResultTypeDef",
     "DeleteExternalModelRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteListRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
@@ -83,37 +85,40 @@
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
     "DetectorTypeDef",
     "EntityTypeDef",
     "EntityTypeTypeDef",
     "EvaluatedExternalModelTypeDef",
     "EvaluatedRuleTypeDef",
+    "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
     "ExternalModelSummaryTypeDef",
     "ModelInputConfigurationTypeDef",
     "ModelOutputConfigurationTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
     "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
     "GetListElementsRequestRequestTypeDef",
+    "GetListElementsResultTypeDef",
     "GetListsMetadataRequestRequestTypeDef",
     "GetModelVersionRequestRequestTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
@@ -125,47 +130,42 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
     "UpdateDetectorVersionStatusRequestRequestTypeDef",
     "UpdateEventLabelRequestRequestTypeDef",
     "UpdateListRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
+    "UpdateModelVersionResultTypeDef",
     "UpdateModelVersionStatusRequestRequestTypeDef",
     "UpdateVariableRequestRequestTypeDef",
     "ATITrainingMetricsValueTypeDef",
     "AggregatedVariablesImportanceMetricsTypeDef",
+    "GetListsMetadataResultTypeDef",
+    "BatchCreateVariableResultTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
     "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
-    "PutEventTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
     "PutOutcomeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
-    "BatchCreateVariableResultTypeDef",
-    "CreateDetectorVersionResultTypeDef",
-    "CreateModelVersionResultTypeDef",
-    "DeleteEventsByEventTypeResultTypeDef",
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
-    "GetListElementsResultTypeDef",
-    "GetListsMetadataResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
     "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
     "CreateRuleResultTypeDef",
@@ -177,14 +177,15 @@
     "UpdateRuleVersionResultTypeDef",
     "DataValidationMetricsTypeDef",
     "DescribeDetectorResultTypeDef",
     "GetDetectorsResultTypeDef",
     "EventTypeDef",
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
+    "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
     "PutExternalModelRequestRequestTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
@@ -304,25 +305,14 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
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
 BatchGetVariableErrorTypeDef = TypedDict(
     "BatchGetVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -432,22 +422,43 @@
     {
         "detectorId": str,
         "ruleId": str,
         "ruleVersion": str,
     },
 )
 
+CreateDetectorVersionResultTypeDef = TypedDict(
+    "CreateDetectorVersionResultTypeDef",
+    {
+        "detectorId": str,
+        "detectorVersionId": str,
+        "status": DetectorVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExternalEventsDetailTypeDef = TypedDict(
     "ExternalEventsDetailTypeDef",
     {
         "dataLocation": str,
         "dataAccessRoleArn": str,
     },
 )
 
+CreateModelVersionResultTypeDef = TypedDict(
+    "CreateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FieldValidationMessageTypeDef = TypedDict(
     "FieldValidationMessageTypeDef",
     {
         "fieldName": str,
         "identifier": str,
         "title": str,
         "content": str,
@@ -532,14 +543,23 @@
 DeleteEventsByEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventsByEventTypeRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
+DeleteEventsByEventTypeResultTypeDef = TypedDict(
+    "DeleteEventsByEventTypeResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteExternalModelRequestRequestTypeDef = TypedDict(
     "DeleteExternalModelRequestRequestTypeDef",
     {
         "modelEndpoint": str,
     },
 )
 
@@ -685,14 +705,21 @@
         "outcomes": List[str],
         "evaluated": bool,
         "matched": bool,
     },
     total=False,
 )
 
+EventOrchestrationTypeDef = TypedDict(
+    "EventOrchestrationTypeDef",
+    {
+        "eventBridgeEnabled": bool,
+    },
+)
+
 EventPredictionSummaryTypeDef = TypedDict(
     "EventPredictionSummaryTypeDef",
     {
         "eventId": str,
         "eventTypeName": str,
         "eventTimestamp": str,
         "predictionTimestamp": str,
@@ -806,14 +833,23 @@
 GetDeleteEventsByEventTypeStatusRequestRequestTypeDef = TypedDict(
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
+GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": AsyncJobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDetectorVersionRequestRequestTypeDef = TypedDict(
     "GetDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
     },
 )
@@ -941,14 +977,23 @@
 )
 
 class GetListElementsRequestRequestTypeDef(
     _RequiredGetListElementsRequestRequestTypeDef, _OptionalGetListElementsRequestRequestTypeDef
 ):
     pass
 
+GetListElementsResultTypeDef = TypedDict(
+    "GetListElementsResultTypeDef",
+    {
+        "elements": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetListsMetadataRequestRequestTypeDef = TypedDict(
     "GetListsMetadataRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1158,14 +1203,25 @@
 PutKMSEncryptionKeyRequestRequestTypeDef = TypedDict(
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     {
         "kmsEncryptionKeyArn": str,
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
 TFIMetricDataPointTypeDef = TypedDict(
     "TFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1247,14 +1303,25 @@
 )
 
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
+UpdateModelVersionResultTypeDef = TypedDict(
+    "UpdateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateModelVersionStatusRequestRequestTypeDef = TypedDict(
     "UpdateModelVersionStatusRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": ModelVersionStatusType,
@@ -1295,14 +1362,31 @@
     "AggregatedVariablesImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[AggregatedLogOddsMetricTypeDef],
     },
     total=False,
 )
 
+GetListsMetadataResultTypeDef = TypedDict(
+    "GetListsMetadataResultTypeDef",
+    {
+        "lists": List[AllowDenyListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchCreateVariableResultTypeDef = TypedDict(
+    "BatchCreateVariableResultTypeDef",
+    {
+        "errors": List[BatchCreateVariableErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBatchImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchImportJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1437,14 +1521,23 @@
 )
 
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1478,38 +1571,14 @@
 )
 
 class PutEntityTypeRequestRequestTypeDef(
     _RequiredPutEntityTypeRequestRequestTypeDef, _OptionalPutEntityTypeRequestRequestTypeDef
 ):
     pass
 
-_RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventTypeRequestRequestTypeDef",
-    {
-        "name": str,
-        "eventVariables": Sequence[str],
-        "entityTypes": Sequence[str],
-    },
-)
-_OptionalPutEventTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventTypeRequestRequestTypeDef",
-    {
-        "description": str,
-        "labels": Sequence[str],
-        "eventIngestion": EventIngestionType,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutEventTypeRequestRequestTypeDef(
-    _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
-):
-    pass
-
 _RequiredPutLabelRequestRequestTypeDef = TypedDict(
     "_RequiredPutLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutLabelRequestRequestTypeDef = TypedDict(
@@ -1570,132 +1639,47 @@
 
 class BatchCreateVariableRequestRequestTypeDef(
     _RequiredBatchCreateVariableRequestRequestTypeDef,
     _OptionalBatchCreateVariableRequestRequestTypeDef,
 ):
     pass
 
-BatchCreateVariableResultTypeDef = TypedDict(
-    "BatchCreateVariableResultTypeDef",
-    {
-        "errors": List[BatchCreateVariableErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDetectorVersionResultTypeDef = TypedDict(
-    "CreateDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "status": DetectorVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateModelVersionResultTypeDef = TypedDict(
-    "CreateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEventsByEventTypeResultTypeDef = TypedDict(
-    "DeleteEventsByEventTypeResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": AsyncJobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetListElementsResultTypeDef = TypedDict(
-    "GetListElementsResultTypeDef",
-    {
-        "elements": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetListsMetadataResultTypeDef = TypedDict(
-    "GetListsMetadataResultTypeDef",
-    {
-        "lists": List[AllowDenyListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateModelVersionResultTypeDef = TypedDict(
-    "UpdateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetVariableResultTypeDef = TypedDict(
     "BatchGetVariableResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "errors": List[BatchGetVariableErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVariablesResultTypeDef = TypedDict(
     "GetVariablesResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBatchImportJobsResultTypeDef = TypedDict(
     "GetBatchImportJobsResultTypeDef",
     {
         "batchImports": List[BatchImportTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBatchPredictionJobsResultTypeDef = TypedDict(
     "GetBatchPredictionJobsResultTypeDef",
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelScoresTypeDef = TypedDict(
     "ModelScoresTypeDef",
     {
         "modelVersion": ModelVersionTypeDef,
@@ -1729,15 +1713,15 @@
 ):
     pass
 
 CreateRuleResultTypeDef = TypedDict(
     "CreateRuleResultTypeDef",
     {
         "rule": RuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
@@ -1754,15 +1738,15 @@
         "modelVersions": List[ModelVersionTypeDef],
         "rules": List[RuleTypeDef],
         "status": DetectorVersionStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "ruleExecutionMode": RuleExecutionModeType,
         "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
@@ -1818,15 +1802,15 @@
 ):
     pass
 
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
         "rule": RuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataValidationMetricsTypeDef = TypedDict(
     "DataValidationMetricsTypeDef",
     {
         "fileLevelMessages": List[FileValidationMessageTypeDef],
@@ -1838,24 +1822,24 @@
 DescribeDetectorResultTypeDef = TypedDict(
     "DescribeDetectorResultTypeDef",
     {
         "detectorId": str,
         "detectorVersionSummaries": List[DetectorVersionSummaryTypeDef],
         "nextToken": str,
         "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDetectorsResultTypeDef = TypedDict(
     "GetDetectorsResultTypeDef",
     {
         "detectors": List[DetectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "eventId": str,
@@ -1894,24 +1878,49 @@
     pass
 
 GetEntityTypesResultTypeDef = TypedDict(
     "GetEntityTypesResultTypeDef",
     {
         "entityTypes": List[EntityTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventTypeRequestRequestTypeDef",
+    {
+        "name": str,
+        "eventVariables": Sequence[str],
+        "entityTypes": Sequence[str],
     },
 )
+_OptionalPutEventTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "labels": Sequence[str],
+        "eventIngestion": EventIngestionType,
+        "tags": Sequence[TagTypeDef],
+        "eventOrchestration": EventOrchestrationTypeDef,
+    },
+    total=False,
+)
+
+class PutEventTypeRequestRequestTypeDef(
+    _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
+):
+    pass
 
 ListEventPredictionsResultTypeDef = TypedDict(
     "ListEventPredictionsResultTypeDef",
     {
         "eventPredictionSummaries": List[EventPredictionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeTypeDef = TypedDict(
     "EventTypeTypeDef",
     {
         "name": str,
@@ -1920,14 +1929,15 @@
         "labels": List[str],
         "entityTypes": List[str],
         "eventIngestion": EventIngestionType,
         "ingestedEventStatistics": IngestedEventStatisticsTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
+        "eventOrchestration": EventOrchestrationTypeDef,
     },
     total=False,
 )
 
 ExternalModelOutputsTypeDef = TypedDict(
     "ExternalModelOutputsTypeDef",
     {
@@ -2003,51 +2013,51 @@
 ):
     pass
 
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLabelsResultTypeDef = TypedDict(
     "GetLabelsResultTypeDef",
     {
         "labels": List[LabelTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetModelsResultTypeDef = TypedDict(
     "GetModelsResultTypeDef",
     {
         "nextToken": str,
         "models": List[ModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOutcomesResultTypeDef = TypedDict(
     "GetOutcomesResultTypeDef",
     {
         "outcomes": List[OutcomeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRulesResultTypeDef = TypedDict(
     "GetRulesResultTypeDef",
     {
         "ruleDetails": List[RuleDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
@@ -2131,43 +2141,43 @@
     total=False,
 )
 
 GetEventResultTypeDef = TypedDict(
     "GetEventResultTypeDef",
     {
         "event": EventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventTypesResultTypeDef = TypedDict(
     "GetEventTypesResultTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventPredictionResultTypeDef = TypedDict(
     "GetEventPredictionResultTypeDef",
     {
         "modelScores": List[ModelScoresTypeDef],
         "ruleResults": List[RuleResultTypeDef],
         "externalModelOutputs": List[ExternalModelOutputsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExternalModelsResultTypeDef = TypedDict(
     "GetExternalModelsResultTypeDef",
     {
         "externalModels": List[ExternalModelTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
@@ -2224,15 +2234,15 @@
         "modelVersionNumber": str,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "status": str,
         "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
@@ -2316,15 +2326,15 @@
         "eventVariables": List[EventVariableSummaryTypeDef],
         "rules": List[EvaluatedRuleTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "outcomes": List[str],
         "evaluatedModelVersions": List[EvaluatedModelVersionTypeDef],
         "evaluatedExternalModels": List[EvaluatedExternalModelTypeDef],
         "predictionTimestamp": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelVersionDetailTypeDef = TypedDict(
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
@@ -2345,10 +2355,10 @@
 )
 
 DescribeModelVersionsResultTypeDef = TypedDict(
     "DescribeModelVersionsResultTypeDef",
     {
         "modelVersionDetails": List[ModelVersionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/PKG-INFO` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.26.72
-Summary: Type annotations for boto3.FraudDetector 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.FraudDetector 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-frauddetector"></a>
 
 # mypy-boto3-frauddetector
 
 [![PyPI - mypy-boto3-frauddetector](https://img.shields.io/pypi/v/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,35 +320,37 @@
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
     AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
+    CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
+    CreateModelVersionResultTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
+    DeleteEventsByEventTypeResultTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
@@ -356,37 +358,40 @@
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
+    EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
     ExternalModelSummaryTypeDef,
     ModelInputConfigurationTypeDef,
     ModelOutputConfigurationTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
+    GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
     GetListElementsRequestRequestTypeDef,
+    GetListElementsResultTypeDef,
     GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
@@ -398,47 +403,42 @@
     ListTagsForResourceRequestRequestTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
     UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
+    UpdateModelVersionResultTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
+    GetListsMetadataResultTypeDef,
+    BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
-    PutEventTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
-    BatchCreateVariableResultTypeDef,
-    CreateDetectorVersionResultTypeDef,
-    CreateModelVersionResultTypeDef,
-    DeleteEventsByEventTypeResultTypeDef,
-    GetDeleteEventsByEventTypeStatusResultTypeDef,
-    GetListElementsResultTypeDef,
-    GetListsMetadataResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
     CreateRuleResultTypeDef,
@@ -450,14 +450,15 @@
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
+    PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
     PutExternalModelRequestRequestTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
@@ -500,42 +501,42 @@
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

### Comparing `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/SOURCES.txt` & `mypy-boto3-frauddetector-1.27.0/mypy_boto3_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.26.72/setup.py` & `mypy-boto3-frauddetector-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-frauddetector.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-frauddetector",
-    version="1.26.72",
+    version="1.27.0",
     packages=["mypy_boto3_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FraudDetector 1.26.72 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.FraudDetector 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/",
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


# Comparing `tmp/mypy-boto3-forecast-1.26.62.tar.gz` & `tmp/mypy-boto3-forecast-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-forecast-1.26.62.tar", last modified: Wed Feb  1 20:26:24 2023, max compression
+gzip compressed data, was "mypy-boto3-forecast-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
```

## Comparing `mypy-boto3-forecast-1.26.62.tar` & `mypy-boto3-forecast-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.131657 mypy-boto3-forecast-1.26.62/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-02-01 20:26:24.131657 mypy-boto3-forecast-1.26.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.131657 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65340 2023-02-01 20:26:02.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65287 2023-02-01 20:26:01.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.131657 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-02-01 20:26:23.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-01 20:26:24.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:26:23.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:26:23.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-01 20:26:23.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-01 20:26:23.000000 mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 20:26:24.131657 mypy-boto3-forecast-1.26.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-01 20:26:00.000000 mypy-boto3-forecast-1.26.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.751274 mypy-boto3-forecast-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-03 19:50:47.751274 mypy-boto3-forecast-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.743274 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65458 2023-07-03 19:37:57.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65405 2023-07-03 19:37:56.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:55.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.751274 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-03 19:50:47.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:47.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:47.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:47.000000 mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.751274 mypy-boto3-forecast-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:37:54.000000 mypy-boto3-forecast-1.27.0/setup.py
```

### Comparing `mypy-boto3-forecast-1.26.62/LICENSE` & `mypy-boto3-forecast-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-forecast-1.26.62/PKG-INFO` & `mypy-boto3-forecast-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.26.62
-Summary: Type annotations for boto3.ForecastService 1.26.62 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ForecastService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-forecast?color=blue)](https://pypistats.org/packages/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,17 +406,30 @@
     BaselineMetricTypeDef,
     CategoricalParameterRangeTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
     ExplainabilityConfigTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -431,110 +444,97 @@
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
     SupplementaryFeatureTypeDef,
     IntegerParameterRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
+    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
+    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
     FeaturizationTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
     InputDataConfigTypeDef,
     ParameterRangesTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
     SchemaTypeDef,
@@ -597,42 +597,42 @@
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

### Comparing `mypy-boto3-forecast-1.26.62/README.md` & `mypy-boto3-forecast-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-forecast?color=blue)](https://pypistats.org/packages/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,17 +374,30 @@
     BaselineMetricTypeDef,
     CategoricalParameterRangeTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
     ExplainabilityConfigTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -399,110 +412,97 @@
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
     SupplementaryFeatureTypeDef,
     IntegerParameterRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
+    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
+    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
     FeaturizationTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
     InputDataConfigTypeDef,
     ParameterRangesTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
     SchemaTypeDef,
@@ -565,42 +565,42 @@
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

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/__init__.py` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/__init__.pyi` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/__main__.py` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ForecastService 1.26.62\nVersion:         1.26.62\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ForecastService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.62")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/client.py` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/client.pyi` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/literals.py` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,14 +119,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -252,14 +254,15 @@
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
@@ -270,14 +273,15 @@
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
@@ -313,14 +317,15 @@
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
@@ -339,16 +344,19 @@
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
@@ -428,18 +436,21 @@
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

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/literals.pyi` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -117,14 +117,15 @@
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
@@ -164,14 +165,15 @@
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
@@ -250,14 +252,15 @@
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
@@ -268,14 +271,15 @@
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
@@ -311,14 +315,15 @@
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
@@ -337,16 +342,19 @@
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
@@ -426,18 +434,21 @@
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

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/paginator.py` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
         """
 
 
@@ -117,30 +117,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
         """
 
 
@@ -150,15 +150,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
         """
 
 
@@ -168,15 +168,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
 
@@ -186,15 +186,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
         """
 
 
@@ -204,15 +204,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
         """
 
 
@@ -223,15 +223,15 @@
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
 
@@ -241,15 +241,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
         """
 
 
@@ -259,15 +259,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
 
@@ -277,15 +277,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
         """
 
 
@@ -295,15 +295,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
         """
 
 
@@ -313,15 +313,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
 
@@ -331,13 +331,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/paginator.pyi` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
         """
 
 class ListDatasetImportJobsPaginator(Paginator):
@@ -113,29 +113,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
         """
 
 class ListExplainabilitiesPaginator(Paginator):
@@ -144,15 +144,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
         """
 
 class ListExplainabilityExportsPaginator(Paginator):
@@ -161,15 +161,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
 class ListForecastExportJobsPaginator(Paginator):
@@ -178,15 +178,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
         """
 
 class ListForecastsPaginator(Paginator):
@@ -195,15 +195,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
         """
 
 class ListMonitorEvaluationsPaginator(Paginator):
@@ -213,15 +213,15 @@
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
 class ListMonitorsPaginator(Paginator):
@@ -230,15 +230,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
         """
 
 class ListPredictorBacktestExportJobsPaginator(Paginator):
@@ -247,15 +247,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
 class ListPredictorsPaginator(Paginator):
@@ -264,15 +264,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
         """
 
 class ListWhatIfAnalysesPaginator(Paginator):
@@ -281,15 +281,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
         """
 
 class ListWhatIfForecastExportsPaginator(Paginator):
@@ -298,15 +298,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
 class ListWhatIfForecastsPaginator(Paginator):
@@ -315,13 +315,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/type_defs.py` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,30 @@
     "BaselineMetricTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAutoPredictorResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateExplainabilityExportResponseTypeDef",
     "ExplainabilityConfigTypeDef",
+    "CreateExplainabilityResponseTypeDef",
+    "CreateForecastExportJobResponseTypeDef",
+    "CreateForecastResponseTypeDef",
+    "CreateMonitorResponseTypeDef",
+    "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
+    "CreatePredictorResponseTypeDef",
+    "CreateWhatIfAnalysisResponseTypeDef",
+    "CreateWhatIfForecastExportResponseTypeDef",
+    "CreateWhatIfForecastResponseTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -76,110 +89,97 @@
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
     "SupplementaryFeatureTypeDef",
     "IntegerParameterRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
+    "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateAutoPredictorResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateExplainabilityExportResponseTypeDef",
-    "CreateExplainabilityResponseTypeDef",
-    "CreateForecastExportJobResponseTypeDef",
-    "CreateForecastResponseTypeDef",
-    "CreateMonitorResponseTypeDef",
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    "CreatePredictorResponseTypeDef",
-    "CreateWhatIfAnalysisResponseTypeDef",
-    "CreateWhatIfForecastExportResponseTypeDef",
-    "CreateWhatIfForecastResponseTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
     "FeaturizationTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
+    "ListForecastsRequestListForecastsPaginateTypeDef",
     "ListForecastsRequestRequestTypeDef",
+    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     "ListMonitorsRequestRequestTypeDef",
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     "ListPredictorsRequestRequestTypeDef",
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
     "InputDataConfigTypeDef",
     "ParameterRangesTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
-    "ListForecastsRequestListForecastsPaginateTypeDef",
-    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
     "SchemaTypeDef",
@@ -342,42 +342,143 @@
         "DayOfMonth": int,
         "DayOfWeek": DayOfWeekType,
         "Hour": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAutoPredictorResponseTypeDef = TypedDict(
+    "CreateAutoPredictorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PredictorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "DatasetImportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateExplainabilityExportResponseTypeDef = TypedDict(
+    "CreateExplainabilityExportResponseTypeDef",
+    {
+        "ExplainabilityExportArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExplainabilityConfigTypeDef = TypedDict(
     "ExplainabilityConfigTypeDef",
     {
         "TimeSeriesGranularity": TimeSeriesGranularityType,
         "TimePointGranularity": TimePointGranularityType,
     },
 )
 
+CreateExplainabilityResponseTypeDef = TypedDict(
+    "CreateExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateForecastExportJobResponseTypeDef = TypedDict(
+    "CreateForecastExportJobResponseTypeDef",
+    {
+        "ForecastExportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateForecastResponseTypeDef = TypedDict(
+    "CreateForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateMonitorResponseTypeDef = TypedDict(
+    "CreateMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    {
+        "PredictorBacktestExportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluationParametersTypeDef = TypedDict(
     "EvaluationParametersTypeDef",
     {
         "NumberOfBacktestWindows": int,
         "BackTestWindowOffset": int,
     },
     total=False,
 )
 
+CreatePredictorResponseTypeDef = TypedDict(
+    "CreatePredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWhatIfAnalysisResponseTypeDef = TypedDict(
+    "CreateWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWhatIfForecastExportResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastExportResponseTypeDef",
+    {
+        "WhatIfForecastExportArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWhatIfForecastResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -553,14 +654,28 @@
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupName": str,
+        "DatasetGroupArn": str,
+        "DatasetArns": List[str],
+        "Domain": DomainType,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetImportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetImportJobRequestRequestTypeDef",
     {
         "DatasetImportJobArn": str,
     },
 )
 
@@ -656,14 +771,21 @@
 DescribeWhatIfForecastRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ErrorMetricTypeDef = TypedDict(
     "ErrorMetricTypeDef",
     {
         "ForecastType": str,
         "WAPE": float,
         "RMSE": float,
         "MASE": float,
@@ -752,33 +874,39 @@
 
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
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
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -856,14 +984,24 @@
         "DatasetImportJobArn": str,
         "ForecastArn": str,
         "PredictorArn": str,
     },
     total=False,
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
 PredictorEventTypeDef = TypedDict(
     "PredictorEventTypeDef",
     {
         "Detail": str,
         "Datetime": datetime,
     },
     total=False,
@@ -876,14 +1014,25 @@
         "TestWindowEnd": datetime,
         "Status": str,
         "Message": str,
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
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -998,160 +1147,27 @@
 
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
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
-CreateAutoPredictorResponseTypeDef = TypedDict(
-    "CreateAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "DatasetImportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExplainabilityExportResponseTypeDef = TypedDict(
-    "CreateExplainabilityExportResponseTypeDef",
-    {
-        "ExplainabilityExportArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExplainabilityResponseTypeDef = TypedDict(
-    "CreateExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateForecastExportJobResponseTypeDef = TypedDict(
-    "CreateForecastExportJobResponseTypeDef",
-    {
-        "ForecastExportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateForecastResponseTypeDef = TypedDict(
-    "CreateForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMonitorResponseTypeDef = TypedDict(
-    "CreateMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    {
-        "PredictorBacktestExportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePredictorResponseTypeDef = TypedDict(
-    "CreatePredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWhatIfAnalysisResponseTypeDef = TypedDict(
-    "CreateWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWhatIfForecastExportResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastExportResponseTypeDef",
-    {
-        "WhatIfForecastExportArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWhatIfForecastResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupName": str,
-        "DatasetGroupArn": str,
-        "DatasetArns": List[str],
-        "Domain": DomainType,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ExplainabilitySummaryTypeDef = TypedDict(
     "ExplainabilitySummaryTypeDef",
     {
         "ExplainabilityArn": str,
@@ -1181,24 +1197,24 @@
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "DatasetGroups": List[DatasetGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PredictorSummaryTypeDef = TypedDict(
     "PredictorSummaryTypeDef",
     {
         "PredictorArn": str,
@@ -1229,348 +1245,332 @@
 )
 
 
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
 
-ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestRequestTypeDef",
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilitiesRequestRequestTypeDef = TypedDict(
-    "ListExplainabilitiesRequestRequestTypeDef",
+ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestRequestTypeDef",
+ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastExportJobsRequestRequestTypeDef = TypedDict(
-    "ListForecastExportJobsRequestRequestTypeDef",
+ListExplainabilitiesRequestRequestTypeDef = TypedDict(
+    "ListExplainabilitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastsRequestRequestTypeDef = TypedDict(
-    "ListForecastsRequestRequestTypeDef",
+ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
-    {
-        "MonitorArn": str,
-    },
-)
-_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
+ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
-class ListMonitorEvaluationsRequestRequestTypeDef(
-    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
-    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
-):
-    pass
-
-
-ListMonitorsRequestRequestTypeDef = TypedDict(
-    "ListMonitorsRequestRequestTypeDef",
+ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
+ListForecastExportJobsRequestRequestTypeDef = TypedDict(
+    "ListForecastExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPredictorsRequestRequestTypeDef = TypedDict(
-    "ListPredictorsRequestRequestTypeDef",
+ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
+    "ListForecastsRequestListForecastsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestRequestTypeDef",
+ListForecastsRequestRequestTypeDef = TypedDict(
+    "ListForecastsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestRequestTypeDef",
+_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filters": Sequence[FilterTypeDef],
+        "MonitorArn": str,
     },
-    total=False,
 )
-
-ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestRequestTypeDef",
+_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastsResponseTypeDef = TypedDict(
-    "ListForecastsResponseTypeDef",
-    {
-        "Forecasts": List[ForecastSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
+class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
+    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
     {
-        "DatasetGroupArn": str,
+        "MonitorArn": str,
     },
 )
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
+_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
     {
-        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+class ListMonitorEvaluationsRequestRequestTypeDef(
+    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
+    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
+):
     pass
 
 
-ParameterRangesTypeDef = TypedDict(
-    "ParameterRangesTypeDef",
+ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
-        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
-        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
-        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+ListMonitorsRequestRequestTypeDef = TypedDict(
+    "ListMonitorsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+ListPredictorsRequestRequestTypeDef = TypedDict(
+    "ListPredictorsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
-    "ListForecastsRequestListForecastsPaginateTypeDef",
+ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    {
-        "MonitorArn": str,
-    },
-)
-_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
-    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-):
-    pass
-
-
-ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+ListForecastsResponseTypeDef = TypedDict(
+    "ListForecastsResponseTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Forecasts": List[ForecastSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
+    {
+        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
+
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+    pass
+
+
+ParameterRangesTypeDef = TypedDict(
+    "ParameterRangesTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
+        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
 ListMonitorsResponseTypeDef = TypedDict(
     "ListMonitorsResponseTypeDef",
     {
         "Monitors": List[MonitorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWhatIfForecastsResponseTypeDef = TypedDict(
     "ListWhatIfForecastsResponseTypeDef",
     {
         "WhatIfForecasts": List[WhatIfForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricsTypeDef = TypedDict(
     "MetricsTypeDef",
     {
         "RMSE": float,
@@ -1676,15 +1676,15 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ExplainabilityInfo": ExplainabilityInfoTypeDef,
         "MonitorInfo": MonitorInfoTypeDef,
         "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
@@ -1693,15 +1693,15 @@
 )
 
 ListExplainabilitiesResponseTypeDef = TypedDict(
     "ListExplainabilitiesResponseTypeDef",
     {
         "Explainabilities": List[ExplainabilitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
     {
         "ExplainabilityExportName": str,
@@ -1809,15 +1809,15 @@
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
@@ -1825,15 +1825,15 @@
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
@@ -1841,15 +1841,15 @@
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
@@ -1858,15 +1858,15 @@
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
@@ -1984,24 +1984,24 @@
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
@@ -2044,15 +2044,15 @@
 )
 
 ListMonitorEvaluationsResponseTypeDef = TypedDict(
     "ListMonitorEvaluationsResponseTypeDef",
     {
         "NextToken": str,
         "PredictorMonitorEvaluations": List[PredictorMonitorEvaluationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PredictorExecutionDetailsTypeDef = TypedDict(
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
@@ -2124,15 +2124,15 @@
         "DatasetType": DatasetTypeType,
         "DataFrequency": str,
         "Schema": SchemaTypeDef,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExplainabilityResponseTypeDef = TypedDict(
     "DescribeExplainabilityResponseTypeDef",
     {
         "ExplainabilityArn": str,
@@ -2145,15 +2145,15 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
@@ -2197,60 +2197,60 @@
         "LastEvaluationTime": datetime,
         "LastEvaluationState": str,
         "Baseline": BaselineTypeDef,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "EstimatedEvaluationTimeRemainingInMinutes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExplainabilityExportsResponseTypeDef = TypedDict(
     "ListExplainabilityExportsResponseTypeDef",
     {
         "ExplainabilityExports": List[ExplainabilityExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListForecastExportJobsResponseTypeDef = TypedDict(
     "ListForecastExportJobsResponseTypeDef",
     {
         "ForecastExportJobs": List[ForecastExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPredictorBacktestExportJobsResponseTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsResponseTypeDef",
     {
         "PredictorBacktestExportJobs": List[PredictorBacktestExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWhatIfForecastExportsResponseTypeDef = TypedDict(
     "ListWhatIfForecastExportsResponseTypeDef",
     {
         "WhatIfForecastExports": List[WhatIfForecastExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
@@ -2316,15 +2316,15 @@
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
@@ -2367,26 +2367,26 @@
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "ForecastTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccuracyMetricsResponseTypeDef = TypedDict(
     "GetAccuracyMetricsResponseTypeDef",
     {
         "PredictorEvaluationResults": List[EvaluationResultTypeDef],
         "IsAutoPredictor": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
         "ForecastName": str,
@@ -2444,15 +2444,15 @@
         "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
     "DescribeWhatIfAnalysisResponseTypeDef",
     {
         "WhatIfAnalysisName": str,
@@ -2460,10 +2460,10 @@
         "ForecastArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast/type_defs.pyi` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,30 @@
     "BaselineMetricTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAutoPredictorResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateExplainabilityExportResponseTypeDef",
     "ExplainabilityConfigTypeDef",
+    "CreateExplainabilityResponseTypeDef",
+    "CreateForecastExportJobResponseTypeDef",
+    "CreateForecastResponseTypeDef",
+    "CreateMonitorResponseTypeDef",
+    "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
+    "CreatePredictorResponseTypeDef",
+    "CreateWhatIfAnalysisResponseTypeDef",
+    "CreateWhatIfForecastExportResponseTypeDef",
+    "CreateWhatIfForecastResponseTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -75,110 +88,97 @@
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
     "SupplementaryFeatureTypeDef",
     "IntegerParameterRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
+    "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateAutoPredictorResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateExplainabilityExportResponseTypeDef",
-    "CreateExplainabilityResponseTypeDef",
-    "CreateForecastExportJobResponseTypeDef",
-    "CreateForecastResponseTypeDef",
-    "CreateMonitorResponseTypeDef",
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    "CreatePredictorResponseTypeDef",
-    "CreateWhatIfAnalysisResponseTypeDef",
-    "CreateWhatIfForecastExportResponseTypeDef",
-    "CreateWhatIfForecastResponseTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
     "FeaturizationTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
+    "ListForecastsRequestListForecastsPaginateTypeDef",
     "ListForecastsRequestRequestTypeDef",
+    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     "ListMonitorsRequestRequestTypeDef",
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     "ListPredictorsRequestRequestTypeDef",
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
     "InputDataConfigTypeDef",
     "ParameterRangesTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
-    "ListForecastsRequestListForecastsPaginateTypeDef",
-    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
     "SchemaTypeDef",
@@ -337,42 +337,143 @@
         "DayOfMonth": int,
         "DayOfWeek": DayOfWeekType,
         "Hour": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAutoPredictorResponseTypeDef = TypedDict(
+    "CreateAutoPredictorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PredictorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "DatasetImportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateExplainabilityExportResponseTypeDef = TypedDict(
+    "CreateExplainabilityExportResponseTypeDef",
+    {
+        "ExplainabilityExportArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExplainabilityConfigTypeDef = TypedDict(
     "ExplainabilityConfigTypeDef",
     {
         "TimeSeriesGranularity": TimeSeriesGranularityType,
         "TimePointGranularity": TimePointGranularityType,
     },
 )
 
+CreateExplainabilityResponseTypeDef = TypedDict(
+    "CreateExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateForecastExportJobResponseTypeDef = TypedDict(
+    "CreateForecastExportJobResponseTypeDef",
+    {
+        "ForecastExportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateForecastResponseTypeDef = TypedDict(
+    "CreateForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateMonitorResponseTypeDef = TypedDict(
+    "CreateMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    {
+        "PredictorBacktestExportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluationParametersTypeDef = TypedDict(
     "EvaluationParametersTypeDef",
     {
         "NumberOfBacktestWindows": int,
         "BackTestWindowOffset": int,
     },
     total=False,
 )
 
+CreatePredictorResponseTypeDef = TypedDict(
+    "CreatePredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWhatIfAnalysisResponseTypeDef = TypedDict(
+    "CreateWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWhatIfForecastExportResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastExportResponseTypeDef",
+    {
+        "WhatIfForecastExportArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWhatIfForecastResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -546,14 +647,28 @@
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupName": str,
+        "DatasetGroupArn": str,
+        "DatasetArns": List[str],
+        "Domain": DomainType,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetImportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetImportJobRequestRequestTypeDef",
     {
         "DatasetImportJobArn": str,
     },
 )
 
@@ -649,14 +764,21 @@
 DescribeWhatIfForecastRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ErrorMetricTypeDef = TypedDict(
     "ErrorMetricTypeDef",
     {
         "ForecastType": str,
         "WAPE": float,
         "RMSE": float,
         "MASE": float,
@@ -741,33 +863,39 @@
 )
 
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
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
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -845,14 +973,24 @@
         "DatasetImportJobArn": str,
         "ForecastArn": str,
         "PredictorArn": str,
     },
     total=False,
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
 PredictorEventTypeDef = TypedDict(
     "PredictorEventTypeDef",
     {
         "Detail": str,
         "Datetime": datetime,
     },
     total=False,
@@ -865,14 +1003,25 @@
         "TestWindowEnd": datetime,
         "Status": str,
         "Message": str,
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
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -981,160 +1130,27 @@
 )
 
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
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
-CreateAutoPredictorResponseTypeDef = TypedDict(
-    "CreateAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "DatasetImportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExplainabilityExportResponseTypeDef = TypedDict(
-    "CreateExplainabilityExportResponseTypeDef",
-    {
-        "ExplainabilityExportArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExplainabilityResponseTypeDef = TypedDict(
-    "CreateExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateForecastExportJobResponseTypeDef = TypedDict(
-    "CreateForecastExportJobResponseTypeDef",
-    {
-        "ForecastExportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateForecastResponseTypeDef = TypedDict(
-    "CreateForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMonitorResponseTypeDef = TypedDict(
-    "CreateMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    {
-        "PredictorBacktestExportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePredictorResponseTypeDef = TypedDict(
-    "CreatePredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWhatIfAnalysisResponseTypeDef = TypedDict(
-    "CreateWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWhatIfForecastExportResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastExportResponseTypeDef",
-    {
-        "WhatIfForecastExportArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWhatIfForecastResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupName": str,
-        "DatasetGroupArn": str,
-        "DatasetArns": List[str],
-        "Domain": DomainType,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ExplainabilitySummaryTypeDef = TypedDict(
     "ExplainabilitySummaryTypeDef",
     {
         "ExplainabilityArn": str,
@@ -1164,24 +1180,24 @@
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "DatasetGroups": List[DatasetGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PredictorSummaryTypeDef = TypedDict(
     "PredictorSummaryTypeDef",
     {
         "PredictorArn": str,
@@ -1210,342 +1226,326 @@
     },
     total=False,
 )
 
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
-ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestRequestTypeDef",
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilitiesRequestRequestTypeDef = TypedDict(
-    "ListExplainabilitiesRequestRequestTypeDef",
+ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestRequestTypeDef",
+ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastExportJobsRequestRequestTypeDef = TypedDict(
-    "ListForecastExportJobsRequestRequestTypeDef",
+ListExplainabilitiesRequestRequestTypeDef = TypedDict(
+    "ListExplainabilitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastsRequestRequestTypeDef = TypedDict(
-    "ListForecastsRequestRequestTypeDef",
+ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
-    {
-        "MonitorArn": str,
-    },
-)
-_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
+ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class ListMonitorEvaluationsRequestRequestTypeDef(
-    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
-    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
-):
-    pass
-
-ListMonitorsRequestRequestTypeDef = TypedDict(
-    "ListMonitorsRequestRequestTypeDef",
+ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
+ListForecastExportJobsRequestRequestTypeDef = TypedDict(
+    "ListForecastExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPredictorsRequestRequestTypeDef = TypedDict(
-    "ListPredictorsRequestRequestTypeDef",
+ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
+    "ListForecastsRequestListForecastsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestRequestTypeDef",
+ListForecastsRequestRequestTypeDef = TypedDict(
+    "ListForecastsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestRequestTypeDef",
+_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filters": Sequence[FilterTypeDef],
+        "MonitorArn": str,
     },
-    total=False,
 )
-
-ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestRequestTypeDef",
+_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastsResponseTypeDef = TypedDict(
-    "ListForecastsResponseTypeDef",
-    {
-        "Forecasts": List[ForecastSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
+    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+):
+    pass
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
+_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
     {
-        "DatasetGroupArn": str,
+        "MonitorArn": str,
     },
 )
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
+_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
     {
-        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+class ListMonitorEvaluationsRequestRequestTypeDef(
+    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
+    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
+):
     pass
 
-ParameterRangesTypeDef = TypedDict(
-    "ParameterRangesTypeDef",
+ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
-        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
-        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
-        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+ListMonitorsRequestRequestTypeDef = TypedDict(
+    "ListMonitorsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+ListPredictorsRequestRequestTypeDef = TypedDict(
+    "ListPredictorsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
-    "ListForecastsRequestListForecastsPaginateTypeDef",
+ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    {
-        "MonitorArn": str,
-    },
-)
-_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
-    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-):
-    pass
-
-ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+ListForecastsResponseTypeDef = TypedDict(
+    "ListForecastsResponseTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Forecasts": List[ForecastSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
+    {
+        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+    pass
+
+ParameterRangesTypeDef = TypedDict(
+    "ParameterRangesTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
+        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
 ListMonitorsResponseTypeDef = TypedDict(
     "ListMonitorsResponseTypeDef",
     {
         "Monitors": List[MonitorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWhatIfForecastsResponseTypeDef = TypedDict(
     "ListWhatIfForecastsResponseTypeDef",
     {
         "WhatIfForecasts": List[WhatIfForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricsTypeDef = TypedDict(
     "MetricsTypeDef",
     {
         "RMSE": float,
@@ -1649,15 +1649,15 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ExplainabilityInfo": ExplainabilityInfoTypeDef,
         "MonitorInfo": MonitorInfoTypeDef,
         "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
@@ -1666,15 +1666,15 @@
 )
 
 ListExplainabilitiesResponseTypeDef = TypedDict(
     "ListExplainabilitiesResponseTypeDef",
     {
         "Explainabilities": List[ExplainabilitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
     {
         "ExplainabilityExportName": str,
@@ -1774,15 +1774,15 @@
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
@@ -1790,15 +1790,15 @@
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
@@ -1806,15 +1806,15 @@
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
@@ -1823,15 +1823,15 @@
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
@@ -1947,24 +1947,24 @@
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
@@ -2005,15 +2005,15 @@
 )
 
 ListMonitorEvaluationsResponseTypeDef = TypedDict(
     "ListMonitorEvaluationsResponseTypeDef",
     {
         "NextToken": str,
         "PredictorMonitorEvaluations": List[PredictorMonitorEvaluationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PredictorExecutionDetailsTypeDef = TypedDict(
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
@@ -2081,15 +2081,15 @@
         "DatasetType": DatasetTypeType,
         "DataFrequency": str,
         "Schema": SchemaTypeDef,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExplainabilityResponseTypeDef = TypedDict(
     "DescribeExplainabilityResponseTypeDef",
     {
         "ExplainabilityArn": str,
@@ -2102,15 +2102,15 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
@@ -2152,60 +2152,60 @@
         "LastEvaluationTime": datetime,
         "LastEvaluationState": str,
         "Baseline": BaselineTypeDef,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "EstimatedEvaluationTimeRemainingInMinutes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExplainabilityExportsResponseTypeDef = TypedDict(
     "ListExplainabilityExportsResponseTypeDef",
     {
         "ExplainabilityExports": List[ExplainabilityExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListForecastExportJobsResponseTypeDef = TypedDict(
     "ListForecastExportJobsResponseTypeDef",
     {
         "ForecastExportJobs": List[ForecastExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPredictorBacktestExportJobsResponseTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsResponseTypeDef",
     {
         "PredictorBacktestExportJobs": List[PredictorBacktestExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWhatIfForecastExportsResponseTypeDef = TypedDict(
     "ListWhatIfForecastExportsResponseTypeDef",
     {
         "WhatIfForecastExports": List[WhatIfForecastExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
@@ -2269,15 +2269,15 @@
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
@@ -2318,26 +2318,26 @@
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "ForecastTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccuracyMetricsResponseTypeDef = TypedDict(
     "GetAccuracyMetricsResponseTypeDef",
     {
         "PredictorEvaluationResults": List[EvaluationResultTypeDef],
         "IsAutoPredictor": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
         "ForecastName": str,
@@ -2391,15 +2391,15 @@
         "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
     "DescribeWhatIfAnalysisResponseTypeDef",
     {
         "WhatIfAnalysisName": str,
@@ -2407,10 +2407,10 @@
         "ForecastArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/PKG-INFO` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.26.62
-Summary: Type annotations for boto3.ForecastService 1.26.62 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ForecastService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-forecast?color=blue)](https://pypistats.org/packages/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,17 +406,30 @@
     BaselineMetricTypeDef,
     CategoricalParameterRangeTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
     ExplainabilityConfigTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -431,110 +444,97 @@
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
     SupplementaryFeatureTypeDef,
     IntegerParameterRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
+    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
+    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
     FeaturizationTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
     InputDataConfigTypeDef,
     ParameterRangesTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
     SchemaTypeDef,
@@ -597,42 +597,42 @@
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

### Comparing `mypy-boto3-forecast-1.26.62/mypy_boto3_forecast.egg-info/SOURCES.txt` & `mypy-boto3-forecast-1.27.0/mypy_boto3_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.26.62/setup.py` & `mypy-boto3-forecast-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-forecast.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-forecast",
-    version="1.26.62",
+    version="1.27.0",
     packages=["mypy_boto3_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ForecastService 1.26.62 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ForecastService 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/",
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


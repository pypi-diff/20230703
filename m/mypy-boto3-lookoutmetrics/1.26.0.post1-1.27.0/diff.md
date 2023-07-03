# Comparing `tmp/mypy-boto3-lookoutmetrics-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-lookoutmetrics-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutmetrics-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:40 2022, max compression
+gzip compressed data, was "mypy-boto3-lookoutmetrics-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1.tar` & `mypy-boto3-lookoutmetrics-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:40.932833 mypy-boto3-lookoutmetrics-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16523 2022-11-01 21:43:40.932833 mypy-boto3-lookoutmetrics-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15054 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:40.924833 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22558 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    22522 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8906 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8904 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    36503 2022-11-01 21:37:32.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    36470 2022-11-01 21:37:32.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:40.932833 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16523 2022-11-01 21:43:40.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-11-01 21:43:40.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:40.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:40.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:40.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-01 21:43:40.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:40.932833 mypy-boto3-lookoutmetrics-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-11-01 21:37:31.000000 mypy-boto3-lookoutmetrics-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.675597 mypy-boto3-lookoutmetrics-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-03 19:51:03.671597 mypy-boto3-lookoutmetrics-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.671597 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-03 19:41:21.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36547 2023-07-03 19:41:22.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36514 2023-07-03 19:41:22.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.671597 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-03 19:51:03.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 19:51:03.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:03.000000 mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.675597 mypy-boto3-lookoutmetrics-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:41:20.000000 mypy-boto3-lookoutmetrics-1.27.0/setup.py
```

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/LICENSE` & `mypy-boto3-lookoutmetrics-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.LookoutMetrics 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LookoutMetrics 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
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
 
 <a id="mypy-boto3-lookoutmetrics"></a>
 
 # mypy-boto3-lookoutmetrics
 
 [![PyPI - mypy-boto3-lookoutmetrics](https://img.shields.io/pypi/v/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutmetrics?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,17 +328,19 @@
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AppFlowConfigTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
+    CreateMetricSetResponseTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
@@ -347,48 +350,46 @@
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
     JsonFormatDescriptorTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
+    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     VpcConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     ActionTypeDef,
     AlertFiltersTypeDef,
+    ListAlertsResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
-    CreateMetricSetResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
-    GetSampleDataResponseTypeDef,
-    ListAlertsResponseTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
     FileFormatDescriptorTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
@@ -433,42 +434,42 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/README.md` & `mypy-boto3-lookoutmetrics-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lookoutmetrics"></a>
 
 # mypy-boto3-lookoutmetrics
 
 [![PyPI - mypy-boto3-lookoutmetrics](https://img.shields.io/pypi/v/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutmetrics?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,17 +296,19 @@
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AppFlowConfigTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
+    CreateMetricSetResponseTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
@@ -316,48 +318,46 @@
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
     JsonFormatDescriptorTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
+    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     VpcConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     ActionTypeDef,
     AlertFiltersTypeDef,
+    ListAlertsResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
-    CreateMetricSetResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
-    GetSampleDataResponseTypeDef,
-    ListAlertsResponseTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
     FileFormatDescriptorTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
@@ -402,42 +402,42 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/__main__.py` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutMetrics 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.LookoutMetrics 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/client.py` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/client.pyi` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/literals.py` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,23 +94,25 @@
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
@@ -120,30 +122,35 @@
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
@@ -169,14 +176,15 @@
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
@@ -221,51 +229,57 @@
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
@@ -278,14 +292,15 @@
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
@@ -297,28 +312,35 @@
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
@@ -327,14 +349,15 @@
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
@@ -345,55 +368,64 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/literals.pyi` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -92,23 +92,25 @@
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
@@ -118,30 +120,35 @@
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
@@ -167,14 +174,15 @@
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
@@ -219,51 +227,57 @@
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
@@ -276,14 +290,15 @@
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
@@ -295,28 +310,35 @@
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
@@ -325,14 +347,15 @@
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
@@ -343,55 +366,64 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/type_defs.py` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
@@ -55,17 +54,19 @@
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
     "AppFlowConfigTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAlertResponseTypeDef",
+    "CreateAnomalyDetectorResponseTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
+    "CreateMetricSetResponseTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
@@ -75,48 +76,46 @@
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
     "JsonFormatDescriptorTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
+    "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "VpcConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAlertResponseTypeDef",
+    "UpdateAnomalyDetectorResponseTypeDef",
+    "UpdateMetricSetResponseTypeDef",
     "ActionTypeDef",
     "AlertFiltersTypeDef",
+    "ListAlertsResponseTypeDef",
+    "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
+    "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
-    "CreateAlertResponseTypeDef",
-    "CreateAnomalyDetectorResponseTypeDef",
-    "CreateMetricSetResponseTypeDef",
-    "DescribeAnomalyDetectorResponseTypeDef",
-    "GetSampleDataResponseTypeDef",
-    "ListAlertsResponseTypeDef",
-    "ListAnomalyDetectorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateAlertResponseTypeDef",
-    "UpdateAnomalyDetectorResponseTypeDef",
-    "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
     "FileFormatDescriptorTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
@@ -172,19 +171,17 @@
     "_OptionalSNSConfigurationTypeDef",
     {
         "SnsFormat": SnsFormatType,
     },
     total=False,
 )
 
-
 class SNSConfigurationTypeDef(_RequiredSNSConfigurationTypeDef, _OptionalSNSConfigurationTypeDef):
     pass
 
-
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
@@ -283,21 +280,19 @@
     "_OptionalAnomalyGroupTimeSeriesTypeDef",
     {
         "TimeSeriesId": str,
     },
     total=False,
 )
 
-
 class AnomalyGroupTimeSeriesTypeDef(
     _RequiredAnomalyGroupTimeSeriesTypeDef, _OptionalAnomalyGroupTimeSeriesTypeDef
 ):
     pass
 
-
 AppFlowConfigTypeDef = TypedDict(
     "AppFlowConfigTypeDef",
     {
         "RoleArn": str,
         "FlowName": str,
     },
     total=False,
@@ -335,22 +330,27 @@
 BackTestAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAlertResponseTypeDef = TypedDict(
+    "CreateAlertResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AlertArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAnomalyDetectorResponseTypeDef = TypedDict(
+    "CreateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "MetricName": str,
@@ -361,28 +361,34 @@
     "_OptionalMetricTypeDef",
     {
         "Namespace": str,
     },
     total=False,
 )
 
-
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
-
 TimestampColumnTypeDef = TypedDict(
     "TimestampColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
+CreateMetricSetResponseTypeDef = TypedDict(
+    "CreateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -443,22 +449,20 @@
         "Timestamp": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAnomalyDetectionExecutionsRequestRequestTypeDef(
     _RequiredDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     _OptionalDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 ExecutionStatusTypeDef = TypedDict(
     "ExecutionStatusTypeDef",
     {
         "Timestamp": str,
         "Status": AnomalyDetectionTaskStatusType,
         "FailureReason": str,
     },
@@ -532,31 +536,38 @@
     "_OptionalGetDataQualityMetricsRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
     total=False,
 )
 
-
 class GetDataQualityMetricsRequestRequestTypeDef(
     _RequiredGetDataQualityMetricsRequestRequestTypeDef,
     _OptionalGetDataQualityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 TimeSeriesFeedbackTypeDef = TypedDict(
     "TimeSeriesFeedbackTypeDef",
     {
         "TimeSeriesId": str,
         "IsAnomaly": bool,
     },
     total=False,
 )
 
+GetSampleDataResponseTypeDef = TypedDict(
+    "GetSampleDataResponseTypeDef",
+    {
+        "HeaderValues": List[str],
+        "SampleRows": List[List[str]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InterMetricImpactDetailsTypeDef = TypedDict(
     "InterMetricImpactDetailsTypeDef",
     {
         "MetricName": str,
         "AnomalyGroupId": str,
         "RelationshipType": RelationshipTypeType,
         "ContributionPercentage": float,
@@ -596,22 +607,20 @@
         "RelationshipTypeFilter": RelationshipTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalyGroupRelatedMetricsRequestRequestTypeDef(
     _RequiredListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     _OptionalListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAnomalyGroupSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupSummariesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "SensitivityThreshold": int,
     },
 )
@@ -620,22 +629,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalyGroupSummariesRequestRequestTypeDef(
     _RequiredListAnomalyGroupSummariesRequestRequestTypeDef,
     _OptionalListAnomalyGroupSummariesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "AnomalyGroupId": str,
         "MetricName": str,
     },
@@ -645,22 +652,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalyGroupTimeSeriesRequestRequestTypeDef(
     _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     _OptionalListAnomalyGroupTimeSeriesRequestRequestTypeDef,
 ):
     pass
 
-
 ListMetricSetsRequestRequestTypeDef = TypedDict(
     "ListMetricSetsRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -684,22 +689,41 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -708,14 +732,38 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateAlertResponseTypeDef = TypedDict(
+    "UpdateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAnomalyDetectorResponseTypeDef = TypedDict(
+    "UpdateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateMetricSetResponseTypeDef = TypedDict(
+    "UpdateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
@@ -726,14 +774,40 @@
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
 )
 
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "AlertSummaryList": List[AlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAnomalyDetectorResponseTypeDef = TypedDict(
+    "DescribeAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "AnomalyDetectorName": str,
+        "AnomalyDetectorDescription": str,
+        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Status": AnomalyDetectorStatusType,
+        "FailureReason": str,
+        "KmsKeyArn": str,
+        "FailureType": AnomalyDetectorFailureTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorName": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
 )
@@ -743,22 +817,20 @@
         "AnomalyDetectorDescription": str,
         "KmsKeyArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAnomalyDetectorRequestRequestTypeDef(
     _RequiredCreateAnomalyDetectorRequestRequestTypeDef,
     _OptionalCreateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 _OptionalUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
@@ -767,21 +839,28 @@
         "KmsKeyArn": str,
         "AnomalyDetectorDescription": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAnomalyDetectorRequestRequestTypeDef(
     _RequiredUpdateAnomalyDetectorRequestRequestTypeDef,
     _OptionalUpdateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
+ListAnomalyDetectorsResponseTypeDef = TypedDict(
+    "ListAnomalyDetectorsResponseTypeDef",
+    {
+        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 AnomalyGroupStatisticsTypeDef = TypedDict(
     "AnomalyGroupStatisticsTypeDef",
     {
         "EvaluationStartDate": str,
         "TotalCount": int,
         "ItemizedMetricStatsList": List[ItemizedMetricStatsTypeDef],
@@ -809,21 +888,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetFeedbackRequestRequestTypeDef(
     _RequiredGetFeedbackRequestRequestTypeDef, _OptionalGetFeedbackRequestRequestTypeDef
 ):
     pass
 
-
 AthenaSourceConfigTypeDef = TypedDict(
     "AthenaSourceConfigTypeDef",
     {
         "RoleArn": str,
         "DatabaseName": str,
         "DataCatalog": str,
         "TableName": str,
@@ -857,129 +934,29 @@
     "AutoDetectionMetricSourceTypeDef",
     {
         "S3SourceConfig": AutoDetectionS3SourceConfigTypeDef,
     },
     total=False,
 )
 
-CreateAlertResponseTypeDef = TypedDict(
-    "CreateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAnomalyDetectorResponseTypeDef = TypedDict(
-    "CreateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMetricSetResponseTypeDef = TypedDict(
-    "CreateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAnomalyDetectorResponseTypeDef = TypedDict(
-    "DescribeAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "AnomalyDetectorName": str,
-        "AnomalyDetectorDescription": str,
-        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Status": AnomalyDetectorStatusType,
-        "FailureReason": str,
-        "KmsKeyArn": str,
-        "FailureType": AnomalyDetectorFailureTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSampleDataResponseTypeDef = TypedDict(
-    "GetSampleDataResponseTypeDef",
-    {
-        "HeaderValues": List[str],
-        "SampleRows": List[List[str]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "AlertSummaryList": List[AlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAnomalyDetectorsResponseTypeDef = TypedDict(
-    "ListAnomalyDetectorsResponseTypeDef",
-    {
-        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAlertResponseTypeDef = TypedDict(
-    "UpdateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalyDetectorResponseTypeDef = TypedDict(
-    "UpdateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMetricSetResponseTypeDef = TypedDict(
-    "UpdateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MetricSetDataQualityMetricTypeDef = TypedDict(
     "MetricSetDataQualityMetricTypeDef",
     {
         "MetricSetArn": str,
         "DataQualityMetricList": List[DataQualityMetricTypeDef],
     },
     total=False,
 )
 
 DescribeAnomalyDetectionExecutionsResponseTypeDef = TypedDict(
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     {
         "ExecutionList": List[ExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DimensionContributionTypeDef = TypedDict(
     "DimensionContributionTypeDef",
     {
         "DimensionName": str,
@@ -1016,33 +993,33 @@
 )
 
 GetFeedbackResponseTypeDef = TypedDict(
     "GetFeedbackResponseTypeDef",
     {
         "AnomalyGroupTimeSeriesFeedback": List[TimeSeriesFeedbackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAnomalyGroupRelatedMetricsResponseTypeDef = TypedDict(
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     {
         "InterMetricImpactList": List[InterMetricImpactDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMetricSetsResponseTypeDef = TypedDict(
     "ListMetricSetsResponseTypeDef",
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -1105,21 +1082,19 @@
         "AlertDescription": str,
         "Tags": Mapping[str, str],
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
-
 class CreateAlertRequestRequestTypeDef(
     _RequiredCreateAlertRequestRequestTypeDef, _OptionalCreateAlertRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlertRequestRequestTypeDef",
     {
         "AlertArn": str,
     },
 )
 _OptionalUpdateAlertRequestRequestTypeDef = TypedDict(
@@ -1129,28 +1104,26 @@
         "AlertSensitivityThreshold": int,
         "Action": ActionTypeDef,
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAlertRequestRequestTypeDef(
     _RequiredUpdateAlertRequestRequestTypeDef, _OptionalUpdateAlertRequestRequestTypeDef
 ):
     pass
 
-
 ListAnomalyGroupSummariesResponseTypeDef = TypedDict(
     "ListAnomalyGroupSummariesResponseTypeDef",
     {
         "AnomalyGroupSummaryList": List[AnomalyGroupSummaryTypeDef],
         "AnomalyGroupStatistics": AnomalyGroupStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectedCsvFormatDescriptorTypeDef = TypedDict(
     "DetectedCsvFormatDescriptorTypeDef",
     {
         "FileCompression": DetectedFieldTypeDef,
@@ -1201,15 +1174,15 @@
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     {
         "AnomalyGroupId": str,
         "MetricName": str,
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
@@ -1232,26 +1205,24 @@
     {
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
     },
     total=False,
 )
 
-
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
-
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectedFileFormatDescriptorTypeDef = TypedDict(
     "DetectedFileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": DetectedCsvFormatDescriptorTypeDef,
@@ -1260,15 +1231,15 @@
     total=False,
 )
 
 GetDataQualityMetricsResponseTypeDef = TypedDict(
     "GetDataQualityMetricsResponseTypeDef",
     {
         "AnomalyDetectorDataQualityMetricList": List[AnomalyDetectorDataQualityMetricTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricLevelImpactTypeDef = TypedDict(
     "MetricLevelImpactTypeDef",
     {
         "MetricName": str,
@@ -1340,21 +1311,19 @@
         "Timezone": str,
         "Tags": Mapping[str, str],
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
-
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeMetricSetResponseTypeDef = TypedDict(
     "DescribeMetricSetResponseTypeDef",
     {
         "MetricSetArn": str,
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricSetDescription": str,
@@ -1364,15 +1333,15 @@
         "MetricList": List[MetricTypeDef],
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": List[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "MetricSource": MetricSourceTypeDef,
         "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
@@ -1389,34 +1358,32 @@
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
-
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
     pass
 
-
 DetectedMetricSourceTypeDef = TypedDict(
     "DetectedMetricSourceTypeDef",
     {
         "S3SourceConfig": DetectedS3SourceConfigTypeDef,
     },
     total=False,
 )
 
 GetAnomalyGroupResponseTypeDef = TypedDict(
     "GetAnomalyGroupResponseTypeDef",
     {
         "AnomalyGroup": AnomalyGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectedMetricSetConfigTypeDef = TypedDict(
     "DetectedMetricSetConfigTypeDef",
     {
         "Offset": DetectedFieldTypeDef,
@@ -1426,10 +1393,10 @@
     total=False,
 )
 
 DetectMetricSetConfigResponseTypeDef = TypedDict(
     "DetectMetricSetConfigResponseTypeDef",
     {
         "DetectedMetricSetConfig": DetectedMetricSetConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics/type_defs.pyi` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
@@ -54,17 +55,19 @@
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
     "AppFlowConfigTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAlertResponseTypeDef",
+    "CreateAnomalyDetectorResponseTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
+    "CreateMetricSetResponseTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
@@ -74,48 +77,46 @@
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
     "JsonFormatDescriptorTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
+    "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "VpcConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAlertResponseTypeDef",
+    "UpdateAnomalyDetectorResponseTypeDef",
+    "UpdateMetricSetResponseTypeDef",
     "ActionTypeDef",
     "AlertFiltersTypeDef",
+    "ListAlertsResponseTypeDef",
+    "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
+    "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
-    "CreateAlertResponseTypeDef",
-    "CreateAnomalyDetectorResponseTypeDef",
-    "CreateMetricSetResponseTypeDef",
-    "DescribeAnomalyDetectorResponseTypeDef",
-    "GetSampleDataResponseTypeDef",
-    "ListAlertsResponseTypeDef",
-    "ListAnomalyDetectorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateAlertResponseTypeDef",
-    "UpdateAnomalyDetectorResponseTypeDef",
-    "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
     "FileFormatDescriptorTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
@@ -171,17 +172,19 @@
     "_OptionalSNSConfigurationTypeDef",
     {
         "SnsFormat": SnsFormatType,
     },
     total=False,
 )
 
+
 class SNSConfigurationTypeDef(_RequiredSNSConfigurationTypeDef, _OptionalSNSConfigurationTypeDef):
     pass
 
+
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
@@ -280,19 +283,21 @@
     "_OptionalAnomalyGroupTimeSeriesTypeDef",
     {
         "TimeSeriesId": str,
     },
     total=False,
 )
 
+
 class AnomalyGroupTimeSeriesTypeDef(
     _RequiredAnomalyGroupTimeSeriesTypeDef, _OptionalAnomalyGroupTimeSeriesTypeDef
 ):
     pass
 
+
 AppFlowConfigTypeDef = TypedDict(
     "AppFlowConfigTypeDef",
     {
         "RoleArn": str,
         "FlowName": str,
     },
     total=False,
@@ -330,22 +335,27 @@
 BackTestAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAlertResponseTypeDef = TypedDict(
+    "CreateAlertResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AlertArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAnomalyDetectorResponseTypeDef = TypedDict(
+    "CreateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "MetricName": str,
@@ -356,26 +366,36 @@
     "_OptionalMetricTypeDef",
     {
         "Namespace": str,
     },
     total=False,
 )
 
+
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
+
 TimestampColumnTypeDef = TypedDict(
     "TimestampColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
+CreateMetricSetResponseTypeDef = TypedDict(
+    "CreateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -436,20 +456,22 @@
         "Timestamp": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAnomalyDetectionExecutionsRequestRequestTypeDef(
     _RequiredDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     _OptionalDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 ExecutionStatusTypeDef = TypedDict(
     "ExecutionStatusTypeDef",
     {
         "Timestamp": str,
         "Status": AnomalyDetectionTaskStatusType,
         "FailureReason": str,
     },
@@ -523,29 +545,40 @@
     "_OptionalGetDataQualityMetricsRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
     total=False,
 )
 
+
 class GetDataQualityMetricsRequestRequestTypeDef(
     _RequiredGetDataQualityMetricsRequestRequestTypeDef,
     _OptionalGetDataQualityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 TimeSeriesFeedbackTypeDef = TypedDict(
     "TimeSeriesFeedbackTypeDef",
     {
         "TimeSeriesId": str,
         "IsAnomaly": bool,
     },
     total=False,
 )
 
+GetSampleDataResponseTypeDef = TypedDict(
+    "GetSampleDataResponseTypeDef",
+    {
+        "HeaderValues": List[str],
+        "SampleRows": List[List[str]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InterMetricImpactDetailsTypeDef = TypedDict(
     "InterMetricImpactDetailsTypeDef",
     {
         "MetricName": str,
         "AnomalyGroupId": str,
         "RelationshipType": RelationshipTypeType,
         "ContributionPercentage": float,
@@ -585,20 +618,22 @@
         "RelationshipTypeFilter": RelationshipTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalyGroupRelatedMetricsRequestRequestTypeDef(
     _RequiredListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     _OptionalListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAnomalyGroupSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupSummariesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "SensitivityThreshold": int,
     },
 )
@@ -607,20 +642,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalyGroupSummariesRequestRequestTypeDef(
     _RequiredListAnomalyGroupSummariesRequestRequestTypeDef,
     _OptionalListAnomalyGroupSummariesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "AnomalyGroupId": str,
         "MetricName": str,
     },
@@ -630,20 +667,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalyGroupTimeSeriesRequestRequestTypeDef(
     _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     _OptionalListAnomalyGroupTimeSeriesRequestRequestTypeDef,
 ):
     pass
 
+
 ListMetricSetsRequestRequestTypeDef = TypedDict(
     "ListMetricSetsRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -667,22 +706,41 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -691,14 +749,38 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateAlertResponseTypeDef = TypedDict(
+    "UpdateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAnomalyDetectorResponseTypeDef = TypedDict(
+    "UpdateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateMetricSetResponseTypeDef = TypedDict(
+    "UpdateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
@@ -709,14 +791,40 @@
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
 )
 
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "AlertSummaryList": List[AlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAnomalyDetectorResponseTypeDef = TypedDict(
+    "DescribeAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "AnomalyDetectorName": str,
+        "AnomalyDetectorDescription": str,
+        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Status": AnomalyDetectorStatusType,
+        "FailureReason": str,
+        "KmsKeyArn": str,
+        "FailureType": AnomalyDetectorFailureTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorName": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
 )
@@ -726,20 +834,22 @@
         "AnomalyDetectorDescription": str,
         "KmsKeyArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAnomalyDetectorRequestRequestTypeDef(
     _RequiredCreateAnomalyDetectorRequestRequestTypeDef,
     _OptionalCreateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 _OptionalUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
@@ -748,20 +858,31 @@
         "KmsKeyArn": str,
         "AnomalyDetectorDescription": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAnomalyDetectorRequestRequestTypeDef(
     _RequiredUpdateAnomalyDetectorRequestRequestTypeDef,
     _OptionalUpdateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
+
+ListAnomalyDetectorsResponseTypeDef = TypedDict(
+    "ListAnomalyDetectorsResponseTypeDef",
+    {
+        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AnomalyGroupStatisticsTypeDef = TypedDict(
     "AnomalyGroupStatisticsTypeDef",
     {
         "EvaluationStartDate": str,
         "TotalCount": int,
         "ItemizedMetricStatsList": List[ItemizedMetricStatsTypeDef],
     },
@@ -788,19 +909,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetFeedbackRequestRequestTypeDef(
     _RequiredGetFeedbackRequestRequestTypeDef, _OptionalGetFeedbackRequestRequestTypeDef
 ):
     pass
 
+
 AthenaSourceConfigTypeDef = TypedDict(
     "AthenaSourceConfigTypeDef",
     {
         "RoleArn": str,
         "DatabaseName": str,
         "DataCatalog": str,
         "TableName": str,
@@ -834,129 +957,29 @@
     "AutoDetectionMetricSourceTypeDef",
     {
         "S3SourceConfig": AutoDetectionS3SourceConfigTypeDef,
     },
     total=False,
 )
 
-CreateAlertResponseTypeDef = TypedDict(
-    "CreateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAnomalyDetectorResponseTypeDef = TypedDict(
-    "CreateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMetricSetResponseTypeDef = TypedDict(
-    "CreateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAnomalyDetectorResponseTypeDef = TypedDict(
-    "DescribeAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "AnomalyDetectorName": str,
-        "AnomalyDetectorDescription": str,
-        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Status": AnomalyDetectorStatusType,
-        "FailureReason": str,
-        "KmsKeyArn": str,
-        "FailureType": AnomalyDetectorFailureTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSampleDataResponseTypeDef = TypedDict(
-    "GetSampleDataResponseTypeDef",
-    {
-        "HeaderValues": List[str],
-        "SampleRows": List[List[str]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "AlertSummaryList": List[AlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAnomalyDetectorsResponseTypeDef = TypedDict(
-    "ListAnomalyDetectorsResponseTypeDef",
-    {
-        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAlertResponseTypeDef = TypedDict(
-    "UpdateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalyDetectorResponseTypeDef = TypedDict(
-    "UpdateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMetricSetResponseTypeDef = TypedDict(
-    "UpdateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MetricSetDataQualityMetricTypeDef = TypedDict(
     "MetricSetDataQualityMetricTypeDef",
     {
         "MetricSetArn": str,
         "DataQualityMetricList": List[DataQualityMetricTypeDef],
     },
     total=False,
 )
 
 DescribeAnomalyDetectionExecutionsResponseTypeDef = TypedDict(
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     {
         "ExecutionList": List[ExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DimensionContributionTypeDef = TypedDict(
     "DimensionContributionTypeDef",
     {
         "DimensionName": str,
@@ -993,33 +1016,33 @@
 )
 
 GetFeedbackResponseTypeDef = TypedDict(
     "GetFeedbackResponseTypeDef",
     {
         "AnomalyGroupTimeSeriesFeedback": List[TimeSeriesFeedbackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAnomalyGroupRelatedMetricsResponseTypeDef = TypedDict(
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     {
         "InterMetricImpactList": List[InterMetricImpactDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMetricSetsResponseTypeDef = TypedDict(
     "ListMetricSetsResponseTypeDef",
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -1082,19 +1105,21 @@
         "AlertDescription": str,
         "Tags": Mapping[str, str],
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
+
 class CreateAlertRequestRequestTypeDef(
     _RequiredCreateAlertRequestRequestTypeDef, _OptionalCreateAlertRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlertRequestRequestTypeDef",
     {
         "AlertArn": str,
     },
 )
 _OptionalUpdateAlertRequestRequestTypeDef = TypedDict(
@@ -1104,26 +1129,28 @@
         "AlertSensitivityThreshold": int,
         "Action": ActionTypeDef,
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAlertRequestRequestTypeDef(
     _RequiredUpdateAlertRequestRequestTypeDef, _OptionalUpdateAlertRequestRequestTypeDef
 ):
     pass
 
+
 ListAnomalyGroupSummariesResponseTypeDef = TypedDict(
     "ListAnomalyGroupSummariesResponseTypeDef",
     {
         "AnomalyGroupSummaryList": List[AnomalyGroupSummaryTypeDef],
         "AnomalyGroupStatistics": AnomalyGroupStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectedCsvFormatDescriptorTypeDef = TypedDict(
     "DetectedCsvFormatDescriptorTypeDef",
     {
         "FileCompression": DetectedFieldTypeDef,
@@ -1174,15 +1201,15 @@
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     {
         "AnomalyGroupId": str,
         "MetricName": str,
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
@@ -1205,24 +1232,26 @@
     {
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
     },
     total=False,
 )
 
+
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
+
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectedFileFormatDescriptorTypeDef = TypedDict(
     "DetectedFileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": DetectedCsvFormatDescriptorTypeDef,
@@ -1231,15 +1260,15 @@
     total=False,
 )
 
 GetDataQualityMetricsResponseTypeDef = TypedDict(
     "GetDataQualityMetricsResponseTypeDef",
     {
         "AnomalyDetectorDataQualityMetricList": List[AnomalyDetectorDataQualityMetricTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricLevelImpactTypeDef = TypedDict(
     "MetricLevelImpactTypeDef",
     {
         "MetricName": str,
@@ -1311,19 +1340,21 @@
         "Timezone": str,
         "Tags": Mapping[str, str],
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
+
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeMetricSetResponseTypeDef = TypedDict(
     "DescribeMetricSetResponseTypeDef",
     {
         "MetricSetArn": str,
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricSetDescription": str,
@@ -1333,15 +1364,15 @@
         "MetricList": List[MetricTypeDef],
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": List[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "MetricSource": MetricSourceTypeDef,
         "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
@@ -1358,32 +1389,34 @@
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
+
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
     pass
 
+
 DetectedMetricSourceTypeDef = TypedDict(
     "DetectedMetricSourceTypeDef",
     {
         "S3SourceConfig": DetectedS3SourceConfigTypeDef,
     },
     total=False,
 )
 
 GetAnomalyGroupResponseTypeDef = TypedDict(
     "GetAnomalyGroupResponseTypeDef",
     {
         "AnomalyGroup": AnomalyGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectedMetricSetConfigTypeDef = TypedDict(
     "DetectedMetricSetConfigTypeDef",
     {
         "Offset": DetectedFieldTypeDef,
@@ -1393,10 +1426,10 @@
     total=False,
 )
 
 DetectMetricSetConfigResponseTypeDef = TypedDict(
     "DetectMetricSetConfigResponseTypeDef",
     {
         "DetectedMetricSetConfig": DetectedMetricSetConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.LookoutMetrics 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LookoutMetrics 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
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
 
 <a id="mypy-boto3-lookoutmetrics"></a>
 
 # mypy-boto3-lookoutmetrics
 
 [![PyPI - mypy-boto3-lookoutmetrics](https://img.shields.io/pypi/v/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutmetrics?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,17 +328,19 @@
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AppFlowConfigTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
+    CreateMetricSetResponseTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
@@ -347,48 +350,46 @@
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
     JsonFormatDescriptorTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
+    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     VpcConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     ActionTypeDef,
     AlertFiltersTypeDef,
+    ListAlertsResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
-    CreateMetricSetResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
-    GetSampleDataResponseTypeDef,
-    ListAlertsResponseTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
     FileFormatDescriptorTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
@@ -433,42 +434,42 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt` & `mypy-boto3-lookoutmetrics-1.27.0/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.26.0.post1/setup.py` & `mypy-boto3-lookoutmetrics-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-lookoutmetrics.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutmetrics",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutMetrics 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.LookoutMetrics 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_lookoutmetrics": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_lookoutmetrics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/",
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


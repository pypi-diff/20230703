# Comparing `tmp/mypy-boto3-devops-guru-1.26.80.tar.gz` & `tmp/mypy-boto3-devops-guru-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devops-guru-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
+gzip compressed data, was "mypy-boto3-devops-guru-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-devops-guru-1.26.80.tar` & `mypy-boto3-devops-guru-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.132040 mypy-boto3-devops-guru-1.26.80/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-02-27 20:35:29.124040 mypy-boto3-devops-guru-1.26.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.124040 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61203 2023-02-27 20:35:03.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61138 2023-02-27 20:35:02.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.124040 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.132040 mypy-boto3-devops-guru-1.26.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.795112 mypy-boto3-devops-guru-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:30.000000 mypy-boto3-devops-guru-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-03 19:50:38.795112 mypy-boto3-devops-guru-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21456 2023-07-03 19:35:30.000000 mypy-boto3-devops-guru-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.791112 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:31.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62087 2023-07-03 19:35:33.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62022 2023-07-03 19:35:33.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:30.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.795112 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-03 19:50:38.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 19:50:38.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:38.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:50:38.000000 mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.795112 mypy-boto3-devops-guru-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 19:35:30.000000 mypy-boto3-devops-guru-1.27.0/setup.py
```

### Comparing `mypy-boto3-devops-guru-1.26.80/LICENSE` & `mypy-boto3-devops-guru-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-devops-guru-1.26.80/PKG-INFO` & `mypy-boto3-devops-guru-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.26.80
-Summary: Type annotations for boto3.DevOpsGuru 1.26.80 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.DevOpsGuru 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-devops-guru"></a>
 
 # mypy-boto3-devops-guru
 
 [![PyPI - mypy-boto3-devops-guru](https://img.shields.io/pypi/v/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,14 +382,15 @@
     OptInStatusType,
     OrganizationResourceCollectionTypeType,
     ResourceCollectionTypeType,
     ResourcePermissionType,
     ResourceTypeFilterType,
     SearchInsightsPaginatorName,
     SearchOrganizationInsightsPaginatorName,
+    ServerSideEncryptionTypeType,
     ServiceNameType,
     UpdateResourceCollectionActionType,
     DevOpsGuruServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -406,93 +407,95 @@
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    ResponseMetadataTypeDef,
+    AddNotificationChannelResponseTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
     CloudFormationCollectionTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
+    DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
     EndTimeRangeTypeDef,
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
+    KMSServerSideEncryptionIntegrationConfigTypeDef,
+    KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
     NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
+    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
     TagCollectionTypeDef,
+    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
-    DescribeAccountHealthResponseTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigTypeDef,
@@ -576,42 +579,42 @@
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

### Comparing `mypy-boto3-devops-guru-1.26.80/README.md` & `mypy-boto3-devops-guru-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-devops-guru"></a>
 
 # mypy-boto3-devops-guru
 
 [![PyPI - mypy-boto3-devops-guru](https://img.shields.io/pypi/v/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,14 +350,15 @@
     OptInStatusType,
     OrganizationResourceCollectionTypeType,
     ResourceCollectionTypeType,
     ResourcePermissionType,
     ResourceTypeFilterType,
     SearchInsightsPaginatorName,
     SearchOrganizationInsightsPaginatorName,
+    ServerSideEncryptionTypeType,
     ServiceNameType,
     UpdateResourceCollectionActionType,
     DevOpsGuruServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -374,93 +375,95 @@
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    ResponseMetadataTypeDef,
+    AddNotificationChannelResponseTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
     CloudFormationCollectionTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
+    DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
     EndTimeRangeTypeDef,
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
+    KMSServerSideEncryptionIntegrationConfigTypeDef,
+    KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
     NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
+    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
     TagCollectionTypeDef,
+    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
-    DescribeAccountHealthResponseTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigTypeDef,
@@ -544,42 +547,42 @@
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

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.py` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.pyi` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__main__.py` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DevOpsGuru 1.26.80\nVersion:         1.26.80\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.DevOpsGuru 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.80")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.py` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.pyi` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.py` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "OptInStatusType",
     "OrganizationResourceCollectionTypeType",
     "ResourceCollectionTypeType",
     "ResourcePermissionType",
     "ResourceTypeFilterType",
     "SearchInsightsPaginatorName",
     "SearchOrganizationInsightsPaginatorName",
+    "ServerSideEncryptionTypeType",
     "ServiceNameType",
     "UpdateResourceCollectionActionType",
     "DevOpsGuruServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
@@ -163,14 +164,15 @@
     "SNS_TOPIC",
     "SQS_QUEUE",
     "STEP_FUNCTIONS_ACTIVITY",
     "STEP_FUNCTIONS_STATE_MACHINE",
 ]
 SearchInsightsPaginatorName = Literal["search_insights"]
 SearchOrganizationInsightsPaginatorName = Literal["search_organization_insights"]
+ServerSideEncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KEY"]
 ServiceNameType = Literal[
     "API_GATEWAY",
     "APPLICATION_ELB",
     "AUTO_SCALING_GROUP",
     "CLOUD_FRONT",
     "DYNAMO_DB",
     "EC2",
@@ -207,14 +209,15 @@
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
@@ -254,14 +257,15 @@
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
@@ -359,14 +363,15 @@
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
@@ -402,14 +407,15 @@
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
@@ -428,16 +434,19 @@
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
@@ -521,15 +530,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.pyi` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "OptInStatusType",
     "OrganizationResourceCollectionTypeType",
     "ResourceCollectionTypeType",
     "ResourcePermissionType",
     "ResourceTypeFilterType",
     "SearchInsightsPaginatorName",
     "SearchOrganizationInsightsPaginatorName",
+    "ServerSideEncryptionTypeType",
     "ServiceNameType",
     "UpdateResourceCollectionActionType",
     "DevOpsGuruServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
@@ -161,14 +162,15 @@
     "SNS_TOPIC",
     "SQS_QUEUE",
     "STEP_FUNCTIONS_ACTIVITY",
     "STEP_FUNCTIONS_STATE_MACHINE",
 ]
 SearchInsightsPaginatorName = Literal["search_insights"]
 SearchOrganizationInsightsPaginatorName = Literal["search_organization_insights"]
+ServerSideEncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KEY"]
 ServiceNameType = Literal[
     "API_GATEWAY",
     "APPLICATION_ELB",
     "AUTO_SCALING_GROUP",
     "CLOUD_FRONT",
     "DYNAMO_DB",
     "EC2",
@@ -205,14 +207,15 @@
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
@@ -252,14 +255,15 @@
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
@@ -357,14 +361,15 @@
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
@@ -400,14 +405,15 @@
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
@@ -426,16 +432,19 @@
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
@@ -519,15 +528,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.py` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -93,275 +93,259 @@
     "ListNotificationChannelsPaginator",
     "ListOrganizationInsightsPaginator",
     "ListRecommendationsPaginator",
     "SearchInsightsPaginator",
     "SearchOrganizationInsightsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeOrganizationResourceCollectionHealthPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
-
 class DescribeResourceCollectionHealthPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
-
 class GetCostEstimationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCostEstimationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
         """
 
-
 class GetResourceCollectionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
-
 class ListAnomaliesForInsightPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomaliesforinsightpaginator)
     """
 
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
-
 class ListAnomalousLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
     """
 
     def paginate(
-        self, *, InsightId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InsightId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAnomalousLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
         """
 
-
 class ListEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listeventspaginator)
         """
 
-
 class ListInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
         """
 
-
 class ListMonitoredResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
-
 class ListNotificationChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNotificationChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
         """
 
-
 class ListOrganizationInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listorganizationinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
-
 class ListRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listrecommendationspaginator)
     """
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listrecommendationspaginator)
         """
 
-
 class SearchInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchinsightspaginator)
         """
 
-
 class SearchOrganizationInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchorganizationinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.pyi` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,259 +93,275 @@
     "ListNotificationChannelsPaginator",
     "ListOrganizationInsightsPaginator",
     "ListRecommendationsPaginator",
     "SearchInsightsPaginator",
     "SearchOrganizationInsightsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeOrganizationResourceCollectionHealthPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
+
 class DescribeResourceCollectionHealthPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
+
 class GetCostEstimationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCostEstimationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
         """
 
+
 class GetResourceCollectionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
+
 class ListAnomaliesForInsightPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomaliesforinsightpaginator)
     """
 
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
+
 class ListAnomalousLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
     """
 
     def paginate(
-        self, *, InsightId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InsightId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAnomalousLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
         """
 
+
 class ListEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listeventspaginator)
         """
 
+
 class ListInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
         """
 
+
 class ListMonitoredResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
+
 class ListNotificationChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNotificationChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
         """
 
+
 class ListOrganizationInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listorganizationinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
+
 class ListRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listrecommendationspaginator)
     """
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listrecommendationspaginator)
         """
 
+
 class SearchInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchinsightspaginator)
         """
 
+
 class SearchOrganizationInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchorganizationinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.py` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,105 +34,107 @@
     LogAnomalyTypeType,
     NotificationMessageTypeType,
     OptInStatusType,
     OrganizationResourceCollectionTypeType,
     ResourceCollectionTypeType,
     ResourcePermissionType,
     ResourceTypeFilterType,
+    ServerSideEncryptionTypeType,
     ServiceNameType,
     UpdateResourceCollectionActionType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInsightHealthTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddNotificationChannelResponseTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
     "CloudFormationCollectionTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
+    "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
+    "DescribeAccountOverviewResponseTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
+    "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeOrganizationOverviewResponseTypeDef",
+    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
+    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
     "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
     "EventTimeRangeTypeDef",
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
+    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
     "InsightTimeRangeTypeDef",
+    "KMSServerSideEncryptionIntegrationConfigTypeDef",
+    "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
     "StartTimeRangeTypeDef",
+    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
+    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
     "NotificationFilterConfigTypeDef",
     "SnsChannelConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
+    "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
     "TagCollectionTypeDef",
+    "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
-    "AddNotificationChannelResponseTypeDef",
-    "DescribeAccountHealthResponseTypeDef",
-    "DescribeAccountOverviewResponseTypeDef",
-    "DescribeOrganizationHealthResponseTypeDef",
-    "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeFeedbackResponseTypeDef",
     "PutFeedbackRequestRequestTypeDef",
-    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListInsightsClosedStatusFilterTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
     "NotificationChannelConfigTypeDef",
@@ -213,22 +215,19 @@
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddNotificationChannelResponseTypeDef = TypedDict(
+    "AddNotificationChannelResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
@@ -246,21 +245,19 @@
     "_OptionalAnomalyReportedTimeRangeTypeDef",
     {
         "CloseTime": datetime,
     },
     total=False,
 )
 
-
 class AnomalyReportedTimeRangeTypeDef(
     _RequiredAnomalyReportedTimeRangeTypeDef, _OptionalAnomalyReportedTimeRangeTypeDef
 ):
     pass
 
-
 AnomalyResourceTypeDef = TypedDict(
     "AnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -286,19 +283,17 @@
     "_OptionalAnomalyTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class AnomalyTimeRangeTypeDef(_RequiredAnomalyTimeRangeTypeDef, _OptionalAnomalyTimeRangeTypeDef):
     pass
 
-
 CloudFormationCollectionFilterTypeDef = TypedDict(
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
@@ -367,35 +362,55 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DescribeAccountHealthResponseTypeDef = TypedDict(
+    "DescribeAccountHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "AnalyzedResourceCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
     {
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
+DescribeAccountOverviewResponseTypeDef = TypedDict(
+    "DescribeAccountOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "MeanTimeToRecoverInMilliseconds": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -403,21 +418,19 @@
     "_OptionalDescribeAnomalyRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DescribeAnomalyRequestRequestTypeDef(
     _RequiredDescribeAnomalyRequestRequestTypeDef, _OptionalDescribeAnomalyRequestRequestTypeDef
 ):
     pass
 
-
 DescribeFeedbackRequestRequestTypeDef = TypedDict(
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
@@ -441,30 +454,39 @@
     "_OptionalDescribeInsightRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DescribeInsightRequestRequestTypeDef(
     _RequiredDescribeInsightRequestRequestTypeDef, _OptionalDescribeInsightRequestRequestTypeDef
 ):
     pass
 
-
 DescribeOrganizationHealthRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationHealthRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
+DescribeOrganizationHealthResponseTypeDef = TypedDict(
+    "DescribeOrganizationHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
@@ -473,32 +495,52 @@
         "ToTime": Union[datetime, str],
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
+DescribeOrganizationOverviewResponseTypeDef = TypedDict(
+    "DescribeOrganizationOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -508,21 +550,39 @@
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+):
+    pass
 
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
@@ -530,22 +590,20 @@
     "_OptionalDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-
 EndTimeRangeTypeDef = TypedDict(
     "EndTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
@@ -565,14 +623,22 @@
     "EventTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
 )
 
+GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -585,54 +651,90 @@
         "Count": int,
         "UnitCost": float,
         "Cost": float,
     },
     total=False,
 )
 
+_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
+    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+):
+    pass
+
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetResourceCollectionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
     "_OptionalInsightTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class InsightTimeRangeTypeDef(_RequiredInsightTimeRangeTypeDef, _OptionalInsightTimeRangeTypeDef):
     pass
 
+KMSServerSideEncryptionIntegrationConfigTypeDef = TypedDict(
+    "KMSServerSideEncryptionIntegrationConfigTypeDef",
+    {
+        "KMSKeyId": str,
+        "OptInStatus": OptInStatusType,
+        "Type": ServerSideEncryptionTypeType,
+    },
+    total=False,
+)
+
+KMSServerSideEncryptionIntegrationTypeDef = TypedDict(
+    "KMSServerSideEncryptionIntegrationTypeDef",
+    {
+        "KMSKeyId": str,
+        "OptInStatus": OptInStatusType,
+        "Type": ServerSideEncryptionTypeType,
+    },
+    total=False,
+)
 
 ServiceCollectionTypeDef = TypedDict(
     "ServiceCollectionTypeDef",
     {
         "ServiceNames": Sequence[ServiceNameType],
     },
     total=False,
@@ -643,14 +745,34 @@
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
+    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -658,22 +780,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalousLogGroupsRequestRequestTypeDef(
     _RequiredListAnomalousLogGroupsRequestRequestTypeDef,
     _OptionalListAnomalousLogGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 ListInsightsOngoingStatusFilterTypeDef = TypedDict(
     "ListInsightsOngoingStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
     },
 )
 
@@ -681,22 +801,52 @@
     "ListMonitoredResourcesFiltersTypeDef",
     {
         "ResourcePermission": ResourcePermissionType,
         "ResourceTypeFilters": Sequence[ResourceTypeFilterType],
     },
 )
 
+ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNotificationChannelsRequestRequestTypeDef = TypedDict(
     "ListNotificationChannelsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "Locale": LocaleType,
+        "AccountId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
+    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -705,22 +855,20 @@
         "NextToken": str,
         "Locale": LocaleType,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 LogAnomalyClassTypeDef = TypedDict(
     "LogAnomalyClassTypeDef",
     {
         "LogStreamName": str,
         "LogAnomalyType": LogAnomalyTypeType,
         "LogAnomalyToken": str,
         "LogEventId": str,
@@ -776,14 +924,24 @@
     "OpsCenterIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
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
 PerformanceInsightsMetricDimensionGroupTypeDef = TypedDict(
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     {
         "Group": str,
         "Dimensions": List[str],
         "Limit": int,
     },
@@ -817,21 +975,19 @@
     "_OptionalPredictionTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
-
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -874,14 +1030,25 @@
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
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
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
@@ -908,64 +1075,14 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
-AddNotificationChannelResponseTypeDef = TypedDict(
-    "AddNotificationChannelResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountHealthResponseTypeDef = TypedDict(
-    "DescribeAccountHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "AnalyzedResourceCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountOverviewResponseTypeDef = TypedDict(
-    "DescribeAccountOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "MeanTimeToRecoverInMilliseconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOrganizationHealthResponseTypeDef = TypedDict(
-    "DescribeOrganizationHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOrganizationOverviewResponseTypeDef = TypedDict(
-    "DescribeOrganizationOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
     total=False,
 )
@@ -1009,157 +1126,26 @@
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "MaxResults": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-
-GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
-    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
-    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-):
-    pass
-
-
-ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "Locale": LocaleType,
-        "AccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
-    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
-):
-    pass
-
-
 ListInsightsClosedStatusFilterTypeDef = TypedDict(
     "ListInsightsClosedStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
         "EndTimeRange": EndTimeRangeTypeDef,
     },
 )
@@ -1180,15 +1166,15 @@
     },
 )
 
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMonitoredResourcesRequestRequestTypeDef = TypedDict(
     "ListMonitoredResourcesRequestRequestTypeDef",
     {
@@ -1217,35 +1203,35 @@
     "_OptionalNotificationChannelConfigTypeDef",
     {
         "Filters": NotificationFilterConfigTypeDef,
     },
     total=False,
 )
 
-
 class NotificationChannelConfigTypeDef(
     _RequiredNotificationChannelConfigTypeDef, _OptionalNotificationChannelConfigTypeDef
 ):
     pass
 
-
 UpdateServiceIntegrationConfigTypeDef = TypedDict(
     "UpdateServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationConfigTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationConfigTypeDef,
+        "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationConfigTypeDef,
     },
     total=False,
 )
 
 ServiceIntegrationConfigTypeDef = TypedDict(
     "ServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationTypeDef,
+        "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationTypeDef,
     },
     total=False,
 )
 
 PerformanceInsightsMetricQueryTypeDef = TypedDict(
     "PerformanceInsightsMetricQueryTypeDef",
     {
@@ -1310,15 +1296,15 @@
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
@@ -1345,15 +1331,15 @@
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
@@ -1363,47 +1349,43 @@
     "_OptionalStartCostEstimationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
@@ -1414,22 +1396,20 @@
         "NextToken": str,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
     },
     total=False,
 )
 
-
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
-
 ListInsightsStatusFilterTypeDef = TypedDict(
     "ListInsightsStatusFilterTypeDef",
     {
         "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
         "Closed": ListInsightsClosedStatusFilterTypeDef,
         "Any": ListInsightsAnyStatusFilterTypeDef,
     },
@@ -1471,15 +1451,15 @@
     },
 )
 
 DescribeServiceIntegrationResponseTypeDef = TypedDict(
     "DescribeServiceIntegrationResponseTypeDef",
     {
         "ServiceIntegration": ServiceIntegrationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PerformanceInsightsReferenceMetricTypeDef = TypedDict(
     "PerformanceInsightsReferenceMetricTypeDef",
     {
         "MetricQuery": PerformanceInsightsMetricQueryTypeDef,
@@ -1498,15 +1478,15 @@
 )
 
 GetResourceCollectionResponseTypeDef = TypedDict(
     "GetResourceCollectionResponseTypeDef",
     {
         "ResourceCollection": ResourceCollectionFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "ResourceCollection": ResourceCollectionTypeDef,
@@ -1667,26 +1647,26 @@
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "Account": List[AccountHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourceCollectionHealthResponseTypeDef = TypedDict(
     "DescribeResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceCollectionRequestRequestTypeDef = TypedDict(
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
@@ -1699,27 +1679,25 @@
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestRequestTypeDef = TypedDict(
@@ -1727,45 +1705,41 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListInsightsRequestRequestTypeDef(
     _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
@@ -1775,38 +1749,36 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListOrganizationInsightsRequestRequestTypeDef(
     _RequiredListOrganizationInsightsRequestRequestTypeDef,
     _OptionalListOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotificationChannelsResponseTypeDef = TypedDict(
     "ListNotificationChannelsResponseTypeDef",
     {
         "Channels": List[NotificationChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PerformanceInsightsReferenceComparisonValuesTypeDef = TypedDict(
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     {
         "ReferenceScalar": PerformanceInsightsReferenceScalarTypeDef,
@@ -1830,41 +1802,39 @@
 )
 
 ListEventsResponseTypeDef = TypedDict(
     "ListEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_RequiredListEventsRequestListEventsPaginateTypeDef",
     {
         "Filters": ListEventsFiltersTypeDef,
     },
 )
 _OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_OptionalListEventsRequestListEventsPaginateTypeDef",
     {
         "AccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListEventsRequestListEventsPaginateTypeDef(
     _RequiredListEventsRequestListEventsPaginateTypeDef,
     _OptionalListEventsRequestListEventsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventsRequestRequestTypeDef",
     {
         "Filters": ListEventsFiltersTypeDef,
     },
 )
 _OptionalListEventsRequestRequestTypeDef = TypedDict(
@@ -1873,76 +1843,74 @@
         "MaxResults": int,
         "NextToken": str,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ListEventsRequestRequestTypeDef(
     _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
 ):
     pass
 
-
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInsightsResponseTypeDef = TypedDict(
     "ListInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchInsightsResponseTypeDef = TypedDict(
     "SearchInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchOrganizationInsightsResponseTypeDef = TypedDict(
     "SearchOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInsightResponseTypeDef = TypedDict(
     "DescribeInsightResponseTypeDef",
     {
         "ProactiveInsight": ProactiveInsightTypeDef,
         "ReactiveInsight": ReactiveInsightTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOrganizationInsightsResponseTypeDef = TypedDict(
     "ListOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
@@ -1955,45 +1923,41 @@
         "Filters": SearchInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchInsightsRequestRequestTypeDef(
     _RequiredSearchInsightsRequestRequestTypeDef, _OptionalSearchInsightsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "Filters": SearchInsightsFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -2004,62 +1968,58 @@
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchOrganizationInsightsRequestRequestTypeDef(
     _RequiredSearchOrganizationInsightsRequestRequestTypeDef,
     _OptionalSearchOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
-
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PerformanceInsightsMetricsDetailTypeDef = TypedDict(
     "PerformanceInsightsMetricsDetailTypeDef",
     {
         "MetricDisplayName": str,
@@ -2165,19 +2125,19 @@
 
 ListAnomaliesForInsightResponseTypeDef = TypedDict(
     "ListAnomaliesForInsightResponseTypeDef",
     {
         "ProactiveAnomalies": List[ProactiveAnomalySummaryTypeDef],
         "ReactiveAnomalies": List[ReactiveAnomalySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAnomalyResponseTypeDef = TypedDict(
     "DescribeAnomalyResponseTypeDef",
     {
         "ProactiveAnomaly": ProactiveAnomalyTypeDef,
         "ReactiveAnomaly": ReactiveAnomalyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.pyi` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,104 +34,108 @@
     LogAnomalyTypeType,
     NotificationMessageTypeType,
     OptInStatusType,
     OrganizationResourceCollectionTypeType,
     ResourceCollectionTypeType,
     ResourcePermissionType,
     ResourceTypeFilterType,
+    ServerSideEncryptionTypeType,
     ServiceNameType,
     UpdateResourceCollectionActionType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountInsightHealthTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddNotificationChannelResponseTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
     "CloudFormationCollectionTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
+    "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
+    "DescribeAccountOverviewResponseTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
+    "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeOrganizationOverviewResponseTypeDef",
+    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
+    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
     "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
     "EventTimeRangeTypeDef",
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
+    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
     "InsightTimeRangeTypeDef",
+    "KMSServerSideEncryptionIntegrationConfigTypeDef",
+    "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
     "StartTimeRangeTypeDef",
+    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
+    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
     "NotificationFilterConfigTypeDef",
     "SnsChannelConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
+    "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
     "TagCollectionTypeDef",
+    "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
-    "AddNotificationChannelResponseTypeDef",
-    "DescribeAccountHealthResponseTypeDef",
-    "DescribeAccountOverviewResponseTypeDef",
-    "DescribeOrganizationHealthResponseTypeDef",
-    "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeFeedbackResponseTypeDef",
     "PutFeedbackRequestRequestTypeDef",
-    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListInsightsClosedStatusFilterTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
     "NotificationChannelConfigTypeDef",
@@ -212,22 +216,19 @@
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddNotificationChannelResponseTypeDef = TypedDict(
+    "AddNotificationChannelResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
@@ -245,19 +246,21 @@
     "_OptionalAnomalyReportedTimeRangeTypeDef",
     {
         "CloseTime": datetime,
     },
     total=False,
 )
 
+
 class AnomalyReportedTimeRangeTypeDef(
     _RequiredAnomalyReportedTimeRangeTypeDef, _OptionalAnomalyReportedTimeRangeTypeDef
 ):
     pass
 
+
 AnomalyResourceTypeDef = TypedDict(
     "AnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -283,17 +286,19 @@
     "_OptionalAnomalyTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class AnomalyTimeRangeTypeDef(_RequiredAnomalyTimeRangeTypeDef, _OptionalAnomalyTimeRangeTypeDef):
     pass
 
+
 CloudFormationCollectionFilterTypeDef = TypedDict(
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
@@ -362,53 +367,79 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DescribeAccountHealthResponseTypeDef = TypedDict(
+    "DescribeAccountHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "AnalyzedResourceCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
     {
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeAccountOverviewResponseTypeDef = TypedDict(
+    "DescribeAccountOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "MeanTimeToRecoverInMilliseconds": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeAnomalyRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DescribeAnomalyRequestRequestTypeDef(
     _RequiredDescribeAnomalyRequestRequestTypeDef, _OptionalDescribeAnomalyRequestRequestTypeDef
 ):
     pass
 
+
 DescribeFeedbackRequestRequestTypeDef = TypedDict(
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
@@ -432,28 +463,41 @@
     "_OptionalDescribeInsightRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DescribeInsightRequestRequestTypeDef(
     _RequiredDescribeInsightRequestRequestTypeDef, _OptionalDescribeInsightRequestRequestTypeDef
 ):
     pass
 
+
 DescribeOrganizationHealthRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationHealthRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
+DescribeOrganizationHealthResponseTypeDef = TypedDict(
+    "DescribeOrganizationHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
@@ -462,30 +506,56 @@
         "ToTime": Union[datetime, str],
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+DescribeOrganizationOverviewResponseTypeDef = TypedDict(
+    "DescribeOrganizationOverviewResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -495,40 +565,66 @@
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+
 EndTimeRangeTypeDef = TypedDict(
     "EndTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
@@ -548,14 +644,22 @@
     "EventTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
 )
 
+GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -568,51 +672,97 @@
         "Count": int,
         "UnitCost": float,
         "Cost": float,
     },
     total=False,
 )
 
+_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
+    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetResourceCollectionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
     "_OptionalInsightTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class InsightTimeRangeTypeDef(_RequiredInsightTimeRangeTypeDef, _OptionalInsightTimeRangeTypeDef):
     pass
 
+
+KMSServerSideEncryptionIntegrationConfigTypeDef = TypedDict(
+    "KMSServerSideEncryptionIntegrationConfigTypeDef",
+    {
+        "KMSKeyId": str,
+        "OptInStatus": OptInStatusType,
+        "Type": ServerSideEncryptionTypeType,
+    },
+    total=False,
+)
+
+KMSServerSideEncryptionIntegrationTypeDef = TypedDict(
+    "KMSServerSideEncryptionIntegrationTypeDef",
+    {
+        "KMSKeyId": str,
+        "OptInStatus": OptInStatusType,
+        "Type": ServerSideEncryptionTypeType,
+    },
+    total=False,
+)
+
 ServiceCollectionTypeDef = TypedDict(
     "ServiceCollectionTypeDef",
     {
         "ServiceNames": Sequence[ServiceNameType],
     },
     total=False,
 )
@@ -622,14 +772,36 @@
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
+    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -637,20 +809,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalousLogGroupsRequestRequestTypeDef(
     _RequiredListAnomalousLogGroupsRequestRequestTypeDef,
     _OptionalListAnomalousLogGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 ListInsightsOngoingStatusFilterTypeDef = TypedDict(
     "ListInsightsOngoingStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
     },
 )
 
@@ -658,22 +832,54 @@
     "ListMonitoredResourcesFiltersTypeDef",
     {
         "ResourcePermission": ResourcePermissionType,
         "ResourceTypeFilters": Sequence[ResourceTypeFilterType],
     },
 )
 
+ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNotificationChannelsRequestRequestTypeDef = TypedDict(
     "ListNotificationChannelsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "Locale": LocaleType,
+        "AccountId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
+    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -682,20 +888,22 @@
         "NextToken": str,
         "Locale": LocaleType,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 LogAnomalyClassTypeDef = TypedDict(
     "LogAnomalyClassTypeDef",
     {
         "LogStreamName": str,
         "LogAnomalyType": LogAnomalyTypeType,
         "LogAnomalyToken": str,
         "LogEventId": str,
@@ -751,14 +959,24 @@
     "OpsCenterIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
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
 PerformanceInsightsMetricDimensionGroupTypeDef = TypedDict(
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     {
         "Group": str,
         "Dimensions": List[str],
         "Limit": int,
     },
@@ -792,19 +1010,21 @@
     "_OptionalPredictionTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
+
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -847,14 +1067,25 @@
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
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
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
@@ -881,64 +1112,14 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
-AddNotificationChannelResponseTypeDef = TypedDict(
-    "AddNotificationChannelResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountHealthResponseTypeDef = TypedDict(
-    "DescribeAccountHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "AnalyzedResourceCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountOverviewResponseTypeDef = TypedDict(
-    "DescribeAccountOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "MeanTimeToRecoverInMilliseconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOrganizationHealthResponseTypeDef = TypedDict(
-    "DescribeOrganizationHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOrganizationOverviewResponseTypeDef = TypedDict(
-    "DescribeOrganizationOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
     total=False,
 )
@@ -982,147 +1163,26 @@
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "MaxResults": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
-    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-):
-    pass
-
-_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
-    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-):
-    pass
-
-ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "Locale": LocaleType,
-        "AccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
-    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
-):
-    pass
-
 ListInsightsClosedStatusFilterTypeDef = TypedDict(
     "ListInsightsClosedStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
         "EndTimeRange": EndTimeRangeTypeDef,
     },
 )
@@ -1143,15 +1203,15 @@
     },
 )
 
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMonitoredResourcesRequestRequestTypeDef = TypedDict(
     "ListMonitoredResourcesRequestRequestTypeDef",
     {
@@ -1180,33 +1240,37 @@
     "_OptionalNotificationChannelConfigTypeDef",
     {
         "Filters": NotificationFilterConfigTypeDef,
     },
     total=False,
 )
 
+
 class NotificationChannelConfigTypeDef(
     _RequiredNotificationChannelConfigTypeDef, _OptionalNotificationChannelConfigTypeDef
 ):
     pass
 
+
 UpdateServiceIntegrationConfigTypeDef = TypedDict(
     "UpdateServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationConfigTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationConfigTypeDef,
+        "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationConfigTypeDef,
     },
     total=False,
 )
 
 ServiceIntegrationConfigTypeDef = TypedDict(
     "ServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationTypeDef,
+        "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationTypeDef,
     },
     total=False,
 )
 
 PerformanceInsightsMetricQueryTypeDef = TypedDict(
     "PerformanceInsightsMetricQueryTypeDef",
     {
@@ -1271,15 +1335,15 @@
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
@@ -1306,15 +1370,15 @@
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
@@ -1324,43 +1388,47 @@
     "_OptionalStartCostEstimationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
@@ -1371,20 +1439,22 @@
         "NextToken": str,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
     },
     total=False,
 )
 
+
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
+
 ListInsightsStatusFilterTypeDef = TypedDict(
     "ListInsightsStatusFilterTypeDef",
     {
         "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
         "Closed": ListInsightsClosedStatusFilterTypeDef,
         "Any": ListInsightsAnyStatusFilterTypeDef,
     },
@@ -1426,15 +1496,15 @@
     },
 )
 
 DescribeServiceIntegrationResponseTypeDef = TypedDict(
     "DescribeServiceIntegrationResponseTypeDef",
     {
         "ServiceIntegration": ServiceIntegrationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PerformanceInsightsReferenceMetricTypeDef = TypedDict(
     "PerformanceInsightsReferenceMetricTypeDef",
     {
         "MetricQuery": PerformanceInsightsMetricQueryTypeDef,
@@ -1453,15 +1523,15 @@
 )
 
 GetResourceCollectionResponseTypeDef = TypedDict(
     "GetResourceCollectionResponseTypeDef",
     {
         "ResourceCollection": ResourceCollectionFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "ResourceCollection": ResourceCollectionTypeDef,
@@ -1622,26 +1692,26 @@
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "Account": List[AccountHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourceCollectionHealthResponseTypeDef = TypedDict(
     "DescribeResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceCollectionRequestRequestTypeDef = TypedDict(
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
@@ -1654,25 +1724,27 @@
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestRequestTypeDef = TypedDict(
@@ -1680,41 +1752,45 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListInsightsRequestRequestTypeDef(
     _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
@@ -1724,36 +1800,38 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListOrganizationInsightsRequestRequestTypeDef(
     _RequiredListOrganizationInsightsRequestRequestTypeDef,
     _OptionalListOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
+
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotificationChannelsResponseTypeDef = TypedDict(
     "ListNotificationChannelsResponseTypeDef",
     {
         "Channels": List[NotificationChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PerformanceInsightsReferenceComparisonValuesTypeDef = TypedDict(
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     {
         "ReferenceScalar": PerformanceInsightsReferenceScalarTypeDef,
@@ -1777,39 +1855,41 @@
 )
 
 ListEventsResponseTypeDef = TypedDict(
     "ListEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_RequiredListEventsRequestListEventsPaginateTypeDef",
     {
         "Filters": ListEventsFiltersTypeDef,
     },
 )
 _OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_OptionalListEventsRequestListEventsPaginateTypeDef",
     {
         "AccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListEventsRequestListEventsPaginateTypeDef(
     _RequiredListEventsRequestListEventsPaginateTypeDef,
     _OptionalListEventsRequestListEventsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventsRequestRequestTypeDef",
     {
         "Filters": ListEventsFiltersTypeDef,
     },
 )
 _OptionalListEventsRequestRequestTypeDef = TypedDict(
@@ -1818,74 +1898,76 @@
         "MaxResults": int,
         "NextToken": str,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ListEventsRequestRequestTypeDef(
     _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
 ):
     pass
 
+
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInsightsResponseTypeDef = TypedDict(
     "ListInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchInsightsResponseTypeDef = TypedDict(
     "SearchInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchOrganizationInsightsResponseTypeDef = TypedDict(
     "SearchOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInsightResponseTypeDef = TypedDict(
     "DescribeInsightResponseTypeDef",
     {
         "ProactiveInsight": ProactiveInsightTypeDef,
         "ReactiveInsight": ReactiveInsightTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOrganizationInsightsResponseTypeDef = TypedDict(
     "ListOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
@@ -1898,41 +1980,45 @@
         "Filters": SearchInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchInsightsRequestRequestTypeDef(
     _RequiredSearchInsightsRequestRequestTypeDef, _OptionalSearchInsightsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "Filters": SearchInsightsFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -1943,58 +2029,62 @@
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchOrganizationInsightsRequestRequestTypeDef(
     _RequiredSearchOrganizationInsightsRequestRequestTypeDef,
     _OptionalSearchOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PerformanceInsightsMetricsDetailTypeDef = TypedDict(
     "PerformanceInsightsMetricsDetailTypeDef",
     {
         "MetricDisplayName": str,
@@ -2100,19 +2190,19 @@
 
 ListAnomaliesForInsightResponseTypeDef = TypedDict(
     "ListAnomaliesForInsightResponseTypeDef",
     {
         "ProactiveAnomalies": List[ProactiveAnomalySummaryTypeDef],
         "ReactiveAnomalies": List[ReactiveAnomalySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAnomalyResponseTypeDef = TypedDict(
     "DescribeAnomalyResponseTypeDef",
     {
         "ProactiveAnomaly": ProactiveAnomalyTypeDef,
         "ReactiveAnomaly": ReactiveAnomalyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/PKG-INFO` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.26.80
-Summary: Type annotations for boto3.DevOpsGuru 1.26.80 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.DevOpsGuru 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-devops-guru"></a>
 
 # mypy-boto3-devops-guru
 
 [![PyPI - mypy-boto3-devops-guru](https://img.shields.io/pypi/v/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,14 +382,15 @@
     OptInStatusType,
     OrganizationResourceCollectionTypeType,
     ResourceCollectionTypeType,
     ResourcePermissionType,
     ResourceTypeFilterType,
     SearchInsightsPaginatorName,
     SearchOrganizationInsightsPaginatorName,
+    ServerSideEncryptionTypeType,
     ServiceNameType,
     UpdateResourceCollectionActionType,
     DevOpsGuruServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -406,93 +407,95 @@
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    ResponseMetadataTypeDef,
+    AddNotificationChannelResponseTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
     CloudFormationCollectionTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
+    DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
     EndTimeRangeTypeDef,
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
+    KMSServerSideEncryptionIntegrationConfigTypeDef,
+    KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
     NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
+    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
     TagCollectionTypeDef,
+    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
-    DescribeAccountHealthResponseTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigTypeDef,
@@ -576,42 +579,42 @@
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

### Comparing `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/SOURCES.txt` & `mypy-boto3-devops-guru-1.27.0/mypy_boto3_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.80/setup.py` & `mypy-boto3-devops-guru-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-devops-guru.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devops-guru",
-    version="1.26.80",
+    version="1.27.0",
     packages=["mypy_boto3_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DevOpsGuru 1.26.80 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.DevOpsGuru 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/",
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


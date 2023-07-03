# Comparing `tmp/mypy-boto3-xray-1.26.9.tar.gz` & `tmp/mypy-boto3-xray-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-xray-1.26.9.tar", last modified: Mon Nov 14 20:49:29 2022, max compression
+gzip compressed data, was "mypy-boto3-xray-1.27.0.tar", last modified: Mon Jul  3 19:51:37 2023, max compression
```

## Comparing `mypy-boto3-xray-1.26.9.tar` & `mypy-boto3-xray-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.632561 mypy-boto3-xray-1.26.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17785 2022-11-14 20:49:29.632561 mypy-boto3-xray-1.26.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16362 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.632561 mypy-boto3-xray-1.26.9/mypy_boto3_xray/
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22880 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    22838 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8928 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8926 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9975 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9965 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    40042 2022-11-14 20:49:19.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    39999 2022-11-14 20:49:18.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.632561 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17785 2022-11-14 20:49:29.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-14 20:49:29.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-14 20:49:29.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-14 20:49:29.000000 mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 20:49:29.632561 mypy-boto3-xray-1.26.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-11-14 20:49:17.000000 mypy-boto3-xray-1.26.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.540167 mypy-boto3-xray-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-03 19:51:37.540167 mypy-boto3-xray-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.540167 mypy-boto3-xray-1.27.0/mypy_boto3_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-07-03 19:49:59.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43345 2023-07-03 19:50:02.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-07-03 19:50:02.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.540167 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-03 19:51:37.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 19:51:37.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:37.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:37.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:37.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:37.000000 mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:37.540167 mypy-boto3-xray-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 19:49:58.000000 mypy-boto3-xray-1.27.0/setup.py
```

### Comparing `mypy-boto3-xray-1.26.9/LICENSE` & `mypy-boto3-xray-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-xray-1.26.9/PKG-INFO` & `mypy-boto3-xray-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.26.9
-Summary: Type annotations for boto3.XRay 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.XRay 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
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
 
 <a id="mypy-boto3-xray"></a>
 
 # mypy-boto3-xray
 
 [![PyPI - mypy-boto3-xray](https://img.shields.io/pypi/v/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-xray?color=blue)](https://pypistats.org/packages/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,14 +287,16 @@
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 
 client: XRayClient = Session().client("xray")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
@@ -306,14 +309,20 @@
 get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = (
     client.get_paginator("get_time_series_service_statistics")
 )
 get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
 get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator(
     "get_trace_summaries"
 )
+list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator(
+    "list_resource_policies"
+)
+list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
+    "list_tags_for_resource"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_xray.literals` module contains literals extracted from shapes that
@@ -329,14 +338,16 @@
     GetSamplingStatisticSummariesPaginatorName,
     GetServiceGraphPaginatorName,
     GetTimeSeriesServiceStatisticsPaginatorName,
     GetTraceGraphPaginatorName,
     GetTraceSummariesPaginatorName,
     InsightCategoryType,
     InsightStateType,
+    ListResourcePoliciesPaginatorName,
+    ListTagsForResourcePaginatorName,
     SamplingStrategyNameType,
     TimeRangeTypeType,
     XRayServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -357,68 +368,74 @@
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    PaginatorConfigTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     BatchGetTracesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
+    DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
     GetInsightImpactGraphRequestRequestTypeDef,
     GetInsightRequestRequestTypeDef,
     GetInsightSummariesRequestRequestTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListResourcePoliciesRequestRequestTypeDef,
+    ResourcePolicyTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
+    PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
+    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
     TelemetryRecordTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
@@ -431,14 +448,16 @@
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
+    ListResourcePoliciesResultTypeDef,
+    PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
@@ -479,42 +498,42 @@
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

### Comparing `mypy-boto3-xray-1.26.9/README.md` & `mypy-boto3-xray-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-xray"></a>
 
 # mypy-boto3-xray
 
 [![PyPI - mypy-boto3-xray](https://img.shields.io/pypi/v/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-xray?color=blue)](https://pypistats.org/packages/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -255,14 +255,16 @@
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 
 client: XRayClient = Session().client("xray")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
@@ -275,14 +277,20 @@
 get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = (
     client.get_paginator("get_time_series_service_statistics")
 )
 get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
 get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator(
     "get_trace_summaries"
 )
+list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator(
+    "list_resource_policies"
+)
+list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
+    "list_tags_for_resource"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_xray.literals` module contains literals extracted from shapes that
@@ -298,14 +306,16 @@
     GetSamplingStatisticSummariesPaginatorName,
     GetServiceGraphPaginatorName,
     GetTimeSeriesServiceStatisticsPaginatorName,
     GetTraceGraphPaginatorName,
     GetTraceSummariesPaginatorName,
     InsightCategoryType,
     InsightStateType,
+    ListResourcePoliciesPaginatorName,
+    ListTagsForResourcePaginatorName,
     SamplingStrategyNameType,
     TimeRangeTypeType,
     XRayServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -326,68 +336,74 @@
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    PaginatorConfigTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     BatchGetTracesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
+    DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
     GetInsightImpactGraphRequestRequestTypeDef,
     GetInsightRequestRequestTypeDef,
     GetInsightSummariesRequestRequestTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListResourcePoliciesRequestRequestTypeDef,
+    ResourcePolicyTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
+    PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
+    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
     TelemetryRecordTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
@@ -400,14 +416,16 @@
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
+    ListResourcePoliciesResultTypeDef,
+    PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
@@ -448,42 +466,42 @@
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

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/__init__.py` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,40 +11,46 @@
         GetGroupsPaginator,
         GetSamplingRulesPaginator,
         GetSamplingStatisticSummariesPaginator,
         GetServiceGraphPaginator,
         GetTimeSeriesServiceStatisticsPaginator,
         GetTraceGraphPaginator,
         GetTraceSummariesPaginator,
+        ListResourcePoliciesPaginator,
+        ListTagsForResourcePaginator,
         XRayClient,
     )
 
     session = Session()
     client: XRayClient = session.client("xray")
 
     batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
     get_groups_paginator: GetGroupsPaginator = client.get_paginator("get_groups")
     get_sampling_rules_paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")
     get_sampling_statistic_summaries_paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")
     get_service_graph_paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")
     get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
     get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
     get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
+    list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
+    list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from .client import XRayClient
 from .paginator import (
     BatchGetTracesPaginator,
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 
 Client = XRayClient
 
 
 __all__ = (
     "BatchGetTracesPaginator",
@@ -52,9 +58,11 @@
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
     "GetServiceGraphPaginator",
     "GetTimeSeriesServiceStatisticsPaginator",
     "GetTraceGraphPaginator",
     "GetTraceSummariesPaginator",
+    "ListResourcePoliciesPaginator",
+    "ListTagsForResourcePaginator",
     "XRayClient",
 )
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/__init__.pyi` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/__init__.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -11,49 +11,57 @@
         GetGroupsPaginator,
         GetSamplingRulesPaginator,
         GetSamplingStatisticSummariesPaginator,
         GetServiceGraphPaginator,
         GetTimeSeriesServiceStatisticsPaginator,
         GetTraceGraphPaginator,
         GetTraceSummariesPaginator,
+        ListResourcePoliciesPaginator,
+        ListTagsForResourcePaginator,
         XRayClient,
     )
 
     session = Session()
     client: XRayClient = session.client("xray")
 
     batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
     get_groups_paginator: GetGroupsPaginator = client.get_paginator("get_groups")
     get_sampling_rules_paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")
     get_sampling_statistic_summaries_paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")
     get_service_graph_paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")
     get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
     get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
     get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
+    list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
+    list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from .client import XRayClient
 from .paginator import (
     BatchGetTracesPaginator,
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 
 Client = XRayClient
 
 __all__ = (
     "BatchGetTracesPaginator",
     "Client",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
     "GetServiceGraphPaginator",
     "GetTimeSeriesServiceStatisticsPaginator",
     "GetTraceGraphPaginator",
     "GetTraceSummariesPaginator",
+    "ListResourcePoliciesPaginator",
+    "ListTagsForResourcePaginator",
     "XRayClient",
 )
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/__main__.py` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.XRay 1.26.9\nVersion:         1.26.9\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.XRay 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.9")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/client.py` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetTracesResultTypeDef,
     CreateGroupResultTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetEncryptionConfigResultTypeDef,
@@ -46,16 +48,18 @@
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetServiceGraphResultTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
+    ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
+    PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     SamplingRuleTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
@@ -64,35 +68,36 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("XRayClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
+    InvalidPolicyRevisionIdException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
+    LockoutPreventionException: Type[BotocoreClientError]
+    MalformedPolicyDocumentException: Type[BotocoreClientError]
+    PolicyCountLimitExceededException: Type[BotocoreClientError]
+    PolicySizeLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     RuleLimitExceededException: Type[BotocoreClientError]
     ThrottledException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class XRayClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/)
     """
 
     meta: ClientMeta
@@ -101,156 +106,150 @@
     def exceptions(self) -> Exceptions:
         """
         XRayClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#exceptions)
         """
-
     def batch_get_traces(
         self, *, TraceIds: Sequence[str], NextToken: str = ...
     ) -> BatchGetTracesResultTypeDef:
         """
         Retrieves a list of traces specified by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.batch_get_traces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#batch_get_traces)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#close)
         """
-
     def create_group(
         self,
         *,
         GroupName: str,
         FilterExpression: str = ...,
         InsightsConfiguration: InsightsConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGroupResultTypeDef:
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_group)
         """
-
     def create_sampling_rule(
         self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_sampling_rule)
         """
-
     def delete_group(self, *, GroupName: str = ..., GroupARN: str = ...) -> Dict[str, Any]:
         """
         Deletes a group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.delete_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#delete_group)
         """
+    def delete_resource_policy(
+        self, *, PolicyName: str, PolicyRevisionId: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes a resource policy from the target Amazon Web Services account.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.delete_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#delete_resource_policy)
+        """
     def delete_sampling_rule(
         self, *, RuleName: str = ..., RuleARN: str = ...
     ) -> DeleteSamplingRuleResultTypeDef:
         """
         Deletes a sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.delete_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#delete_sampling_rule)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#generate_presigned_url)
         """
-
     def get_encryption_config(self) -> GetEncryptionConfigResultTypeDef:
         """
         Retrieves the current encryption configuration for X-Ray data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_encryption_config)
         """
-
     def get_group(self, *, GroupName: str = ..., GroupARN: str = ...) -> GetGroupResultTypeDef:
         """
         Retrieves group resource details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_group)
         """
-
     def get_groups(self, *, NextToken: str = ...) -> GetGroupsResultTypeDef:
         """
         Retrieves all active group details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_groups)
         """
-
     def get_insight(self, *, InsightId: str) -> GetInsightResultTypeDef:
         """
         Retrieves the summary information of an insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight)
         """
-
     def get_insight_events(
         self, *, InsightId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetInsightEventsResultTypeDef:
         """
         X-Ray reevaluates insights periodically until they're resolved, and records each
         intermediate state as an event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_events)
         """
-
     def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         NextToken: str = ...
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_impact_graph)
         """
-
     def get_insight_summaries(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
@@ -261,44 +260,40 @@
         """
         Retrieves the summaries of all insights in the specified group matching the
         provided filter values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_summaries)
         """
-
     def get_sampling_rules(self, *, NextToken: str = ...) -> GetSamplingRulesResultTypeDef:
         """
         Retrieves all sampling rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_rules)
         """
-
     def get_sampling_statistic_summaries(
         self, *, NextToken: str = ...
     ) -> GetSamplingStatisticSummariesResultTypeDef:
         """
         Retrieves information about recent sampling results for all sampling rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_statistic_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_statistic_summaries)
         """
-
     def get_sampling_targets(
         self, *, SamplingStatisticsDocuments: Sequence[SamplingStatisticsDocumentTypeDef]
     ) -> GetSamplingTargetsResultTypeDef:
         """
         Requests a sampling quota for rules that the service is using to sample
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_targets)
         """
-
     def get_service_graph(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
@@ -307,15 +302,14 @@
         """
         Retrieves a document that describes services that process incoming requests, and
         downstream services that they call as a result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_service_graph)
         """
-
     def get_time_series_service_statistics(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
@@ -326,25 +320,23 @@
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
         """
         Get an aggregation of service statistics defined by a specific time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_time_series_service_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_time_series_service_statistics)
         """
-
     def get_trace_graph(
         self, *, TraceIds: Sequence[str], NextToken: str = ...
     ) -> GetTraceGraphResultTypeDef:
         """
         Retrieves a service graph for one or more specific trace IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_trace_graph)
         """
-
     def get_trace_summaries(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
@@ -355,160 +347,182 @@
         """
         Retrieves IDs and annotations for traces available for a specified time frame
         using an optional filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_trace_summaries)
         """
+    def list_resource_policies(self, *, NextToken: str = ...) -> ListResourcePoliciesResultTypeDef:
+        """
+        Returns the list of resource policies in the target Amazon Web Services account.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.list_resource_policies)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#list_resource_policies)
+        """
     def list_tags_for_resource(
         self, *, ResourceARN: str, NextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags that are applied to the specified Amazon Web Services
         X-Ray group or sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#list_tags_for_resource)
         """
-
     def put_encryption_config(
         self, *, Type: EncryptionTypeType, KeyId: str = ...
     ) -> PutEncryptionConfigResultTypeDef:
         """
         Updates the encryption configuration for X-Ray data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_encryption_config)
         """
+    def put_resource_policy(
+        self,
+        *,
+        PolicyName: str,
+        PolicyDocument: str,
+        PolicyRevisionId: str = ...,
+        BypassPolicyLockoutCheck: bool = ...
+    ) -> PutResourcePolicyResultTypeDef:
+        """
+        Sets the resource policy to grant one or more Amazon Web Services services and
+        accounts permissions to access X-Ray.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_resource_policy)
+        """
     def put_telemetry_records(
         self,
         *,
         TelemetryRecords: Sequence[TelemetryRecordTypeDef],
         EC2InstanceId: str = ...,
         Hostname: str = ...,
         ResourceARN: str = ...
     ) -> Dict[str, Any]:
         """
         Used by the Amazon Web Services X-Ray daemon to upload telemetry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_telemetry_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_telemetry_records)
         """
-
     def put_trace_segments(
         self, *, TraceSegmentDocuments: Sequence[str]
     ) -> PutTraceSegmentsResultTypeDef:
         """
         Uploads segment documents to Amazon Web Services X-Ray.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_trace_segments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_trace_segments)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Applies tags to an existing Amazon Web Services X-Ray group or sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an Amazon Web Services X-Ray group or sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#untag_resource)
         """
-
     def update_group(
         self,
         *,
         GroupName: str = ...,
         GroupARN: str = ...,
         FilterExpression: str = ...,
         InsightsConfiguration: InsightsConfigurationTypeDef = ...
     ) -> UpdateGroupResultTypeDef:
         """
         Updates a group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.update_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#update_group)
         """
-
     def update_sampling_rule(
         self, *, SamplingRuleUpdate: SamplingRuleUpdateTypeDef
     ) -> UpdateSamplingRuleResultTypeDef:
         """
         Modifies a sampling rule's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.update_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#update_sampling_rule)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["batch_get_traces"]) -> BatchGetTracesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_groups"]) -> GetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_sampling_rules"]
     ) -> GetSamplingRulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_sampling_statistic_summaries"]
     ) -> GetSamplingStatisticSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_service_graph"]
     ) -> GetServiceGraphPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_time_series_service_statistics"]
     ) -> GetTimeSeriesServiceStatisticsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_trace_graph"]) -> GetTraceGraphPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_trace_summaries"]
     ) -> GetTraceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_resource_policies"]
+    ) -> ListResourcePoliciesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_tags_for_resource"]
+    ) -> ListTagsForResourcePaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/client.pyi` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetTracesResultTypeDef,
     CreateGroupResultTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetEncryptionConfigResultTypeDef,
@@ -46,16 +48,18 @@
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetServiceGraphResultTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
+    ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
+    PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     SamplingRuleTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
@@ -64,31 +68,40 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("XRayClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
+    InvalidPolicyRevisionIdException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
+    LockoutPreventionException: Type[BotocoreClientError]
+    MalformedPolicyDocumentException: Type[BotocoreClientError]
+    PolicyCountLimitExceededException: Type[BotocoreClientError]
+    PolicySizeLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     RuleLimitExceededException: Type[BotocoreClientError]
     ThrottledException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class XRayClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/)
     """
 
     meta: ClientMeta
@@ -97,141 +110,166 @@
     def exceptions(self) -> Exceptions:
         """
         XRayClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#exceptions)
         """
+
     def batch_get_traces(
         self, *, TraceIds: Sequence[str], NextToken: str = ...
     ) -> BatchGetTracesResultTypeDef:
         """
         Retrieves a list of traces specified by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.batch_get_traces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#batch_get_traces)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#close)
         """
+
     def create_group(
         self,
         *,
         GroupName: str,
         FilterExpression: str = ...,
         InsightsConfiguration: InsightsConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGroupResultTypeDef:
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_group)
         """
+
     def create_sampling_rule(
         self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_sampling_rule)
         """
+
     def delete_group(self, *, GroupName: str = ..., GroupARN: str = ...) -> Dict[str, Any]:
         """
         Deletes a group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.delete_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#delete_group)
         """
+
+    def delete_resource_policy(
+        self, *, PolicyName: str, PolicyRevisionId: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes a resource policy from the target Amazon Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.delete_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#delete_resource_policy)
+        """
+
     def delete_sampling_rule(
         self, *, RuleName: str = ..., RuleARN: str = ...
     ) -> DeleteSamplingRuleResultTypeDef:
         """
         Deletes a sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.delete_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#delete_sampling_rule)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#generate_presigned_url)
         """
+
     def get_encryption_config(self) -> GetEncryptionConfigResultTypeDef:
         """
         Retrieves the current encryption configuration for X-Ray data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_encryption_config)
         """
+
     def get_group(self, *, GroupName: str = ..., GroupARN: str = ...) -> GetGroupResultTypeDef:
         """
         Retrieves group resource details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_group)
         """
+
     def get_groups(self, *, NextToken: str = ...) -> GetGroupsResultTypeDef:
         """
         Retrieves all active group details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_groups)
         """
+
     def get_insight(self, *, InsightId: str) -> GetInsightResultTypeDef:
         """
         Retrieves the summary information of an insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight)
         """
+
     def get_insight_events(
         self, *, InsightId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetInsightEventsResultTypeDef:
         """
         X-Ray reevaluates insights periodically until they're resolved, and records each
         intermediate state as an event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_events)
         """
+
     def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         NextToken: str = ...
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_impact_graph)
         """
+
     def get_insight_summaries(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
@@ -242,40 +280,44 @@
         """
         Retrieves the summaries of all insights in the specified group matching the
         provided filter values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_insight_summaries)
         """
+
     def get_sampling_rules(self, *, NextToken: str = ...) -> GetSamplingRulesResultTypeDef:
         """
         Retrieves all sampling rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_rules)
         """
+
     def get_sampling_statistic_summaries(
         self, *, NextToken: str = ...
     ) -> GetSamplingStatisticSummariesResultTypeDef:
         """
         Retrieves information about recent sampling results for all sampling rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_statistic_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_statistic_summaries)
         """
+
     def get_sampling_targets(
         self, *, SamplingStatisticsDocuments: Sequence[SamplingStatisticsDocumentTypeDef]
     ) -> GetSamplingTargetsResultTypeDef:
         """
         Requests a sampling quota for rules that the service is using to sample
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_sampling_targets)
         """
+
     def get_service_graph(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
@@ -284,14 +326,15 @@
         """
         Retrieves a document that describes services that process incoming requests, and
         downstream services that they call as a result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_service_graph)
         """
+
     def get_time_series_service_statistics(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
@@ -302,23 +345,25 @@
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
         """
         Get an aggregation of service statistics defined by a specific time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_time_series_service_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_time_series_service_statistics)
         """
+
     def get_trace_graph(
         self, *, TraceIds: Sequence[str], NextToken: str = ...
     ) -> GetTraceGraphResultTypeDef:
         """
         Retrieves a service graph for one or more specific trace IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_graph)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_trace_graph)
         """
+
     def get_trace_summaries(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
@@ -329,144 +374,202 @@
         """
         Retrieves IDs and annotations for traces available for a specified time frame
         using an optional filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_trace_summaries)
         """
+
+    def list_resource_policies(self, *, NextToken: str = ...) -> ListResourcePoliciesResultTypeDef:
+        """
+        Returns the list of resource policies in the target Amazon Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.list_resource_policies)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#list_resource_policies)
+        """
+
     def list_tags_for_resource(
         self, *, ResourceARN: str, NextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags that are applied to the specified Amazon Web Services
         X-Ray group or sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#list_tags_for_resource)
         """
+
     def put_encryption_config(
         self, *, Type: EncryptionTypeType, KeyId: str = ...
     ) -> PutEncryptionConfigResultTypeDef:
         """
         Updates the encryption configuration for X-Ray data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_encryption_config)
         """
+
+    def put_resource_policy(
+        self,
+        *,
+        PolicyName: str,
+        PolicyDocument: str,
+        PolicyRevisionId: str = ...,
+        BypassPolicyLockoutCheck: bool = ...
+    ) -> PutResourcePolicyResultTypeDef:
+        """
+        Sets the resource policy to grant one or more Amazon Web Services services and
+        accounts permissions to access X-Ray.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_resource_policy)
+        """
+
     def put_telemetry_records(
         self,
         *,
         TelemetryRecords: Sequence[TelemetryRecordTypeDef],
         EC2InstanceId: str = ...,
         Hostname: str = ...,
         ResourceARN: str = ...
     ) -> Dict[str, Any]:
         """
         Used by the Amazon Web Services X-Ray daemon to upload telemetry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_telemetry_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_telemetry_records)
         """
+
     def put_trace_segments(
         self, *, TraceSegmentDocuments: Sequence[str]
     ) -> PutTraceSegmentsResultTypeDef:
         """
         Uploads segment documents to Amazon Web Services X-Ray.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_trace_segments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#put_trace_segments)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Applies tags to an existing Amazon Web Services X-Ray group or sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an Amazon Web Services X-Ray group or sampling rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#untag_resource)
         """
+
     def update_group(
         self,
         *,
         GroupName: str = ...,
         GroupARN: str = ...,
         FilterExpression: str = ...,
         InsightsConfiguration: InsightsConfigurationTypeDef = ...
     ) -> UpdateGroupResultTypeDef:
         """
         Updates a group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.update_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#update_group)
         """
+
     def update_sampling_rule(
         self, *, SamplingRuleUpdate: SamplingRuleUpdateTypeDef
     ) -> UpdateSamplingRuleResultTypeDef:
         """
         Modifies a sampling rule's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.update_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#update_sampling_rule)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["batch_get_traces"]) -> BatchGetTracesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_groups"]) -> GetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_sampling_rules"]
     ) -> GetSamplingRulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_sampling_statistic_summaries"]
     ) -> GetSamplingStatisticSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_service_graph"]
     ) -> GetServiceGraphPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_time_series_service_statistics"]
     ) -> GetTimeSeriesServiceStatisticsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_trace_graph"]) -> GetTraceGraphPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_trace_summaries"]
     ) -> GetTraceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_resource_policies"]
+    ) -> ListResourcePoliciesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_tags_for_resource"]
+    ) -> ListTagsForResourcePaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/literals.py` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/literals.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     "GetSamplingStatisticSummariesPaginatorName",
     "GetServiceGraphPaginatorName",
     "GetTimeSeriesServiceStatisticsPaginatorName",
     "GetTraceGraphPaginatorName",
     "GetTraceSummariesPaginatorName",
     "InsightCategoryType",
     "InsightStateType",
+    "ListResourcePoliciesPaginatorName",
+    "ListTagsForResourcePaginatorName",
     "SamplingStrategyNameType",
     "TimeRangeTypeType",
     "XRayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
@@ -50,14 +52,16 @@
 GetSamplingStatisticSummariesPaginatorName = Literal["get_sampling_statistic_summaries"]
 GetServiceGraphPaginatorName = Literal["get_service_graph"]
 GetTimeSeriesServiceStatisticsPaginatorName = Literal["get_time_series_service_statistics"]
 GetTraceGraphPaginatorName = Literal["get_trace_graph"]
 GetTraceSummariesPaginatorName = Literal["get_trace_summaries"]
 InsightCategoryType = Literal["FAULT"]
 InsightStateType = Literal["ACTIVE", "CLOSED"]
+ListResourcePoliciesPaginatorName = Literal["list_resource_policies"]
+ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 SamplingStrategyNameType = Literal["FixedRate", "PartialScan"]
 TimeRangeTypeType = Literal["Event", "TraceId"]
 XRayServiceName = Literal["xray"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -68,23 +72,25 @@
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
@@ -94,30 +100,35 @@
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
@@ -143,14 +154,15 @@
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
@@ -195,51 +207,57 @@
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
@@ -252,14 +270,15 @@
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
@@ -271,28 +290,35 @@
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
@@ -320,56 +346,64 @@
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
@@ -396,30 +430,35 @@
     "get_groups",
     "get_sampling_rules",
     "get_sampling_statistic_summaries",
     "get_service_graph",
     "get_time_series_service_statistics",
     "get_trace_graph",
     "get_trace_summaries",
+    "list_resource_policies",
+    "list_tags_for_resource",
 ]
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
     "eu-central-2",
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

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/literals.pyi` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/literals.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     "GetSamplingStatisticSummariesPaginatorName",
     "GetServiceGraphPaginatorName",
     "GetTimeSeriesServiceStatisticsPaginatorName",
     "GetTraceGraphPaginatorName",
     "GetTraceSummariesPaginatorName",
     "InsightCategoryType",
     "InsightStateType",
+    "ListResourcePoliciesPaginatorName",
+    "ListTagsForResourcePaginatorName",
     "SamplingStrategyNameType",
     "TimeRangeTypeType",
     "XRayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
@@ -48,14 +50,16 @@
 GetSamplingStatisticSummariesPaginatorName = Literal["get_sampling_statistic_summaries"]
 GetServiceGraphPaginatorName = Literal["get_service_graph"]
 GetTimeSeriesServiceStatisticsPaginatorName = Literal["get_time_series_service_statistics"]
 GetTraceGraphPaginatorName = Literal["get_trace_graph"]
 GetTraceSummariesPaginatorName = Literal["get_trace_summaries"]
 InsightCategoryType = Literal["FAULT"]
 InsightStateType = Literal["ACTIVE", "CLOSED"]
+ListResourcePoliciesPaginatorName = Literal["list_resource_policies"]
+ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 SamplingStrategyNameType = Literal["FixedRate", "PartialScan"]
 TimeRangeTypeType = Literal["Event", "TraceId"]
 XRayServiceName = Literal["xray"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -66,23 +70,25 @@
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
@@ -92,30 +98,35 @@
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
@@ -141,14 +152,15 @@
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
@@ -193,51 +205,57 @@
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
@@ -250,14 +268,15 @@
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
@@ -269,28 +288,35 @@
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
@@ -318,56 +344,64 @@
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
@@ -394,30 +428,35 @@
     "get_groups",
     "get_sampling_rules",
     "get_sampling_statistic_summaries",
     "get_service_graph",
     "get_time_series_service_statistics",
     "get_trace_graph",
     "get_trace_summaries",
+    "list_resource_policies",
+    "list_tags_for_resource",
 ]
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
     "eu-central-2",
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

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/paginator.py` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,31 @@
         GetGroupsPaginator,
         GetSamplingRulesPaginator,
         GetSamplingStatisticSummariesPaginator,
         GetServiceGraphPaginator,
         GetTimeSeriesServiceStatisticsPaginator,
         GetTraceGraphPaginator,
         GetTraceSummariesPaginator,
+        ListResourcePoliciesPaginator,
+        ListTagsForResourcePaginator,
     )
 
     session = Session()
     client: XRayClient = session.client("xray")
 
     batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
     get_groups_paginator: GetGroupsPaginator = client.get_paginator("get_groups")
     get_sampling_rules_paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")
     get_sampling_statistic_summaries_paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")
     get_service_graph_paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")
     get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
     get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
     get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
+    list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
+    list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
@@ -44,27 +48,31 @@
     GetGroupsResultTypeDef,
     GetSamplingRulesResultTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetServiceGraphResultTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
+    ListResourcePoliciesResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     SamplingStrategyTypeDef,
 )
 
 __all__ = (
     "BatchGetTracesPaginator",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
     "GetServiceGraphPaginator",
     "GetTimeSeriesServiceStatisticsPaginator",
     "GetTraceGraphPaginator",
     "GetTraceSummariesPaginator",
+    "ListResourcePoliciesPaginator",
+    "ListTagsForResourcePaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -77,60 +85,60 @@
 class BatchGetTracesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[BatchGetTracesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
         """
 
 
 class GetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
         """
 
 
 class GetSamplingRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSamplingRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
         """
 
 
 class GetSamplingStatisticSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSamplingStatisticSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
         """
 
 
@@ -143,15 +151,15 @@
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
         """
 
 
@@ -167,30 +175,30 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 
 class GetTraceGraphPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTraceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
         """
 
 
@@ -205,13 +213,43 @@
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracesummariespaginator)
         """
+
+
+class ListResourcePoliciesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListResourcePoliciesResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
+        """
+
+
+class ListTagsForResourcePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
+    """
+
+    def paginate(
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
+        """
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/paginator.pyi` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/paginator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,31 @@
         GetGroupsPaginator,
         GetSamplingRulesPaginator,
         GetSamplingStatisticSummariesPaginator,
         GetServiceGraphPaginator,
         GetTimeSeriesServiceStatisticsPaginator,
         GetTraceGraphPaginator,
         GetTraceSummariesPaginator,
+        ListResourcePoliciesPaginator,
+        ListTagsForResourcePaginator,
     )
 
     session = Session()
     client: XRayClient = session.client("xray")
 
     batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
     get_groups_paginator: GetGroupsPaginator = client.get_paginator("get_groups")
     get_sampling_rules_paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")
     get_sampling_statistic_summaries_paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")
     get_service_graph_paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")
     get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
     get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
     get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
+    list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
+    list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
@@ -44,27 +48,31 @@
     GetGroupsResultTypeDef,
     GetSamplingRulesResultTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetServiceGraphResultTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
+    ListResourcePoliciesResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     SamplingStrategyTypeDef,
 )
 
 __all__ = (
     "BatchGetTracesPaginator",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
     "GetServiceGraphPaginator",
     "GetTimeSeriesServiceStatisticsPaginator",
     "GetTraceGraphPaginator",
     "GetTraceSummariesPaginator",
+    "ListResourcePoliciesPaginator",
+    "ListTagsForResourcePaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
@@ -74,57 +82,57 @@
 class BatchGetTracesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[BatchGetTracesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
         """
 
 class GetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
         """
 
 class GetSamplingRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSamplingRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
         """
 
 class GetSamplingStatisticSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSamplingStatisticSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
         """
 
 class GetServiceGraphPaginator(Paginator):
@@ -136,15 +144,15 @@
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
         """
 
 class GetTimeSeriesServiceStatisticsPaginator(Paginator):
@@ -159,29 +167,29 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 class GetTraceGraphPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTraceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
         """
 
 class GetTraceSummariesPaginator(Paginator):
@@ -195,13 +203,41 @@
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracesummariespaginator)
         """
+
+class ListResourcePoliciesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListResourcePoliciesResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
+        """
+
+class ListTagsForResourcePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
+    """
+
+    def paginate(
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
+        """
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/type_defs.py` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,68 +35,74 @@
 
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
-    "PaginatorConfigTypeDef",
+    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     "BatchGetTracesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "InsightsConfigurationTypeDef",
     "TagTypeDef",
     "SamplingRuleTypeDef",
     "DeleteGroupRequestRequestTypeDef",
+    "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSamplingRuleRequestRequestTypeDef",
     "ErrorStatisticsTypeDef",
     "FaultStatisticsTypeDef",
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
     "GetInsightImpactGraphRequestRequestTypeDef",
     "GetInsightRequestRequestTypeDef",
     "GetInsightSummariesRequestRequestTypeDef",
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
     "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     "GetServiceGraphRequestRequestTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    "ListResourcePoliciesRequestRequestTypeDef",
+    "ResourcePolicyTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
     "TelemetryRecordTypeDef",
-    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
@@ -109,14 +115,16 @@
     "FaultRootCauseEntityTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
+    "ListResourcePoliciesResultTypeDef",
+    "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
@@ -197,24 +205,36 @@
         "HTTPCode5XXCount": int,
         "UnknownHostCount": int,
         "OtherCount": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
+    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestRequestTypeDef = TypedDict(
@@ -228,25 +248,14 @@
 
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
 ):
     pass
 
 
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
 InsightsConfigurationTypeDef = TypedDict(
     "InsightsConfigurationTypeDef",
     {
         "InsightsEnabled": bool,
         "NotificationsEnabled": bool,
     },
     total=False,
@@ -295,14 +304,36 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
+_RequiredDeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyName": str,
+    },
+)
+_OptionalDeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyRevisionId": str,
+    },
+    total=False,
+)
+
+
+class DeleteResourcePolicyRequestRequestTypeDef(
+    _RequiredDeleteResourcePolicyRequestRequestTypeDef,
+    _OptionalDeleteResourcePolicyRequestRequestTypeDef,
+):
+    pass
+
+
 DeleteSamplingRuleRequestRequestTypeDef = TypedDict(
     "DeleteSamplingRuleRequestRequestTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
     },
     total=False,
@@ -369,14 +400,22 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
+GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetGroupsRequestRequestTypeDef = TypedDict(
     "GetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -457,22 +496,38 @@
 class GetInsightSummariesRequestRequestTypeDef(
     _RequiredGetInsightSummariesRequestRequestTypeDef,
     _OptionalGetInsightSummariesRequestRequestTypeDef,
 ):
     pass
 
 
+GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSamplingStatisticSummariesRequestRequestTypeDef = TypedDict(
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -532,14 +587,39 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -556,14 +636,42 @@
 
 class GetServiceGraphRequestRequestTypeDef(
     _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -584,14 +692,36 @@
 class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
+    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
@@ -652,14 +782,63 @@
     "InstanceIdDetailTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListResourcePoliciesRequestRequestTypeDef = TypedDict(
+    "ListResourcePoliciesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ResourcePolicyTypeDef = TypedDict(
+    "ResourcePolicyTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "PolicyRevisionId": str,
+        "LastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
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
@@ -674,14 +853,24 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
@@ -696,14 +885,37 @@
 class PutEncryptionConfigRequestRequestTypeDef(
     _RequiredPutEncryptionConfigRequestRequestTypeDef,
     _OptionalPutEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyDocument": str,
+    },
+)
+_OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "BypassPolicyLockoutCheck": bool,
+    },
+    total=False,
+)
+
+
+class PutResourcePolicyRequestRequestTypeDef(
+    _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
+):
+    pass
+
+
 PutTraceSegmentsRequestRequestTypeDef = TypedDict(
     "PutTraceSegmentsRequestRequestTypeDef",
     {
         "TraceSegmentDocuments": Sequence[str],
     },
 )
 
@@ -721,14 +933,25 @@
     "ResourceARNDetailTypeDef",
     {
         "ARN": str,
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
 ResponseTimeRootCauseEntityTypeDef = TypedDict(
     "ResponseTimeRootCauseEntityTypeDef",
     {
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
@@ -816,135 +1039,14 @@
 )
 
 
 class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
     pass
 
 
-_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
-    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-):
-    pass
-
-
-GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
-    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-):
-    pass
-
-
 GroupSummaryTypeDef = TypedDict(
     "GroupSummaryTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -998,15 +1100,15 @@
 
 
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
@@ -1070,23 +1172,23 @@
     total=False,
 )
 
 GetEncryptionConfigResultTypeDef = TypedDict(
     "GetEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEncryptionConfigResultTypeDef = TypedDict(
     "PutEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorRootCauseEntityTypeDef = TypedDict(
     "ErrorRootCauseEntityTypeDef",
     {
         "Name": str,
@@ -1107,15 +1209,15 @@
 )
 
 GetSamplingStatisticSummariesResultTypeDef = TypedDict(
     "GetSamplingStatisticSummariesResultTypeDef",
     {
         "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSamplingTargetsRequestRequestTypeDef = TypedDict(
     "GetSamplingTargetsRequestRequestTypeDef",
     {
         "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
@@ -1124,15 +1226,15 @@
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
         "LastRuleModification": datetime,
         "UnprocessedStatistics": List[UnprocessedStatisticsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "StartTime": Union[datetime, str],
@@ -1142,15 +1244,15 @@
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
@@ -1194,19 +1296,36 @@
         "Names": List[str],
         "AccountId": str,
         "Edges": List[InsightImpactGraphEdgeTypeDef],
     },
     total=False,
 )
 
+ListResourcePoliciesResultTypeDef = TypedDict(
+    "ListResourcePoliciesResultTypeDef",
+    {
+        "ResourcePolicies": List[ResourcePolicyTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutResourcePolicyResultTypeDef = TypedDict(
+    "PutResourcePolicyResultTypeDef",
+    {
+        "ResourcePolicy": ResourcePolicyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseTimeRootCauseServiceTypeDef = TypedDict(
     "ResponseTimeRootCauseServiceTypeDef",
     {
         "Name": str,
@@ -1313,72 +1432,72 @@
 
 
 GetGroupsResultTypeDef = TypedDict(
     "GetGroupsResultTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGroupResultTypeDef = TypedDict(
     "CreateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupResultTypeDef = TypedDict(
     "GetGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupResultTypeDef = TypedDict(
     "UpdateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSamplingRuleResultTypeDef = TypedDict(
     "CreateSamplingRuleResultTypeDef",
     {
         "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSamplingRuleResultTypeDef = TypedDict(
     "DeleteSamplingRuleResultTypeDef",
     {
         "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSamplingRulesResultTypeDef = TypedDict(
     "GetSamplingRulesResultTypeDef",
     {
         "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSamplingRuleResultTypeDef = TypedDict(
     "UpdateSamplingRuleResultTypeDef",
     {
         "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
@@ -1437,15 +1556,15 @@
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
         "ServiceGraphEndTime": datetime,
         "Services": List[InsightImpactGraphServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseTimeRootCauseTypeDef = TypedDict(
     "ResponseTimeRootCauseTypeDef",
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
@@ -1456,41 +1575,41 @@
 
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightEventsResultTypeDef = TypedDict(
     "GetInsightEventsResultTypeDef",
     {
         "InsightEvents": List[InsightEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightSummariesResultTypeDef = TypedDict(
     "GetInsightSummariesResultTypeDef",
     {
         "InsightSummaries": List[InsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightResultTypeDef = TypedDict(
     "GetInsightResultTypeDef",
     {
         "Insight": InsightTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "ReferenceId": int,
@@ -1512,15 +1631,15 @@
 
 GetTimeSeriesServiceStatisticsResultTypeDef = TypedDict(
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     {
         "TimeSeriesServiceStatistics": List[TimeSeriesServiceStatisticsTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorRootCauseTypeDef = TypedDict(
     "ErrorRootCauseTypeDef",
     {
         "Services": List[ErrorRootCauseServiceTypeDef],
@@ -1542,24 +1661,24 @@
     "GetServiceGraphResultTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
         "Services": List[ServiceTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTraceGraphResultTypeDef = TypedDict(
     "GetTraceGraphResultTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TraceSummaryTypeDef = TypedDict(
     "TraceSummaryTypeDef",
     {
         "Id": str,
@@ -1589,10 +1708,10 @@
 GetTraceSummariesResultTypeDef = TypedDict(
     "GetTraceSummariesResultTypeDef",
     {
         "TraceSummaries": List[TraceSummaryTypeDef],
         "ApproximateTime": datetime,
         "TracesProcessedCount": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray/type_defs.pyi` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,68 +34,74 @@
 
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
-    "PaginatorConfigTypeDef",
+    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     "BatchGetTracesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "InsightsConfigurationTypeDef",
     "TagTypeDef",
     "SamplingRuleTypeDef",
     "DeleteGroupRequestRequestTypeDef",
+    "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSamplingRuleRequestRequestTypeDef",
     "ErrorStatisticsTypeDef",
     "FaultStatisticsTypeDef",
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
     "GetInsightImpactGraphRequestRequestTypeDef",
     "GetInsightRequestRequestTypeDef",
     "GetInsightSummariesRequestRequestTypeDef",
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
     "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     "GetServiceGraphRequestRequestTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    "ListResourcePoliciesRequestRequestTypeDef",
+    "ResourcePolicyTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
     "TelemetryRecordTypeDef",
-    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
@@ -108,14 +114,16 @@
     "FaultRootCauseEntityTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
+    "ListResourcePoliciesResultTypeDef",
+    "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
@@ -196,24 +204,34 @@
         "HTTPCode5XXCount": int,
         "UnknownHostCount": int,
         "OtherCount": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
+    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+):
+    pass
+
 _RequiredBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestRequestTypeDef = TypedDict(
@@ -225,25 +243,14 @@
 )
 
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
 ):
     pass
 
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
 InsightsConfigurationTypeDef = TypedDict(
     "InsightsConfigurationTypeDef",
     {
         "InsightsEnabled": bool,
         "NotificationsEnabled": bool,
     },
     total=False,
@@ -290,14 +297,34 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
+_RequiredDeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyName": str,
+    },
+)
+_OptionalDeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyRevisionId": str,
+    },
+    total=False,
+)
+
+class DeleteResourcePolicyRequestRequestTypeDef(
+    _RequiredDeleteResourcePolicyRequestRequestTypeDef,
+    _OptionalDeleteResourcePolicyRequestRequestTypeDef,
+):
+    pass
+
 DeleteSamplingRuleRequestRequestTypeDef = TypedDict(
     "DeleteSamplingRuleRequestRequestTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
     },
     total=False,
@@ -364,14 +391,22 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
+GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetGroupsRequestRequestTypeDef = TypedDict(
     "GetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -446,22 +481,38 @@
 
 class GetInsightSummariesRequestRequestTypeDef(
     _RequiredGetInsightSummariesRequestRequestTypeDef,
     _OptionalGetInsightSummariesRequestRequestTypeDef,
 ):
     pass
 
+GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSamplingStatisticSummariesRequestRequestTypeDef = TypedDict(
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -519,14 +570,37 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
 _RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -541,14 +615,40 @@
 )
 
 class GetServiceGraphRequestRequestTypeDef(
     _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -567,14 +667,34 @@
 
 class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
+    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+):
+    pass
+
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
@@ -633,14 +753,61 @@
     "InstanceIdDetailTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListResourcePoliciesRequestRequestTypeDef = TypedDict(
+    "ListResourcePoliciesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ResourcePolicyTypeDef = TypedDict(
+    "ResourcePolicyTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "PolicyRevisionId": str,
+        "LastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
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
@@ -653,14 +820,24 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
@@ -673,14 +850,35 @@
 
 class PutEncryptionConfigRequestRequestTypeDef(
     _RequiredPutEncryptionConfigRequestRequestTypeDef,
     _OptionalPutEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyDocument": str,
+    },
+)
+_OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "BypassPolicyLockoutCheck": bool,
+    },
+    total=False,
+)
+
+class PutResourcePolicyRequestRequestTypeDef(
+    _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
+):
+    pass
+
 PutTraceSegmentsRequestRequestTypeDef = TypedDict(
     "PutTraceSegmentsRequestRequestTypeDef",
     {
         "TraceSegmentDocuments": Sequence[str],
     },
 )
 
@@ -698,14 +896,25 @@
     "ResourceARNDetailTypeDef",
     {
         "ARN": str,
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
 ResponseTimeRootCauseEntityTypeDef = TypedDict(
     "ResponseTimeRootCauseEntityTypeDef",
     {
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
@@ -791,127 +1000,14 @@
     },
     total=False,
 )
 
 class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
     pass
 
-_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
-    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-):
-    pass
-
-GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
-    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-):
-    pass
-
 GroupSummaryTypeDef = TypedDict(
     "GroupSummaryTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -963,15 +1059,15 @@
     pass
 
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
@@ -1033,23 +1129,23 @@
     total=False,
 )
 
 GetEncryptionConfigResultTypeDef = TypedDict(
     "GetEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEncryptionConfigResultTypeDef = TypedDict(
     "PutEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorRootCauseEntityTypeDef = TypedDict(
     "ErrorRootCauseEntityTypeDef",
     {
         "Name": str,
@@ -1070,15 +1166,15 @@
 )
 
 GetSamplingStatisticSummariesResultTypeDef = TypedDict(
     "GetSamplingStatisticSummariesResultTypeDef",
     {
         "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSamplingTargetsRequestRequestTypeDef = TypedDict(
     "GetSamplingTargetsRequestRequestTypeDef",
     {
         "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
@@ -1087,15 +1183,15 @@
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
         "LastRuleModification": datetime,
         "UnprocessedStatistics": List[UnprocessedStatisticsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "StartTime": Union[datetime, str],
@@ -1105,15 +1201,15 @@
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
@@ -1153,19 +1249,36 @@
         "Names": List[str],
         "AccountId": str,
         "Edges": List[InsightImpactGraphEdgeTypeDef],
     },
     total=False,
 )
 
+ListResourcePoliciesResultTypeDef = TypedDict(
+    "ListResourcePoliciesResultTypeDef",
+    {
+        "ResourcePolicies": List[ResourcePolicyTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutResourcePolicyResultTypeDef = TypedDict(
+    "PutResourcePolicyResultTypeDef",
+    {
+        "ResourcePolicy": ResourcePolicyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseTimeRootCauseServiceTypeDef = TypedDict(
     "ResponseTimeRootCauseServiceTypeDef",
     {
         "Name": str,
@@ -1270,72 +1383,72 @@
     pass
 
 GetGroupsResultTypeDef = TypedDict(
     "GetGroupsResultTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGroupResultTypeDef = TypedDict(
     "CreateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupResultTypeDef = TypedDict(
     "GetGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupResultTypeDef = TypedDict(
     "UpdateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSamplingRuleResultTypeDef = TypedDict(
     "CreateSamplingRuleResultTypeDef",
     {
         "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSamplingRuleResultTypeDef = TypedDict(
     "DeleteSamplingRuleResultTypeDef",
     {
         "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSamplingRulesResultTypeDef = TypedDict(
     "GetSamplingRulesResultTypeDef",
     {
         "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSamplingRuleResultTypeDef = TypedDict(
     "UpdateSamplingRuleResultTypeDef",
     {
         "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
@@ -1394,15 +1507,15 @@
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
         "ServiceGraphEndTime": datetime,
         "Services": List[InsightImpactGraphServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseTimeRootCauseTypeDef = TypedDict(
     "ResponseTimeRootCauseTypeDef",
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
@@ -1413,41 +1526,41 @@
 
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightEventsResultTypeDef = TypedDict(
     "GetInsightEventsResultTypeDef",
     {
         "InsightEvents": List[InsightEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightSummariesResultTypeDef = TypedDict(
     "GetInsightSummariesResultTypeDef",
     {
         "InsightSummaries": List[InsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightResultTypeDef = TypedDict(
     "GetInsightResultTypeDef",
     {
         "Insight": InsightTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "ReferenceId": int,
@@ -1469,15 +1582,15 @@
 
 GetTimeSeriesServiceStatisticsResultTypeDef = TypedDict(
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     {
         "TimeSeriesServiceStatistics": List[TimeSeriesServiceStatisticsTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorRootCauseTypeDef = TypedDict(
     "ErrorRootCauseTypeDef",
     {
         "Services": List[ErrorRootCauseServiceTypeDef],
@@ -1499,24 +1612,24 @@
     "GetServiceGraphResultTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
         "Services": List[ServiceTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTraceGraphResultTypeDef = TypedDict(
     "GetTraceGraphResultTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TraceSummaryTypeDef = TypedDict(
     "TraceSummaryTypeDef",
     {
         "Id": str,
@@ -1546,10 +1659,10 @@
 GetTraceSummariesResultTypeDef = TypedDict(
     "GetTraceSummariesResultTypeDef",
     {
         "TraceSummaries": List[TraceSummaryTypeDef],
         "ApproximateTime": datetime,
         "TracesProcessedCount": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/PKG-INFO` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.26.9
-Summary: Type annotations for boto3.XRay 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.XRay 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
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
 
 <a id="mypy-boto3-xray"></a>
 
 # mypy-boto3-xray
 
 [![PyPI - mypy-boto3-xray](https://img.shields.io/pypi/v/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-xray?color=blue)](https://pypistats.org/packages/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,14 +287,16 @@
     GetGroupsPaginator,
     GetSamplingRulesPaginator,
     GetSamplingStatisticSummariesPaginator,
     GetServiceGraphPaginator,
     GetTimeSeriesServiceStatisticsPaginator,
     GetTraceGraphPaginator,
     GetTraceSummariesPaginator,
+    ListResourcePoliciesPaginator,
+    ListTagsForResourcePaginator,
 )
 
 client: XRayClient = Session().client("xray")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 batch_get_traces_paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")
@@ -306,14 +309,20 @@
 get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = (
     client.get_paginator("get_time_series_service_statistics")
 )
 get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
 get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator(
     "get_trace_summaries"
 )
+list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator(
+    "list_resource_policies"
+)
+list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
+    "list_tags_for_resource"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_xray.literals` module contains literals extracted from shapes that
@@ -329,14 +338,16 @@
     GetSamplingStatisticSummariesPaginatorName,
     GetServiceGraphPaginatorName,
     GetTimeSeriesServiceStatisticsPaginatorName,
     GetTraceGraphPaginatorName,
     GetTraceSummariesPaginatorName,
     InsightCategoryType,
     InsightStateType,
+    ListResourcePoliciesPaginatorName,
+    ListTagsForResourcePaginatorName,
     SamplingStrategyNameType,
     TimeRangeTypeType,
     XRayServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -357,68 +368,74 @@
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    PaginatorConfigTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     BatchGetTracesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
+    DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
     GetInsightImpactGraphRequestRequestTypeDef,
     GetInsightRequestRequestTypeDef,
     GetInsightSummariesRequestRequestTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListResourcePoliciesRequestRequestTypeDef,
+    ResourcePolicyTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
+    PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
+    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
     TelemetryRecordTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
@@ -431,14 +448,16 @@
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
+    ListResourcePoliciesResultTypeDef,
+    PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
@@ -479,42 +498,42 @@
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

### Comparing `mypy-boto3-xray-1.26.9/mypy_boto3_xray.egg-info/SOURCES.txt` & `mypy-boto3-xray-1.27.0/mypy_boto3_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.26.9/setup.py` & `mypy-boto3-xray-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-xray.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-xray",
-    version="1.26.9",
+    version="1.27.0",
     packages=["mypy_boto3_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.XRay 1.26.9 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.XRay 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 xray type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_xray": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_xray": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/",
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


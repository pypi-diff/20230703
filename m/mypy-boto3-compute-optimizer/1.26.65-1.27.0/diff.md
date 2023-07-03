# Comparing `tmp/mypy-boto3-compute-optimizer-1.26.65.tar.gz` & `tmp/mypy-boto3-compute-optimizer-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-compute-optimizer-1.26.65.tar", last modified: Mon Feb  6 20:47:28 2023, max compression
+gzip compressed data, was "mypy-boto3-compute-optimizer-1.27.0.tar", last modified: Mon Jul  3 19:50:35 2023, max compression
```

## Comparing `mypy-boto3-compute-optimizer-1.26.65.tar` & `mypy-boto3-compute-optimizer-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22921 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22919 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-02-06 20:47:03.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40922 2023-02-06 20:47:03.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:35.695056 mypy-boto3-compute-optimizer-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-03 19:50:35.695056 mypy-boto3-compute-optimizer-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:35.695056 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23909 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42033 2023-07-03 19:34:47.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-07-03 19:34:47.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:35.695056 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-03 19:50:35.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:50:35.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:35.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:35.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:35.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:35.000000 mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:35.695056 mypy-boto3-compute-optimizer-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:34:46.000000 mypy-boto3-compute-optimizer-1.27.0/setup.py
```

### Comparing `mypy-boto3-compute-optimizer-1.26.65/LICENSE` & `mypy-boto3-compute-optimizer-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-compute-optimizer-1.26.65/PKG-INFO` & `mypy-boto3-compute-optimizer-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.26.65
-Summary: Type annotations for boto3.ComputeOptimizer 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ComputeOptimizer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-compute-optimizer"></a>
 
 # mypy-boto3-compute-optimizer
 
 [![PyPI - mypy-boto3-compute-optimizer](https://img.shields.io/pypi/v/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,26 +339,28 @@
     EnhancedInfrastructureMetricsType,
     EnrollmentFilterNameType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
     ExportableInstanceFieldType,
     ExportableLambdaFunctionFieldType,
     ExportableVolumeFieldType,
+    ExternalMetricStatusCodeType,
     ExternalMetricsSourceType,
     FileFormatType,
     FilterNameType,
     FindingReasonCodeType,
     FindingType,
     GetEnrollmentStatusesForOrganizationPaginatorName,
     GetLambdaFunctionRecommendationsPaginatorName,
     GetRecommendationPreferencesPaginatorName,
     GetRecommendationSummariesPaginatorName,
     InferredWorkloadTypeType,
     InferredWorkloadTypesPreferenceType,
     InstanceRecommendationFindingReasonCodeType,
+    InstanceStateType,
     JobFilterNameType,
     JobStatusType,
     LambdaFunctionMemoryMetricNameType,
     LambdaFunctionMemoryMetricStatisticType,
     LambdaFunctionMetricNameType,
     LambdaFunctionMetricStatisticType,
     LambdaFunctionRecommendationFilterNameType,
@@ -397,61 +399,64 @@
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
+    TagTypeDef,
     ExternalMetricsPreferenceTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
+    ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
+    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestRequestTypeDef,
     DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
+    DescribeRecommendationExportJobsRequestRequestTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
     PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
+    InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
@@ -500,42 +505,42 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.26.65/README.md` & `mypy-boto3-compute-optimizer-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-compute-optimizer"></a>
 
 # mypy-boto3-compute-optimizer
 
 [![PyPI - mypy-boto3-compute-optimizer](https://img.shields.io/pypi/v/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,26 +307,28 @@
     EnhancedInfrastructureMetricsType,
     EnrollmentFilterNameType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
     ExportableInstanceFieldType,
     ExportableLambdaFunctionFieldType,
     ExportableVolumeFieldType,
+    ExternalMetricStatusCodeType,
     ExternalMetricsSourceType,
     FileFormatType,
     FilterNameType,
     FindingReasonCodeType,
     FindingType,
     GetEnrollmentStatusesForOrganizationPaginatorName,
     GetLambdaFunctionRecommendationsPaginatorName,
     GetRecommendationPreferencesPaginatorName,
     GetRecommendationSummariesPaginatorName,
     InferredWorkloadTypeType,
     InferredWorkloadTypesPreferenceType,
     InstanceRecommendationFindingReasonCodeType,
+    InstanceStateType,
     JobFilterNameType,
     JobStatusType,
     LambdaFunctionMemoryMetricNameType,
     LambdaFunctionMemoryMetricStatisticType,
     LambdaFunctionMetricNameType,
     LambdaFunctionMetricStatisticType,
     LambdaFunctionRecommendationFilterNameType,
@@ -365,61 +367,64 @@
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
+    TagTypeDef,
     ExternalMetricsPreferenceTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
+    ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
+    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestRequestTypeDef,
     DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
+    DescribeRecommendationExportJobsRequestRequestTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
     PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
+    InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
@@ -468,42 +473,42 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.py` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.pyi` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__main__.py` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComputeOptimizer 1.26.65\nVersion:         1.26.65\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ComputeOptimizer 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.65")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.py` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.pyi` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.py` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,28 @@
     "EnhancedInfrastructureMetricsType",
     "EnrollmentFilterNameType",
     "ExportableAutoScalingGroupFieldType",
     "ExportableECSServiceFieldType",
     "ExportableInstanceFieldType",
     "ExportableLambdaFunctionFieldType",
     "ExportableVolumeFieldType",
+    "ExternalMetricStatusCodeType",
     "ExternalMetricsSourceType",
     "FileFormatType",
     "FilterNameType",
     "FindingReasonCodeType",
     "FindingType",
     "GetEnrollmentStatusesForOrganizationPaginatorName",
     "GetLambdaFunctionRecommendationsPaginatorName",
     "GetRecommendationPreferencesPaginatorName",
     "GetRecommendationSummariesPaginatorName",
     "InferredWorkloadTypeType",
     "InferredWorkloadTypesPreferenceType",
     "InstanceRecommendationFindingReasonCodeType",
+    "InstanceStateType",
     "JobFilterNameType",
     "JobStatusType",
     "LambdaFunctionMemoryMetricNameType",
     "LambdaFunctionMemoryMetricStatisticType",
     "LambdaFunctionMetricNameType",
     "LambdaFunctionMetricStatisticType",
     "LambdaFunctionRecommendationFilterNameType",
@@ -176,14 +178,15 @@
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsMemory",
     "RecommendationOptionsProjectedUtilizationMetricsCpuMaximum",
     "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum",
     "RecommendationOptionsSavingsOpportunityPercentage",
     "ServiceArn",
+    "Tags",
     "UtilizationMetricsCpuMaximum",
     "UtilizationMetricsMemoryMaximum",
 ]
 ExportableInstanceFieldType = Literal[
     "AccountId",
     "CurrentInstanceType",
     "CurrentMemory",
@@ -194,19 +197,22 @@
     "CurrentStandardThreeYearNoUpfrontReservedPrice",
     "CurrentStorage",
     "CurrentVCpus",
     "EffectiveRecommendationPreferencesCpuVendorArchitectures",
     "EffectiveRecommendationPreferencesEnhancedInfrastructureMetrics",
     "EffectiveRecommendationPreferencesExternalMetricsSource",
     "EffectiveRecommendationPreferencesInferredWorkloadTypes",
+    "ExternalMetricStatusCode",
+    "ExternalMetricStatusReason",
     "Finding",
     "FindingReasonCodes",
     "InferredWorkloadTypes",
     "InstanceArn",
     "InstanceName",
+    "InstanceState",
     "LastRefreshTimestamp",
     "LookbackPeriodInDays",
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsInstanceType",
     "RecommendationOptionsMemory",
     "RecommendationOptionsMigrationEffort",
@@ -219,14 +225,15 @@
     "RecommendationOptionsSavingsOpportunityPercentage",
     "RecommendationOptionsStandardOneYearNoUpfrontReservedPrice",
     "RecommendationOptionsStandardThreeYearNoUpfrontReservedPrice",
     "RecommendationOptionsStorage",
     "RecommendationOptionsVcpus",
     "RecommendationsSourcesRecommendationSourceArn",
     "RecommendationsSourcesRecommendationSourceType",
+    "Tags",
     "UtilizationMetricsCpuMaximum",
     "UtilizationMetricsDiskReadBytesPerSecondMaximum",
     "UtilizationMetricsDiskReadOpsPerSecondMaximum",
     "UtilizationMetricsDiskWriteBytesPerSecondMaximum",
     "UtilizationMetricsDiskWriteOpsPerSecondMaximum",
     "UtilizationMetricsEbsReadBytesPerSecondMaximum",
     "UtilizationMetricsEbsReadOpsPerSecondMaximum",
@@ -257,14 +264,15 @@
     "RecommendationOptionsCostLow",
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsProjectedUtilizationMetricsDurationExpected",
     "RecommendationOptionsProjectedUtilizationMetricsDurationLowerBound",
     "RecommendationOptionsProjectedUtilizationMetricsDurationUpperBound",
     "RecommendationOptionsSavingsOpportunityPercentage",
+    "Tags",
     "UtilizationMetricsDurationAverage",
     "UtilizationMetricsDurationMaximum",
     "UtilizationMetricsMemoryAverage",
     "UtilizationMetricsMemoryMaximum",
 ]
 ExportableVolumeFieldType = Literal[
     "AccountId",
@@ -286,23 +294,39 @@
     "RecommendationOptionsConfigurationVolumeSize",
     "RecommendationOptionsConfigurationVolumeType",
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsMonthlyPrice",
     "RecommendationOptionsPerformanceRisk",
     "RecommendationOptionsSavingsOpportunityPercentage",
+    "RootVolume",
+    "Tags",
     "UtilizationMetricsVolumeReadBytesPerSecondMaximum",
     "UtilizationMetricsVolumeReadOpsPerSecondMaximum",
     "UtilizationMetricsVolumeWriteBytesPerSecondMaximum",
     "UtilizationMetricsVolumeWriteOpsPerSecondMaximum",
     "VolumeArn",
 ]
+ExternalMetricStatusCodeType = Literal[
+    "DATADOG_INTEGRATION_ERROR",
+    "DYNATRACE_INTEGRATION_ERROR",
+    "INSTANA_INTEGRATION_ERROR",
+    "INSUFFICIENT_DATADOG_METRICS",
+    "INSUFFICIENT_DYNATRACE_METRICS",
+    "INSUFFICIENT_INSTANA_METRICS",
+    "INSUFFICIENT_NEWRELIC_METRICS",
+    "INTEGRATION_SUCCESS",
+    "NEWRELIC_INTEGRATION_ERROR",
+    "NO_EXTERNAL_METRIC_SET",
+]
 ExternalMetricsSourceType = Literal["Datadog", "Dynatrace", "Instana", "NewRelic"]
 FileFormatType = Literal["Csv"]
-FilterNameType = Literal["Finding", "FindingReasonCodes", "RecommendationSourceType"]
+FilterNameType = Literal[
+    "Finding", "FindingReasonCodes", "InferredWorkloadTypes", "RecommendationSourceType"
+]
 FindingReasonCodeType = Literal["MemoryOverprovisioned", "MemoryUnderprovisioned"]
 FindingType = Literal["NotOptimized", "Optimized", "Overprovisioned", "Underprovisioned"]
 GetEnrollmentStatusesForOrganizationPaginatorName = Literal[
     "get_enrollment_statuses_for_organization"
 ]
 GetLambdaFunctionRecommendationsPaginatorName = Literal["get_lambda_function_recommendations"]
 GetRecommendationPreferencesPaginatorName = Literal["get_recommendation_preferences"]
@@ -312,14 +336,15 @@
     "ApacheCassandra",
     "ApacheHadoop",
     "Kafka",
     "Memcached",
     "Nginx",
     "PostgreSql",
     "Redis",
+    "SQLServer",
 ]
 InferredWorkloadTypesPreferenceType = Literal["Active", "Inactive"]
 InstanceRecommendationFindingReasonCodeType = Literal[
     "CPUOverprovisioned",
     "CPUUnderprovisioned",
     "DiskIOPSOverprovisioned",
     "DiskIOPSUnderprovisioned",
@@ -332,14 +357,17 @@
     "MemoryOverprovisioned",
     "MemoryUnderprovisioned",
     "NetworkBandwidthOverprovisioned",
     "NetworkBandwidthUnderprovisioned",
     "NetworkPPSOverprovisioned",
     "NetworkPPSUnderprovisioned",
 ]
+InstanceStateType = Literal[
+    "pending", "running", "shutting-down", "stopped", "stopping", "terminated"
+]
 JobFilterNameType = Literal["JobStatus", "ResourceType"]
 JobStatusType = Literal["Complete", "Failed", "InProgress", "Queued"]
 LambdaFunctionMemoryMetricNameType = Literal["Duration"]
 LambdaFunctionMemoryMetricStatisticType = Literal["Expected", "LowerBound", "UpperBound"]
 LambdaFunctionMetricNameType = Literal["Duration", "Memory"]
 LambdaFunctionMetricStatisticType = Literal["Average", "Maximum"]
 LambdaFunctionRecommendationFilterNameType = Literal["Finding", "FindingReasonCode"]
@@ -396,14 +424,15 @@
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
@@ -443,14 +472,15 @@
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
@@ -529,14 +559,15 @@
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
@@ -547,14 +578,15 @@
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
@@ -590,14 +622,15 @@
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
@@ -616,16 +649,19 @@
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
@@ -705,18 +741,21 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.pyi` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,28 @@
     "EnhancedInfrastructureMetricsType",
     "EnrollmentFilterNameType",
     "ExportableAutoScalingGroupFieldType",
     "ExportableECSServiceFieldType",
     "ExportableInstanceFieldType",
     "ExportableLambdaFunctionFieldType",
     "ExportableVolumeFieldType",
+    "ExternalMetricStatusCodeType",
     "ExternalMetricsSourceType",
     "FileFormatType",
     "FilterNameType",
     "FindingReasonCodeType",
     "FindingType",
     "GetEnrollmentStatusesForOrganizationPaginatorName",
     "GetLambdaFunctionRecommendationsPaginatorName",
     "GetRecommendationPreferencesPaginatorName",
     "GetRecommendationSummariesPaginatorName",
     "InferredWorkloadTypeType",
     "InferredWorkloadTypesPreferenceType",
     "InstanceRecommendationFindingReasonCodeType",
+    "InstanceStateType",
     "JobFilterNameType",
     "JobStatusType",
     "LambdaFunctionMemoryMetricNameType",
     "LambdaFunctionMemoryMetricStatisticType",
     "LambdaFunctionMetricNameType",
     "LambdaFunctionMetricStatisticType",
     "LambdaFunctionRecommendationFilterNameType",
@@ -174,14 +176,15 @@
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsMemory",
     "RecommendationOptionsProjectedUtilizationMetricsCpuMaximum",
     "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum",
     "RecommendationOptionsSavingsOpportunityPercentage",
     "ServiceArn",
+    "Tags",
     "UtilizationMetricsCpuMaximum",
     "UtilizationMetricsMemoryMaximum",
 ]
 ExportableInstanceFieldType = Literal[
     "AccountId",
     "CurrentInstanceType",
     "CurrentMemory",
@@ -192,19 +195,22 @@
     "CurrentStandardThreeYearNoUpfrontReservedPrice",
     "CurrentStorage",
     "CurrentVCpus",
     "EffectiveRecommendationPreferencesCpuVendorArchitectures",
     "EffectiveRecommendationPreferencesEnhancedInfrastructureMetrics",
     "EffectiveRecommendationPreferencesExternalMetricsSource",
     "EffectiveRecommendationPreferencesInferredWorkloadTypes",
+    "ExternalMetricStatusCode",
+    "ExternalMetricStatusReason",
     "Finding",
     "FindingReasonCodes",
     "InferredWorkloadTypes",
     "InstanceArn",
     "InstanceName",
+    "InstanceState",
     "LastRefreshTimestamp",
     "LookbackPeriodInDays",
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsInstanceType",
     "RecommendationOptionsMemory",
     "RecommendationOptionsMigrationEffort",
@@ -217,14 +223,15 @@
     "RecommendationOptionsSavingsOpportunityPercentage",
     "RecommendationOptionsStandardOneYearNoUpfrontReservedPrice",
     "RecommendationOptionsStandardThreeYearNoUpfrontReservedPrice",
     "RecommendationOptionsStorage",
     "RecommendationOptionsVcpus",
     "RecommendationsSourcesRecommendationSourceArn",
     "RecommendationsSourcesRecommendationSourceType",
+    "Tags",
     "UtilizationMetricsCpuMaximum",
     "UtilizationMetricsDiskReadBytesPerSecondMaximum",
     "UtilizationMetricsDiskReadOpsPerSecondMaximum",
     "UtilizationMetricsDiskWriteBytesPerSecondMaximum",
     "UtilizationMetricsDiskWriteOpsPerSecondMaximum",
     "UtilizationMetricsEbsReadBytesPerSecondMaximum",
     "UtilizationMetricsEbsReadOpsPerSecondMaximum",
@@ -255,14 +262,15 @@
     "RecommendationOptionsCostLow",
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsProjectedUtilizationMetricsDurationExpected",
     "RecommendationOptionsProjectedUtilizationMetricsDurationLowerBound",
     "RecommendationOptionsProjectedUtilizationMetricsDurationUpperBound",
     "RecommendationOptionsSavingsOpportunityPercentage",
+    "Tags",
     "UtilizationMetricsDurationAverage",
     "UtilizationMetricsDurationMaximum",
     "UtilizationMetricsMemoryAverage",
     "UtilizationMetricsMemoryMaximum",
 ]
 ExportableVolumeFieldType = Literal[
     "AccountId",
@@ -284,23 +292,39 @@
     "RecommendationOptionsConfigurationVolumeSize",
     "RecommendationOptionsConfigurationVolumeType",
     "RecommendationOptionsEstimatedMonthlySavingsCurrency",
     "RecommendationOptionsEstimatedMonthlySavingsValue",
     "RecommendationOptionsMonthlyPrice",
     "RecommendationOptionsPerformanceRisk",
     "RecommendationOptionsSavingsOpportunityPercentage",
+    "RootVolume",
+    "Tags",
     "UtilizationMetricsVolumeReadBytesPerSecondMaximum",
     "UtilizationMetricsVolumeReadOpsPerSecondMaximum",
     "UtilizationMetricsVolumeWriteBytesPerSecondMaximum",
     "UtilizationMetricsVolumeWriteOpsPerSecondMaximum",
     "VolumeArn",
 ]
+ExternalMetricStatusCodeType = Literal[
+    "DATADOG_INTEGRATION_ERROR",
+    "DYNATRACE_INTEGRATION_ERROR",
+    "INSTANA_INTEGRATION_ERROR",
+    "INSUFFICIENT_DATADOG_METRICS",
+    "INSUFFICIENT_DYNATRACE_METRICS",
+    "INSUFFICIENT_INSTANA_METRICS",
+    "INSUFFICIENT_NEWRELIC_METRICS",
+    "INTEGRATION_SUCCESS",
+    "NEWRELIC_INTEGRATION_ERROR",
+    "NO_EXTERNAL_METRIC_SET",
+]
 ExternalMetricsSourceType = Literal["Datadog", "Dynatrace", "Instana", "NewRelic"]
 FileFormatType = Literal["Csv"]
-FilterNameType = Literal["Finding", "FindingReasonCodes", "RecommendationSourceType"]
+FilterNameType = Literal[
+    "Finding", "FindingReasonCodes", "InferredWorkloadTypes", "RecommendationSourceType"
+]
 FindingReasonCodeType = Literal["MemoryOverprovisioned", "MemoryUnderprovisioned"]
 FindingType = Literal["NotOptimized", "Optimized", "Overprovisioned", "Underprovisioned"]
 GetEnrollmentStatusesForOrganizationPaginatorName = Literal[
     "get_enrollment_statuses_for_organization"
 ]
 GetLambdaFunctionRecommendationsPaginatorName = Literal["get_lambda_function_recommendations"]
 GetRecommendationPreferencesPaginatorName = Literal["get_recommendation_preferences"]
@@ -310,14 +334,15 @@
     "ApacheCassandra",
     "ApacheHadoop",
     "Kafka",
     "Memcached",
     "Nginx",
     "PostgreSql",
     "Redis",
+    "SQLServer",
 ]
 InferredWorkloadTypesPreferenceType = Literal["Active", "Inactive"]
 InstanceRecommendationFindingReasonCodeType = Literal[
     "CPUOverprovisioned",
     "CPUUnderprovisioned",
     "DiskIOPSOverprovisioned",
     "DiskIOPSUnderprovisioned",
@@ -330,14 +355,17 @@
     "MemoryOverprovisioned",
     "MemoryUnderprovisioned",
     "NetworkBandwidthOverprovisioned",
     "NetworkBandwidthUnderprovisioned",
     "NetworkPPSOverprovisioned",
     "NetworkPPSUnderprovisioned",
 ]
+InstanceStateType = Literal[
+    "pending", "running", "shutting-down", "stopped", "stopping", "terminated"
+]
 JobFilterNameType = Literal["JobStatus", "ResourceType"]
 JobStatusType = Literal["Complete", "Failed", "InProgress", "Queued"]
 LambdaFunctionMemoryMetricNameType = Literal["Duration"]
 LambdaFunctionMemoryMetricStatisticType = Literal["Expected", "LowerBound", "UpperBound"]
 LambdaFunctionMetricNameType = Literal["Duration", "Memory"]
 LambdaFunctionMetricStatisticType = Literal["Average", "Maximum"]
 LambdaFunctionRecommendationFilterNameType = Literal["Finding", "FindingReasonCode"]
@@ -394,14 +422,15 @@
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
@@ -441,14 +470,15 @@
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
@@ -527,14 +557,15 @@
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
@@ -545,14 +576,15 @@
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
@@ -588,14 +620,15 @@
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
@@ -614,16 +647,19 @@
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
@@ -703,18 +739,21 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.py` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
 
@@ -89,15 +89,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
 
@@ -109,15 +109,15 @@
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
 
@@ -128,28 +128,28 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
 
 class GetRecommendationSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
         """
```

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.pyi` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
 class GetEnrollmentStatusesForOrganizationPaginator(Paginator):
@@ -85,15 +85,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
 class GetLambdaFunctionRecommendationsPaginator(Paginator):
@@ -104,15 +104,15 @@
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
 class GetRecommendationPreferencesPaginator(Paginator):
@@ -122,27 +122,27 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
 class GetRecommendationSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
         """
```

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.py` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     EnhancedInfrastructureMetricsType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
     ExportableInstanceFieldType,
     ExportableLambdaFunctionFieldType,
     ExportableVolumeFieldType,
     ExternalMetricsSourceType,
+    ExternalMetricStatusCodeType,
     FilterNameType,
     FindingReasonCodeType,
     FindingType,
     InferredWorkloadTypesPreferenceType,
     InferredWorkloadTypeType,
     InstanceRecommendationFindingReasonCodeType,
+    InstanceStateType,
     JobFilterNameType,
     JobStatusType,
     LambdaFunctionMemoryMetricStatisticType,
     LambdaFunctionMetricNameType,
     LambdaFunctionMetricStatisticType,
     LambdaFunctionRecommendationFilterNameType,
     LambdaFunctionRecommendationFindingReasonCodeType,
@@ -74,61 +76,64 @@
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
     "ScopeTypeDef",
     "JobFilterTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
+    "TagTypeDef",
     "ExternalMetricsPreferenceTypeDef",
     "EnrollmentFilterTypeDef",
     "EstimatedMonthlySavingsTypeDef",
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
+    "ExternalMetricStatusTypeDef",
     "GetRecommendationErrorTypeDef",
     "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
+    "GetEnrollmentStatusResponseTypeDef",
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
+    "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
+    "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
     "DeleteRecommendationPreferencesRequestRequestTypeDef",
+    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     "GetRecommendationPreferencesRequestRequestTypeDef",
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
-    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
-    "GetEnrollmentStatusResponseTypeDef",
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
-    "UpdateEnrollmentStatusResponseTypeDef",
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
+    "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
     "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "ExportEBSVolumeRecommendationsRequestRequestTypeDef",
     "ExportEC2InstanceRecommendationsRequestRequestTypeDef",
@@ -235,35 +240,14 @@
     {
         "name": JobFilterNameType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
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
 EBSFilterTypeDef = TypedDict(
     "EBSFilterTypeDef",
     {
         "name": Literal["Finding"],
         "values": Sequence[str],
     },
     total=False,
@@ -316,14 +300,23 @@
         "name": ECSServiceMetricNameType,
         "statistic": ECSServiceMetricStatisticType,
         "value": float,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 ExternalMetricsPreferenceTypeDef = TypedDict(
     "ExternalMetricsPreferenceTypeDef",
     {
         "source": ExternalMetricsSourceType,
     },
     total=False,
 )
@@ -387,14 +380,23 @@
     {
         "name": LambdaFunctionRecommendationFilterNameType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+ExternalMetricStatusTypeDef = TypedDict(
+    "ExternalMetricStatusTypeDef",
+    {
+        "statusCode": ExternalMetricStatusCodeType,
+        "statusReason": str,
+    },
+    total=False,
+)
+
 GetRecommendationErrorTypeDef = TypedDict(
     "GetRecommendationErrorTypeDef",
     {
         "identifier": str,
         "code": str,
         "message": str,
     },
@@ -415,14 +417,35 @@
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+GetEnrollmentStatusResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "memberAccountsEnrolled": bool,
+        "lastUpdatedTimestamp": datetime,
+        "numberOfMemberAccountsOptedIn": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRecommendationSummariesRequestRequestTypeDef = TypedDict(
     "GetRecommendationSummariesRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -454,14 +477,24 @@
         "name": LambdaFunctionMetricNameType,
         "statistic": LambdaFunctionMetricStatisticType,
         "value": float,
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
 ProjectedMetricTypeDef = TypedDict(
     "ProjectedMetricTypeDef",
     {
         "name": MetricNameType,
         "timestamps": List[datetime],
         "values": List[float],
     },
@@ -473,14 +506,25 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
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
 _RequiredUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnrollmentStatusRequestRequestTypeDef",
     {
         "status": StatusType,
     },
 )
 _OptionalUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
@@ -495,27 +539,46 @@
 class UpdateEnrollmentStatusRequestRequestTypeDef(
     _RequiredUpdateEnrollmentStatusRequestRequestTypeDef,
     _OptionalUpdateEnrollmentStatusRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateEnrollmentStatusResponseTypeDef = TypedDict(
+    "UpdateEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VolumeConfigurationTypeDef = TypedDict(
     "VolumeConfigurationTypeDef",
     {
         "volumeType": str,
         "volumeSize": int,
         "volumeBaselineIOPS": int,
         "volumeBurstIOPS": int,
         "volumeBaselineThroughput": int,
         "volumeBurstThroughput": int,
+        "rootVolume": bool,
     },
     total=False,
 )
 
+GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    {
+        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ContainerConfigurationTypeDef = TypedDict(
     "ContainerConfigurationTypeDef",
     {
         "containerName": str,
         "memorySizeConfiguration": MemorySizeConfigurationTypeDef,
         "cpu": int,
     },
@@ -551,119 +614,80 @@
 class DeleteRecommendationPreferencesRequestRequestTypeDef(
     _RequiredDeleteRecommendationPreferencesRequestRequestTypeDef,
     _OptionalDeleteRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
+_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
+_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "scope": ScopeTypeDef,
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class GetRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
+class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
+    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
 ):
     pass
 
 
-DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
-    {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
-    {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "scope": ScopeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
-    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+class GetRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
 
-GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     {
-        "accountIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-GetEnrollmentStatusResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "memberAccountsEnrolled": bool,
-        "lastUpdatedTimestamp": datetime,
-        "numberOfMemberAccountsOptedIn": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     {
-        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEnrollmentStatusResponseTypeDef = TypedDict(
-    "UpdateEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "maxResults": int,
     },
+    total=False,
 )
 
 GetEBSVolumeRecommendationsRequestRequestTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     {
         "volumeArns": Sequence[str],
         "nextToken": str,
@@ -708,15 +732,15 @@
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
@@ -753,29 +777,38 @@
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+InferredWorkloadSavingTypeDef = TypedDict(
+    "InferredWorkloadSavingTypeDef",
+    {
+        "inferredWorkloadTypes": List[InferredWorkloadTypeType],
+        "estimatedMonthlySavings": EstimatedMonthlySavingsTypeDef,
+    },
+    total=False,
+)
+
 SavingsOpportunityTypeDef = TypedDict(
     "SavingsOpportunityTypeDef",
     {
         "savingsOpportunityPercentage": float,
         "estimatedMonthlySavings": EstimatedMonthlySavingsTypeDef,
     },
     total=False,
@@ -940,15 +973,15 @@
 
 
 ExportAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportDestinationTypeDef = TypedDict(
     "ExportDestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
@@ -957,42 +990,42 @@
 )
 
 ExportEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportECSServiceRecommendationsResponseTypeDef = TypedDict(
     "ExportECSServiceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
@@ -1020,15 +1053,15 @@
 
 GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     {
         "functionArns": Sequence[str],
         "accountIds": Sequence[str],
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
@@ -1075,24 +1108,24 @@
 
 GetECSServiceRecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetRecommendationPreferencesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
@@ -1167,26 +1200,27 @@
     total=False,
 )
 
 GetEC2RecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[RecommendedOptionProjectedMetricTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "summaries": List[SummaryTypeDef],
         "recommendationResourceType": RecommendationSourceTypeType,
         "accountId": str,
         "savingsOpportunity": SavingsOpportunityTypeDef,
         "currentPerformanceRiskRatings": CurrentPerformanceRiskRatingsTypeDef,
+        "inferredWorkloadSavings": List[InferredWorkloadSavingTypeDef],
     },
     total=False,
 )
 
 AutoScalingGroupRecommendationTypeDef = TypedDict(
     "AutoScalingGroupRecommendationTypeDef",
     {
@@ -1216,14 +1250,15 @@
         "lookbackPeriodInDays": float,
         "launchType": ECSServiceLaunchTypeType,
         "lastRefreshTimestamp": datetime,
         "finding": ECSServiceRecommendationFindingType,
         "findingReasonCodes": List[ECSServiceRecommendationFindingReasonCodeType],
         "serviceRecommendationOptions": List[ECSServiceRecommendationOptionTypeDef],
         "currentPerformanceRisk": CurrentPerformanceRiskType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 InstanceRecommendationTypeDef = TypedDict(
     "InstanceRecommendationTypeDef",
     {
@@ -1237,14 +1272,17 @@
         "lookBackPeriodInDays": float,
         "recommendationOptions": List[InstanceRecommendationOptionTypeDef],
         "recommendationSources": List[RecommendationSourceTypeDef],
         "lastRefreshTimestamp": datetime,
         "currentPerformanceRisk": CurrentPerformanceRiskType,
         "effectiveRecommendationPreferences": EffectiveRecommendationPreferencesTypeDef,
         "inferredWorkloadTypes": List[InferredWorkloadTypeType],
+        "instanceState": InstanceStateType,
+        "tags": List[TagTypeDef],
+        "externalMetricStatus": ExternalMetricStatusTypeDef,
     },
     total=False,
 )
 
 LambdaFunctionRecommendationTypeDef = TypedDict(
     "LambdaFunctionRecommendationTypeDef",
     {
@@ -1256,14 +1294,15 @@
         "utilizationMetrics": List[LambdaFunctionUtilizationMetricTypeDef],
         "lookbackPeriodInDays": float,
         "lastRefreshTimestamp": datetime,
         "finding": LambdaFunctionRecommendationFindingType,
         "findingReasonCodes": List[LambdaFunctionRecommendationFindingReasonCodeType],
         "memorySizeRecommendationOptions": List[LambdaFunctionMemoryRecommendationOptionTypeDef],
         "currentPerformanceRisk": CurrentPerformanceRiskType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 VolumeRecommendationTypeDef = TypedDict(
     "VolumeRecommendationTypeDef",
     {
@@ -1272,77 +1311,78 @@
         "currentConfiguration": VolumeConfigurationTypeDef,
         "finding": EBSFindingType,
         "utilizationMetrics": List[EBSUtilizationMetricTypeDef],
         "lookBackPeriodInDays": float,
         "volumeRecommendationOptions": List[VolumeRecommendationOptionTypeDef],
         "lastRefreshTimestamp": datetime,
         "currentPerformanceRisk": CurrentPerformanceRiskType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 DescribeRecommendationExportJobsResponseTypeDef = TypedDict(
     "DescribeRecommendationExportJobsResponseTypeDef",
     {
         "recommendationExportJobs": List[RecommendationExportJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommendationSummariesResponseTypeDef = TypedDict(
     "GetRecommendationSummariesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationSummaries": List[RecommendationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "GetAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "autoScalingGroupRecommendations": List[AutoScalingGroupRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetECSServiceRecommendationsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "ecsServiceRecommendations": List[ECSServiceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "GetEC2InstanceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "instanceRecommendations": List[InstanceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "lambdaFunctionRecommendations": List[LambdaFunctionRecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "volumeRecommendations": List[VolumeRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.pyi` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     EnhancedInfrastructureMetricsType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
     ExportableInstanceFieldType,
     ExportableLambdaFunctionFieldType,
     ExportableVolumeFieldType,
     ExternalMetricsSourceType,
+    ExternalMetricStatusCodeType,
     FilterNameType,
     FindingReasonCodeType,
     FindingType,
     InferredWorkloadTypesPreferenceType,
     InferredWorkloadTypeType,
     InstanceRecommendationFindingReasonCodeType,
+    InstanceStateType,
     JobFilterNameType,
     JobStatusType,
     LambdaFunctionMemoryMetricStatisticType,
     LambdaFunctionMetricNameType,
     LambdaFunctionMetricStatisticType,
     LambdaFunctionRecommendationFilterNameType,
     LambdaFunctionRecommendationFindingReasonCodeType,
@@ -73,61 +75,64 @@
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
     "ScopeTypeDef",
     "JobFilterTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
+    "TagTypeDef",
     "ExternalMetricsPreferenceTypeDef",
     "EnrollmentFilterTypeDef",
     "EstimatedMonthlySavingsTypeDef",
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
+    "ExternalMetricStatusTypeDef",
     "GetRecommendationErrorTypeDef",
     "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
+    "GetEnrollmentStatusResponseTypeDef",
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
+    "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
+    "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
     "DeleteRecommendationPreferencesRequestRequestTypeDef",
+    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     "GetRecommendationPreferencesRequestRequestTypeDef",
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
-    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
-    "GetEnrollmentStatusResponseTypeDef",
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
-    "UpdateEnrollmentStatusResponseTypeDef",
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
+    "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
     "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "ExportEBSVolumeRecommendationsRequestRequestTypeDef",
     "ExportEC2InstanceRecommendationsRequestRequestTypeDef",
@@ -234,35 +239,14 @@
     {
         "name": JobFilterNameType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
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
 EBSFilterTypeDef = TypedDict(
     "EBSFilterTypeDef",
     {
         "name": Literal["Finding"],
         "values": Sequence[str],
     },
     total=False,
@@ -315,14 +299,23 @@
         "name": ECSServiceMetricNameType,
         "statistic": ECSServiceMetricStatisticType,
         "value": float,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 ExternalMetricsPreferenceTypeDef = TypedDict(
     "ExternalMetricsPreferenceTypeDef",
     {
         "source": ExternalMetricsSourceType,
     },
     total=False,
 )
@@ -386,14 +379,23 @@
     {
         "name": LambdaFunctionRecommendationFilterNameType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+ExternalMetricStatusTypeDef = TypedDict(
+    "ExternalMetricStatusTypeDef",
+    {
+        "statusCode": ExternalMetricStatusCodeType,
+        "statusReason": str,
+    },
+    total=False,
+)
+
 GetRecommendationErrorTypeDef = TypedDict(
     "GetRecommendationErrorTypeDef",
     {
         "identifier": str,
         "code": str,
         "message": str,
     },
@@ -414,14 +416,35 @@
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+GetEnrollmentStatusResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "memberAccountsEnrolled": bool,
+        "lastUpdatedTimestamp": datetime,
+        "numberOfMemberAccountsOptedIn": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRecommendationSummariesRequestRequestTypeDef = TypedDict(
     "GetRecommendationSummariesRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -453,14 +476,24 @@
         "name": LambdaFunctionMetricNameType,
         "statistic": LambdaFunctionMetricStatisticType,
         "value": float,
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
 ProjectedMetricTypeDef = TypedDict(
     "ProjectedMetricTypeDef",
     {
         "name": MetricNameType,
         "timestamps": List[datetime],
         "values": List[float],
     },
@@ -472,14 +505,25 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
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
 _RequiredUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnrollmentStatusRequestRequestTypeDef",
     {
         "status": StatusType,
     },
 )
 _OptionalUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
@@ -492,27 +536,46 @@
 
 class UpdateEnrollmentStatusRequestRequestTypeDef(
     _RequiredUpdateEnrollmentStatusRequestRequestTypeDef,
     _OptionalUpdateEnrollmentStatusRequestRequestTypeDef,
 ):
     pass
 
+UpdateEnrollmentStatusResponseTypeDef = TypedDict(
+    "UpdateEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VolumeConfigurationTypeDef = TypedDict(
     "VolumeConfigurationTypeDef",
     {
         "volumeType": str,
         "volumeSize": int,
         "volumeBaselineIOPS": int,
         "volumeBurstIOPS": int,
         "volumeBaselineThroughput": int,
         "volumeBurstThroughput": int,
+        "rootVolume": bool,
     },
     total=False,
 )
 
+GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    {
+        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ContainerConfigurationTypeDef = TypedDict(
     "ContainerConfigurationTypeDef",
     {
         "containerName": str,
         "memorySizeConfiguration": MemorySizeConfigurationTypeDef,
         "cpu": int,
     },
@@ -546,115 +609,76 @@
 
 class DeleteRecommendationPreferencesRequestRequestTypeDef(
     _RequiredDeleteRecommendationPreferencesRequestRequestTypeDef,
     _OptionalDeleteRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
+_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
+_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "scope": ScopeTypeDef,
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class GetRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
+class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
+    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
 ):
     pass
 
-DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
-    {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
-    {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "scope": ScopeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
-    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+class GetRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
-GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     {
-        "accountIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-GetEnrollmentStatusResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "memberAccountsEnrolled": bool,
-        "lastUpdatedTimestamp": datetime,
-        "numberOfMemberAccountsOptedIn": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     {
-        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEnrollmentStatusResponseTypeDef = TypedDict(
-    "UpdateEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "maxResults": int,
     },
+    total=False,
 )
 
 GetEBSVolumeRecommendationsRequestRequestTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     {
         "volumeArns": Sequence[str],
         "nextToken": str,
@@ -699,15 +723,15 @@
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
@@ -742,29 +766,38 @@
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+InferredWorkloadSavingTypeDef = TypedDict(
+    "InferredWorkloadSavingTypeDef",
+    {
+        "inferredWorkloadTypes": List[InferredWorkloadTypeType],
+        "estimatedMonthlySavings": EstimatedMonthlySavingsTypeDef,
+    },
+    total=False,
+)
+
 SavingsOpportunityTypeDef = TypedDict(
     "SavingsOpportunityTypeDef",
     {
         "savingsOpportunityPercentage": float,
         "estimatedMonthlySavings": EstimatedMonthlySavingsTypeDef,
     },
     total=False,
@@ -919,15 +952,15 @@
     pass
 
 ExportAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportDestinationTypeDef = TypedDict(
     "ExportDestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
@@ -936,42 +969,42 @@
 )
 
 ExportEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportECSServiceRecommendationsResponseTypeDef = TypedDict(
     "ExportECSServiceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
@@ -997,15 +1030,15 @@
 
 GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     {
         "functionArns": Sequence[str],
         "accountIds": Sequence[str],
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
@@ -1052,24 +1085,24 @@
 
 GetECSServiceRecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetRecommendationPreferencesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
@@ -1144,26 +1177,27 @@
     total=False,
 )
 
 GetEC2RecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[RecommendedOptionProjectedMetricTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "summaries": List[SummaryTypeDef],
         "recommendationResourceType": RecommendationSourceTypeType,
         "accountId": str,
         "savingsOpportunity": SavingsOpportunityTypeDef,
         "currentPerformanceRiskRatings": CurrentPerformanceRiskRatingsTypeDef,
+        "inferredWorkloadSavings": List[InferredWorkloadSavingTypeDef],
     },
     total=False,
 )
 
 AutoScalingGroupRecommendationTypeDef = TypedDict(
     "AutoScalingGroupRecommendationTypeDef",
     {
@@ -1193,14 +1227,15 @@
         "lookbackPeriodInDays": float,
         "launchType": ECSServiceLaunchTypeType,
         "lastRefreshTimestamp": datetime,
         "finding": ECSServiceRecommendationFindingType,
         "findingReasonCodes": List[ECSServiceRecommendationFindingReasonCodeType],
         "serviceRecommendationOptions": List[ECSServiceRecommendationOptionTypeDef],
         "currentPerformanceRisk": CurrentPerformanceRiskType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 InstanceRecommendationTypeDef = TypedDict(
     "InstanceRecommendationTypeDef",
     {
@@ -1214,14 +1249,17 @@
         "lookBackPeriodInDays": float,
         "recommendationOptions": List[InstanceRecommendationOptionTypeDef],
         "recommendationSources": List[RecommendationSourceTypeDef],
         "lastRefreshTimestamp": datetime,
         "currentPerformanceRisk": CurrentPerformanceRiskType,
         "effectiveRecommendationPreferences": EffectiveRecommendationPreferencesTypeDef,
         "inferredWorkloadTypes": List[InferredWorkloadTypeType],
+        "instanceState": InstanceStateType,
+        "tags": List[TagTypeDef],
+        "externalMetricStatus": ExternalMetricStatusTypeDef,
     },
     total=False,
 )
 
 LambdaFunctionRecommendationTypeDef = TypedDict(
     "LambdaFunctionRecommendationTypeDef",
     {
@@ -1233,14 +1271,15 @@
         "utilizationMetrics": List[LambdaFunctionUtilizationMetricTypeDef],
         "lookbackPeriodInDays": float,
         "lastRefreshTimestamp": datetime,
         "finding": LambdaFunctionRecommendationFindingType,
         "findingReasonCodes": List[LambdaFunctionRecommendationFindingReasonCodeType],
         "memorySizeRecommendationOptions": List[LambdaFunctionMemoryRecommendationOptionTypeDef],
         "currentPerformanceRisk": CurrentPerformanceRiskType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 VolumeRecommendationTypeDef = TypedDict(
     "VolumeRecommendationTypeDef",
     {
@@ -1249,77 +1288,78 @@
         "currentConfiguration": VolumeConfigurationTypeDef,
         "finding": EBSFindingType,
         "utilizationMetrics": List[EBSUtilizationMetricTypeDef],
         "lookBackPeriodInDays": float,
         "volumeRecommendationOptions": List[VolumeRecommendationOptionTypeDef],
         "lastRefreshTimestamp": datetime,
         "currentPerformanceRisk": CurrentPerformanceRiskType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 DescribeRecommendationExportJobsResponseTypeDef = TypedDict(
     "DescribeRecommendationExportJobsResponseTypeDef",
     {
         "recommendationExportJobs": List[RecommendationExportJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommendationSummariesResponseTypeDef = TypedDict(
     "GetRecommendationSummariesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationSummaries": List[RecommendationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "GetAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "autoScalingGroupRecommendations": List[AutoScalingGroupRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetECSServiceRecommendationsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "ecsServiceRecommendations": List[ECSServiceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "GetEC2InstanceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "instanceRecommendations": List[InstanceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "lambdaFunctionRecommendations": List[LambdaFunctionRecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "volumeRecommendations": List[VolumeRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/PKG-INFO` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.26.65
-Summary: Type annotations for boto3.ComputeOptimizer 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ComputeOptimizer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-compute-optimizer"></a>
 
 # mypy-boto3-compute-optimizer
 
 [![PyPI - mypy-boto3-compute-optimizer](https://img.shields.io/pypi/v/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,26 +339,28 @@
     EnhancedInfrastructureMetricsType,
     EnrollmentFilterNameType,
     ExportableAutoScalingGroupFieldType,
     ExportableECSServiceFieldType,
     ExportableInstanceFieldType,
     ExportableLambdaFunctionFieldType,
     ExportableVolumeFieldType,
+    ExternalMetricStatusCodeType,
     ExternalMetricsSourceType,
     FileFormatType,
     FilterNameType,
     FindingReasonCodeType,
     FindingType,
     GetEnrollmentStatusesForOrganizationPaginatorName,
     GetLambdaFunctionRecommendationsPaginatorName,
     GetRecommendationPreferencesPaginatorName,
     GetRecommendationSummariesPaginatorName,
     InferredWorkloadTypeType,
     InferredWorkloadTypesPreferenceType,
     InstanceRecommendationFindingReasonCodeType,
+    InstanceStateType,
     JobFilterNameType,
     JobStatusType,
     LambdaFunctionMemoryMetricNameType,
     LambdaFunctionMemoryMetricStatisticType,
     LambdaFunctionMetricNameType,
     LambdaFunctionMetricStatisticType,
     LambdaFunctionRecommendationFilterNameType,
@@ -397,61 +399,64 @@
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
+    TagTypeDef,
     ExternalMetricsPreferenceTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
+    ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
+    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestRequestTypeDef,
     DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
+    DescribeRecommendationExportJobsRequestRequestTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
     PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
+    InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
@@ -500,42 +505,42 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt` & `mypy-boto3-compute-optimizer-1.27.0/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.65/setup.py` & `mypy-boto3-compute-optimizer-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-compute-optimizer.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-compute-optimizer",
-    version="1.26.65",
+    version="1.27.0",
     packages=["mypy_boto3_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComputeOptimizer 1.26.65 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ComputeOptimizer 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/",
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


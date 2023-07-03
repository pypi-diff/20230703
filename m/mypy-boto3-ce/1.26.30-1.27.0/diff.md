# Comparing `tmp/mypy-boto3-ce-1.26.30.tar.gz` & `tmp/mypy-boto3-ce-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.26.30.tar", last modified: Wed Dec 14 20:47:11 2022, max compression
+gzip compressed data, was "mypy-boto3-ce-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-ce-1.26.30.tar` & `mypy-boto3-ce-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.637212 mypy-boto3-ce-1.26.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18809 2022-12-14 20:47:11.637212 mypy-boto3-ce-1.26.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.625212 mypy-boto3-ce-1.26.30/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31940 2022-12-14 20:46:53.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31896 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2022-12-14 20:46:53.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2022-12-14 20:46:53.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63350 2022-12-14 20:46:54.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63281 2022-12-14 20:46:54.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.637212 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18809 2022-12-14 20:47:11.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-14 20:47:11.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:47:11.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:47:11.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-14 20:47:11.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-14 20:47:11.000000 mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 20:47:11.637212 mypy-boto3-ce-1.26.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2022-12-14 20:46:52.000000 mypy-boto3-ce-1.26.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17305 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31896 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-07-03 19:33:15.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-03 19:33:15.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63440 2023-07-03 19:33:17.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63371 2023-07-03 19:33:16.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/setup.py
```

### Comparing `mypy-boto3-ce-1.26.30/LICENSE` & `mypy-boto3-ce-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ce-1.26.30/PKG-INFO` & `mypy-boto3-ce-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.26.30
-Summary: Type annotations for boto3.CostExplorer 1.26.30 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.CostExplorer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,19 +346,22 @@
     CostCategorySplitChargeRuleParameterTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
     TagValuesTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
@@ -368,67 +371,64 @@
     ElastiCacheInstanceDetailsTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
+    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
+    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
+    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
-    GetCostCategoriesResponseTypeDef,
-    GetTagsResponseTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ExpressionTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
@@ -495,42 +495,42 @@
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

### Comparing `mypy-boto3-ce-1.26.30/README.md` & `mypy-boto3-ce-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,19 +314,22 @@
     CostCategorySplitChargeRuleParameterTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
     TagValuesTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
@@ -336,67 +339,64 @@
     ElastiCacheInstanceDetailsTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
+    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
+    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
+    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
-    GetCostCategoriesResponseTypeDef,
-    GetTagsResponseTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ExpressionTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
@@ -463,42 +463,42 @@
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

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/__main__.py` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.26.30\nVersion:         1.26.30\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.CostExplorer 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.30")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountScopeType",
     "AnomalyFeedbackTypeType",
     "AnomalySubscriptionFrequencyType",
     "ContextType",
     "CostAllocationTagStatusType",
     "CostAllocationTagTypeType",
@@ -56,15 +55,14 @@
     "SupportedSavingsPlansTypeType",
     "TermInYearsType",
     "CostExplorerServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 AccountScopeType = Literal["LINKED", "PAYER"]
 AnomalyFeedbackTypeType = Literal["NO", "PLANNED_ACTIVITY", "YES"]
 AnomalySubscriptionFrequencyType = Literal["DAILY", "IMMEDIATE", "WEEKLY"]
 ContextType = Literal["COST_AND_USAGE", "RESERVATIONS", "SAVINGS_PLANS"]
 CostAllocationTagStatusType = Literal["Active", "Inactive"]
 CostAllocationTagTypeType = Literal["AWSGenerated", "UserDefined"]
 CostCategoryInheritedValueDimensionNameType = Literal["LINKED_ACCOUNT_NAME", "TAG"]
@@ -192,14 +190,15 @@
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
@@ -220,31 +219,34 @@
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
@@ -323,14 +325,15 @@
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
@@ -341,34 +344,38 @@
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
@@ -381,14 +388,15 @@
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
@@ -407,16 +415,19 @@
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
@@ -496,18 +507,21 @@
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

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccountScopeType",
     "AnomalyFeedbackTypeType",
     "AnomalySubscriptionFrequencyType",
     "ContextType",
     "CostAllocationTagStatusType",
     "CostAllocationTagTypeType",
@@ -55,14 +56,15 @@
     "SupportedSavingsPlansTypeType",
     "TermInYearsType",
     "CostExplorerServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
+
 AccountScopeType = Literal["LINKED", "PAYER"]
 AnomalyFeedbackTypeType = Literal["NO", "PLANNED_ACTIVITY", "YES"]
 AnomalySubscriptionFrequencyType = Literal["DAILY", "IMMEDIATE", "WEEKLY"]
 ContextType = Literal["COST_AND_USAGE", "RESERVATIONS", "SAVINGS_PLANS"]
 CostAllocationTagStatusType = Literal["Active", "Inactive"]
 CostAllocationTagTypeType = Literal["AWSGenerated", "UserDefined"]
 CostCategoryInheritedValueDimensionNameType = Literal["LINKED_ACCOUNT_NAME", "TAG"]
@@ -190,14 +192,15 @@
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
@@ -218,31 +221,34 @@
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
@@ -321,14 +327,15 @@
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
@@ -339,34 +346,38 @@
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
@@ -379,14 +390,15 @@
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
@@ -405,16 +417,19 @@
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
@@ -494,18 +509,21 @@
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

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,22 @@
     "CostCategorySplitChargeRuleParameterTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
     "TagValuesTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
@@ -94,67 +97,64 @@
     "ElastiCacheInstanceDetailsTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
+    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
+    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
-    "GetCostCategoriesResponseTypeDef",
-    "GetTagsResponseTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ExpressionTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
@@ -407,22 +407,36 @@
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagValuesTypeDef = TypedDict(
     "TagValuesTypeDef",
     {
         "Key": str,
@@ -449,14 +463,23 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
@@ -670,14 +693,26 @@
 )
 
 
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
 
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
     total=False,
@@ -780,14 +815,25 @@
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
     total=False,
 )
 
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "DatabaseEngine": str,
@@ -856,24 +902,43 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
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
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
     total=False,
@@ -944,14 +1009,24 @@
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
     total=False,
 )
 
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
     },
 )
@@ -974,24 +1049,58 @@
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1071,14 +1180,23 @@
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionTypeDef,
         "Type": CostCategoryRuleTypeType,
@@ -1211,145 +1329,27 @@
 class CreateAnomalyMonitorRequestRequestTypeDef(
     _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
     _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-)
-
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 
 ExpressionTypeDef = TypedDict(
     "ExpressionTypeDef",
     {
         "Or": Sequence[Dict[str, Any]],
@@ -1365,15 +1365,15 @@
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
@@ -1403,15 +1403,15 @@
 )
 
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1848,15 +1848,15 @@
     total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -1879,33 +1879,33 @@
 
 
 GetAnomalySubscriptionsResponseTypeDef = TypedDict(
     "GetAnomalySubscriptionsResponseTypeDef",
     {
         "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCostCategoryTypeDef = TypedDict(
     "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
@@ -1985,24 +1985,24 @@
 
 
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
@@ -2097,59 +2097,61 @@
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "SavingsPlansPurchaseRecommendationDetails": List[
             SavingsPlansPurchaseRecommendationDetailTypeDef
         ],
-        "SavingsPlansPurchaseRecommendationSummary": SavingsPlansPurchaseRecommendationSummaryTypeDef,
+        "SavingsPlansPurchaseRecommendationSummary": (
+            SavingsPlansPurchaseRecommendationSummaryTypeDef
+        ),
     },
     total=False,
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
         "TimePeriod": DateIntervalTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
@@ -2194,36 +2196,36 @@
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2239,25 +2241,25 @@
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
@@ -2267,15 +2269,15 @@
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
@@ -2292,10 +2294,10 @@
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,22 @@
     "CostCategorySplitChargeRuleParameterTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
     "TagValuesTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
@@ -93,67 +96,64 @@
     "ElastiCacheInstanceDetailsTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
+    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
+    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
-    "GetCostCategoriesResponseTypeDef",
-    "GetTagsResponseTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ExpressionTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
@@ -400,22 +400,36 @@
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagValuesTypeDef = TypedDict(
     "TagValuesTypeDef",
     {
         "Key": str,
@@ -442,14 +456,23 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
@@ -657,14 +680,26 @@
     },
     total=False,
 )
 
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
     total=False,
@@ -765,14 +800,25 @@
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
     total=False,
 )
 
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "DatabaseEngine": str,
@@ -841,24 +887,43 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
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
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
     total=False,
@@ -929,14 +994,24 @@
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
     total=False,
 )
 
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
     },
 )
@@ -957,24 +1032,58 @@
 
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1048,14 +1157,23 @@
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionTypeDef,
         "Type": CostCategoryRuleTypeType,
@@ -1180,145 +1298,27 @@
 
 class CreateAnomalyMonitorRequestRequestTypeDef(
     _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
     _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-)
-
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 
 ExpressionTypeDef = TypedDict(
     "ExpressionTypeDef",
     {
         "Or": Sequence[Dict[str, Any]],
@@ -1334,15 +1334,15 @@
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
@@ -1372,15 +1372,15 @@
 )
 
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1789,15 +1789,15 @@
     total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -1818,33 +1818,33 @@
     pass
 
 GetAnomalySubscriptionsResponseTypeDef = TypedDict(
     "GetAnomalySubscriptionsResponseTypeDef",
     {
         "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCostCategoryTypeDef = TypedDict(
     "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
@@ -1918,24 +1918,24 @@
     pass
 
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
@@ -2028,59 +2028,61 @@
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "SavingsPlansPurchaseRecommendationDetails": List[
             SavingsPlansPurchaseRecommendationDetailTypeDef
         ],
-        "SavingsPlansPurchaseRecommendationSummary": SavingsPlansPurchaseRecommendationSummaryTypeDef,
+        "SavingsPlansPurchaseRecommendationSummary": (
+            SavingsPlansPurchaseRecommendationSummaryTypeDef
+        ),
     },
     total=False,
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
         "TimePeriod": DateIntervalTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
@@ -2125,36 +2127,36 @@
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2170,25 +2172,25 @@
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
@@ -2198,15 +2200,15 @@
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
@@ -2223,10 +2225,10 @@
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.26.30
-Summary: Type annotations for boto3.CostExplorer 1.26.30 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.CostExplorer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,19 +346,22 @@
     CostCategorySplitChargeRuleParameterTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
     TagValuesTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
@@ -368,67 +371,64 @@
     ElastiCacheInstanceDetailsTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
+    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
+    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
+    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
-    GetCostCategoriesResponseTypeDef,
-    GetTagsResponseTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ExpressionTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
@@ -495,42 +495,42 @@
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

### Comparing `mypy-boto3-ce-1.26.30/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.26.30/setup.py` & `mypy-boto3-ce-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-ce.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.26.30",
+    version="1.27.0",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostExplorer 1.26.30 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.CostExplorer 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/",
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


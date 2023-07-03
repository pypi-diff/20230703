# Comparing `tmp/mypy-boto3-personalize-1.26.143.tar.gz` & `tmp/mypy-boto3-personalize-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-1.26.143.tar", last modified: Tue May 30 19:32:53 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-1.27.0.tar", last modified: Mon Jul  3 19:51:14 2023, max compression
```

## Comparing `mypy-boto3-personalize-1.26.143.tar` & `mypy-boto3-personalize-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23648 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22143 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:53.419270 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50910 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-30 19:32:22.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-05-30 19:32:22.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62496 2023-05-30 19:32:23.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62461 2023-05-30 19:32:23.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23648 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.703795 mypy-boto3-personalize-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23642 2023-07-03 19:51:14.703795 mypy-boto3-personalize-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22141 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.699795 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-07-03 19:43:22.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50910 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-03 19:43:22.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-03 19:43:22.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-07-03 19:43:22.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-03 19:43:22.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62638 2023-07-03 19:43:23.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62603 2023-07-03 19:43:23.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.703795 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23642 2023-07-03 19:51:14.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 19:51:14.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:14.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:51:14.000000 mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:14.703795 mypy-boto3-personalize-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:43:21.000000 mypy-boto3-personalize-1.27.0/setup.py
```

### Comparing `mypy-boto3-personalize-1.26.143/LICENSE` & `mypy-boto3-personalize-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.143/PKG-INFO` & `mypy-boto3-personalize-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.26.143
-Summary: Type annotations for boto3.Personalize 1.26.143 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Personalize 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.26.143](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -401,18 +401,31 @@
     BatchInferenceJobSummaryTypeDef,
     BatchSegmentJobSummaryTypeDef,
     CampaignConfigTypeDef,
     CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
     DataSourceTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
     MetricAttributeTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
     DatasetSummaryTypeDef,
@@ -446,89 +459,92 @@
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     RecipeTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTrackerSummaryTypeDef,
     FilterSummaryTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
+    GetSolutionMetricsResponseTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
     IntegerHyperParameterRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
     ListBatchInferenceJobsRequestRequestTypeDef,
+    ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
     ListBatchSegmentJobsRequestRequestTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef,
     ListDatasetExportJobsRequestRequestTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListEventTrackersRequestListEventTrackersPaginateTypeDef,
     ListEventTrackersRequestRequestTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
+    ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
+    ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
     MetricAttributionSummaryTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
     RecipeSummaryTypeDef,
+    ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
+    ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
     SolutionVersionSummaryTypeDef,
+    ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
     SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OptimizationObjectiveTypeDef,
+    PaginatorConfigTypeDef,
     TrainingDataConfigTypeDef,
+    ResponseMetadataTypeDef,
     TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
+    StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
+    StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateCampaignResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
     CampaignUpdateSummaryTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    ListCampaignsResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartRecommenderResponseTypeDef,
-    StopRecommenderResponseTypeDef,
-    UpdateCampaignResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
@@ -540,30 +556,14 @@
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     HyperParameterRangesTypeDef,
-    ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
-    ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
-    ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListEventTrackersRequestListEventTrackersPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
-    ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
-    ListRecommendersRequestListRecommendersPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
-    ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListSolutionsResponseTypeDef,
     RecommenderConfigTypeDef,
     BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-personalize-1.26.143/README.md` & `mypy-boto3-personalize-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.26.143](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -369,18 +369,31 @@
     BatchInferenceJobSummaryTypeDef,
     BatchSegmentJobSummaryTypeDef,
     CampaignConfigTypeDef,
     CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
     DataSourceTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
     MetricAttributeTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
     DatasetSummaryTypeDef,
@@ -414,89 +427,92 @@
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     RecipeTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTrackerSummaryTypeDef,
     FilterSummaryTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
+    GetSolutionMetricsResponseTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
     IntegerHyperParameterRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
     ListBatchInferenceJobsRequestRequestTypeDef,
+    ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
     ListBatchSegmentJobsRequestRequestTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef,
     ListDatasetExportJobsRequestRequestTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListEventTrackersRequestListEventTrackersPaginateTypeDef,
     ListEventTrackersRequestRequestTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
+    ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
+    ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
     MetricAttributionSummaryTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
     RecipeSummaryTypeDef,
+    ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
+    ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
     SolutionVersionSummaryTypeDef,
+    ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
     SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OptimizationObjectiveTypeDef,
+    PaginatorConfigTypeDef,
     TrainingDataConfigTypeDef,
+    ResponseMetadataTypeDef,
     TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
+    StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
+    StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateCampaignResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
     CampaignUpdateSummaryTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    ListCampaignsResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartRecommenderResponseTypeDef,
-    StopRecommenderResponseTypeDef,
-    UpdateCampaignResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
@@ -508,30 +524,14 @@
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     HyperParameterRangesTypeDef,
-    ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
-    ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
-    ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListEventTrackersRequestListEventTrackersPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
-    ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
-    ListRecommendersRequestListRecommendersPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
-    ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListSolutionsResponseTypeDef,
     RecommenderConfigTypeDef,
     BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.py` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.pyi` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__main__.py` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.26.143\nVersion:         1.26.143\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Personalize 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.143")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.py` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.pyi` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.py` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
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
@@ -131,14 +132,15 @@
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
@@ -310,14 +312,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
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
@@ -401,14 +405,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.pyi` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
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
@@ -129,14 +130,15 @@
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
@@ -308,14 +310,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
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
@@ -399,14 +403,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.py` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,165 +114,165 @@
 class ListBatchInferenceJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
     """
 
     def paginate(
-        self, *, solutionVersionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchInferenceJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
         """
 
 
 class ListBatchSegmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
     """
 
     def paginate(
-        self, *, solutionVersionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchSegmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
         """
 
 
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
     """
 
     def paginate(
-        self, *, solutionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
         """
 
 
 class ListDatasetExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
     """
 
     def paginate(
-        self, *, datasetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
         """
 
 
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
         """
 
 
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
-        self, *, datasetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
         """
 
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
         """
 
 
 class ListEventTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
         """
 
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
         """
 
 
 class ListMetricAttributionMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
     """
 
     def paginate(
-        self, *, metricAttributionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, metricAttributionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMetricAttributionMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
         """
 
 
 class ListMetricAttributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMetricAttributionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
         """
 
 
@@ -283,73 +283,73 @@
     """
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecipespaginator)
         """
 
 
 class ListRecommendersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecommendersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
         """
 
 
 class ListSolutionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
     """
 
     def paginate(
-        self, *, solutionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolutionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
         """
 
 
 class ListSolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
         """
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.pyi` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -110,155 +110,155 @@
 class ListBatchInferenceJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
     """
 
     def paginate(
-        self, *, solutionVersionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchInferenceJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
         """
 
 class ListBatchSegmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
     """
 
     def paginate(
-        self, *, solutionVersionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchSegmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
         """
 
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
     """
 
     def paginate(
-        self, *, solutionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
         """
 
 class ListDatasetExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
     """
 
     def paginate(
-        self, *, datasetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
         """
 
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
         """
 
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
-        self, *, datasetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
         """
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
         """
 
 class ListEventTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
         """
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
         """
 
 class ListMetricAttributionMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
     """
 
     def paginate(
-        self, *, metricAttributionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, metricAttributionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMetricAttributionMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
         """
 
 class ListMetricAttributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMetricAttributionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
         """
 
 class ListRecipesPaginator(Paginator):
@@ -268,69 +268,69 @@
     """
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecipespaginator)
         """
 
 class ListRecommendersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecommendersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
         """
 
 class ListSolutionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
     """
 
     def paginate(
-        self, *, solutionArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolutionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
         """
 
 class ListSolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
     """
 
     def paginate(
-        self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
         """
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.py` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,32 +28,44 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlgorithmImageTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBatchInferenceJobResponseTypeDef",
+    "CreateBatchSegmentJobResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDatasetExportJobResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
     "DataSourceTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateEventTrackerResponseTypeDef",
+    "CreateFilterResponseTypeDef",
     "MetricAttributeTypeDef",
+    "CreateMetricAttributionResponseTypeDef",
+    "CreateRecommenderResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "CreateSolutionResponseTypeDef",
+    "CreateSolutionVersionResponseTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
@@ -87,89 +99,92 @@
     "DescribeMetricAttributionRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "RecipeTypeDef",
     "DescribeRecommenderRequestRequestTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
     "DescribeSolutionRequestRequestTypeDef",
     "DescribeSolutionVersionRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventTrackerSummaryTypeDef",
     "FilterSummaryTypeDef",
     "GetSolutionMetricsRequestRequestTypeDef",
+    "GetSolutionMetricsResponseTypeDef",
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
     "IntegerHyperParameterRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchInferenceJobsRequestRequestTypeDef",
+    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestRequestTypeDef",
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
     "ListDatasetExportJobsRequestRequestTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
+    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
     "ListEventTrackersRequestRequestTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
+    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
+    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     "ListMetricAttributionsRequestRequestTypeDef",
     "MetricAttributionSummaryTypeDef",
+    "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
     "RecipeSummaryTypeDef",
+    "ListRecommendersRequestListRecommendersPaginateTypeDef",
     "ListRecommendersRequestRequestTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
+    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
+    "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
+    "PaginatorConfigTypeDef",
     "TrainingDataConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
+    "StartRecommenderResponseTypeDef",
     "StopRecommenderRequestRequestTypeDef",
+    "StopRecommenderResponseTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateCampaignResponseTypeDef",
+    "UpdateMetricAttributionResponseTypeDef",
+    "UpdateRecommenderResponseTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
+    "ListBatchInferenceJobsResponseTypeDef",
+    "ListBatchSegmentJobsResponseTypeDef",
     "CampaignUpdateSummaryTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
+    "ListCampaignsResponseTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateBatchInferenceJobResponseTypeDef",
-    "CreateBatchSegmentJobResponseTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDatasetExportJobResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateEventTrackerResponseTypeDef",
-    "CreateFilterResponseTypeDef",
-    "CreateMetricAttributionResponseTypeDef",
-    "CreateRecommenderResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "CreateSolutionResponseTypeDef",
-    "CreateSolutionVersionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetSolutionMetricsResponseTypeDef",
-    "ListBatchInferenceJobsResponseTypeDef",
-    "ListBatchSegmentJobsResponseTypeDef",
-    "ListCampaignsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartRecommenderResponseTypeDef",
-    "StopRecommenderResponseTypeDef",
-    "UpdateCampaignResponseTypeDef",
-    "UpdateMetricAttributionResponseTypeDef",
-    "UpdateRecommenderResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
@@ -181,30 +196,14 @@
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ListFiltersResponseTypeDef",
     "HyperParameterRangesTypeDef",
-    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
-    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
-    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    "ListRecommendersRequestListRecommendersPaginateTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
-    "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
     "RecommenderConfigTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
@@ -250,19 +249,17 @@
     "_OptionalAlgorithmImageTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-
 class AlgorithmImageTypeDef(_RequiredAlgorithmImageTypeDef, _OptionalAlgorithmImageTypeDef):
     pass
 
-
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
@@ -294,19 +291,17 @@
     "_OptionalS3DataConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class S3DataConfigTypeDef(_RequiredS3DataConfigTypeDef, _OptionalS3DataConfigTypeDef):
     pass
 
-
 BatchInferenceJobSummaryTypeDef = TypedDict(
     "BatchInferenceJobSummaryTypeDef",
     {
         "batchInferenceJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
@@ -375,42 +370,121 @@
     "TagTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBatchInferenceJobResponseTypeDef = TypedDict(
+    "CreateBatchInferenceJobResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "batchInferenceJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateBatchSegmentJobResponseTypeDef = TypedDict(
+    "CreateBatchSegmentJobResponseTypeDef",
+    {
+        "batchSegmentJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "campaignArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetExportJobResponseTypeDef = TypedDict(
+    "CreateDatasetExportJobResponseTypeDef",
+    {
+        "datasetExportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "datasetGroupArn": str,
+        "domain": DomainType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "dataLocation": str,
     },
     total=False,
 )
 
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "datasetImportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "datasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEventTrackerResponseTypeDef = TypedDict(
+    "CreateEventTrackerResponseTypeDef",
+    {
+        "eventTrackerArn": str,
+        "trackingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "filterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricAttributeTypeDef = TypedDict(
     "MetricAttributeTypeDef",
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
+CreateMetricAttributionResponseTypeDef = TypedDict(
+    "CreateMetricAttributionResponseTypeDef",
+    {
+        "metricAttributionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRecommenderResponseTypeDef = TypedDict(
+    "CreateRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "name": str,
         "schema": str,
     },
 )
@@ -418,20 +492,42 @@
     "_OptionalCreateSchemaRequestRequestTypeDef",
     {
         "domain": DomainType,
     },
     total=False,
 )
 
-
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "schemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSolutionResponseTypeDef = TypedDict(
+    "CreateSolutionResponseTypeDef",
+    {
+        "solutionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSolutionVersionResponseTypeDef = TypedDict(
+    "CreateSolutionVersionResponseTypeDef",
+    {
+        "solutionVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DatasetExportJobSummaryTypeDef = TypedDict(
     "DatasetExportJobSummaryTypeDef",
     {
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
@@ -808,14 +904,21 @@
 DescribeSolutionVersionRequestRequestTypeDef = TypedDict(
     "DescribeSolutionVersionRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventTrackerSummaryTypeDef = TypedDict(
     "EventTrackerSummaryTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
@@ -841,14 +944,23 @@
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
+GetSolutionMetricsResponseTypeDef = TypedDict(
+    "GetSolutionMetricsResponseTypeDef",
+    {
+        "solutionVersionArn": str,
+        "metrics": Dict[str, float],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HPOObjectiveTypeDef = TypedDict(
     "HPOObjectiveTypeDef",
     {
         "type": str,
         "metricName": str,
         "metricRegex": str,
     },
@@ -870,123 +982,211 @@
         "name": str,
         "minValue": int,
         "maxValue": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef = TypedDict(
+    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "solutionVersionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBatchInferenceJobsRequestRequestTypeDef = TypedDict(
     "ListBatchInferenceJobsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef = TypedDict(
+    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
+    {
+        "solutionVersionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBatchSegmentJobsRequestRequestTypeDef = TypedDict(
     "ListBatchSegmentJobsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    {
+        "solutionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
+    {
+        "datasetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetExportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetExportJobsRequestRequestTypeDef",
     {
         "datasetArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    {
+        "datasetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "datasetArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListEventTrackersRequestListEventTrackersPaginateTypeDef = TypedDict(
+    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEventTrackersRequestRequestTypeDef = TypedDict(
     "ListEventTrackersRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef = TypedDict(
+    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
+    {
+        "metricAttributionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMetricAttributionMetricsRequestRequestTypeDef = TypedDict(
     "ListMetricAttributionMetricsRequestRequestTypeDef",
     {
         "metricAttributionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef = TypedDict(
+    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMetricAttributionsRequestRequestTypeDef = TypedDict(
     "ListMetricAttributionsRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1002,14 +1202,24 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
     total=False,
 )
 
+ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
+    "ListRecipesRequestListRecipesPaginateTypeDef",
+    {
+        "recipeProvider": Literal["SERVICE"],
+        "domain": DomainType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "recipeProvider": Literal["SERVICE"],
         "nextToken": str,
         "maxResults": int,
         "domain": DomainType,
@@ -1026,33 +1236,59 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
     total=False,
 )
 
+ListRecommendersRequestListRecommendersPaginateTypeDef = TypedDict(
+    "ListRecommendersRequestListRecommendersPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecommendersRequestRequestTypeDef = TypedDict(
     "ListRecommendersRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchemasRequestRequestTypeDef = TypedDict(
     "ListSchemasRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef = TypedDict(
+    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
+    {
+        "solutionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolutionVersionsRequestRequestTypeDef = TypedDict(
     "ListSolutionVersionsRequestRequestTypeDef",
     {
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1067,14 +1303,23 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
     total=False,
 )
 
+ListSolutionsRequestListSolutionsPaginateTypeDef = TypedDict(
+    "ListSolutionsRequestListSolutionsPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolutionsRequestRequestTypeDef = TypedDict(
     "ListSolutionsRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1106,22 +1351,43 @@
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
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
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
         "excludedDatasetColumns": Mapping[str, Sequence[str]],
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
 TunedHPOParamsTypeDef = TypedDict(
     "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
     total=False,
 )
@@ -1129,21 +1395,37 @@
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
+StartRecommenderResponseTypeDef = TypedDict(
+    "StartRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopRecommenderRequestRequestTypeDef = TypedDict(
     "StopRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
+StopRecommenderResponseTypeDef = TypedDict(
+    "StopRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopSolutionVersionCreationRequestRequestTypeDef = TypedDict(
     "StopSolutionVersionCreationRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
@@ -1151,14 +1433,38 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
+    {
+        "campaignArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateMetricAttributionResponseTypeDef = TypedDict(
+    "UpdateMetricAttributionResponseTypeDef",
+    {
+        "metricAttributionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRecommenderResponseTypeDef = TypedDict(
+    "UpdateRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 
@@ -1200,20 +1506,36 @@
     "_OptionalMetricAttributionOutputTypeDef",
     {
         "s3DataDestination": S3DataConfigTypeDef,
     },
     total=False,
 )
 
-
 class MetricAttributionOutputTypeDef(
     _RequiredMetricAttributionOutputTypeDef, _OptionalMetricAttributionOutputTypeDef
 ):
     pass
 
+ListBatchInferenceJobsResponseTypeDef = TypedDict(
+    "ListBatchInferenceJobsResponseTypeDef",
+    {
+        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBatchSegmentJobsResponseTypeDef = TypedDict(
+    "ListBatchSegmentJobsResponseTypeDef",
+    {
+        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CampaignUpdateSummaryTypeDef = TypedDict(
     "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
@@ -1237,20 +1559,27 @@
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
+ListCampaignsResponseTypeDef = TypedDict(
+    "ListCampaignsResponseTypeDef",
+    {
+        "campaigns": List[CampaignSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
     },
@@ -1261,21 +1590,19 @@
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDatasetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetGroupRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateDatasetGroupRequestRequestTypeDef = TypedDict(
@@ -1285,22 +1612,20 @@
         "kmsKeyArn": str,
         "domain": DomainType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "datasetGroupArn": str,
         "datasetType": str,
@@ -1310,21 +1635,19 @@
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateEventTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventTrackerRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
     },
 )
@@ -1332,22 +1655,20 @@
     "_OptionalCreateEventTrackerRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEventTrackerRequestRequestTypeDef(
     _RequiredCreateEventTrackerRequestRequestTypeDef,
     _OptionalCreateEventTrackerRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "filterExpression": str,
     },
@@ -1356,21 +1677,19 @@
     "_OptionalCreateFilterRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateSolutionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSolutionVersionRequestRequestTypeDef",
     {
         "solutionArn": str,
     },
 )
 _OptionalCreateSolutionVersionRequestRequestTypeDef = TypedDict(
@@ -1379,232 +1698,33 @@
         "name": str,
         "trainingMode": TrainingModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSolutionVersionRequestRequestTypeDef(
     _RequiredCreateSolutionVersionRequestRequestTypeDef,
     _OptionalCreateSolutionVersionRequestRequestTypeDef,
 ):
     pass
 
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateBatchInferenceJobResponseTypeDef = TypedDict(
-    "CreateBatchInferenceJobResponseTypeDef",
-    {
-        "batchInferenceJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBatchSegmentJobResponseTypeDef = TypedDict(
-    "CreateBatchSegmentJobResponseTypeDef",
-    {
-        "batchSegmentJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "campaignArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetExportJobResponseTypeDef = TypedDict(
-    "CreateDatasetExportJobResponseTypeDef",
-    {
-        "datasetExportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "datasetGroupArn": str,
-        "domain": DomainType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "datasetImportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "datasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventTrackerResponseTypeDef = TypedDict(
-    "CreateEventTrackerResponseTypeDef",
-    {
-        "eventTrackerArn": str,
-        "trackingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "filterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMetricAttributionResponseTypeDef = TypedDict(
-    "CreateMetricAttributionResponseTypeDef",
-    {
-        "metricAttributionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRecommenderResponseTypeDef = TypedDict(
-    "CreateRecommenderResponseTypeDef",
-    {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "schemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolutionResponseTypeDef = TypedDict(
-    "CreateSolutionResponseTypeDef",
-    {
-        "solutionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolutionVersionResponseTypeDef = TypedDict(
-    "CreateSolutionVersionResponseTypeDef",
-    {
-        "solutionVersionArn": str,
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
-GetSolutionMetricsResponseTypeDef = TypedDict(
-    "GetSolutionMetricsResponseTypeDef",
-    {
-        "solutionVersionArn": str,
-        "metrics": Dict[str, float],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBatchInferenceJobsResponseTypeDef = TypedDict(
-    "ListBatchInferenceJobsResponseTypeDef",
-    {
-        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBatchSegmentJobsResponseTypeDef = TypedDict(
-    "ListBatchSegmentJobsResponseTypeDef",
-    {
-        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCampaignsResponseTypeDef = TypedDict(
-    "ListCampaignsResponseTypeDef",
-    {
-        "campaigns": List[CampaignSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartRecommenderResponseTypeDef = TypedDict(
-    "StartRecommenderResponseTypeDef",
-    {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopRecommenderResponseTypeDef = TypedDict(
-    "StopRecommenderResponseTypeDef",
-    {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
-    {
-        "campaignArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMetricAttributionResponseTypeDef = TypedDict(
-    "UpdateMetricAttributionResponseTypeDef",
-    {
-        "metricAttributionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRecommenderResponseTypeDef = TypedDict(
-    "UpdateRecommenderResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -1619,22 +1739,20 @@
         "tags": Sequence[TagTypeDef],
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
     total=False,
 )
 
-
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DatasetImportJobTypeDef = TypedDict(
     "DatasetImportJobTypeDef",
     {
         "jobName": str,
         "datasetImportJobArn": str,
         "datasetArn": str,
         "dataSource": DataSourceTypeDef,
@@ -1650,84 +1768,84 @@
 )
 
 ListMetricAttributionMetricsResponseTypeDef = TypedDict(
     "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetExportJobsResponseTypeDef = TypedDict(
     "ListDatasetExportJobsResponseTypeDef",
     {
         "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "datasetGroups": List[DatasetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetGroupResponseTypeDef = TypedDict(
     "DescribeDatasetGroupResponseTypeDef",
     {
         "datasetGroup": DatasetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "datasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "schemas": List[DatasetSchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSchemaResponseTypeDef = TypedDict(
     "DescribeSchemaResponseTypeDef",
     {
         "schema": DatasetSchemaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefaultHyperParameterRangesTypeDef = TypedDict(
     "DefaultHyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
@@ -1737,246 +1855,103 @@
     total=False,
 )
 
 DescribeEventTrackerResponseTypeDef = TypedDict(
     "DescribeEventTrackerResponseTypeDef",
     {
         "eventTracker": EventTrackerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFeatureTransformationResponseTypeDef = TypedDict(
     "DescribeFeatureTransformationResponseTypeDef",
     {
         "featureTransformation": FeatureTransformationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFilterResponseTypeDef = TypedDict(
     "DescribeFilterResponseTypeDef",
     {
         "filter": FilterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "recipe": RecipeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventTrackersResponseTypeDef = TypedDict(
     "ListEventTrackersResponseTypeDef",
     {
         "eventTrackers": List[EventTrackerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef = TypedDict(
-    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
-    {
-        "solutionVersionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef = TypedDict(
-    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
-    {
-        "solutionVersionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    {
-        "solutionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
-    {
-        "datasetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    {
-        "datasetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventTrackersRequestListEventTrackersPaginateTypeDef = TypedDict(
-    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef = TypedDict(
-    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
-    {
-        "metricAttributionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef = TypedDict(
-    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    {
-        "recipeProvider": Literal["SERVICE"],
-        "domain": DomainType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecommendersRequestListRecommendersPaginateTypeDef = TypedDict(
-    "ListRecommendersRequestListRecommendersPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef = TypedDict(
-    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
-    {
-        "solutionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolutionsRequestListSolutionsPaginateTypeDef = TypedDict(
-    "ListSolutionsRequestListSolutionsPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMetricAttributionsResponseTypeDef = TypedDict(
     "ListMetricAttributionsResponseTypeDef",
     {
         "metricAttributions": List[MetricAttributionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecipesResponseTypeDef = TypedDict(
     "ListRecipesResponseTypeDef",
     {
         "recipes": List[RecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolutionVersionsResponseTypeDef = TypedDict(
     "ListSolutionVersionsResponseTypeDef",
     {
         "solutionVersions": List[SolutionVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolutionsResponseTypeDef = TypedDict(
     "ListSolutionsResponseTypeDef",
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
@@ -2023,22 +1998,20 @@
         "numResults": int,
         "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBatchInferenceJobRequestRequestTypeDef(
     _RequiredCreateBatchInferenceJobRequestRequestTypeDef,
     _OptionalCreateBatchInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-
 BatchSegmentJobTypeDef = TypedDict(
     "BatchSegmentJobTypeDef",
     {
         "jobName": str,
         "batchSegmentJobArn": str,
         "filterArn": str,
         "failureReason": str,
@@ -2070,22 +2043,20 @@
         "filterArn": str,
         "numResults": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBatchSegmentJobRequestRequestTypeDef(
     _RequiredCreateBatchSegmentJobRequestRequestTypeDef,
     _OptionalCreateBatchSegmentJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDatasetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetExportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "roleArn": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
@@ -2096,22 +2067,20 @@
     {
         "ingestionMode": IngestionModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetExportJobRequestRequestTypeDef(
     _RequiredCreateDatasetExportJobRequestRequestTypeDef,
     _OptionalCreateDatasetExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DatasetExportJobTypeDef = TypedDict(
     "DatasetExportJobTypeDef",
     {
         "jobName": str,
         "datasetExportJobArn": str,
         "datasetArn": str,
         "ingestionMode": IngestionModeType,
@@ -2178,15 +2147,15 @@
     total=False,
 )
 
 DescribeDatasetImportJobResponseTypeDef = TypedDict(
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
@@ -2226,21 +2195,19 @@
     {
         "recommenderConfig": RecommenderConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRecommenderRequestRequestTypeDef(
     _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
 ):
     pass
 
-
 RecommenderSummaryTypeDef = TypedDict(
     "RecommenderSummaryTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
@@ -2272,55 +2239,55 @@
     },
 )
 
 DescribeBatchInferenceJobResponseTypeDef = TypedDict(
     "DescribeBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJob": BatchInferenceJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBatchSegmentJobResponseTypeDef = TypedDict(
     "DescribeBatchSegmentJobResponseTypeDef",
     {
         "batchSegmentJob": BatchSegmentJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetExportJobResponseTypeDef = TypedDict(
     "DescribeDatasetExportJobResponseTypeDef",
     {
         "datasetExportJob": DatasetExportJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricAttributionResponseTypeDef = TypedDict(
     "DescribeMetricAttributionResponseTypeDef",
     {
         "metricAttribution": MetricAttributionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCampaignResponseTypeDef = TypedDict(
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAlgorithmResponseTypeDef = TypedDict(
     "DescribeAlgorithmResponseTypeDef",
     {
         "algorithm": AlgorithmTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": str,
@@ -2335,15 +2302,15 @@
 )
 
 ListRecommendersResponseTypeDef = TypedDict(
     "ListRecommendersResponseTypeDef",
     {
         "recommenders": List[RecommenderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommenderTypeDef = TypedDict(
     "RecommenderTypeDef",
     {
         "recommenderArn": str,
@@ -2377,21 +2344,19 @@
         "eventType": str,
         "solutionConfig": SolutionConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSolutionRequestRequestTypeDef(
     _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
 ):
     pass
 
-
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
@@ -2431,26 +2396,26 @@
     total=False,
 )
 
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSolutionResponseTypeDef = TypedDict(
     "DescribeSolutionResponseTypeDef",
     {
         "solution": SolutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSolutionVersionResponseTypeDef = TypedDict(
     "DescribeSolutionVersionResponseTypeDef",
     {
         "solutionVersion": SolutionVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.pyi` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,31 +28,45 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlgorithmImageTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBatchInferenceJobResponseTypeDef",
+    "CreateBatchSegmentJobResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDatasetExportJobResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
     "DataSourceTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateEventTrackerResponseTypeDef",
+    "CreateFilterResponseTypeDef",
     "MetricAttributeTypeDef",
+    "CreateMetricAttributionResponseTypeDef",
+    "CreateRecommenderResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "CreateSolutionResponseTypeDef",
+    "CreateSolutionVersionResponseTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
@@ -86,89 +100,92 @@
     "DescribeMetricAttributionRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "RecipeTypeDef",
     "DescribeRecommenderRequestRequestTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
     "DescribeSolutionRequestRequestTypeDef",
     "DescribeSolutionVersionRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventTrackerSummaryTypeDef",
     "FilterSummaryTypeDef",
     "GetSolutionMetricsRequestRequestTypeDef",
+    "GetSolutionMetricsResponseTypeDef",
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
     "IntegerHyperParameterRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchInferenceJobsRequestRequestTypeDef",
+    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestRequestTypeDef",
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
     "ListDatasetExportJobsRequestRequestTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
+    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
     "ListEventTrackersRequestRequestTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
+    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
+    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     "ListMetricAttributionsRequestRequestTypeDef",
     "MetricAttributionSummaryTypeDef",
+    "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
     "RecipeSummaryTypeDef",
+    "ListRecommendersRequestListRecommendersPaginateTypeDef",
     "ListRecommendersRequestRequestTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
+    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
+    "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
+    "PaginatorConfigTypeDef",
     "TrainingDataConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
+    "StartRecommenderResponseTypeDef",
     "StopRecommenderRequestRequestTypeDef",
+    "StopRecommenderResponseTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateCampaignResponseTypeDef",
+    "UpdateMetricAttributionResponseTypeDef",
+    "UpdateRecommenderResponseTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
+    "ListBatchInferenceJobsResponseTypeDef",
+    "ListBatchSegmentJobsResponseTypeDef",
     "CampaignUpdateSummaryTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
+    "ListCampaignsResponseTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateBatchInferenceJobResponseTypeDef",
-    "CreateBatchSegmentJobResponseTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDatasetExportJobResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateEventTrackerResponseTypeDef",
-    "CreateFilterResponseTypeDef",
-    "CreateMetricAttributionResponseTypeDef",
-    "CreateRecommenderResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "CreateSolutionResponseTypeDef",
-    "CreateSolutionVersionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetSolutionMetricsResponseTypeDef",
-    "ListBatchInferenceJobsResponseTypeDef",
-    "ListBatchSegmentJobsResponseTypeDef",
-    "ListCampaignsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartRecommenderResponseTypeDef",
-    "StopRecommenderResponseTypeDef",
-    "UpdateCampaignResponseTypeDef",
-    "UpdateMetricAttributionResponseTypeDef",
-    "UpdateRecommenderResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
@@ -180,30 +197,14 @@
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ListFiltersResponseTypeDef",
     "HyperParameterRangesTypeDef",
-    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
-    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
-    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    "ListRecommendersRequestListRecommendersPaginateTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
-    "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
     "RecommenderConfigTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
@@ -249,17 +250,19 @@
     "_OptionalAlgorithmImageTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
+
 class AlgorithmImageTypeDef(_RequiredAlgorithmImageTypeDef, _OptionalAlgorithmImageTypeDef):
     pass
 
+
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
@@ -291,17 +294,19 @@
     "_OptionalS3DataConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class S3DataConfigTypeDef(_RequiredS3DataConfigTypeDef, _OptionalS3DataConfigTypeDef):
     pass
 
+
 BatchInferenceJobSummaryTypeDef = TypedDict(
     "BatchInferenceJobSummaryTypeDef",
     {
         "batchInferenceJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
@@ -370,42 +375,121 @@
     "TagTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBatchInferenceJobResponseTypeDef = TypedDict(
+    "CreateBatchInferenceJobResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "batchInferenceJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateBatchSegmentJobResponseTypeDef = TypedDict(
+    "CreateBatchSegmentJobResponseTypeDef",
+    {
+        "batchSegmentJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "campaignArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetExportJobResponseTypeDef = TypedDict(
+    "CreateDatasetExportJobResponseTypeDef",
+    {
+        "datasetExportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "datasetGroupArn": str,
+        "domain": DomainType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "dataLocation": str,
     },
     total=False,
 )
 
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "datasetImportJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "datasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEventTrackerResponseTypeDef = TypedDict(
+    "CreateEventTrackerResponseTypeDef",
+    {
+        "eventTrackerArn": str,
+        "trackingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "filterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricAttributeTypeDef = TypedDict(
     "MetricAttributeTypeDef",
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
+CreateMetricAttributionResponseTypeDef = TypedDict(
+    "CreateMetricAttributionResponseTypeDef",
+    {
+        "metricAttributionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRecommenderResponseTypeDef = TypedDict(
+    "CreateRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "name": str,
         "schema": str,
     },
 )
@@ -413,19 +497,45 @@
     "_OptionalCreateSchemaRequestRequestTypeDef",
     {
         "domain": DomainType,
     },
     total=False,
 )
 
+
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "schemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSolutionResponseTypeDef = TypedDict(
+    "CreateSolutionResponseTypeDef",
+    {
+        "solutionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSolutionVersionResponseTypeDef = TypedDict(
+    "CreateSolutionVersionResponseTypeDef",
+    {
+        "solutionVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatasetExportJobSummaryTypeDef = TypedDict(
     "DatasetExportJobSummaryTypeDef",
     {
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
@@ -801,14 +911,21 @@
 DescribeSolutionVersionRequestRequestTypeDef = TypedDict(
     "DescribeSolutionVersionRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventTrackerSummaryTypeDef = TypedDict(
     "EventTrackerSummaryTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
@@ -834,14 +951,23 @@
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
+GetSolutionMetricsResponseTypeDef = TypedDict(
+    "GetSolutionMetricsResponseTypeDef",
+    {
+        "solutionVersionArn": str,
+        "metrics": Dict[str, float],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HPOObjectiveTypeDef = TypedDict(
     "HPOObjectiveTypeDef",
     {
         "type": str,
         "metricName": str,
         "metricRegex": str,
     },
@@ -863,123 +989,211 @@
         "name": str,
         "minValue": int,
         "maxValue": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef = TypedDict(
+    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "solutionVersionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBatchInferenceJobsRequestRequestTypeDef = TypedDict(
     "ListBatchInferenceJobsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef = TypedDict(
+    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
+    {
+        "solutionVersionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBatchSegmentJobsRequestRequestTypeDef = TypedDict(
     "ListBatchSegmentJobsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    {
+        "solutionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
+    {
+        "datasetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetExportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetExportJobsRequestRequestTypeDef",
     {
         "datasetArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    {
+        "datasetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "datasetArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListEventTrackersRequestListEventTrackersPaginateTypeDef = TypedDict(
+    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEventTrackersRequestRequestTypeDef = TypedDict(
     "ListEventTrackersRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef = TypedDict(
+    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
+    {
+        "metricAttributionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMetricAttributionMetricsRequestRequestTypeDef = TypedDict(
     "ListMetricAttributionMetricsRequestRequestTypeDef",
     {
         "metricAttributionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef = TypedDict(
+    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMetricAttributionsRequestRequestTypeDef = TypedDict(
     "ListMetricAttributionsRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -995,14 +1209,24 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
     total=False,
 )
 
+ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
+    "ListRecipesRequestListRecipesPaginateTypeDef",
+    {
+        "recipeProvider": Literal["SERVICE"],
+        "domain": DomainType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "recipeProvider": Literal["SERVICE"],
         "nextToken": str,
         "maxResults": int,
         "domain": DomainType,
@@ -1019,33 +1243,59 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
     total=False,
 )
 
+ListRecommendersRequestListRecommendersPaginateTypeDef = TypedDict(
+    "ListRecommendersRequestListRecommendersPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecommendersRequestRequestTypeDef = TypedDict(
     "ListRecommendersRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchemasRequestRequestTypeDef = TypedDict(
     "ListSchemasRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef = TypedDict(
+    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
+    {
+        "solutionArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolutionVersionsRequestRequestTypeDef = TypedDict(
     "ListSolutionVersionsRequestRequestTypeDef",
     {
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1060,14 +1310,23 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
     total=False,
 )
 
+ListSolutionsRequestListSolutionsPaginateTypeDef = TypedDict(
+    "ListSolutionsRequestListSolutionsPaginateTypeDef",
+    {
+        "datasetGroupArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolutionsRequestRequestTypeDef = TypedDict(
     "ListSolutionsRequestRequestTypeDef",
     {
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1099,22 +1358,43 @@
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
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
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
         "excludedDatasetColumns": Mapping[str, Sequence[str]],
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
 TunedHPOParamsTypeDef = TypedDict(
     "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
     total=False,
 )
@@ -1122,21 +1402,37 @@
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
+StartRecommenderResponseTypeDef = TypedDict(
+    "StartRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopRecommenderRequestRequestTypeDef = TypedDict(
     "StopRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
+StopRecommenderResponseTypeDef = TypedDict(
+    "StopRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopSolutionVersionCreationRequestRequestTypeDef = TypedDict(
     "StopSolutionVersionCreationRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
@@ -1144,14 +1440,38 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
+    {
+        "campaignArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateMetricAttributionResponseTypeDef = TypedDict(
+    "UpdateMetricAttributionResponseTypeDef",
+    {
+        "metricAttributionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRecommenderResponseTypeDef = TypedDict(
+    "UpdateRecommenderResponseTypeDef",
+    {
+        "recommenderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 
@@ -1193,19 +1513,39 @@
     "_OptionalMetricAttributionOutputTypeDef",
     {
         "s3DataDestination": S3DataConfigTypeDef,
     },
     total=False,
 )
 
+
 class MetricAttributionOutputTypeDef(
     _RequiredMetricAttributionOutputTypeDef, _OptionalMetricAttributionOutputTypeDef
 ):
     pass
 
+
+ListBatchInferenceJobsResponseTypeDef = TypedDict(
+    "ListBatchInferenceJobsResponseTypeDef",
+    {
+        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBatchSegmentJobsResponseTypeDef = TypedDict(
+    "ListBatchSegmentJobsResponseTypeDef",
+    {
+        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CampaignUpdateSummaryTypeDef = TypedDict(
     "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
         "status": str,
@@ -1228,19 +1568,30 @@
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
+
+ListCampaignsResponseTypeDef = TypedDict(
+    "ListCampaignsResponseTypeDef",
+    {
+        "campaigns": List[CampaignSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
     },
 )
@@ -1250,19 +1601,21 @@
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDatasetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetGroupRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateDatasetGroupRequestRequestTypeDef = TypedDict(
@@ -1272,20 +1625,22 @@
         "kmsKeyArn": str,
         "domain": DomainType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "datasetGroupArn": str,
         "datasetType": str,
@@ -1295,19 +1650,21 @@
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateEventTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventTrackerRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
     },
 )
@@ -1315,20 +1672,22 @@
     "_OptionalCreateEventTrackerRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEventTrackerRequestRequestTypeDef(
     _RequiredCreateEventTrackerRequestRequestTypeDef,
     _OptionalCreateEventTrackerRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "filterExpression": str,
     },
@@ -1337,19 +1696,21 @@
     "_OptionalCreateFilterRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateSolutionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSolutionVersionRequestRequestTypeDef",
     {
         "solutionArn": str,
     },
 )
 _OptionalCreateSolutionVersionRequestRequestTypeDef = TypedDict(
@@ -1358,230 +1719,35 @@
         "name": str,
         "trainingMode": TrainingModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSolutionVersionRequestRequestTypeDef(
     _RequiredCreateSolutionVersionRequestRequestTypeDef,
     _OptionalCreateSolutionVersionRequestRequestTypeDef,
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateBatchInferenceJobResponseTypeDef = TypedDict(
-    "CreateBatchInferenceJobResponseTypeDef",
-    {
-        "batchInferenceJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBatchSegmentJobResponseTypeDef = TypedDict(
-    "CreateBatchSegmentJobResponseTypeDef",
-    {
-        "batchSegmentJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "campaignArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetExportJobResponseTypeDef = TypedDict(
-    "CreateDatasetExportJobResponseTypeDef",
-    {
-        "datasetExportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "datasetGroupArn": str,
-        "domain": DomainType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "datasetImportJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "datasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventTrackerResponseTypeDef = TypedDict(
-    "CreateEventTrackerResponseTypeDef",
-    {
-        "eventTrackerArn": str,
-        "trackingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "filterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMetricAttributionResponseTypeDef = TypedDict(
-    "CreateMetricAttributionResponseTypeDef",
-    {
-        "metricAttributionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRecommenderResponseTypeDef = TypedDict(
-    "CreateRecommenderResponseTypeDef",
-    {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "schemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolutionResponseTypeDef = TypedDict(
-    "CreateSolutionResponseTypeDef",
-    {
-        "solutionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolutionVersionResponseTypeDef = TypedDict(
-    "CreateSolutionVersionResponseTypeDef",
-    {
-        "solutionVersionArn": str,
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
-GetSolutionMetricsResponseTypeDef = TypedDict(
-    "GetSolutionMetricsResponseTypeDef",
-    {
-        "solutionVersionArn": str,
-        "metrics": Dict[str, float],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBatchInferenceJobsResponseTypeDef = TypedDict(
-    "ListBatchInferenceJobsResponseTypeDef",
-    {
-        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBatchSegmentJobsResponseTypeDef = TypedDict(
-    "ListBatchSegmentJobsResponseTypeDef",
-    {
-        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCampaignsResponseTypeDef = TypedDict(
-    "ListCampaignsResponseTypeDef",
-    {
-        "campaigns": List[CampaignSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRecommenderResponseTypeDef = TypedDict(
-    "StartRecommenderResponseTypeDef",
-    {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopRecommenderResponseTypeDef = TypedDict(
-    "StopRecommenderResponseTypeDef",
-    {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
-    {
-        "campaignArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMetricAttributionResponseTypeDef = TypedDict(
-    "UpdateMetricAttributionResponseTypeDef",
-    {
-        "metricAttributionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRecommenderResponseTypeDef = TypedDict(
-    "UpdateRecommenderResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "recommenderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -1596,20 +1762,22 @@
         "tags": Sequence[TagTypeDef],
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
     total=False,
 )
 
+
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DatasetImportJobTypeDef = TypedDict(
     "DatasetImportJobTypeDef",
     {
         "jobName": str,
         "datasetImportJobArn": str,
         "datasetArn": str,
         "dataSource": DataSourceTypeDef,
@@ -1625,84 +1793,84 @@
 )
 
 ListMetricAttributionMetricsResponseTypeDef = TypedDict(
     "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetExportJobsResponseTypeDef = TypedDict(
     "ListDatasetExportJobsResponseTypeDef",
     {
         "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "datasetGroups": List[DatasetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetGroupResponseTypeDef = TypedDict(
     "DescribeDatasetGroupResponseTypeDef",
     {
         "datasetGroup": DatasetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "datasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "schemas": List[DatasetSchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSchemaResponseTypeDef = TypedDict(
     "DescribeSchemaResponseTypeDef",
     {
         "schema": DatasetSchemaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefaultHyperParameterRangesTypeDef = TypedDict(
     "DefaultHyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
@@ -1712,246 +1880,103 @@
     total=False,
 )
 
 DescribeEventTrackerResponseTypeDef = TypedDict(
     "DescribeEventTrackerResponseTypeDef",
     {
         "eventTracker": EventTrackerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFeatureTransformationResponseTypeDef = TypedDict(
     "DescribeFeatureTransformationResponseTypeDef",
     {
         "featureTransformation": FeatureTransformationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFilterResponseTypeDef = TypedDict(
     "DescribeFilterResponseTypeDef",
     {
         "filter": FilterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "recipe": RecipeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventTrackersResponseTypeDef = TypedDict(
     "ListEventTrackersResponseTypeDef",
     {
         "eventTrackers": List[EventTrackerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef = TypedDict(
-    "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
-    {
-        "solutionVersionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef = TypedDict(
-    "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
-    {
-        "solutionVersionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    {
-        "solutionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
-    {
-        "datasetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    {
-        "datasetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventTrackersRequestListEventTrackersPaginateTypeDef = TypedDict(
-    "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef = TypedDict(
-    "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
-    {
-        "metricAttributionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef = TypedDict(
-    "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    {
-        "recipeProvider": Literal["SERVICE"],
-        "domain": DomainType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecommendersRequestListRecommendersPaginateTypeDef = TypedDict(
-    "ListRecommendersRequestListRecommendersPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef = TypedDict(
-    "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
-    {
-        "solutionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolutionsRequestListSolutionsPaginateTypeDef = TypedDict(
-    "ListSolutionsRequestListSolutionsPaginateTypeDef",
-    {
-        "datasetGroupArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMetricAttributionsResponseTypeDef = TypedDict(
     "ListMetricAttributionsResponseTypeDef",
     {
         "metricAttributions": List[MetricAttributionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecipesResponseTypeDef = TypedDict(
     "ListRecipesResponseTypeDef",
     {
         "recipes": List[RecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolutionVersionsResponseTypeDef = TypedDict(
     "ListSolutionVersionsResponseTypeDef",
     {
         "solutionVersions": List[SolutionVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolutionsResponseTypeDef = TypedDict(
     "ListSolutionsResponseTypeDef",
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
@@ -1998,20 +2023,22 @@
         "numResults": int,
         "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBatchInferenceJobRequestRequestTypeDef(
     _RequiredCreateBatchInferenceJobRequestRequestTypeDef,
     _OptionalCreateBatchInferenceJobRequestRequestTypeDef,
 ):
     pass
 
+
 BatchSegmentJobTypeDef = TypedDict(
     "BatchSegmentJobTypeDef",
     {
         "jobName": str,
         "batchSegmentJobArn": str,
         "filterArn": str,
         "failureReason": str,
@@ -2043,20 +2070,22 @@
         "filterArn": str,
         "numResults": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBatchSegmentJobRequestRequestTypeDef(
     _RequiredCreateBatchSegmentJobRequestRequestTypeDef,
     _OptionalCreateBatchSegmentJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDatasetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetExportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "roleArn": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
@@ -2067,20 +2096,22 @@
     {
         "ingestionMode": IngestionModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetExportJobRequestRequestTypeDef(
     _RequiredCreateDatasetExportJobRequestRequestTypeDef,
     _OptionalCreateDatasetExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DatasetExportJobTypeDef = TypedDict(
     "DatasetExportJobTypeDef",
     {
         "jobName": str,
         "datasetExportJobArn": str,
         "datasetArn": str,
         "ingestionMode": IngestionModeType,
@@ -2147,15 +2178,15 @@
     total=False,
 )
 
 DescribeDatasetImportJobResponseTypeDef = TypedDict(
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
@@ -2195,19 +2226,21 @@
     {
         "recommenderConfig": RecommenderConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRecommenderRequestRequestTypeDef(
     _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
 ):
     pass
 
+
 RecommenderSummaryTypeDef = TypedDict(
     "RecommenderSummaryTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
@@ -2239,55 +2272,55 @@
     },
 )
 
 DescribeBatchInferenceJobResponseTypeDef = TypedDict(
     "DescribeBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJob": BatchInferenceJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBatchSegmentJobResponseTypeDef = TypedDict(
     "DescribeBatchSegmentJobResponseTypeDef",
     {
         "batchSegmentJob": BatchSegmentJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetExportJobResponseTypeDef = TypedDict(
     "DescribeDatasetExportJobResponseTypeDef",
     {
         "datasetExportJob": DatasetExportJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricAttributionResponseTypeDef = TypedDict(
     "DescribeMetricAttributionResponseTypeDef",
     {
         "metricAttribution": MetricAttributionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCampaignResponseTypeDef = TypedDict(
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAlgorithmResponseTypeDef = TypedDict(
     "DescribeAlgorithmResponseTypeDef",
     {
         "algorithm": AlgorithmTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": str,
@@ -2302,15 +2335,15 @@
 )
 
 ListRecommendersResponseTypeDef = TypedDict(
     "ListRecommendersResponseTypeDef",
     {
         "recommenders": List[RecommenderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommenderTypeDef = TypedDict(
     "RecommenderTypeDef",
     {
         "recommenderArn": str,
@@ -2344,19 +2377,21 @@
         "eventType": str,
         "solutionConfig": SolutionConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSolutionRequestRequestTypeDef(
     _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
 ):
     pass
 
+
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
@@ -2396,26 +2431,26 @@
     total=False,
 )
 
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSolutionResponseTypeDef = TypedDict(
     "DescribeSolutionResponseTypeDef",
     {
         "solution": SolutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSolutionVersionResponseTypeDef = TypedDict(
     "DescribeSolutionVersionResponseTypeDef",
     {
         "solutionVersion": SolutionVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.26.143
-Summary: Type annotations for boto3.Personalize 1.26.143 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Personalize 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.26.143](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -401,18 +401,31 @@
     BatchInferenceJobSummaryTypeDef,
     BatchSegmentJobSummaryTypeDef,
     CampaignConfigTypeDef,
     CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
     DataSourceTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
     MetricAttributeTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
     DatasetSummaryTypeDef,
@@ -446,89 +459,92 @@
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     RecipeTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTrackerSummaryTypeDef,
     FilterSummaryTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
+    GetSolutionMetricsResponseTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
     IntegerHyperParameterRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
     ListBatchInferenceJobsRequestRequestTypeDef,
+    ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
     ListBatchSegmentJobsRequestRequestTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef,
     ListDatasetExportJobsRequestRequestTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListEventTrackersRequestListEventTrackersPaginateTypeDef,
     ListEventTrackersRequestRequestTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
+    ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
+    ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
     MetricAttributionSummaryTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
     RecipeSummaryTypeDef,
+    ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
+    ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
     SolutionVersionSummaryTypeDef,
+    ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
     SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OptimizationObjectiveTypeDef,
+    PaginatorConfigTypeDef,
     TrainingDataConfigTypeDef,
+    ResponseMetadataTypeDef,
     TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
+    StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
+    StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateCampaignResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
     CampaignUpdateSummaryTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    ListCampaignsResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartRecommenderResponseTypeDef,
-    StopRecommenderResponseTypeDef,
-    UpdateCampaignResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
@@ -540,30 +556,14 @@
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     HyperParameterRangesTypeDef,
-    ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
-    ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
-    ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListEventTrackersRequestListEventTrackersPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
-    ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
-    ListRecommendersRequestListRecommendersPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
-    ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListSolutionsResponseTypeDef,
     RecommenderConfigTypeDef,
     BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy-boto3-personalize-1.27.0/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.143/setup.py` & `mypy-boto3-personalize-1.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.26.143",
+    version="1.27.0",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Personalize 1.26.143 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Personalize 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


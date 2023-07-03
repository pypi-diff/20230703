# Comparing `tmp/mypy-boto3-comprehend-1.26.99.tar.gz` & `tmp/mypy-boto3-comprehend-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehend-1.26.99.tar", last modified: Fri Mar 24 19:32:25 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehend-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-comprehend-1.26.99.tar` & `mypy-boto3-comprehend-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25955 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-03-24 19:32:05.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97427 2023-03-24 19:32:07.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97352 2023-03-24 19:32:05.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.347031 mypy-boto3-comprehend-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27612 2023-07-03 19:50:34.347031 mypy-boto3-comprehend-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26115 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.335031 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-07-03 19:34:40.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-07-03 19:34:40.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-03 19:34:41.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-07-03 19:34:40.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-03 19:34:40.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-03 19:34:40.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98639 2023-07-03 19:34:43.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98562 2023-07-03 19:34:42.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.347031 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27612 2023-07-03 19:50:34.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:34.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:34.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:34.000000 mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.347031 mypy-boto3-comprehend-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:34:39.000000 mypy-boto3-comprehend-1.27.0/setup.py
```

### Comparing `mypy-boto3-comprehend-1.26.99/LICENSE` & `mypy-boto3-comprehend-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.99/PKG-INFO` & `mypy-boto3-comprehend-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.26.99
-Summary: Type annotations for boto3.Comprehend 1.26.99 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Comprehend 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-comprehend"></a>
 
 # mypy-boto3-comprehend
 
 [![PyPI - mypy-boto3-comprehend](https://img.shields.io/pypi/v/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,14 +340,15 @@
 from mypy_boto3_comprehend.literals import (
     AugmentedManifestsDocumentTypeFormatType,
     BlockTypeType,
     DatasetDataFormatType,
     DatasetStatusType,
     DatasetTypeType,
     DocumentClassifierDataFormatType,
+    DocumentClassifierDocumentTypeFormatType,
     DocumentClassifierModeType,
     DocumentReadActionType,
     DocumentReadFeatureTypesType,
     DocumentReadModeType,
     DocumentTypeType,
     EndpointStatusType,
     EntityRecognizerDataFormatType,
@@ -366,14 +367,15 @@
     ListKeyPhrasesDetectionJobsPaginatorName,
     ListPiiEntitiesDetectionJobsPaginatorName,
     ListSentimentDetectionJobsPaginatorName,
     ListTopicsDetectionJobsPaginatorName,
     ModelStatusType,
     ModelTypeType,
     PageBasedErrorCodeType,
+    PageBasedWarningCodeType,
     PartOfSpeechTagTypeType,
     PiiEntitiesDetectionMaskModeType,
     PiiEntitiesDetectionModeType,
     PiiEntityTypeType,
     RelationshipTypeType,
     SentimentTypeType,
     SplitType,
@@ -400,15 +402,14 @@
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
-    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
@@ -417,19 +418,25 @@
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
+    WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
+    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
     DatasetPropertiesTypeDef,
@@ -448,27 +455,29 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
+    DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
@@ -482,68 +491,62 @@
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
+    ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
-    DetectDominantLanguageResponseTypeDef,
-    ImportModelResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
@@ -560,55 +563,54 @@
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
-    CreateDocumentClassifierRequestRequestTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
-    DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
@@ -621,27 +623,27 @@
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
     DatasetInputDataConfigTypeDef,
+    CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -653,14 +655,16 @@
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
```

### Comparing `mypy-boto3-comprehend-1.26.99/README.md` & `mypy-boto3-comprehend-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-comprehend"></a>
 
 # mypy-boto3-comprehend
 
 [![PyPI - mypy-boto3-comprehend](https://img.shields.io/pypi/v/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,14 +308,15 @@
 from mypy_boto3_comprehend.literals import (
     AugmentedManifestsDocumentTypeFormatType,
     BlockTypeType,
     DatasetDataFormatType,
     DatasetStatusType,
     DatasetTypeType,
     DocumentClassifierDataFormatType,
+    DocumentClassifierDocumentTypeFormatType,
     DocumentClassifierModeType,
     DocumentReadActionType,
     DocumentReadFeatureTypesType,
     DocumentReadModeType,
     DocumentTypeType,
     EndpointStatusType,
     EntityRecognizerDataFormatType,
@@ -334,14 +335,15 @@
     ListKeyPhrasesDetectionJobsPaginatorName,
     ListPiiEntitiesDetectionJobsPaginatorName,
     ListSentimentDetectionJobsPaginatorName,
     ListTopicsDetectionJobsPaginatorName,
     ModelStatusType,
     ModelTypeType,
     PageBasedErrorCodeType,
+    PageBasedWarningCodeType,
     PartOfSpeechTagTypeType,
     PiiEntitiesDetectionMaskModeType,
     PiiEntitiesDetectionModeType,
     PiiEntityTypeType,
     RelationshipTypeType,
     SentimentTypeType,
     SplitType,
@@ -368,15 +370,14 @@
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
-    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
@@ -385,19 +386,25 @@
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
+    WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
+    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
     DatasetPropertiesTypeDef,
@@ -416,27 +423,29 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
+    DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
@@ -450,68 +459,62 @@
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
+    ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
-    DetectDominantLanguageResponseTypeDef,
-    ImportModelResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
@@ -528,55 +531,54 @@
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
-    CreateDocumentClassifierRequestRequestTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
-    DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
@@ -589,27 +591,27 @@
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
     DatasetInputDataConfigTypeDef,
+    CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -621,14 +623,16 @@
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.py` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.pyi` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__main__.py` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Comprehend 1.26.99\nVersion:         1.26.99\nBuilder version:"
-        " 7.14.2\nDocs:           "
+        "Type annotations for boto3.Comprehend 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.99")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.py` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.pyi` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.py` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "AugmentedManifestsDocumentTypeFormatType",
     "BlockTypeType",
     "DatasetDataFormatType",
     "DatasetStatusType",
     "DatasetTypeType",
     "DocumentClassifierDataFormatType",
+    "DocumentClassifierDocumentTypeFormatType",
     "DocumentClassifierModeType",
     "DocumentReadActionType",
     "DocumentReadFeatureTypesType",
     "DocumentReadModeType",
     "DocumentTypeType",
     "EndpointStatusType",
     "EntityRecognizerDataFormatType",
@@ -48,14 +49,15 @@
     "ListKeyPhrasesDetectionJobsPaginatorName",
     "ListPiiEntitiesDetectionJobsPaginatorName",
     "ListSentimentDetectionJobsPaginatorName",
     "ListTopicsDetectionJobsPaginatorName",
     "ModelStatusType",
     "ModelTypeType",
     "PageBasedErrorCodeType",
+    "PageBasedWarningCodeType",
     "PartOfSpeechTagTypeType",
     "PiiEntitiesDetectionMaskModeType",
     "PiiEntitiesDetectionModeType",
     "PiiEntityTypeType",
     "RelationshipTypeType",
     "SentimentTypeType",
     "SplitType",
@@ -73,14 +75,17 @@
     "PLAIN_TEXT_DOCUMENT", "SEMI_STRUCTURED_DOCUMENT"
 ]
 BlockTypeType = Literal["LINE", "WORD"]
 DatasetDataFormatType = Literal["AUGMENTED_MANIFEST", "COMPREHEND_CSV"]
 DatasetStatusType = Literal["COMPLETED", "CREATING", "FAILED"]
 DatasetTypeType = Literal["TEST", "TRAIN"]
 DocumentClassifierDataFormatType = Literal["AUGMENTED_MANIFEST", "COMPREHEND_CSV"]
+DocumentClassifierDocumentTypeFormatType = Literal[
+    "PLAIN_TEXT_DOCUMENT", "SEMI_STRUCTURED_DOCUMENT"
+]
 DocumentClassifierModeType = Literal["MULTI_CLASS", "MULTI_LABEL"]
 DocumentReadActionType = Literal["TEXTRACT_ANALYZE_DOCUMENT", "TEXTRACT_DETECT_DOCUMENT_TEXT"]
 DocumentReadFeatureTypesType = Literal["FORMS", "TABLES"]
 DocumentReadModeType = Literal["FORCE_DOCUMENT_READ_ACTION", "SERVICE_DEFAULT"]
 DocumentTypeType = Literal[
     "IMAGE",
     "MS_WORD",
@@ -138,14 +143,18 @@
 PageBasedErrorCodeType = Literal[
     "INTERNAL_SERVER_ERROR",
     "PAGE_CHARACTERS_EXCEEDED",
     "PAGE_SIZE_EXCEEDED",
     "TEXTRACT_BAD_PAGE",
     "TEXTRACT_PROVISIONED_THROUGHPUT_EXCEEDED",
 ]
+PageBasedWarningCodeType = Literal[
+    "INFERENCING_NATIVE_DOCUMENT_WITH_PLAINTEXT_TRAINED_MODEL",
+    "INFERENCING_PLAINTEXT_WITH_NATIVE_TRAINED_MODEL",
+]
 PartOfSpeechTagTypeType = Literal[
     "ADJ",
     "ADP",
     "ADV",
     "AUX",
     "CCONJ",
     "CONJ",
@@ -238,14 +247,15 @@
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
@@ -285,14 +295,15 @@
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
@@ -434,14 +445,15 @@
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
@@ -460,16 +472,19 @@
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
@@ -553,15 +568,17 @@
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

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.pyi` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 __all__ = (
     "AugmentedManifestsDocumentTypeFormatType",
     "BlockTypeType",
     "DatasetDataFormatType",
     "DatasetStatusType",
     "DatasetTypeType",
     "DocumentClassifierDataFormatType",
+    "DocumentClassifierDocumentTypeFormatType",
     "DocumentClassifierModeType",
     "DocumentReadActionType",
     "DocumentReadFeatureTypesType",
     "DocumentReadModeType",
     "DocumentTypeType",
     "EndpointStatusType",
     "EntityRecognizerDataFormatType",
@@ -47,14 +48,15 @@
     "ListKeyPhrasesDetectionJobsPaginatorName",
     "ListPiiEntitiesDetectionJobsPaginatorName",
     "ListSentimentDetectionJobsPaginatorName",
     "ListTopicsDetectionJobsPaginatorName",
     "ModelStatusType",
     "ModelTypeType",
     "PageBasedErrorCodeType",
+    "PageBasedWarningCodeType",
     "PartOfSpeechTagTypeType",
     "PiiEntitiesDetectionMaskModeType",
     "PiiEntitiesDetectionModeType",
     "PiiEntityTypeType",
     "RelationshipTypeType",
     "SentimentTypeType",
     "SplitType",
@@ -71,14 +73,17 @@
     "PLAIN_TEXT_DOCUMENT", "SEMI_STRUCTURED_DOCUMENT"
 ]
 BlockTypeType = Literal["LINE", "WORD"]
 DatasetDataFormatType = Literal["AUGMENTED_MANIFEST", "COMPREHEND_CSV"]
 DatasetStatusType = Literal["COMPLETED", "CREATING", "FAILED"]
 DatasetTypeType = Literal["TEST", "TRAIN"]
 DocumentClassifierDataFormatType = Literal["AUGMENTED_MANIFEST", "COMPREHEND_CSV"]
+DocumentClassifierDocumentTypeFormatType = Literal[
+    "PLAIN_TEXT_DOCUMENT", "SEMI_STRUCTURED_DOCUMENT"
+]
 DocumentClassifierModeType = Literal["MULTI_CLASS", "MULTI_LABEL"]
 DocumentReadActionType = Literal["TEXTRACT_ANALYZE_DOCUMENT", "TEXTRACT_DETECT_DOCUMENT_TEXT"]
 DocumentReadFeatureTypesType = Literal["FORMS", "TABLES"]
 DocumentReadModeType = Literal["FORCE_DOCUMENT_READ_ACTION", "SERVICE_DEFAULT"]
 DocumentTypeType = Literal[
     "IMAGE",
     "MS_WORD",
@@ -136,14 +141,18 @@
 PageBasedErrorCodeType = Literal[
     "INTERNAL_SERVER_ERROR",
     "PAGE_CHARACTERS_EXCEEDED",
     "PAGE_SIZE_EXCEEDED",
     "TEXTRACT_BAD_PAGE",
     "TEXTRACT_PROVISIONED_THROUGHPUT_EXCEEDED",
 ]
+PageBasedWarningCodeType = Literal[
+    "INFERENCING_NATIVE_DOCUMENT_WITH_PLAINTEXT_TRAINED_MODEL",
+    "INFERENCING_PLAINTEXT_WITH_NATIVE_TRAINED_MODEL",
+]
 PartOfSpeechTagTypeType = Literal[
     "ADJ",
     "ADP",
     "ADV",
     "AUX",
     "CCONJ",
     "CONJ",
@@ -236,14 +245,15 @@
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
@@ -283,14 +293,15 @@
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
@@ -432,14 +443,15 @@
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
@@ -458,16 +470,19 @@
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
@@ -551,15 +566,17 @@
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

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.py` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 
@@ -113,15 +113,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 
@@ -131,30 +131,33 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self, *, Filter: EndpointFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        Filter: EndpointFilterTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
         """
 
 
@@ -164,15 +167,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 
@@ -182,15 +185,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEntityRecognizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 
@@ -200,15 +203,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 
@@ -218,15 +221,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 
@@ -236,15 +239,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSentimentDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 
@@ -254,13 +257,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTopicsDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.pyi` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 class ListDocumentClassifiersPaginator(Paginator):
@@ -109,15 +109,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 class ListDominantLanguageDetectionJobsPaginator(Paginator):
@@ -126,29 +126,32 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self, *, Filter: EndpointFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        Filter: EndpointFilterTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
         """
 
 class ListEntitiesDetectionJobsPaginator(Paginator):
@@ -157,15 +160,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 class ListEntityRecognizersPaginator(Paginator):
@@ -174,15 +177,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEntityRecognizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 class ListKeyPhrasesDetectionJobsPaginator(Paginator):
@@ -191,15 +194,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 class ListPiiEntitiesDetectionJobsPaginator(Paginator):
@@ -208,15 +211,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 class ListSentimentDetectionJobsPaginator(Paginator):
@@ -225,15 +228,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSentimentDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 class ListTopicsDetectionJobsPaginator(Paginator):
@@ -242,13 +245,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTopicsDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.py` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .literals import (
     AugmentedManifestsDocumentTypeFormatType,
     BlockTypeType,
     DatasetDataFormatType,
     DatasetStatusType,
     DatasetTypeType,
     DocumentClassifierDataFormatType,
+    DocumentClassifierDocumentTypeFormatType,
     DocumentClassifierModeType,
     DocumentReadActionType,
     DocumentReadFeatureTypesType,
     DocumentReadModeType,
     DocumentTypeType,
     EndpointStatusType,
     EntityRecognizerDataFormatType,
@@ -36,14 +37,15 @@
     FlywheelStatusType,
     InputFormatType,
     JobStatusType,
     LanguageCodeType,
     ModelStatusType,
     ModelTypeType,
     PageBasedErrorCodeType,
+    PageBasedWarningCodeType,
     PartOfSpeechTagTypeType,
     PiiEntitiesDetectionMaskModeType,
     PiiEntitiesDetectionModeType,
     PiiEntityTypeType,
     SentimentTypeType,
     SplitType,
     SyntaxLanguageCodeType,
@@ -61,15 +63,14 @@
 
 
 __all__ = (
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
@@ -78,19 +79,25 @@
     "BoundingBoxTypeDef",
     "ClassifierEvaluationMetricsTypeDef",
     "DocumentReaderConfigTypeDef",
     "DocumentClassTypeDef",
     "DocumentLabelTypeDef",
     "DocumentTypeListItemTypeDef",
     "ErrorsListItemTypeDef",
+    "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
+    "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
+    "CreateDocumentClassifierResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreateEntityRecognizerResponseTypeDef",
+    "CreateFlywheelResponseTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "DatasetFilterTypeDef",
     "DatasetPropertiesTypeDef",
@@ -109,27 +116,29 @@
     "DescribeEntityRecognizerRequestRequestTypeDef",
     "DescribeEventsDetectionJobRequestRequestTypeDef",
     "DescribeFlywheelIterationRequestRequestTypeDef",
     "DescribeFlywheelRequestRequestTypeDef",
     "DescribeKeyPhrasesDetectionJobRequestRequestTypeDef",
     "DescribePiiEntitiesDetectionJobRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTargetedSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTopicsDetectionJobRequestRequestTypeDef",
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
     "DocumentClassificationConfigTypeDef",
     "DocumentClassificationJobFilterTypeDef",
     "OutputDataConfigTypeDef",
+    "DocumentClassifierDocumentsTypeDef",
     "DocumentClassifierFilterTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
     "EntityTypesListItemTypeDef",
@@ -143,68 +152,62 @@
     "EntityRecognizerSummaryTypeDef",
     "EventsDetectionJobFilterTypeDef",
     "FlywheelFilterTypeDef",
     "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
+    "ImportModelResponseTypeDef",
     "KeyPhrasesDetectionJobFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "PiiEntitiesDetectionJobFilterTypeDef",
     "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TargetedSentimentDetectionJobFilterTypeDef",
     "TopicsDetectionJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
     "RedactionConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "StartFlywheelIterationRequestRequestTypeDef",
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
-    "StopEventsDetectionJobRequestRequestTypeDef",
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
-    "StopSentimentDetectionJobRequestRequestTypeDef",
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
-    "DocumentClassifierInputDataConfigTypeDef",
-    "BatchDetectDominantLanguageItemResultTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateDocumentClassifierResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreateEntityRecognizerResponseTypeDef",
-    "CreateFlywheelResponseTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
-    "DetectDominantLanguageResponseTypeDef",
-    "ImportModelResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
+    "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
     "StartKeyPhrasesDetectionJobResponseTypeDef",
     "StartPiiEntitiesDetectionJobResponseTypeDef",
     "StartSentimentDetectionJobResponseTypeDef",
     "StartTargetedSentimentDetectionJobResponseTypeDef",
     "StartTopicsDetectionJobResponseTypeDef",
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobResponseTypeDef",
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobResponseTypeDef",
+    "StopEventsDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobResponseTypeDef",
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobResponseTypeDef",
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobResponseTypeDef",
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobResponseTypeDef",
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StopTargetedSentimentDetectionJobResponseTypeDef",
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
+    "BatchDetectDominantLanguageItemResultTypeDef",
+    "DetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesItemResultTypeDef",
     "DetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentItemResultTypeDef",
     "DetectSentimentResponseTypeDef",
     "MentionSentimentTypeDef",
     "BlockReferenceTypeDef",
     "ClassifierMetadataTypeDef",
@@ -221,55 +224,54 @@
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigTypeDef",
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
+    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     "EntityRecognitionConfigTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
     "ListFlywheelIterationHistoryRequestRequestTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
-    "CreateDocumentClassifierRequestRequestTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
-    "DocumentClassifierPropertiesTypeDef",
     "DocumentClassificationJobPropertiesTypeDef",
     "DominantLanguageDetectionJobPropertiesTypeDef",
     "EntitiesDetectionJobPropertiesTypeDef",
     "EventsDetectionJobPropertiesTypeDef",
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     "PiiEntitiesDetectionJobPropertiesTypeDef",
     "SentimentDetectionJobPropertiesTypeDef",
@@ -282,27 +284,27 @@
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
     "TargetedSentimentDetectionJobPropertiesTypeDef",
     "TopicsDetectionJobPropertiesTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
     "DatasetInputDataConfigTypeDef",
+    "CreateDocumentClassifierRequestRequestTypeDef",
+    "DocumentClassifierPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -314,14 +316,16 @@
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "CreateFlywheelRequestRequestTypeDef",
     "FlywheelPropertiesTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
@@ -380,25 +384,14 @@
         "Index": int,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 BatchDetectEntitiesRequestRequestTypeDef = TypedDict(
     "BatchDetectEntitiesRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -559,14 +552,24 @@
         "Page": int,
         "ErrorCode": PageBasedErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+WarningsListItemTypeDef = TypedDict(
+    "WarningsListItemTypeDef",
+    {
+        "Page": int,
+        "WarnCode": PageBasedWarningCodeType,
+        "WarnMessage": str,
+    },
+    total=False,
+)
+
 ContainsPiiEntitiesRequestRequestTypeDef = TypedDict(
     "ContainsPiiEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -595,14 +598,22 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -613,14 +624,48 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
+CreateDocumentClassifierResponseTypeDef = TypedDict(
+    "CreateDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
+    {
+        "EndpointArn": str,
+        "ModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEntityRecognizerResponseTypeDef = TypedDict(
+    "CreateEntityRecognizerResponseTypeDef",
+    {
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFlywheelResponseTypeDef = TypedDict(
+    "CreateFlywheelResponseTypeDef",
+    {
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
         "S3Uri": str,
     },
 )
@@ -885,14 +930,25 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1015,14 +1071,35 @@
 )
 
 
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 
+_RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
+    "_RequiredDocumentClassifierDocumentsTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalDocumentClassifierDocumentsTypeDef = TypedDict(
+    "_OptionalDocumentClassifierDocumentsTypeDef",
+    {
+        "TestS3Uri": str,
+    },
+    total=False,
+)
+
+
+class DocumentClassifierDocumentsTypeDef(
+    _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
+):
+    pass
+
+
 DocumentClassifierFilterTypeDef = TypedDict(
     "DocumentClassifierFilterTypeDef",
     {
         "Status": ModelStatusType,
         "DocumentClassifierName": str,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
@@ -1254,35 +1331,33 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
+ImportModelResponseTypeDef = TypedDict(
+    "ImportModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
     "KeyPhrasesDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
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
 ListDocumentClassifierSummariesRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1344,14 +1419,24 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
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
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1406,398 +1491,336 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-    },
-)
-_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class StartFlywheelIterationRequestRequestTypeDef(
-    _RequiredStartFlywheelIterationRequestRequestTypeDef,
-    _OptionalStartFlywheelIterationRequestRequestTypeDef,
-):
-    pass
-
-
-StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
-    {
-        "JobId": str,
-    },
-)
-
-StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
-    {
-        "JobId": str,
-    },
-)
-
-StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEventsDetectionJobRequestRequestTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "JobId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+StartDocumentClassificationJobResponseTypeDef = TypedDict(
+    "StartDocumentClassificationJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopSentimentDetectionJobRequestRequestTypeDef",
+StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StartDominantLanguageDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+StartEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
-    },
-)
-
-StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    {
-        "DocumentClassifierArn": str,
-    },
-)
-
-StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    {
+        "JobArn": str,
+        "JobStatus": JobStatusType,
         "EntityRecognizerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartEventsDetectionJobResponseTypeDef = TypedDict(
+    "StartEventsDetectionJobResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
-        "EndpointArn": str,
+        "FlywheelArn": str,
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
     {
-        "DesiredModelArn": str,
-        "DesiredInferenceUnits": int,
-        "DesiredDataAccessRoleArn": str,
-        "FlywheelArn": str,
+        "ClientRequestToken": str,
     },
     total=False,
 )
 
 
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+class StartFlywheelIterationRequestRequestTypeDef(
+    _RequiredStartFlywheelIterationRequestRequestTypeDef,
+    _OptionalStartFlywheelIterationRequestRequestTypeDef,
 ):
     pass
 
 
-DocumentClassifierInputDataConfigTypeDef = TypedDict(
-    "DocumentClassifierInputDataConfigTypeDef",
-    {
-        "DataFormat": DocumentClassifierDataFormatType,
-        "S3Uri": str,
-        "TestS3Uri": str,
-        "LabelDelimiter": str,
-        "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
-    },
-    total=False,
-)
-
-BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
-    "BatchDetectDominantLanguageItemResultTypeDef",
+StartFlywheelIterationResponseTypeDef = TypedDict(
+    "StartFlywheelIterationResponseTypeDef",
     {
-        "Index": int,
-        "Languages": List[DominantLanguageTypeDef],
+        "FlywheelArn": str,
+        "FlywheelIterationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
+StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StartKeyPhrasesDetectionJobResponseTypeDef",
     {
-        "DatasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDocumentClassifierResponseTypeDef = TypedDict(
-    "CreateDocumentClassifierResponseTypeDef",
+StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartPiiEntitiesDetectionJobResponseTypeDef",
     {
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
+StartSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartSentimentDetectionJobResponseTypeDef",
     {
-        "EndpointArn": str,
-        "ModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEntityRecognizerResponseTypeDef = TypedDict(
-    "CreateEntityRecognizerResponseTypeDef",
+StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartTargetedSentimentDetectionJobResponseTypeDef",
     {
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFlywheelResponseTypeDef = TypedDict(
-    "CreateFlywheelResponseTypeDef",
+StartTopicsDetectionJobResponseTypeDef = TypedDict(
+    "StartTopicsDetectionJobResponseTypeDef",
     {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
+StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
-        "ResourcePolicy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "PolicyRevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
     },
 )
 
-DetectDominantLanguageResponseTypeDef = TypedDict(
-    "DetectDominantLanguageResponseTypeDef",
+StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobResponseTypeDef",
     {
-        "Languages": List[DominantLanguageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ImportModelResponseTypeDef = TypedDict(
-    "ImportModelResponseTypeDef",
+StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "ModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
     },
 )
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+StopEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionJobResponseTypeDef",
     {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDocumentClassificationJobResponseTypeDef = TypedDict(
-    "StartDocumentClassificationJobResponseTypeDef",
+StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEventsDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StartDominantLanguageDetectionJobResponseTypeDef",
+StopEventsDetectionJobResponseTypeDef = TypedDict(
+    "StopEventsDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartEventsDetectionJobResponseTypeDef = TypedDict(
-    "StartEventsDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartFlywheelIterationResponseTypeDef = TypedDict(
-    "StartFlywheelIterationResponseTypeDef",
+StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "FlywheelArn": str,
-        "FlywheelIterationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
     },
 )
 
-StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StartKeyPhrasesDetectionJobResponseTypeDef",
+StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartPiiEntitiesDetectionJobResponseTypeDef",
+StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartSentimentDetectionJobResponseTypeDef",
+StopSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartTargetedSentimentDetectionJobResponseTypeDef",
+StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTopicsDetectionJobResponseTypeDef = TypedDict(
-    "StartTopicsDetectionJobResponseTypeDef",
+StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobResponseTypeDef",
+StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DocumentClassifierArn": str,
     },
 )
 
-StopEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionJobResponseTypeDef",
+StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EntityRecognizerArn": str,
     },
 )
 
-StopEventsDetectionJobResponseTypeDef = TypedDict(
-    "StopEventsDetectionJobResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobResponseTypeDef",
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EndpointArn": str,
     },
 )
-
-StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobResponseTypeDef",
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DesiredModelArn": str,
+        "DesiredInferenceUnits": int,
+        "DesiredDataAccessRoleArn": str,
+        "FlywheelArn": str,
     },
+    total=False,
 )
 
-StopSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopSentimentDetectionJobResponseTypeDef",
+
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+):
+    pass
+
+
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DesiredModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobResponseTypeDef",
+BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
+    "BatchDetectDominantLanguageItemResultTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Index": int,
+        "Languages": List[DominantLanguageTypeDef],
     },
+    total=False,
 )
 
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+DetectDominantLanguageResponseTypeDef = TypedDict(
+    "DetectDominantLanguageResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Languages": List[DominantLanguageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectKeyPhrasesItemResultTypeDef = TypedDict(
     "BatchDetectKeyPhrasesItemResultTypeDef",
     {
         "Index": int,
@@ -1806,15 +1829,15 @@
     total=False,
 )
 
 DetectKeyPhrasesResponseTypeDef = TypedDict(
     "DetectKeyPhrasesResponseTypeDef",
     {
         "KeyPhrases": List[KeyPhraseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectSentimentItemResultTypeDef = TypedDict(
     "BatchDetectSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -1825,15 +1848,15 @@
 )
 
 DetectSentimentResponseTypeDef = TypedDict(
     "DetectSentimentResponseTypeDef",
     {
         "Sentiment": SentimentTypeType,
         "SentimentScore": SentimentScoreTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MentionSentimentTypeDef = TypedDict(
     "MentionSentimentTypeDef",
     {
         "Sentiment": SentimentTypeType,
@@ -1919,15 +1942,15 @@
     pass
 
 
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
@@ -1979,15 +2002,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -2050,62 +2073,95 @@
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetProperties": DatasetPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "DatasetPropertiesList": List[DatasetPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "EndpointProperties": EndpointPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "EndpointPropertiesList": List[EndpointPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectPiiEntitiesResponseTypeDef = TypedDict(
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     {
         "Filter": DocumentClassificationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DocumentClassifierInputDataConfigTypeDef = TypedDict(
+    "DocumentClassifierInputDataConfigTypeDef",
+    {
+        "DataFormat": DocumentClassifierDataFormatType,
+        "S3Uri": str,
+        "TestS3Uri": str,
+        "LabelDelimiter": str,
+        "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
+        "DocumentType": DocumentClassifierDocumentTypeFormatType,
+        "Documents": DocumentClassifierDocumentsTypeDef,
+        "DocumentReaderConfig": DocumentReaderConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifiersRequestRequestTypeDef",
     {
         "Filter": DocumentClassifierFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2113,47 +2169,76 @@
 )
 
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
 ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     {
         "Filter": DominantLanguageDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "Filter": EndpointFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EntitiesDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2188,14 +2273,23 @@
 
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
 
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEntityRecognizersRequestRequestTypeDef = TypedDict(
     "ListEntityRecognizersRequestRequestTypeDef",
     {
         "Filter": EntityRecognizerFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2213,15 +2307,15 @@
 )
 
 ListEntityRecognizerSummariesResponseTypeDef = TypedDict(
     "ListEntityRecognizerSummariesResponseTypeDef",
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEventsDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EventsDetectionJobFilterTypeDef,
@@ -2284,107 +2378,51 @@
 )
 
 ListFlywheelsResponseTypeDef = TypedDict(
     "ListFlywheelsResponseTypeDef",
     {
         "FlywheelSummaryList": List[FlywheelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     {
         "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     {
@@ -2395,15 +2433,15 @@
     total=False,
 )
 
 ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     {
         "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     {
@@ -2424,15 +2462,15 @@
     total=False,
 )
 
 ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     {
         "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     {
@@ -2451,71 +2489,38 @@
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
-    {
-        "DocumentClassifierName": str,
-        "DataAccessRoleArn": str,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-    },
-)
-_OptionalCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDocumentClassifierRequestRequestTypeDef",
-    {
-        "VersionName": str,
-        "Tags": Sequence[TagTypeDef],
-        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
-        "ClientRequestToken": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "Mode": DocumentClassifierModeType,
-        "ModelKmsKeyId": str,
-        "ModelPolicy": str,
-    },
-    total=False,
-)
-
-
-class CreateDocumentClassifierRequestRequestTypeDef(
-    _RequiredCreateDocumentClassifierRequestRequestTypeDef,
-    _OptionalCreateDocumentClassifierRequestRequestTypeDef,
-):
-    pass
-
-
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectKeyPhrasesResponseTypeDef = TypedDict(
     "BatchDetectKeyPhrasesResponseTypeDef",
     {
         "ResultList": List[BatchDetectKeyPhrasesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectSentimentResponseTypeDef = TypedDict(
     "BatchDetectSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetedSentimentMentionTypeDef = TypedDict(
     "TargetedSentimentMentionTypeDef",
     {
         "Score": float,
@@ -2538,40 +2543,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
-DocumentClassifierPropertiesTypeDef = TypedDict(
-    "DocumentClassifierPropertiesTypeDef",
-    {
-        "DocumentClassifierArn": str,
-        "LanguageCode": LanguageCodeType,
-        "Status": ModelStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "TrainingStartTime": datetime,
-        "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
-        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
-        "ClassifierMetadata": ClassifierMetadataTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "Mode": DocumentClassifierModeType,
-        "ModelKmsKeyId": str,
-        "VersionName": str,
-        "SourceModelArn": str,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
 DocumentClassificationJobPropertiesTypeDef = TypedDict(
     "DocumentClassificationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
@@ -3041,23 +3020,83 @@
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
+    {
+        "DocumentClassifierName": str,
+        "DataAccessRoleArn": str,
+        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+    },
+)
+_OptionalCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDocumentClassifierRequestRequestTypeDef",
+    {
+        "VersionName": str,
+        "Tags": Sequence[TagTypeDef],
+        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
+        "ClientRequestToken": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "Mode": DocumentClassifierModeType,
+        "ModelKmsKeyId": str,
+        "ModelPolicy": str,
+    },
+    total=False,
+)
+
+
+class CreateDocumentClassifierRequestRequestTypeDef(
+    _RequiredCreateDocumentClassifierRequestRequestTypeDef,
+    _OptionalCreateDocumentClassifierRequestRequestTypeDef,
+):
+    pass
+
+
+DocumentClassifierPropertiesTypeDef = TypedDict(
+    "DocumentClassifierPropertiesTypeDef",
+    {
+        "DocumentClassifierArn": str,
+        "LanguageCode": LanguageCodeType,
+        "Status": ModelStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "TrainingStartTime": datetime,
+        "TrainingEndTime": datetime,
+        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
+        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
+        "ClassifierMetadata": ClassifierMetadataTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "Mode": DocumentClassifierModeType,
+        "ModelKmsKeyId": str,
+        "VersionName": str,
+        "SourceModelArn": str,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Warnings": List[WarningsListItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
@@ -3119,24 +3158,24 @@
     total=False,
 )
 
 DescribeFlywheelIterationResponseTypeDef = TypedDict(
     "DescribeFlywheelIterationResponseTypeDef",
     {
         "FlywheelIterationProperties": FlywheelIterationPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFlywheelIterationHistoryResponseTypeDef = TypedDict(
     "ListFlywheelIterationHistoryResponseTypeDef",
     {
         "FlywheelIterationPropertiesList": List[FlywheelIterationPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "Id": str,
@@ -3158,15 +3197,15 @@
     total=False,
 )
 
 DetectSyntaxResponseTypeDef = TypedDict(
     "DetectSyntaxResponseTypeDef",
     {
         "SyntaxTokens": List[SyntaxTokenTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetedSentimentEntityTypeDef = TypedDict(
     "TargetedSentimentEntityTypeDef",
     {
         "DescriptiveMentionIndex": List[int],
@@ -3180,185 +3219,168 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDocumentClassificationJobsResponseTypeDef = TypedDict(
     "ListDocumentClassificationJobsResponseTypeDef",
     {
         "DocumentClassificationJobPropertiesList": List[DocumentClassificationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDominantLanguageDetectionJobResponseTypeDef = TypedDict(
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     {
         "DominantLanguageDetectionJobProperties": DominantLanguageDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDominantLanguageDetectionJobsResponseTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     {
         "DominantLanguageDetectionJobPropertiesList": List[
             DominantLanguageDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionJobResponseTypeDef",
     {
         "EntitiesDetectionJobProperties": EntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionJobsResponseTypeDef",
     {
         "EntitiesDetectionJobPropertiesList": List[EntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsDetectionJobResponseTypeDef = TypedDict(
     "DescribeEventsDetectionJobResponseTypeDef",
     {
         "EventsDetectionJobProperties": EventsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventsDetectionJobsResponseTypeDef = TypedDict(
     "ListEventsDetectionJobsResponseTypeDef",
     {
         "EventsDetectionJobPropertiesList": List[EventsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
     "DescribeKeyPhrasesDetectionJobResponseTypeDef",
     {
         "KeyPhrasesDetectionJobProperties": KeyPhrasesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKeyPhrasesDetectionJobsResponseTypeDef = TypedDict(
     "ListKeyPhrasesDetectionJobsResponseTypeDef",
     {
         "KeyPhrasesDetectionJobPropertiesList": List[KeyPhrasesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePiiEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribePiiEntitiesDetectionJobResponseTypeDef",
     {
         "PiiEntitiesDetectionJobProperties": PiiEntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPiiEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     {
         "PiiEntitiesDetectionJobPropertiesList": List[PiiEntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeSentimentDetectionJobResponseTypeDef",
     {
         "SentimentDetectionJobProperties": SentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListSentimentDetectionJobsResponseTypeDef",
     {
         "SentimentDetectionJobPropertiesList": List[SentimentDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     {
         "TargetedSentimentDetectionJobProperties": TargetedSentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetedSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     {
         "TargetedSentimentDetectionJobPropertiesList": List[
             TargetedSentimentDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTopicsDetectionJobResponseTypeDef = TypedDict(
     "DescribeTopicsDetectionJobResponseTypeDef",
     {
         "TopicsDetectionJobProperties": TopicsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTopicsDetectionJobsResponseTypeDef = TypedDict(
     "ListTopicsDetectionJobsResponseTypeDef",
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "FlywheelArn": str,
@@ -3380,14 +3402,31 @@
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
 
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3460,24 +3499,24 @@
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Blocks": List[BlockTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectSyntaxResponseTypeDef = TypedDict(
     "BatchDetectSyntaxResponseTypeDef",
     {
         "ResultList": List[BatchDetectSyntaxItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectTargetedSentimentItemResultTypeDef = TypedDict(
     "BatchDetectTargetedSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -3486,61 +3525,61 @@
     total=False,
 )
 
 DetectTargetedSentimentResponseTypeDef = TypedDict(
     "DetectTargetedSentimentResponseTypeDef",
     {
         "Entities": List[TargetedSentimentEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectEntitiesResponseTypeDef = TypedDict(
     "BatchDetectEntitiesResponseTypeDef",
     {
         "ResultList": List[BatchDetectEntitiesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFlywheelResponseTypeDef = TypedDict(
     "DescribeFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlywheelResponseTypeDef = TypedDict(
     "UpdateFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntityRecognizerResponseTypeDef = TypedDict(
     "DescribeEntityRecognizerResponseTypeDef",
     {
         "EntityRecognizerProperties": EntityRecognizerPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntityRecognizersResponseTypeDef = TypedDict(
     "ListEntityRecognizersResponseTypeDef",
     {
         "EntityRecognizerPropertiesList": List[EntityRecognizerPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectTargetedSentimentResponseTypeDef = TypedDict(
     "BatchDetectTargetedSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectTargetedSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.pyi` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .literals import (
     AugmentedManifestsDocumentTypeFormatType,
     BlockTypeType,
     DatasetDataFormatType,
     DatasetStatusType,
     DatasetTypeType,
     DocumentClassifierDataFormatType,
+    DocumentClassifierDocumentTypeFormatType,
     DocumentClassifierModeType,
     DocumentReadActionType,
     DocumentReadFeatureTypesType,
     DocumentReadModeType,
     DocumentTypeType,
     EndpointStatusType,
     EntityRecognizerDataFormatType,
@@ -36,14 +37,15 @@
     FlywheelStatusType,
     InputFormatType,
     JobStatusType,
     LanguageCodeType,
     ModelStatusType,
     ModelTypeType,
     PageBasedErrorCodeType,
+    PageBasedWarningCodeType,
     PartOfSpeechTagTypeType,
     PiiEntitiesDetectionMaskModeType,
     PiiEntitiesDetectionModeType,
     PiiEntityTypeType,
     SentimentTypeType,
     SplitType,
     SyntaxLanguageCodeType,
@@ -60,15 +62,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
@@ -77,19 +78,25 @@
     "BoundingBoxTypeDef",
     "ClassifierEvaluationMetricsTypeDef",
     "DocumentReaderConfigTypeDef",
     "DocumentClassTypeDef",
     "DocumentLabelTypeDef",
     "DocumentTypeListItemTypeDef",
     "ErrorsListItemTypeDef",
+    "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
+    "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
+    "CreateDocumentClassifierResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreateEntityRecognizerResponseTypeDef",
+    "CreateFlywheelResponseTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "DatasetFilterTypeDef",
     "DatasetPropertiesTypeDef",
@@ -108,27 +115,29 @@
     "DescribeEntityRecognizerRequestRequestTypeDef",
     "DescribeEventsDetectionJobRequestRequestTypeDef",
     "DescribeFlywheelIterationRequestRequestTypeDef",
     "DescribeFlywheelRequestRequestTypeDef",
     "DescribeKeyPhrasesDetectionJobRequestRequestTypeDef",
     "DescribePiiEntitiesDetectionJobRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTargetedSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTopicsDetectionJobRequestRequestTypeDef",
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
     "DocumentClassificationConfigTypeDef",
     "DocumentClassificationJobFilterTypeDef",
     "OutputDataConfigTypeDef",
+    "DocumentClassifierDocumentsTypeDef",
     "DocumentClassifierFilterTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
     "EntityTypesListItemTypeDef",
@@ -142,68 +151,62 @@
     "EntityRecognizerSummaryTypeDef",
     "EventsDetectionJobFilterTypeDef",
     "FlywheelFilterTypeDef",
     "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
+    "ImportModelResponseTypeDef",
     "KeyPhrasesDetectionJobFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "PiiEntitiesDetectionJobFilterTypeDef",
     "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TargetedSentimentDetectionJobFilterTypeDef",
     "TopicsDetectionJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
     "RedactionConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "StartFlywheelIterationRequestRequestTypeDef",
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
-    "StopEventsDetectionJobRequestRequestTypeDef",
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
-    "StopSentimentDetectionJobRequestRequestTypeDef",
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
-    "DocumentClassifierInputDataConfigTypeDef",
-    "BatchDetectDominantLanguageItemResultTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateDocumentClassifierResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreateEntityRecognizerResponseTypeDef",
-    "CreateFlywheelResponseTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
-    "DetectDominantLanguageResponseTypeDef",
-    "ImportModelResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
+    "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
     "StartKeyPhrasesDetectionJobResponseTypeDef",
     "StartPiiEntitiesDetectionJobResponseTypeDef",
     "StartSentimentDetectionJobResponseTypeDef",
     "StartTargetedSentimentDetectionJobResponseTypeDef",
     "StartTopicsDetectionJobResponseTypeDef",
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobResponseTypeDef",
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobResponseTypeDef",
+    "StopEventsDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobResponseTypeDef",
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobResponseTypeDef",
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobResponseTypeDef",
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobResponseTypeDef",
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StopTargetedSentimentDetectionJobResponseTypeDef",
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
+    "BatchDetectDominantLanguageItemResultTypeDef",
+    "DetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesItemResultTypeDef",
     "DetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentItemResultTypeDef",
     "DetectSentimentResponseTypeDef",
     "MentionSentimentTypeDef",
     "BlockReferenceTypeDef",
     "ClassifierMetadataTypeDef",
@@ -220,55 +223,54 @@
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigTypeDef",
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
+    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     "EntityRecognitionConfigTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
     "ListFlywheelIterationHistoryRequestRequestTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
-    "CreateDocumentClassifierRequestRequestTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
-    "DocumentClassifierPropertiesTypeDef",
     "DocumentClassificationJobPropertiesTypeDef",
     "DominantLanguageDetectionJobPropertiesTypeDef",
     "EntitiesDetectionJobPropertiesTypeDef",
     "EventsDetectionJobPropertiesTypeDef",
     "KeyPhrasesDetectionJobPropertiesTypeDef",
     "PiiEntitiesDetectionJobPropertiesTypeDef",
     "SentimentDetectionJobPropertiesTypeDef",
@@ -281,27 +283,27 @@
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
     "TargetedSentimentDetectionJobPropertiesTypeDef",
     "TopicsDetectionJobPropertiesTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
     "DatasetInputDataConfigTypeDef",
+    "CreateDocumentClassifierRequestRequestTypeDef",
+    "DocumentClassifierPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -313,14 +315,16 @@
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "CreateFlywheelRequestRequestTypeDef",
     "FlywheelPropertiesTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
@@ -377,25 +381,14 @@
         "Index": int,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 BatchDetectEntitiesRequestRequestTypeDef = TypedDict(
     "BatchDetectEntitiesRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -554,14 +547,24 @@
         "Page": int,
         "ErrorCode": PageBasedErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+WarningsListItemTypeDef = TypedDict(
+    "WarningsListItemTypeDef",
+    {
+        "Page": int,
+        "WarnCode": PageBasedWarningCodeType,
+        "WarnMessage": str,
+    },
+    total=False,
+)
+
 ContainsPiiEntitiesRequestRequestTypeDef = TypedDict(
     "ContainsPiiEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -588,14 +591,22 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -606,14 +617,48 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
+CreateDocumentClassifierResponseTypeDef = TypedDict(
+    "CreateDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
+    {
+        "EndpointArn": str,
+        "ModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEntityRecognizerResponseTypeDef = TypedDict(
+    "CreateEntityRecognizerResponseTypeDef",
+    {
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFlywheelResponseTypeDef = TypedDict(
+    "CreateFlywheelResponseTypeDef",
+    {
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
         "S3Uri": str,
     },
 )
@@ -870,14 +915,25 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -996,14 +1052,33 @@
     },
     total=False,
 )
 
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
+_RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
+    "_RequiredDocumentClassifierDocumentsTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalDocumentClassifierDocumentsTypeDef = TypedDict(
+    "_OptionalDocumentClassifierDocumentsTypeDef",
+    {
+        "TestS3Uri": str,
+    },
+    total=False,
+)
+
+class DocumentClassifierDocumentsTypeDef(
+    _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
+):
+    pass
+
 DocumentClassifierFilterTypeDef = TypedDict(
     "DocumentClassifierFilterTypeDef",
     {
         "Status": ModelStatusType,
         "DocumentClassifierName": str,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
@@ -1231,35 +1306,33 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
+ImportModelResponseTypeDef = TypedDict(
+    "ImportModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
     "KeyPhrasesDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
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
 ListDocumentClassifierSummariesRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1321,14 +1394,24 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
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
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1379,394 +1462,332 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-    },
-)
-_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-class StartFlywheelIterationRequestRequestTypeDef(
-    _RequiredStartFlywheelIterationRequestRequestTypeDef,
-    _OptionalStartFlywheelIterationRequestRequestTypeDef,
-):
-    pass
-
-StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
-    {
-        "JobId": str,
-    },
-)
-
-StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
-    {
-        "JobId": str,
-    },
-)
-
-StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEventsDetectionJobRequestRequestTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "JobId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+StartDocumentClassificationJobResponseTypeDef = TypedDict(
+    "StartDocumentClassificationJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopSentimentDetectionJobRequestRequestTypeDef",
+StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StartDominantLanguageDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+StartEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
-    },
-)
-
-StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    {
-        "DocumentClassifierArn": str,
-    },
-)
-
-StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    {
+        "JobArn": str,
+        "JobStatus": JobStatusType,
         "EntityRecognizerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartEventsDetectionJobResponseTypeDef = TypedDict(
+    "StartEventsDetectionJobResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
-        "EndpointArn": str,
+        "FlywheelArn": str,
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
     {
-        "DesiredModelArn": str,
-        "DesiredInferenceUnits": int,
-        "DesiredDataAccessRoleArn": str,
-        "FlywheelArn": str,
+        "ClientRequestToken": str,
     },
     total=False,
 )
 
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+class StartFlywheelIterationRequestRequestTypeDef(
+    _RequiredStartFlywheelIterationRequestRequestTypeDef,
+    _OptionalStartFlywheelIterationRequestRequestTypeDef,
 ):
     pass
 
-DocumentClassifierInputDataConfigTypeDef = TypedDict(
-    "DocumentClassifierInputDataConfigTypeDef",
-    {
-        "DataFormat": DocumentClassifierDataFormatType,
-        "S3Uri": str,
-        "TestS3Uri": str,
-        "LabelDelimiter": str,
-        "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
-    },
-    total=False,
-)
-
-BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
-    "BatchDetectDominantLanguageItemResultTypeDef",
+StartFlywheelIterationResponseTypeDef = TypedDict(
+    "StartFlywheelIterationResponseTypeDef",
     {
-        "Index": int,
-        "Languages": List[DominantLanguageTypeDef],
+        "FlywheelArn": str,
+        "FlywheelIterationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
+StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StartKeyPhrasesDetectionJobResponseTypeDef",
     {
-        "DatasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDocumentClassifierResponseTypeDef = TypedDict(
-    "CreateDocumentClassifierResponseTypeDef",
+StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartPiiEntitiesDetectionJobResponseTypeDef",
     {
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
+StartSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartSentimentDetectionJobResponseTypeDef",
     {
-        "EndpointArn": str,
-        "ModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEntityRecognizerResponseTypeDef = TypedDict(
-    "CreateEntityRecognizerResponseTypeDef",
+StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartTargetedSentimentDetectionJobResponseTypeDef",
     {
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFlywheelResponseTypeDef = TypedDict(
-    "CreateFlywheelResponseTypeDef",
+StartTopicsDetectionJobResponseTypeDef = TypedDict(
+    "StartTopicsDetectionJobResponseTypeDef",
     {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
+StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
-        "ResourcePolicy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "PolicyRevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
     },
 )
 
-DetectDominantLanguageResponseTypeDef = TypedDict(
-    "DetectDominantLanguageResponseTypeDef",
+StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobResponseTypeDef",
     {
-        "Languages": List[DominantLanguageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ImportModelResponseTypeDef = TypedDict(
-    "ImportModelResponseTypeDef",
+StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "ModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
     },
 )
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+StopEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionJobResponseTypeDef",
     {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDocumentClassificationJobResponseTypeDef = TypedDict(
-    "StartDocumentClassificationJobResponseTypeDef",
+StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEventsDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StartDominantLanguageDetectionJobResponseTypeDef",
+StopEventsDetectionJobResponseTypeDef = TypedDict(
+    "StopEventsDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartEventsDetectionJobResponseTypeDef = TypedDict(
-    "StartEventsDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartFlywheelIterationResponseTypeDef = TypedDict(
-    "StartFlywheelIterationResponseTypeDef",
+StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "FlywheelArn": str,
-        "FlywheelIterationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
     },
 )
 
-StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StartKeyPhrasesDetectionJobResponseTypeDef",
+StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartPiiEntitiesDetectionJobResponseTypeDef",
+StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartSentimentDetectionJobResponseTypeDef",
+StopSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartTargetedSentimentDetectionJobResponseTypeDef",
+StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTopicsDetectionJobResponseTypeDef = TypedDict(
-    "StartTopicsDetectionJobResponseTypeDef",
+StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobResponseTypeDef",
+StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DocumentClassifierArn": str,
     },
 )
 
-StopEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionJobResponseTypeDef",
+StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EntityRecognizerArn": str,
     },
 )
 
-StopEventsDetectionJobResponseTypeDef = TypedDict(
-    "StopEventsDetectionJobResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobResponseTypeDef",
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EndpointArn": str,
     },
 )
-
-StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobResponseTypeDef",
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DesiredModelArn": str,
+        "DesiredInferenceUnits": int,
+        "DesiredDataAccessRoleArn": str,
+        "FlywheelArn": str,
     },
+    total=False,
 )
 
-StopSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopSentimentDetectionJobResponseTypeDef",
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+):
+    pass
+
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DesiredModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobResponseTypeDef",
+BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
+    "BatchDetectDominantLanguageItemResultTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Index": int,
+        "Languages": List[DominantLanguageTypeDef],
     },
+    total=False,
 )
 
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+DetectDominantLanguageResponseTypeDef = TypedDict(
+    "DetectDominantLanguageResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Languages": List[DominantLanguageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectKeyPhrasesItemResultTypeDef = TypedDict(
     "BatchDetectKeyPhrasesItemResultTypeDef",
     {
         "Index": int,
@@ -1775,15 +1796,15 @@
     total=False,
 )
 
 DetectKeyPhrasesResponseTypeDef = TypedDict(
     "DetectKeyPhrasesResponseTypeDef",
     {
         "KeyPhrases": List[KeyPhraseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectSentimentItemResultTypeDef = TypedDict(
     "BatchDetectSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -1794,15 +1815,15 @@
 )
 
 DetectSentimentResponseTypeDef = TypedDict(
     "DetectSentimentResponseTypeDef",
     {
         "Sentiment": SentimentTypeType,
         "SentimentScore": SentimentScoreTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MentionSentimentTypeDef = TypedDict(
     "MentionSentimentTypeDef",
     {
         "Sentiment": SentimentTypeType,
@@ -1884,15 +1905,15 @@
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
@@ -1940,15 +1961,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -2009,62 +2030,95 @@
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetProperties": DatasetPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "DatasetPropertiesList": List[DatasetPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "EndpointProperties": EndpointPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "EndpointPropertiesList": List[EndpointPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectPiiEntitiesResponseTypeDef = TypedDict(
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     {
         "Filter": DocumentClassificationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DocumentClassifierInputDataConfigTypeDef = TypedDict(
+    "DocumentClassifierInputDataConfigTypeDef",
+    {
+        "DataFormat": DocumentClassifierDataFormatType,
+        "S3Uri": str,
+        "TestS3Uri": str,
+        "LabelDelimiter": str,
+        "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
+        "DocumentType": DocumentClassifierDocumentTypeFormatType,
+        "Documents": DocumentClassifierDocumentsTypeDef,
+        "DocumentReaderConfig": DocumentReaderConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifiersRequestRequestTypeDef",
     {
         "Filter": DocumentClassifierFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2072,47 +2126,76 @@
 )
 
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
 ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     {
         "Filter": DominantLanguageDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "Filter": EndpointFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EntitiesDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2145,14 +2228,23 @@
 )
 
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEntityRecognizersRequestRequestTypeDef = TypedDict(
     "ListEntityRecognizersRequestRequestTypeDef",
     {
         "Filter": EntityRecognizerFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2170,15 +2262,15 @@
 )
 
 ListEntityRecognizerSummariesResponseTypeDef = TypedDict(
     "ListEntityRecognizerSummariesResponseTypeDef",
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEventsDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EventsDetectionJobFilterTypeDef,
@@ -2239,107 +2331,51 @@
 )
 
 ListFlywheelsResponseTypeDef = TypedDict(
     "ListFlywheelsResponseTypeDef",
     {
         "FlywheelSummaryList": List[FlywheelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     {
         "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     {
@@ -2350,15 +2386,15 @@
     total=False,
 )
 
 ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     {
         "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     {
@@ -2379,15 +2415,15 @@
     total=False,
 )
 
 ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     {
         "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     {
@@ -2406,69 +2442,38 @@
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
-    {
-        "DocumentClassifierName": str,
-        "DataAccessRoleArn": str,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-    },
-)
-_OptionalCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDocumentClassifierRequestRequestTypeDef",
-    {
-        "VersionName": str,
-        "Tags": Sequence[TagTypeDef],
-        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
-        "ClientRequestToken": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "Mode": DocumentClassifierModeType,
-        "ModelKmsKeyId": str,
-        "ModelPolicy": str,
-    },
-    total=False,
-)
-
-class CreateDocumentClassifierRequestRequestTypeDef(
-    _RequiredCreateDocumentClassifierRequestRequestTypeDef,
-    _OptionalCreateDocumentClassifierRequestRequestTypeDef,
-):
-    pass
-
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectKeyPhrasesResponseTypeDef = TypedDict(
     "BatchDetectKeyPhrasesResponseTypeDef",
     {
         "ResultList": List[BatchDetectKeyPhrasesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectSentimentResponseTypeDef = TypedDict(
     "BatchDetectSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetedSentimentMentionTypeDef = TypedDict(
     "TargetedSentimentMentionTypeDef",
     {
         "Score": float,
@@ -2491,40 +2496,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
-DocumentClassifierPropertiesTypeDef = TypedDict(
-    "DocumentClassifierPropertiesTypeDef",
-    {
-        "DocumentClassifierArn": str,
-        "LanguageCode": LanguageCodeType,
-        "Status": ModelStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "TrainingStartTime": datetime,
-        "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
-        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
-        "ClassifierMetadata": ClassifierMetadataTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "Mode": DocumentClassifierModeType,
-        "ModelKmsKeyId": str,
-        "VersionName": str,
-        "SourceModelArn": str,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
 DocumentClassificationJobPropertiesTypeDef = TypedDict(
     "DocumentClassificationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
@@ -2974,23 +2953,81 @@
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDocumentClassifierRequestRequestTypeDef",
+    {
+        "DocumentClassifierName": str,
+        "DataAccessRoleArn": str,
+        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+    },
+)
+_OptionalCreateDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDocumentClassifierRequestRequestTypeDef",
+    {
+        "VersionName": str,
+        "Tags": Sequence[TagTypeDef],
+        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
+        "ClientRequestToken": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "Mode": DocumentClassifierModeType,
+        "ModelKmsKeyId": str,
+        "ModelPolicy": str,
+    },
+    total=False,
+)
+
+class CreateDocumentClassifierRequestRequestTypeDef(
+    _RequiredCreateDocumentClassifierRequestRequestTypeDef,
+    _OptionalCreateDocumentClassifierRequestRequestTypeDef,
+):
+    pass
+
+DocumentClassifierPropertiesTypeDef = TypedDict(
+    "DocumentClassifierPropertiesTypeDef",
+    {
+        "DocumentClassifierArn": str,
+        "LanguageCode": LanguageCodeType,
+        "Status": ModelStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "TrainingStartTime": datetime,
+        "TrainingEndTime": datetime,
+        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
+        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
+        "ClassifierMetadata": ClassifierMetadataTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "Mode": DocumentClassifierModeType,
+        "ModelKmsKeyId": str,
+        "VersionName": str,
+        "SourceModelArn": str,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Warnings": List[WarningsListItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
@@ -3048,24 +3085,24 @@
     total=False,
 )
 
 DescribeFlywheelIterationResponseTypeDef = TypedDict(
     "DescribeFlywheelIterationResponseTypeDef",
     {
         "FlywheelIterationProperties": FlywheelIterationPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFlywheelIterationHistoryResponseTypeDef = TypedDict(
     "ListFlywheelIterationHistoryResponseTypeDef",
     {
         "FlywheelIterationPropertiesList": List[FlywheelIterationPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "Id": str,
@@ -3087,15 +3124,15 @@
     total=False,
 )
 
 DetectSyntaxResponseTypeDef = TypedDict(
     "DetectSyntaxResponseTypeDef",
     {
         "SyntaxTokens": List[SyntaxTokenTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetedSentimentEntityTypeDef = TypedDict(
     "TargetedSentimentEntityTypeDef",
     {
         "DescriptiveMentionIndex": List[int],
@@ -3109,185 +3146,168 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDocumentClassificationJobsResponseTypeDef = TypedDict(
     "ListDocumentClassificationJobsResponseTypeDef",
     {
         "DocumentClassificationJobPropertiesList": List[DocumentClassificationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDominantLanguageDetectionJobResponseTypeDef = TypedDict(
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     {
         "DominantLanguageDetectionJobProperties": DominantLanguageDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDominantLanguageDetectionJobsResponseTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     {
         "DominantLanguageDetectionJobPropertiesList": List[
             DominantLanguageDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionJobResponseTypeDef",
     {
         "EntitiesDetectionJobProperties": EntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionJobsResponseTypeDef",
     {
         "EntitiesDetectionJobPropertiesList": List[EntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsDetectionJobResponseTypeDef = TypedDict(
     "DescribeEventsDetectionJobResponseTypeDef",
     {
         "EventsDetectionJobProperties": EventsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventsDetectionJobsResponseTypeDef = TypedDict(
     "ListEventsDetectionJobsResponseTypeDef",
     {
         "EventsDetectionJobPropertiesList": List[EventsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
     "DescribeKeyPhrasesDetectionJobResponseTypeDef",
     {
         "KeyPhrasesDetectionJobProperties": KeyPhrasesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKeyPhrasesDetectionJobsResponseTypeDef = TypedDict(
     "ListKeyPhrasesDetectionJobsResponseTypeDef",
     {
         "KeyPhrasesDetectionJobPropertiesList": List[KeyPhrasesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePiiEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribePiiEntitiesDetectionJobResponseTypeDef",
     {
         "PiiEntitiesDetectionJobProperties": PiiEntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPiiEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     {
         "PiiEntitiesDetectionJobPropertiesList": List[PiiEntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeSentimentDetectionJobResponseTypeDef",
     {
         "SentimentDetectionJobProperties": SentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListSentimentDetectionJobsResponseTypeDef",
     {
         "SentimentDetectionJobPropertiesList": List[SentimentDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     {
         "TargetedSentimentDetectionJobProperties": TargetedSentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetedSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     {
         "TargetedSentimentDetectionJobPropertiesList": List[
             TargetedSentimentDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTopicsDetectionJobResponseTypeDef = TypedDict(
     "DescribeTopicsDetectionJobResponseTypeDef",
     {
         "TopicsDetectionJobProperties": TopicsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTopicsDetectionJobsResponseTypeDef = TypedDict(
     "ListTopicsDetectionJobsResponseTypeDef",
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "FlywheelArn": str,
@@ -3307,14 +3327,31 @@
 )
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3385,24 +3422,24 @@
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Blocks": List[BlockTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectSyntaxResponseTypeDef = TypedDict(
     "BatchDetectSyntaxResponseTypeDef",
     {
         "ResultList": List[BatchDetectSyntaxItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectTargetedSentimentItemResultTypeDef = TypedDict(
     "BatchDetectTargetedSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -3411,61 +3448,61 @@
     total=False,
 )
 
 DetectTargetedSentimentResponseTypeDef = TypedDict(
     "DetectTargetedSentimentResponseTypeDef",
     {
         "Entities": List[TargetedSentimentEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectEntitiesResponseTypeDef = TypedDict(
     "BatchDetectEntitiesResponseTypeDef",
     {
         "ResultList": List[BatchDetectEntitiesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFlywheelResponseTypeDef = TypedDict(
     "DescribeFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlywheelResponseTypeDef = TypedDict(
     "UpdateFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntityRecognizerResponseTypeDef = TypedDict(
     "DescribeEntityRecognizerResponseTypeDef",
     {
         "EntityRecognizerProperties": EntityRecognizerPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntityRecognizersResponseTypeDef = TypedDict(
     "ListEntityRecognizersResponseTypeDef",
     {
         "EntityRecognizerPropertiesList": List[EntityRecognizerPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDetectTargetedSentimentResponseTypeDef = TypedDict(
     "BatchDetectTargetedSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectTargetedSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/PKG-INFO` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.26.99
-Summary: Type annotations for boto3.Comprehend 1.26.99 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Comprehend 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-comprehend"></a>
 
 # mypy-boto3-comprehend
 
 [![PyPI - mypy-boto3-comprehend](https://img.shields.io/pypi/v/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,14 +340,15 @@
 from mypy_boto3_comprehend.literals import (
     AugmentedManifestsDocumentTypeFormatType,
     BlockTypeType,
     DatasetDataFormatType,
     DatasetStatusType,
     DatasetTypeType,
     DocumentClassifierDataFormatType,
+    DocumentClassifierDocumentTypeFormatType,
     DocumentClassifierModeType,
     DocumentReadActionType,
     DocumentReadFeatureTypesType,
     DocumentReadModeType,
     DocumentTypeType,
     EndpointStatusType,
     EntityRecognizerDataFormatType,
@@ -366,14 +367,15 @@
     ListKeyPhrasesDetectionJobsPaginatorName,
     ListPiiEntitiesDetectionJobsPaginatorName,
     ListSentimentDetectionJobsPaginatorName,
     ListTopicsDetectionJobsPaginatorName,
     ModelStatusType,
     ModelTypeType,
     PageBasedErrorCodeType,
+    PageBasedWarningCodeType,
     PartOfSpeechTagTypeType,
     PiiEntitiesDetectionMaskModeType,
     PiiEntitiesDetectionModeType,
     PiiEntityTypeType,
     RelationshipTypeType,
     SentimentTypeType,
     SplitType,
@@ -400,15 +402,14 @@
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
-    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
@@ -417,19 +418,25 @@
     BoundingBoxTypeDef,
     ClassifierEvaluationMetricsTypeDef,
     DocumentReaderConfigTypeDef,
     DocumentClassTypeDef,
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
+    WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
+    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
     DatasetPropertiesTypeDef,
@@ -448,27 +455,29 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
     OutputDataConfigTypeDef,
+    DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityTypesListItemTypeDef,
@@ -482,68 +491,62 @@
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
+    ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
-    DocumentClassifierInputDataConfigTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
-    DetectDominantLanguageResponseTypeDef,
-    ImportModelResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
@@ -560,55 +563,54 @@
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
-    CreateDocumentClassifierRequestRequestTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
-    DocumentClassifierPropertiesTypeDef,
     DocumentClassificationJobPropertiesTypeDef,
     DominantLanguageDetectionJobPropertiesTypeDef,
     EntitiesDetectionJobPropertiesTypeDef,
     EventsDetectionJobPropertiesTypeDef,
     KeyPhrasesDetectionJobPropertiesTypeDef,
     PiiEntitiesDetectionJobPropertiesTypeDef,
     SentimentDetectionJobPropertiesTypeDef,
@@ -621,27 +623,27 @@
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
     TargetedSentimentDetectionJobPropertiesTypeDef,
     TopicsDetectionJobPropertiesTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
     DatasetInputDataConfigTypeDef,
+    CreateDocumentClassifierRequestRequestTypeDef,
+    DocumentClassifierPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -653,14 +655,16 @@
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
```

### Comparing `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/SOURCES.txt` & `mypy-boto3-comprehend-1.27.0/mypy_boto3_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.99/setup.py` & `mypy-boto3-comprehend-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehend",
-    version="1.26.99",
+    version="1.27.0",
     packages=["mypy_boto3_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Comprehend 1.26.99 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.Comprehend 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


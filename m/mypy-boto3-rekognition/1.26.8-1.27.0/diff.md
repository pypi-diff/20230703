# Comparing `tmp/mypy-boto3-rekognition-1.26.8.tar.gz` & `tmp/mypy-boto3-rekognition-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.27.0.tar", last modified: Mon Jul  3 19:51:19 2023, max compression
```

## Comparing `mypy-boto3-rekognition-1.26.8.tar` & `mypy-boto3-rekognition-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.082122 mypy-boto3-rekognition-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    24573 2022-11-11 21:07:54.078122 mypy-boto3-rekognition-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23122 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.070122 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    50861 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    50781 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12528 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12526 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9820 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    83084 2022-11-11 21:07:34.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    82983 2022-11-11 21:07:33.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.078122 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24573 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.082122 mypy-boto3-rekognition-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-11 21:07:31.000000 mypy-boto3-rekognition-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.527875 mypy-boto3-rekognition-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-03 19:51:19.519875 mypy-boto3-rekognition-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24890 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.515874 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97128 2023-07-03 19:46:14.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97009 2023-07-03 19:46:13.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-03 19:46:12.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.519875 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-03 19:51:19.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 19:51:19.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:51:19.000000 mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:19.527875 mypy-boto3-rekognition-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:46:11.000000 mypy-boto3-rekognition-1.27.0/setup.py
```

### Comparing `mypy-boto3-rekognition-1.26.8/LICENSE` & `mypy-boto3-rekognition-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-rekognition-1.26.8/PKG-INFO` & `mypy-boto3-rekognition-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.26.8
-Summary: Type annotations for boto3.Rekognition 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Rekognition 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
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
 
 <a id="mypy-boto3-rekognition"></a>
 
 # mypy-boto3-rekognition
 
 [![PyPI - mypy-boto3-rekognition](https://img.shields.io/pypi/v/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,14 +288,15 @@
     DescribeProjectsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 
 client: RekognitionClient = Session().client("rekognition")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_project_versions_paginator: DescribeProjectVersionsPaginator = client.get_paginator(
@@ -311,14 +313,15 @@
 list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
 list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator(
     "list_project_policies"
 )
 list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator(
     "list_stream_processors"
 )
+list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
 ```
 
 <a id="waiters-annotations"></a>
 
 ### Waiters annotations
 
 `mypy_boto3_rekognition.waiter` module contains type annotations for all
@@ -354,48 +357,58 @@
 
 ```python
 from mypy_boto3_rekognition.literals import (
     AttributeType,
     BodyPartType,
     CelebrityRecognitionSortByType,
     ContentClassifierType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetStatusMessageCodeType,
     DatasetStatusType,
     DatasetTypeType,
     DescribeProjectVersionsPaginatorName,
     DescribeProjectsPaginatorName,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
+    LabelDetectionAggregateByType,
+    LabelDetectionFeatureNameType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     ListCollectionsPaginatorName,
     ListDatasetEntriesPaginatorName,
     ListDatasetLabelsPaginatorName,
     ListFacesPaginatorName,
     ListProjectPoliciesPaginatorName,
     ListStreamProcessorsPaginatorName,
+    ListUsersPaginatorName,
+    LivenessSessionStatusType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionRunningWaiterName,
     ProjectVersionStatusType,
     ProjectVersionTrainingCompletedWaiterName,
     ProtectiveEquipmentTypeType,
     QualityFilterType,
     ReasonType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
     StreamProcessorStatusType,
     TechnicalCueTypeType,
     TextTypesType,
+    UnsearchedFaceReasonType,
+    UnsuccessfulFaceAssociationReasonType,
+    UnsuccessfulFaceDeletionReasonType,
+    UnsuccessfulFaceDisassociationReasonType,
+    UserStatusType,
     VideoColorRangeType,
     VideoJobStatusType,
     RekognitionServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
@@ -413,256 +426,293 @@
 
 `mypy_boto3_rekognition.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
+    AssociateFacesRequestRequestTypeDef,
+    AssociatedFaceTypeDef,
+    UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
+    BoundingBoxTypeDef,
+    S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
-    BoundingBoxTypeDef,
     KnownGenderTypeDef,
-    ResponseMetadataTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
+    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    LivenessOutputConfigTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    CreateUserRequestRequestTypeDef,
     DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
+    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
+    UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
+    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
+    DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
+    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
     DetectionFilterTypeDef,
+    DisassociateFacesRequestRequestTypeDef,
+    DisassociatedFaceTypeDef,
+    UnsuccessfulFaceDisassociationTypeDef,
     DistributeDatasetTypeDef,
+    EyeDirectionTypeDef,
     EyeOpenTypeDef,
     EyeglassesTypeDef,
+    FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
     FaceSearchSettingsTypeDef,
     PointTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
+    GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
+    GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
+    GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
-    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListUsersRequestRequestTypeDef,
+    UserTypeDef,
+    MatchedUserTypeDef,
     NotificationChannelTypeDef,
+    PaginatorConfigTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
+    PutProjectPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
+    SearchUsersRequestRequestTypeDef,
+    SearchedFaceTypeDef,
+    SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
-    StartShotDetectionFilterTypeDef,
-    StreamProcessingStopSelectorTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    StartTechnicalCueDetectionFilterTypeDef,
-    ComparedSourceImageFaceTypeDef,
-    FaceTypeDef,
-    CopyProjectVersionResponseTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
-    CreateStreamProcessorResponseTypeDef,
-    DeleteCollectionResponseTypeDef,
-    DeleteFacesResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    DeleteProjectVersionResponseTypeDef,
-    DescribeCollectionResponseTypeDef,
-    GetCelebrityInfoResponseTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
+    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
+    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    AssociateFacesResponseTypeDef,
+    ComparedSourceImageFaceTypeDef,
+    FaceTypeDef,
+    AuditImageTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
+    SummaryTypeDef,
+    VideoTypeDef,
+    StartTechnicalCueDetectionFilterTypeDef,
+    GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
+    CreateFaceLivenessSessionRequestSettingsTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    DeleteFacesResponseTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
+    LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
+    DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
-    SummaryTypeDef,
-    VideoTypeDef,
     HumanLoopConfigTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
+    ListUsersResponseTypeDef,
+    UserMatchTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
+    GetFaceLivenessSessionResultsResponseTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
+    CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
+    SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
+    UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
     StartTextDetectionFiltersTypeDef,
     UpdateStreamProcessorRequestRequestTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
+    SearchUsersResponseTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
-    StartSegmentDetectionRequestRequestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
+    ValidationDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
     GetFaceDetectionResponseTypeDef,
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
+    SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
-    ValidationDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
+    TestingDataResultTypeDef,
+    TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
-    TestingDataResultTypeDef,
-    TrainingDataResultTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
@@ -671,42 +721,42 @@
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

### Comparing `mypy-boto3-rekognition-1.26.8/README.md` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-rekognition
+Version: 1.27.0
+Summary: Type annotations for boto3.Rekognition 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-rekognition"></a>
 
 # mypy-boto3-rekognition
 
 [![PyPI - mypy-boto3-rekognition](https://img.shields.io/pypi/v/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -256,14 +288,15 @@
     DescribeProjectsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 
 client: RekognitionClient = Session().client("rekognition")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_project_versions_paginator: DescribeProjectVersionsPaginator = client.get_paginator(
@@ -280,14 +313,15 @@
 list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
 list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator(
     "list_project_policies"
 )
 list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator(
     "list_stream_processors"
 )
+list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
 ```
 
 <a id="waiters-annotations"></a>
 
 ### Waiters annotations
 
 `mypy_boto3_rekognition.waiter` module contains type annotations for all
@@ -323,48 +357,58 @@
 
 ```python
 from mypy_boto3_rekognition.literals import (
     AttributeType,
     BodyPartType,
     CelebrityRecognitionSortByType,
     ContentClassifierType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetStatusMessageCodeType,
     DatasetStatusType,
     DatasetTypeType,
     DescribeProjectVersionsPaginatorName,
     DescribeProjectsPaginatorName,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
+    LabelDetectionAggregateByType,
+    LabelDetectionFeatureNameType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     ListCollectionsPaginatorName,
     ListDatasetEntriesPaginatorName,
     ListDatasetLabelsPaginatorName,
     ListFacesPaginatorName,
     ListProjectPoliciesPaginatorName,
     ListStreamProcessorsPaginatorName,
+    ListUsersPaginatorName,
+    LivenessSessionStatusType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionRunningWaiterName,
     ProjectVersionStatusType,
     ProjectVersionTrainingCompletedWaiterName,
     ProtectiveEquipmentTypeType,
     QualityFilterType,
     ReasonType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
     StreamProcessorStatusType,
     TechnicalCueTypeType,
     TextTypesType,
+    UnsearchedFaceReasonType,
+    UnsuccessfulFaceAssociationReasonType,
+    UnsuccessfulFaceDeletionReasonType,
+    UnsuccessfulFaceDisassociationReasonType,
+    UserStatusType,
     VideoColorRangeType,
     VideoJobStatusType,
     RekognitionServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
@@ -382,256 +426,293 @@
 
 `mypy_boto3_rekognition.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
+    AssociateFacesRequestRequestTypeDef,
+    AssociatedFaceTypeDef,
+    UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
+    BoundingBoxTypeDef,
+    S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
-    BoundingBoxTypeDef,
     KnownGenderTypeDef,
-    ResponseMetadataTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
+    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    LivenessOutputConfigTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    CreateUserRequestRequestTypeDef,
     DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
+    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
+    UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
+    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
+    DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
+    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
     DetectionFilterTypeDef,
+    DisassociateFacesRequestRequestTypeDef,
+    DisassociatedFaceTypeDef,
+    UnsuccessfulFaceDisassociationTypeDef,
     DistributeDatasetTypeDef,
+    EyeDirectionTypeDef,
     EyeOpenTypeDef,
     EyeglassesTypeDef,
+    FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
     FaceSearchSettingsTypeDef,
     PointTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
+    GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
+    GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
+    GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
-    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListUsersRequestRequestTypeDef,
+    UserTypeDef,
+    MatchedUserTypeDef,
     NotificationChannelTypeDef,
+    PaginatorConfigTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
+    PutProjectPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
+    SearchUsersRequestRequestTypeDef,
+    SearchedFaceTypeDef,
+    SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
-    StartShotDetectionFilterTypeDef,
-    StreamProcessingStopSelectorTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    StartTechnicalCueDetectionFilterTypeDef,
-    ComparedSourceImageFaceTypeDef,
-    FaceTypeDef,
-    CopyProjectVersionResponseTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
-    CreateStreamProcessorResponseTypeDef,
-    DeleteCollectionResponseTypeDef,
-    DeleteFacesResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    DeleteProjectVersionResponseTypeDef,
-    DescribeCollectionResponseTypeDef,
-    GetCelebrityInfoResponseTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
+    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
+    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    AssociateFacesResponseTypeDef,
+    ComparedSourceImageFaceTypeDef,
+    FaceTypeDef,
+    AuditImageTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
+    SummaryTypeDef,
+    VideoTypeDef,
+    StartTechnicalCueDetectionFilterTypeDef,
+    GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
+    CreateFaceLivenessSessionRequestSettingsTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    DeleteFacesResponseTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
+    LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
+    DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
-    SummaryTypeDef,
-    VideoTypeDef,
     HumanLoopConfigTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
+    ListUsersResponseTypeDef,
+    UserMatchTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
+    GetFaceLivenessSessionResultsResponseTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
+    CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
+    SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
+    UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
     StartTextDetectionFiltersTypeDef,
     UpdateStreamProcessorRequestRequestTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
+    SearchUsersResponseTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
-    StartSegmentDetectionRequestRequestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
+    ValidationDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
     GetFaceDetectionResponseTypeDef,
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
+    SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
-    ValidationDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
+    TestingDataResultTypeDef,
+    TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
-    TestingDataResultTypeDef,
-    TrainingDataResultTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
@@ -640,42 +721,42 @@
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

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         DescribeProjectsPaginator,
         ListCollectionsPaginator,
         ListDatasetEntriesPaginator,
         ListDatasetLabelsPaginator,
         ListFacesPaginator,
         ListProjectPoliciesPaginator,
         ListStreamProcessorsPaginator,
+        ListUsersPaginator,
         ProjectVersionRunningWaiter,
         ProjectVersionTrainingCompletedWaiter,
         RekognitionClient,
     )
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
@@ -30,26 +31,28 @@
     describe_projects_paginator: DescribeProjectsPaginator = client.get_paginator("describe_projects")
     list_collections_paginator: ListCollectionsPaginator = client.get_paginator("list_collections")
     list_dataset_entries_paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
     list_dataset_labels_paginator: ListDatasetLabelsPaginator = client.get_paginator("list_dataset_labels")
     list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
     list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator("list_project_policies")
     list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator("list_stream_processors")
+    list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
     ```
 """
 from .client import RekognitionClient
 from .paginator import (
     DescribeProjectsPaginator,
     DescribeProjectVersionsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 Client = RekognitionClient
 
 
 __all__ = (
@@ -58,11 +61,12 @@
     "DescribeProjectsPaginator",
     "ListCollectionsPaginator",
     "ListDatasetEntriesPaginator",
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
+    "ListUsersPaginator",
     "ProjectVersionRunningWaiter",
     "ProjectVersionTrainingCompletedWaiter",
     "RekognitionClient",
 )
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         DescribeProjectsPaginator,
         ListCollectionsPaginator,
         ListDatasetEntriesPaginator,
         ListDatasetLabelsPaginator,
         ListFacesPaginator,
         ListProjectPoliciesPaginator,
         ListStreamProcessorsPaginator,
+        ListUsersPaginator,
         ProjectVersionRunningWaiter,
         ProjectVersionTrainingCompletedWaiter,
         RekognitionClient,
     )
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
@@ -30,26 +31,28 @@
     describe_projects_paginator: DescribeProjectsPaginator = client.get_paginator("describe_projects")
     list_collections_paginator: ListCollectionsPaginator = client.get_paginator("list_collections")
     list_dataset_entries_paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
     list_dataset_labels_paginator: ListDatasetLabelsPaginator = client.get_paginator("list_dataset_labels")
     list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
     list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator("list_project_policies")
     list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator("list_stream_processors")
+    list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
     ```
 """
 from .client import RekognitionClient
 from .paginator import (
     DescribeProjectsPaginator,
     DescribeProjectVersionsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 Client = RekognitionClient
 
 __all__ = (
     "Client",
@@ -57,11 +60,12 @@
     "DescribeProjectsPaginator",
     "ListCollectionsPaginator",
     "ListDatasetEntriesPaginator",
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
+    "ListUsersPaginator",
     "ProjectVersionRunningWaiter",
     "ProjectVersionTrainingCompletedWaiter",
     "RekognitionClient",
 )
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.26.8\nVersion:         1.26.8\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Rekognition 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.8")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AttributeType,
     CelebrityRecognitionSortByType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     FaceAttributesType,
     FaceSearchSortByType,
+    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     PersonTrackingSortByType,
     QualityFilterType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
 )
 from .paginator import (
@@ -37,20 +39,24 @@
     DescribeProjectVersionsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 from .type_defs import (
+    AssociateFacesResponseTypeDef,
     CompareFacesResponseTypeDef,
     CopyProjectVersionResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionRequestSettingsTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateProjectVersionResponseTypeDef,
     CreateStreamProcessorResponseTypeDef,
     DatasetChangesTypeDef,
     DatasetSourceTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteFacesResponseTypeDef,
@@ -65,42 +71,48 @@
     DetectFacesResponseTypeDef,
     DetectLabelsResponseTypeDef,
     DetectLabelsSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     DetectTextFiltersTypeDef,
     DetectTextResponseTypeDef,
+    DisassociateFacesResponseTypeDef,
     DistributeDatasetTypeDef,
     GetCelebrityInfoResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetContentModerationResponseTypeDef,
     GetFaceDetectionResponseTypeDef,
+    GetFaceLivenessSessionResultsResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     HumanLoopConfigTypeDef,
     ImageTypeDef,
     IndexFacesResponseTypeDef,
+    LabelDetectionSettingsTypeDef,
     ListCollectionsResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     ListFacesResponseTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    SearchUsersByImageResponseTypeDef,
+    SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
     StartProjectVersionResponseTypeDef,
@@ -140,14 +152,15 @@
         self.response: Dict[str, Any]
         self.operation_name: str
 
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     HumanLoopQuotaExceededException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     ImageTooLargeException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     InvalidImageFormatException: Type[BotocoreClientError]
     InvalidPaginationTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -157,14 +170,15 @@
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     ProvisionedThroughputExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
+    SessionNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     VideoTooLargeException: Type[BotocoreClientError]
 
 
 class RekognitionClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
@@ -178,14 +192,30 @@
         """
         RekognitionClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#exceptions)
         """
 
+    def associate_faces(
+        self,
+        *,
+        CollectionId: str,
+        UserId: str,
+        FaceIds: Sequence[str],
+        UserMatchThreshold: float = ...,
+        ClientRequestToken: str = ...
+    ) -> AssociateFacesResponseTypeDef:
+        """
+        Associates one or more faces with an existing UserID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.associate_faces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#associate_faces)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#can_paginate)
         """
@@ -253,14 +283,28 @@
         """
         Creates a new Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_dataset)
         """
 
+    def create_face_liveness_session(
+        self,
+        *,
+        KmsKeyId: str = ...,
+        Settings: CreateFaceLivenessSessionRequestSettingsTypeDef = ...,
+        ClientRequestToken: str = ...
+    ) -> CreateFaceLivenessSessionResponseTypeDef:
+        """
+        This API operation initiates a Face Liveness session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_face_liveness_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_face_liveness_session)
+        """
+
     def create_project(self, *, ProjectName: str) -> CreateProjectResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_project)
         """
@@ -301,14 +345,24 @@
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_stream_processor)
         """
 
+    def create_user(
+        self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Creates a new User within a collection specified by `CollectionId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_user)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_user)
+        """
+
     def delete_collection(self, *, CollectionId: str) -> DeleteCollectionResponseTypeDef:
         """
         Deletes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#delete_collection)
         """
@@ -363,14 +417,24 @@
         """
         Deletes the stream processor identified by `Name`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#delete_stream_processor)
         """
 
+    def delete_user(
+        self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes the specified UserID within the collection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_user)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#delete_user)
+        """
+
     def describe_collection(self, *, CollectionId: str) -> DescribeCollectionResponseTypeDef:
         """
         Describes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#describe_collection)
         """
@@ -493,14 +557,30 @@
         """
         Detects text in the input image and converts it into machine-readable text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#detect_text)
         """
 
+    def disassociate_faces(
+        self,
+        *,
+        CollectionId: str,
+        UserId: str,
+        FaceIds: Sequence[str],
+        ClientRequestToken: str = ...
+    ) -> DisassociateFacesResponseTypeDef:
+        """
+        Removes the association between a `Face` supplied in an array of `FaceIds` and
+        the User.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.disassociate_faces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#disassociate_faces)
+        """
+
     def distribute_dataset_entries(
         self, *, Datasets: Sequence[DistributeDatasetTypeDef]
     ) -> Dict[str, Any]:
         """
         Distributes the entries (images) in a training dataset across the training
         dataset and the test dataset for a project.
 
@@ -537,47 +617,58 @@
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: CelebrityRecognitionSortByType = ...
     ) -> GetCelebrityRecognitionResponseTypeDef:
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
-        started by  StartCelebrityRecognition .
+        started by  StartCelebrityRecognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_celebrity_recognition)
         """
 
     def get_content_moderation(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: ContentModerationSortByType = ...
+        SortBy: ContentModerationSortByType = ...,
+        AggregateBy: ContentModerationAggregateByType = ...
     ) -> GetContentModerationResponseTypeDef:
         """
         Gets the inappropriate, unwanted, or offensive content analysis results for a
         Amazon Rekognition Video analysis started by  StartContentModeration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_content_moderation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_content_moderation)
         """
 
     def get_face_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetFaceDetectionResponseTypeDef:
         """
         Gets face detection results for a Amazon Rekognition Video analysis started by
-        StartFaceDetection .
+        StartFaceDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_face_detection)
         """
 
+    def get_face_liveness_session_results(
+        self, *, SessionId: str
+    ) -> GetFaceLivenessSessionResultsResponseTypeDef:
+        """
+        Retrieves the results of a specific Face Liveness session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_liveness_session_results)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_face_liveness_session_results)
+        """
+
     def get_face_search(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: FaceSearchSortByType = ...
@@ -592,19 +683,20 @@
 
     def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: LabelDetectionSortByType = ...
+        SortBy: LabelDetectionSortByType = ...,
+        AggregateBy: LabelDetectionAggregateByType = ...
     ) -> GetLabelDetectionResponseTypeDef:
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
-        by  StartLabelDetection .
+        by  StartLabelDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_label_detection)
         """
 
     def get_person_tracking(
         self,
@@ -612,37 +704,37 @@
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: PersonTrackingSortByType = ...
     ) -> GetPersonTrackingResponseTypeDef:
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started by
-        StartPersonTracking .
+        StartPersonTracking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_person_tracking)
         """
 
     def get_segment_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetSegmentDetectionResponseTypeDef:
         """
         Gets the segment detection results of a Amazon Rekognition Video analysis
-        started by  StartSegmentDetection .
+        started by  StartSegmentDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_segment_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_segment_detection)
         """
 
     def get_text_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetTextDetectionResponseTypeDef:
         """
         Gets the text detection results of a Amazon Rekognition Video analysis started
-        by  StartTextDetection .
+        by  StartTextDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_text_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_text_detection)
         """
 
     def index_faces(
         self,
@@ -696,15 +788,21 @@
         Lists the labels in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_dataset_labels)
         """
 
     def list_faces(
-        self, *, CollectionId: str, NextToken: str = ..., MaxResults: int = ...
+        self,
+        *,
+        CollectionId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        UserId: str = ...,
+        FaceIds: Sequence[str] = ...
     ) -> ListFacesResponseTypeDef:
         """
         Returns metadata for faces in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_faces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_faces)
         """
@@ -720,29 +818,39 @@
         """
 
     def list_stream_processors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListStreamProcessorsResponseTypeDef:
         """
         Gets a list of stream processors that you have created with
-        CreateStreamProcessor .
+        CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_stream_processors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_stream_processors)
         """
 
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags in an Amazon Rekognition collection, stream processor, or
         Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_tags_for_resource)
         """
 
+    def list_users(
+        self, *, CollectionId: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListUsersResponseTypeDef:
+        """
+        Returns metadata of the User such as `UserID` in the specified collection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_users)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_users)
+        """
+
     def put_project_policy(
         self, *, ProjectArn: str, PolicyName: str, PolicyDocument: str, PolicyRevisionId: str = ...
     ) -> PutProjectPolicyResponseTypeDef:
         """
         Attaches a project policy to a Amazon Rekognition Custom Labels project in a
         trusting AWS account.
 
@@ -787,14 +895,46 @@
         For a given input image, first detects the largest face in the image, and then
         searches the specified collection for matching faces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces_by_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#search_faces_by_image)
         """
 
+    def search_users(
+        self,
+        *,
+        CollectionId: str,
+        UserId: str = ...,
+        FaceId: str = ...,
+        UserMatchThreshold: float = ...,
+        MaxUsers: int = ...
+    ) -> SearchUsersResponseTypeDef:
+        """
+        Searches for UserIDs within a collection based on a `FaceId` or `UserId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#search_users)
+        """
+
+    def search_users_by_image(
+        self,
+        *,
+        CollectionId: str,
+        Image: ImageTypeDef,
+        UserMatchThreshold: float = ...,
+        MaxUsers: int = ...,
+        QualityFilter: QualityFilterType = ...
+    ) -> SearchUsersByImageResponseTypeDef:
+        """
+        Searches for UserIDs using a supplied image.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users_by_image)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#search_users_by_image)
+        """
+
     def start_celebrity_recognition(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...
@@ -860,15 +1000,17 @@
     def start_label_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
+        Features: Sequence[Literal["GENERAL_LABELS"]] = ...,
+        Settings: LabelDetectionSettingsTypeDef = ...
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#start_label_detection)
         """
@@ -951,15 +1093,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_project_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_project_version)
         """
 
     def stop_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
-        Stops a running stream processor that was created by  CreateStreamProcessor .
+        Stops a running stream processor that was created by  CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_stream_processor)
         """
 
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
@@ -1072,14 +1214,21 @@
     ) -> ListStreamProcessorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(self, operation_name: Literal["list_users"]) -> ListUsersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_paginator)
+        """
+
+    @overload
     def get_waiter(
         self, waiter_name: Literal["project_version_running"]
     ) -> ProjectVersionRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AttributeType,
     CelebrityRecognitionSortByType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     FaceAttributesType,
     FaceSearchSortByType,
+    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     PersonTrackingSortByType,
     QualityFilterType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
 )
 from .paginator import (
@@ -37,20 +39,24 @@
     DescribeProjectVersionsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 from .type_defs import (
+    AssociateFacesResponseTypeDef,
     CompareFacesResponseTypeDef,
     CopyProjectVersionResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionRequestSettingsTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateProjectVersionResponseTypeDef,
     CreateStreamProcessorResponseTypeDef,
     DatasetChangesTypeDef,
     DatasetSourceTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteFacesResponseTypeDef,
@@ -65,42 +71,48 @@
     DetectFacesResponseTypeDef,
     DetectLabelsResponseTypeDef,
     DetectLabelsSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     DetectTextFiltersTypeDef,
     DetectTextResponseTypeDef,
+    DisassociateFacesResponseTypeDef,
     DistributeDatasetTypeDef,
     GetCelebrityInfoResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetContentModerationResponseTypeDef,
     GetFaceDetectionResponseTypeDef,
+    GetFaceLivenessSessionResultsResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     HumanLoopConfigTypeDef,
     ImageTypeDef,
     IndexFacesResponseTypeDef,
+    LabelDetectionSettingsTypeDef,
     ListCollectionsResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     ListFacesResponseTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    SearchUsersByImageResponseTypeDef,
+    SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
     StartProjectVersionResponseTypeDef,
@@ -137,14 +149,15 @@
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     HumanLoopQuotaExceededException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     ImageTooLargeException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     InvalidImageFormatException: Type[BotocoreClientError]
     InvalidPaginationTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -154,14 +167,15 @@
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     ProvisionedThroughputExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
+    SessionNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     VideoTooLargeException: Type[BotocoreClientError]
 
 class RekognitionClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/)
@@ -173,14 +187,29 @@
     def exceptions(self) -> Exceptions:
         """
         RekognitionClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#exceptions)
         """
+    def associate_faces(
+        self,
+        *,
+        CollectionId: str,
+        UserId: str,
+        FaceIds: Sequence[str],
+        UserMatchThreshold: float = ...,
+        ClientRequestToken: str = ...
+    ) -> AssociateFacesResponseTypeDef:
+        """
+        Associates one or more faces with an existing UserID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.associate_faces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#associate_faces)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#can_paginate)
         """
@@ -242,14 +271,27 @@
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_dataset)
         """
+    def create_face_liveness_session(
+        self,
+        *,
+        KmsKeyId: str = ...,
+        Settings: CreateFaceLivenessSessionRequestSettingsTypeDef = ...,
+        ClientRequestToken: str = ...
+    ) -> CreateFaceLivenessSessionResponseTypeDef:
+        """
+        This API operation initiates a Face Liveness session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_face_liveness_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_face_liveness_session)
+        """
     def create_project(self, *, ProjectName: str) -> CreateProjectResponseTypeDef:
         """
         Creates a new Amazon Rekognition Custom Labels project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_project)
         """
@@ -287,14 +329,23 @@
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_stream_processor)
         """
+    def create_user(
+        self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Creates a new User within a collection specified by `CollectionId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_user)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#create_user)
+        """
     def delete_collection(self, *, CollectionId: str) -> DeleteCollectionResponseTypeDef:
         """
         Deletes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#delete_collection)
         """
@@ -342,14 +393,23 @@
     def delete_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes the stream processor identified by `Name`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#delete_stream_processor)
         """
+    def delete_user(
+        self, *, CollectionId: str, UserId: str, ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes the specified UserID within the collection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.delete_user)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#delete_user)
+        """
     def describe_collection(self, *, CollectionId: str) -> DescribeCollectionResponseTypeDef:
         """
         Describes the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#describe_collection)
         """
@@ -461,14 +521,29 @@
     ) -> DetectTextResponseTypeDef:
         """
         Detects text in the input image and converts it into machine-readable text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#detect_text)
         """
+    def disassociate_faces(
+        self,
+        *,
+        CollectionId: str,
+        UserId: str,
+        FaceIds: Sequence[str],
+        ClientRequestToken: str = ...
+    ) -> DisassociateFacesResponseTypeDef:
+        """
+        Removes the association between a `Face` supplied in an array of `FaceIds` and
+        the User.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.disassociate_faces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#disassociate_faces)
+        """
     def distribute_dataset_entries(
         self, *, Datasets: Sequence[DistributeDatasetTypeDef]
     ) -> Dict[str, Any]:
         """
         Distributes the entries (images) in a training dataset across the training
         dataset and the test dataset for a project.
 
@@ -502,44 +577,54 @@
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: CelebrityRecognitionSortByType = ...
     ) -> GetCelebrityRecognitionResponseTypeDef:
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
-        started by  StartCelebrityRecognition .
+        started by  StartCelebrityRecognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_celebrity_recognition)
         """
     def get_content_moderation(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: ContentModerationSortByType = ...
+        SortBy: ContentModerationSortByType = ...,
+        AggregateBy: ContentModerationAggregateByType = ...
     ) -> GetContentModerationResponseTypeDef:
         """
         Gets the inappropriate, unwanted, or offensive content analysis results for a
         Amazon Rekognition Video analysis started by  StartContentModeration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_content_moderation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_content_moderation)
         """
     def get_face_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetFaceDetectionResponseTypeDef:
         """
         Gets face detection results for a Amazon Rekognition Video analysis started by
-        StartFaceDetection .
+        StartFaceDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_face_detection)
         """
+    def get_face_liveness_session_results(
+        self, *, SessionId: str
+    ) -> GetFaceLivenessSessionResultsResponseTypeDef:
+        """
+        Retrieves the results of a specific Face Liveness session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_liveness_session_results)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_face_liveness_session_results)
+        """
     def get_face_search(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: FaceSearchSortByType = ...
@@ -553,54 +638,55 @@
         """
     def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: LabelDetectionSortByType = ...
+        SortBy: LabelDetectionSortByType = ...,
+        AggregateBy: LabelDetectionAggregateByType = ...
     ) -> GetLabelDetectionResponseTypeDef:
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
-        by  StartLabelDetection .
+        by  StartLabelDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_label_detection)
         """
     def get_person_tracking(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: PersonTrackingSortByType = ...
     ) -> GetPersonTrackingResponseTypeDef:
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started by
-        StartPersonTracking .
+        StartPersonTracking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_person_tracking)
         """
     def get_segment_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetSegmentDetectionResponseTypeDef:
         """
         Gets the segment detection results of a Amazon Rekognition Video analysis
-        started by  StartSegmentDetection .
+        started by  StartSegmentDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_segment_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_segment_detection)
         """
     def get_text_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetTextDetectionResponseTypeDef:
         """
         Gets the text detection results of a Amazon Rekognition Video analysis started
-        by  StartTextDetection .
+        by  StartTextDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_text_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_text_detection)
         """
     def index_faces(
         self,
         *,
@@ -649,15 +735,21 @@
         """
         Lists the labels in a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_dataset_labels)
         """
     def list_faces(
-        self, *, CollectionId: str, NextToken: str = ..., MaxResults: int = ...
+        self,
+        *,
+        CollectionId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        UserId: str = ...,
+        FaceIds: Sequence[str] = ...
     ) -> ListFacesResponseTypeDef:
         """
         Returns metadata for faces in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_faces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_faces)
         """
@@ -671,27 +763,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_project_policies)
         """
     def list_stream_processors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListStreamProcessorsResponseTypeDef:
         """
         Gets a list of stream processors that you have created with
-        CreateStreamProcessor .
+        CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_stream_processors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_stream_processors)
         """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags in an Amazon Rekognition collection, stream processor, or
         Custom Labels model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_tags_for_resource)
         """
+    def list_users(
+        self, *, CollectionId: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListUsersResponseTypeDef:
+        """
+        Returns metadata of the User such as `UserID` in the specified collection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_users)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_users)
+        """
     def put_project_policy(
         self, *, ProjectArn: str, PolicyName: str, PolicyDocument: str, PolicyRevisionId: str = ...
     ) -> PutProjectPolicyResponseTypeDef:
         """
         Attaches a project policy to a Amazon Rekognition Custom Labels project in a
         trusting AWS account.
 
@@ -732,14 +833,44 @@
         """
         For a given input image, first detects the largest face in the image, and then
         searches the specified collection for matching faces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces_by_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#search_faces_by_image)
         """
+    def search_users(
+        self,
+        *,
+        CollectionId: str,
+        UserId: str = ...,
+        FaceId: str = ...,
+        UserMatchThreshold: float = ...,
+        MaxUsers: int = ...
+    ) -> SearchUsersResponseTypeDef:
+        """
+        Searches for UserIDs within a collection based on a `FaceId` or `UserId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#search_users)
+        """
+    def search_users_by_image(
+        self,
+        *,
+        CollectionId: str,
+        Image: ImageTypeDef,
+        UserMatchThreshold: float = ...,
+        MaxUsers: int = ...,
+        QualityFilter: QualityFilterType = ...
+    ) -> SearchUsersByImageResponseTypeDef:
+        """
+        Searches for UserIDs using a supplied image.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users_by_image)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#search_users_by_image)
+        """
     def start_celebrity_recognition(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...
@@ -801,15 +932,17 @@
     def start_label_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
+        Features: Sequence[Literal["GENERAL_LABELS"]] = ...,
+        Settings: LabelDetectionSettingsTypeDef = ...
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#start_label_detection)
         """
@@ -885,15 +1018,15 @@
         Stops a running model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_project_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_project_version)
         """
     def stop_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
-        Stops a running stream processor that was created by  CreateStreamProcessor .
+        Stops a running stream processor that was created by  CreateStreamProcessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_stream_processor)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more key-value tags to an Amazon Rekognition collection, stream
@@ -993,14 +1126,20 @@
         self, operation_name: Literal["list_stream_processors"]
     ) -> ListStreamProcessorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_paginator)
         """
     @overload
+    def get_paginator(self, operation_name: Literal["list_users"]) -> ListUsersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_paginator)
+        """
+    @overload
     def get_waiter(
         self, waiter_name: Literal["project_version_running"]
     ) -> ProjectVersionRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/literals.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -4,79 +4,103 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/literals/)
 
 Usage::
 
     ```python
     from mypy_boto3_rekognition.literals import AttributeType
 
-    data: AttributeType = "ALL"
+    data: AttributeType = "AGE_RANGE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AttributeType",
     "BodyPartType",
     "CelebrityRecognitionSortByType",
     "ContentClassifierType",
+    "ContentModerationAggregateByType",
     "ContentModerationSortByType",
     "DatasetStatusMessageCodeType",
     "DatasetStatusType",
     "DatasetTypeType",
     "DescribeProjectVersionsPaginatorName",
     "DescribeProjectsPaginatorName",
     "DetectLabelsFeatureNameType",
     "EmotionNameType",
     "FaceAttributesType",
     "FaceSearchSortByType",
     "GenderTypeType",
     "KnownGenderTypeType",
+    "LabelDetectionAggregateByType",
+    "LabelDetectionFeatureNameType",
     "LabelDetectionSortByType",
     "LandmarkTypeType",
     "ListCollectionsPaginatorName",
     "ListDatasetEntriesPaginatorName",
     "ListDatasetLabelsPaginatorName",
     "ListFacesPaginatorName",
     "ListProjectPoliciesPaginatorName",
     "ListStreamProcessorsPaginatorName",
+    "ListUsersPaginatorName",
+    "LivenessSessionStatusType",
     "OrientationCorrectionType",
     "PersonTrackingSortByType",
     "ProjectStatusType",
     "ProjectVersionRunningWaiterName",
     "ProjectVersionStatusType",
     "ProjectVersionTrainingCompletedWaiterName",
     "ProtectiveEquipmentTypeType",
     "QualityFilterType",
     "ReasonType",
     "SegmentTypeType",
     "StreamProcessorParameterToDeleteType",
     "StreamProcessorStatusType",
     "TechnicalCueTypeType",
     "TextTypesType",
+    "UnsearchedFaceReasonType",
+    "UnsuccessfulFaceAssociationReasonType",
+    "UnsuccessfulFaceDeletionReasonType",
+    "UnsuccessfulFaceDisassociationReasonType",
+    "UserStatusType",
     "VideoColorRangeType",
     "VideoJobStatusType",
     "RekognitionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
-AttributeType = Literal["ALL", "DEFAULT"]
+AttributeType = Literal[
+    "AGE_RANGE",
+    "ALL",
+    "BEARD",
+    "DEFAULT",
+    "EMOTIONS",
+    "EYEGLASSES",
+    "EYES_OPEN",
+    "EYE_DIRECTION",
+    "FACE_OCCLUDED",
+    "GENDER",
+    "MOUTH_OPEN",
+    "MUSTACHE",
+    "SMILE",
+    "SUNGLASSES",
+]
 BodyPartType = Literal["FACE", "HEAD", "LEFT_HAND", "RIGHT_HAND"]
 CelebrityRecognitionSortByType = Literal["ID", "TIMESTAMP"]
 ContentClassifierType = Literal["FreeOfAdultContent", "FreeOfPersonallyIdentifiableInformation"]
+ContentModerationAggregateByType = Literal["SEGMENTS", "TIMESTAMPS"]
 ContentModerationSortByType = Literal["NAME", "TIMESTAMP"]
 DatasetStatusMessageCodeType = Literal["CLIENT_ERROR", "SERVICE_ERROR", "SUCCESS"]
 DatasetStatusType = Literal[
     "CREATE_COMPLETE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETE_IN_PROGRESS",
@@ -91,14 +115,16 @@
 EmotionNameType = Literal[
     "ANGRY", "CALM", "CONFUSED", "DISGUSTED", "FEAR", "HAPPY", "SAD", "SURPRISED", "UNKNOWN"
 ]
 FaceAttributesType = Literal["ALL", "DEFAULT"]
 FaceSearchSortByType = Literal["INDEX", "TIMESTAMP"]
 GenderTypeType = Literal["Female", "Male"]
 KnownGenderTypeType = Literal["Female", "Male", "Nonbinary", "Unlisted"]
+LabelDetectionAggregateByType = Literal["SEGMENTS", "TIMESTAMPS"]
+LabelDetectionFeatureNameType = Literal["GENERAL_LABELS"]
 LabelDetectionSortByType = Literal["NAME", "TIMESTAMP"]
 LandmarkTypeType = Literal[
     "chinBottom",
     "eyeLeft",
     "eyeRight",
     "leftEyeBrowLeft",
     "leftEyeBrowRight",
@@ -130,14 +156,16 @@
 ]
 ListCollectionsPaginatorName = Literal["list_collections"]
 ListDatasetEntriesPaginatorName = Literal["list_dataset_entries"]
 ListDatasetLabelsPaginatorName = Literal["list_dataset_labels"]
 ListFacesPaginatorName = Literal["list_faces"]
 ListProjectPoliciesPaginatorName = Literal["list_project_policies"]
 ListStreamProcessorsPaginatorName = Literal["list_stream_processors"]
+ListUsersPaginatorName = Literal["list_users"]
+LivenessSessionStatusType = Literal["CREATED", "EXPIRED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 OrientationCorrectionType = Literal["ROTATE_0", "ROTATE_180", "ROTATE_270", "ROTATE_90"]
 PersonTrackingSortByType = Literal["INDEX", "TIMESTAMP"]
 ProjectStatusType = Literal["CREATED", "CREATING", "DELETING"]
 ProjectVersionRunningWaiterName = Literal["project_version_running"]
 ProjectVersionStatusType = Literal[
     "COPYING_COMPLETED",
     "COPYING_FAILED",
@@ -169,14 +197,32 @@
 StreamProcessorStatusType = Literal[
     "FAILED", "RUNNING", "STARTING", "STOPPED", "STOPPING", "UPDATING"
 ]
 TechnicalCueTypeType = Literal[
     "BlackFrames", "ColorBars", "Content", "EndCredits", "OpeningCredits", "Slate", "StudioLogo"
 ]
 TextTypesType = Literal["LINE", "WORD"]
+UnsearchedFaceReasonType = Literal[
+    "EXCEEDS_MAX_FACES",
+    "EXTREME_POSE",
+    "FACE_NOT_LARGEST",
+    "LOW_BRIGHTNESS",
+    "LOW_CONFIDENCE",
+    "LOW_FACE_QUALITY",
+    "LOW_SHARPNESS",
+    "SMALL_BOUNDING_BOX",
+]
+UnsuccessfulFaceAssociationReasonType = Literal[
+    "ASSOCIATED_TO_A_DIFFERENT_USER", "FACE_NOT_FOUND", "LOW_MATCH_CONFIDENCE"
+]
+UnsuccessfulFaceDeletionReasonType = Literal["ASSOCIATED_TO_AN_EXISTING_USER", "FACE_NOT_FOUND"]
+UnsuccessfulFaceDisassociationReasonType = Literal[
+    "ASSOCIATED_TO_A_DIFFERENT_USER", "FACE_NOT_FOUND"
+]
+UserStatusType = Literal["ACTIVE", "CREATED", "CREATING", "UPDATING"]
 VideoColorRangeType = Literal["FULL", "LIMITED"]
 VideoJobStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 RekognitionServiceName = Literal["rekognition"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -187,23 +233,25 @@
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
@@ -213,30 +261,35 @@
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
@@ -262,14 +315,15 @@
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
@@ -314,51 +368,57 @@
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
@@ -371,14 +431,15 @@
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
@@ -390,28 +451,35 @@
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
@@ -439,56 +507,64 @@
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
@@ -515,14 +591,15 @@
     "describe_projects",
     "list_collections",
     "list_dataset_entries",
     "list_dataset_labels",
     "list_faces",
     "list_project_policies",
     "list_stream_processors",
+    "list_users",
 ]
 WaiterName = Literal["project_version_running", "project_version_training_completed"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/literals.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,77 +4,105 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/literals/)
 
 Usage::
 
     ```python
     from mypy_boto3_rekognition.literals import AttributeType
 
-    data: AttributeType = "ALL"
+    data: AttributeType = "AGE_RANGE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AttributeType",
     "BodyPartType",
     "CelebrityRecognitionSortByType",
     "ContentClassifierType",
+    "ContentModerationAggregateByType",
     "ContentModerationSortByType",
     "DatasetStatusMessageCodeType",
     "DatasetStatusType",
     "DatasetTypeType",
     "DescribeProjectVersionsPaginatorName",
     "DescribeProjectsPaginatorName",
     "DetectLabelsFeatureNameType",
     "EmotionNameType",
     "FaceAttributesType",
     "FaceSearchSortByType",
     "GenderTypeType",
     "KnownGenderTypeType",
+    "LabelDetectionAggregateByType",
+    "LabelDetectionFeatureNameType",
     "LabelDetectionSortByType",
     "LandmarkTypeType",
     "ListCollectionsPaginatorName",
     "ListDatasetEntriesPaginatorName",
     "ListDatasetLabelsPaginatorName",
     "ListFacesPaginatorName",
     "ListProjectPoliciesPaginatorName",
     "ListStreamProcessorsPaginatorName",
+    "ListUsersPaginatorName",
+    "LivenessSessionStatusType",
     "OrientationCorrectionType",
     "PersonTrackingSortByType",
     "ProjectStatusType",
     "ProjectVersionRunningWaiterName",
     "ProjectVersionStatusType",
     "ProjectVersionTrainingCompletedWaiterName",
     "ProtectiveEquipmentTypeType",
     "QualityFilterType",
     "ReasonType",
     "SegmentTypeType",
     "StreamProcessorParameterToDeleteType",
     "StreamProcessorStatusType",
     "TechnicalCueTypeType",
     "TextTypesType",
+    "UnsearchedFaceReasonType",
+    "UnsuccessfulFaceAssociationReasonType",
+    "UnsuccessfulFaceDeletionReasonType",
+    "UnsuccessfulFaceDisassociationReasonType",
+    "UserStatusType",
     "VideoColorRangeType",
     "VideoJobStatusType",
     "RekognitionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-AttributeType = Literal["ALL", "DEFAULT"]
+
+AttributeType = Literal[
+    "AGE_RANGE",
+    "ALL",
+    "BEARD",
+    "DEFAULT",
+    "EMOTIONS",
+    "EYEGLASSES",
+    "EYES_OPEN",
+    "EYE_DIRECTION",
+    "FACE_OCCLUDED",
+    "GENDER",
+    "MOUTH_OPEN",
+    "MUSTACHE",
+    "SMILE",
+    "SUNGLASSES",
+]
 BodyPartType = Literal["FACE", "HEAD", "LEFT_HAND", "RIGHT_HAND"]
 CelebrityRecognitionSortByType = Literal["ID", "TIMESTAMP"]
 ContentClassifierType = Literal["FreeOfAdultContent", "FreeOfPersonallyIdentifiableInformation"]
+ContentModerationAggregateByType = Literal["SEGMENTS", "TIMESTAMPS"]
 ContentModerationSortByType = Literal["NAME", "TIMESTAMP"]
 DatasetStatusMessageCodeType = Literal["CLIENT_ERROR", "SERVICE_ERROR", "SUCCESS"]
 DatasetStatusType = Literal[
     "CREATE_COMPLETE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETE_IN_PROGRESS",
@@ -89,14 +117,16 @@
 EmotionNameType = Literal[
     "ANGRY", "CALM", "CONFUSED", "DISGUSTED", "FEAR", "HAPPY", "SAD", "SURPRISED", "UNKNOWN"
 ]
 FaceAttributesType = Literal["ALL", "DEFAULT"]
 FaceSearchSortByType = Literal["INDEX", "TIMESTAMP"]
 GenderTypeType = Literal["Female", "Male"]
 KnownGenderTypeType = Literal["Female", "Male", "Nonbinary", "Unlisted"]
+LabelDetectionAggregateByType = Literal["SEGMENTS", "TIMESTAMPS"]
+LabelDetectionFeatureNameType = Literal["GENERAL_LABELS"]
 LabelDetectionSortByType = Literal["NAME", "TIMESTAMP"]
 LandmarkTypeType = Literal[
     "chinBottom",
     "eyeLeft",
     "eyeRight",
     "leftEyeBrowLeft",
     "leftEyeBrowRight",
@@ -128,14 +158,16 @@
 ]
 ListCollectionsPaginatorName = Literal["list_collections"]
 ListDatasetEntriesPaginatorName = Literal["list_dataset_entries"]
 ListDatasetLabelsPaginatorName = Literal["list_dataset_labels"]
 ListFacesPaginatorName = Literal["list_faces"]
 ListProjectPoliciesPaginatorName = Literal["list_project_policies"]
 ListStreamProcessorsPaginatorName = Literal["list_stream_processors"]
+ListUsersPaginatorName = Literal["list_users"]
+LivenessSessionStatusType = Literal["CREATED", "EXPIRED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 OrientationCorrectionType = Literal["ROTATE_0", "ROTATE_180", "ROTATE_270", "ROTATE_90"]
 PersonTrackingSortByType = Literal["INDEX", "TIMESTAMP"]
 ProjectStatusType = Literal["CREATED", "CREATING", "DELETING"]
 ProjectVersionRunningWaiterName = Literal["project_version_running"]
 ProjectVersionStatusType = Literal[
     "COPYING_COMPLETED",
     "COPYING_FAILED",
@@ -167,14 +199,32 @@
 StreamProcessorStatusType = Literal[
     "FAILED", "RUNNING", "STARTING", "STOPPED", "STOPPING", "UPDATING"
 ]
 TechnicalCueTypeType = Literal[
     "BlackFrames", "ColorBars", "Content", "EndCredits", "OpeningCredits", "Slate", "StudioLogo"
 ]
 TextTypesType = Literal["LINE", "WORD"]
+UnsearchedFaceReasonType = Literal[
+    "EXCEEDS_MAX_FACES",
+    "EXTREME_POSE",
+    "FACE_NOT_LARGEST",
+    "LOW_BRIGHTNESS",
+    "LOW_CONFIDENCE",
+    "LOW_FACE_QUALITY",
+    "LOW_SHARPNESS",
+    "SMALL_BOUNDING_BOX",
+]
+UnsuccessfulFaceAssociationReasonType = Literal[
+    "ASSOCIATED_TO_A_DIFFERENT_USER", "FACE_NOT_FOUND", "LOW_MATCH_CONFIDENCE"
+]
+UnsuccessfulFaceDeletionReasonType = Literal["ASSOCIATED_TO_AN_EXISTING_USER", "FACE_NOT_FOUND"]
+UnsuccessfulFaceDisassociationReasonType = Literal[
+    "ASSOCIATED_TO_A_DIFFERENT_USER", "FACE_NOT_FOUND"
+]
+UserStatusType = Literal["ACTIVE", "CREATED", "CREATING", "UPDATING"]
 VideoColorRangeType = Literal["FULL", "LIMITED"]
 VideoJobStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 RekognitionServiceName = Literal["rekognition"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -185,23 +235,25 @@
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
@@ -211,30 +263,35 @@
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
@@ -260,14 +317,15 @@
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
@@ -312,51 +370,57 @@
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
@@ -369,14 +433,15 @@
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
@@ -388,28 +453,35 @@
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
@@ -437,56 +509,64 @@
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
@@ -513,14 +593,15 @@
     "describe_projects",
     "list_collections",
     "list_dataset_entries",
     "list_dataset_labels",
     "list_faces",
     "list_project_policies",
     "list_stream_processors",
+    "list_users",
 ]
 WaiterName = Literal["project_version_running", "project_version_training_completed"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,29 @@
         DescribeProjectsPaginator,
         ListCollectionsPaginator,
         ListDatasetEntriesPaginator,
         ListDatasetLabelsPaginator,
         ListFacesPaginator,
         ListProjectPoliciesPaginator,
         ListStreamProcessorsPaginator,
+        ListUsersPaginator,
     )
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
 
     describe_project_versions_paginator: DescribeProjectVersionsPaginator = client.get_paginator("describe_project_versions")
     describe_projects_paginator: DescribeProjectsPaginator = client.get_paginator("describe_projects")
     list_collections_paginator: ListCollectionsPaginator = client.get_paginator("list_collections")
     list_dataset_entries_paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
     list_dataset_labels_paginator: ListDatasetLabelsPaginator = client.get_paginator("list_dataset_labels")
     list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
     list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator("list_project_policies")
     list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator("list_stream_processors")
+    list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
@@ -42,26 +44,28 @@
     DescribeProjectVersionsResponseTypeDef,
     ListCollectionsResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     ListFacesResponseTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
+    ListUsersResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeProjectVersionsPaginator",
     "DescribeProjectsPaginator",
     "ListCollectionsPaginator",
     "ListDatasetEntriesPaginator",
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
+    "ListUsersPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -78,45 +82,45 @@
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeProjectVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectversionspaginator)
         """
 
 
 class DescribeProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
     """
 
     def paginate(
-        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
         """
 
 
 class ListCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
         """
 
 
@@ -130,73 +134,93 @@
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetentriespaginator)
         """
 
 
 class ListDatasetLabelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
     """
 
     def paginate(
-        self, *, DatasetArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DatasetArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetLabelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
         """
 
 
 class ListFacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        CollectionId: str,
+        UserId: str = ...,
+        FaceIds: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
         """
 
 
 class ListProjectPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
     """
 
     def paginate(
-        self, *, ProjectArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
         """
 
 
 class ListStreamProcessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamProcessorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
         """
+
+
+class ListUsersPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
+    """
+
+    def paginate(
+        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
+        """
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,29 @@
         DescribeProjectsPaginator,
         ListCollectionsPaginator,
         ListDatasetEntriesPaginator,
         ListDatasetLabelsPaginator,
         ListFacesPaginator,
         ListProjectPoliciesPaginator,
         ListStreamProcessorsPaginator,
+        ListUsersPaginator,
     )
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
 
     describe_project_versions_paginator: DescribeProjectVersionsPaginator = client.get_paginator("describe_project_versions")
     describe_projects_paginator: DescribeProjectsPaginator = client.get_paginator("describe_projects")
     list_collections_paginator: ListCollectionsPaginator = client.get_paginator("list_collections")
     list_dataset_entries_paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
     list_dataset_labels_paginator: ListDatasetLabelsPaginator = client.get_paginator("list_dataset_labels")
     list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
     list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator("list_project_policies")
     list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator("list_stream_processors")
+    list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
@@ -42,26 +44,28 @@
     DescribeProjectVersionsResponseTypeDef,
     ListCollectionsResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     ListFacesResponseTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
+    ListUsersResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeProjectVersionsPaginator",
     "DescribeProjectsPaginator",
     "ListCollectionsPaginator",
     "ListDatasetEntriesPaginator",
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
+    "ListUsersPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
@@ -75,43 +79,43 @@
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeProjectVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectversionspaginator)
         """
 
 class DescribeProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
     """
 
     def paginate(
-        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
         """
 
 class ListCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
         """
 
 class ListDatasetEntriesPaginator(Paginator):
@@ -124,69 +128,88 @@
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetentriespaginator)
         """
 
 class ListDatasetLabelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
     """
 
     def paginate(
-        self, *, DatasetArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DatasetArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetLabelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
         """
 
 class ListFacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        CollectionId: str,
+        UserId: str = ...,
+        FaceIds: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
         """
 
 class ListProjectPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
     """
 
     def paginate(
-        self, *, ProjectArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
         """
 
 class ListStreamProcessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamProcessorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
         """
+
+class ListUsersPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
+    """
+
+    def paginate(
+        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
+        """
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,316 +18,426 @@
 from botocore.response import StreamingBody
 
 from .literals import (
     AttributeType,
     BodyPartType,
     CelebrityRecognitionSortByType,
     ContentClassifierType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetStatusMessageCodeType,
     DatasetStatusType,
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
+    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     LandmarkTypeType,
+    LivenessSessionStatusType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionStatusType,
     ProtectiveEquipmentTypeType,
     QualityFilterType,
     ReasonType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
     StreamProcessorStatusType,
     TechnicalCueTypeType,
     TextTypesType,
+    UnsearchedFaceReasonType,
+    UnsuccessfulFaceAssociationReasonType,
+    UnsuccessfulFaceDeletionReasonType,
+    UnsuccessfulFaceDisassociationReasonType,
+    UserStatusType,
     VideoColorRangeType,
     VideoJobStatusType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AgeRangeTypeDef",
+    "AssociateFacesRequestRequestTypeDef",
+    "AssociatedFaceTypeDef",
+    "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
+    "BoundingBoxTypeDef",
+    "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
-    "BoundingBoxTypeDef",
     "KnownGenderTypeDef",
-    "ResponseMetadataTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
+    "CopyProjectVersionResponseTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
+    "CreateCollectionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "LivenessOutputConfigTypeDef",
+    "CreateFaceLivenessSessionResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateProjectVersionResponseTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
+    "CreateStreamProcessorResponseTypeDef",
+    "CreateUserRequestRequestTypeDef",
     "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
+    "DeleteCollectionResponseTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
+    "UnsuccessfulFaceDeletionTypeDef",
     "DeleteProjectPolicyRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResponseTypeDef",
     "DeleteProjectVersionRequestRequestTypeDef",
+    "DeleteProjectVersionResponseTypeDef",
     "DeleteStreamProcessorRequestRequestTypeDef",
+    "DeleteUserRequestRequestTypeDef",
     "DescribeCollectionRequestRequestTypeDef",
+    "DescribeCollectionResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ProtectiveEquipmentSummarizationAttributesTypeDef",
     "ProtectiveEquipmentSummaryTypeDef",
     "DetectionFilterTypeDef",
+    "DisassociateFacesRequestRequestTypeDef",
+    "DisassociatedFaceTypeDef",
+    "UnsuccessfulFaceDisassociationTypeDef",
     "DistributeDatasetTypeDef",
+    "EyeDirectionTypeDef",
     "EyeOpenTypeDef",
     "EyeglassesTypeDef",
+    "FaceOccludedTypeDef",
     "GenderTypeDef",
     "MouthOpenTypeDef",
     "MustacheTypeDef",
     "SunglassesTypeDef",
     "FaceSearchSettingsTypeDef",
     "PointTypeDef",
     "GetCelebrityInfoRequestRequestTypeDef",
     "GetCelebrityRecognitionRequestRequestTypeDef",
     "VideoMetadataTypeDef",
+    "GetContentModerationRequestMetadataTypeDef",
     "GetContentModerationRequestRequestTypeDef",
     "GetFaceDetectionRequestRequestTypeDef",
+    "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     "GetFaceSearchRequestRequestTypeDef",
+    "GetLabelDetectionRequestMetadataTypeDef",
     "GetLabelDetectionRequestRequestTypeDef",
     "GetPersonTrackingRequestRequestTypeDef",
     "GetSegmentDetectionRequestRequestTypeDef",
     "SegmentTypeInfoTypeDef",
     "GetTextDetectionRequestRequestTypeDef",
-    "S3ObjectTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
     "ListCollectionsRequestRequestTypeDef",
+    "ListCollectionsResponseTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     "ListDatasetLabelsRequestRequestTypeDef",
+    "ListFacesRequestListFacesPaginateTypeDef",
     "ListFacesRequestRequestTypeDef",
+    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     "ListProjectPoliciesRequestRequestTypeDef",
     "ProjectPolicyTypeDef",
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListUsersRequestRequestTypeDef",
+    "UserTypeDef",
+    "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
+    "PaginatorConfigTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
+    "PutProjectPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
+    "SearchUsersRequestRequestTypeDef",
+    "SearchedFaceTypeDef",
+    "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
     "TechnicalCueSegmentTypeDef",
-    "StartProjectVersionRequestRequestTypeDef",
-    "StartShotDetectionFilterTypeDef",
-    "StreamProcessingStopSelectorTypeDef",
-    "StopProjectVersionRequestRequestTypeDef",
-    "StopStreamProcessorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "StartTechnicalCueDetectionFilterTypeDef",
-    "ComparedSourceImageFaceTypeDef",
-    "FaceTypeDef",
-    "CopyProjectVersionResponseTypeDef",
-    "CreateCollectionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateProjectVersionResponseTypeDef",
-    "CreateStreamProcessorResponseTypeDef",
-    "DeleteCollectionResponseTypeDef",
-    "DeleteFacesResponseTypeDef",
-    "DeleteProjectResponseTypeDef",
-    "DeleteProjectVersionResponseTypeDef",
-    "DescribeCollectionResponseTypeDef",
-    "GetCelebrityInfoResponseTypeDef",
-    "ListCollectionsResponseTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutProjectPolicyResponseTypeDef",
     "StartCelebrityRecognitionResponseTypeDef",
     "StartContentModerationResponseTypeDef",
     "StartFaceDetectionResponseTypeDef",
     "StartFaceSearchResponseTypeDef",
     "StartLabelDetectionResponseTypeDef",
     "StartPersonTrackingResponseTypeDef",
+    "StartProjectVersionRequestRequestTypeDef",
     "StartProjectVersionResponseTypeDef",
+    "StartShotDetectionFilterTypeDef",
     "StartSegmentDetectionResponseTypeDef",
+    "StreamProcessingStopSelectorTypeDef",
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
+    "StopProjectVersionRequestRequestTypeDef",
     "StopProjectVersionResponseTypeDef",
+    "StopStreamProcessorRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "AssociateFacesResponseTypeDef",
+    "ComparedSourceImageFaceTypeDef",
+    "FaceTypeDef",
+    "AuditImageTypeDef",
+    "GroundTruthManifestTypeDef",
+    "ImageTypeDef",
+    "SummaryTypeDef",
+    "VideoTypeDef",
+    "StartTechnicalCueDetectionFilterTypeDef",
+    "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
+    "CreateFaceLivenessSessionRequestSettingsTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
-    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    "ListFacesRequestListFacesPaginateTypeDef",
-    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    "DeleteFacesResponseTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
+    "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
+    "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
     "RegionOfInterestTypeDef",
-    "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
-    "SummaryTypeDef",
-    "VideoTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "UserMatchTypeDef",
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
-    "StartSegmentDetectionFiltersTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
+    "GetFaceLivenessSessionResultsResponseTypeDef",
+    "AssetTypeDef",
+    "DatasetSourceTypeDef",
+    "CompareFacesRequestRequestTypeDef",
+    "DetectCustomLabelsRequestRequestTypeDef",
+    "DetectFacesRequestRequestTypeDef",
+    "DetectProtectiveEquipmentRequestRequestTypeDef",
+    "IndexFacesRequestRequestTypeDef",
+    "RecognizeCelebritiesRequestRequestTypeDef",
+    "SearchFacesByImageRequestRequestTypeDef",
+    "SearchUsersByImageRequestRequestTypeDef",
+    "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
+    "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
     "DescribeProjectsResponseTypeDef",
     "DetectLabelsImagePropertiesTypeDef",
     "LabelTypeDef",
+    "DetectLabelsRequestRequestTypeDef",
+    "StartLabelDetectionRequestRequestTypeDef",
     "CelebrityDetailTypeDef",
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
+    "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
+    "UnsearchedFaceTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
     "StartTextDetectionFiltersTypeDef",
     "UpdateStreamProcessorRequestRequestTypeDef",
-    "AssetTypeDef",
-    "DatasetSourceTypeDef",
-    "CompareFacesRequestRequestTypeDef",
-    "DetectCustomLabelsRequestRequestTypeDef",
-    "DetectFacesRequestRequestTypeDef",
-    "DetectLabelsRequestRequestTypeDef",
-    "DetectProtectiveEquipmentRequestRequestTypeDef",
-    "IndexFacesRequestRequestTypeDef",
-    "RecognizeCelebritiesRequestRequestTypeDef",
-    "SearchFacesByImageRequestRequestTypeDef",
-    "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartLabelDetectionRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
+    "SearchUsersResponseTypeDef",
     "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
-    "StartSegmentDetectionRequestRequestTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
+    "TestingDataTypeDef",
+    "TrainingDataTypeDef",
+    "ValidationDataTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
     "DetectLabelsResponseTypeDef",
     "LabelDetectionTypeDef",
     "CelebrityRecognitionTypeDef",
     "GetFaceDetectionResponseTypeDef",
     "PersonDetectionTypeDef",
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
+    "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "TestingDataTypeDef",
-    "TrainingDataTypeDef",
-    "ValidationDataTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
+    "CreateProjectVersionRequestRequestTypeDef",
+    "TestingDataResultTypeDef",
+    "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
     "GetTextDetectionResponseTypeDef",
-    "CreateProjectVersionRequestRequestTypeDef",
-    "TestingDataResultTypeDef",
-    "TrainingDataResultTypeDef",
     "ProjectVersionDescriptionTypeDef",
     "DescribeProjectVersionsResponseTypeDef",
 )
 
 AgeRangeTypeDef = TypedDict(
     "AgeRangeTypeDef",
     {
         "Low": int,
         "High": int,
     },
     total=False,
 )
 
+_RequiredAssociateFacesRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateFacesRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+        "FaceIds": Sequence[str],
+    },
+)
+_OptionalAssociateFacesRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateFacesRequestRequestTypeDef",
+    {
+        "UserMatchThreshold": float,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class AssociateFacesRequestRequestTypeDef(
+    _RequiredAssociateFacesRequestRequestTypeDef, _OptionalAssociateFacesRequestRequestTypeDef
+):
+    pass
+
+AssociatedFaceTypeDef = TypedDict(
+    "AssociatedFaceTypeDef",
+    {
+        "FaceId": str,
+    },
+    total=False,
+)
+
+UnsuccessfulFaceAssociationTypeDef = TypedDict(
+    "UnsuccessfulFaceAssociationTypeDef",
+    {
+        "FaceId": str,
+        "UserId": str,
+        "Confidence": float,
+        "Reasons": List[UnsuccessfulFaceAssociationReasonType],
+    },
+    total=False,
+)
+
 AudioMetadataTypeDef = TypedDict(
     "AudioMetadataTypeDef",
     {
         "Codec": str,
         "DurationMillis": int,
         "SampleRate": int,
         "NumberOfChannels": int,
     },
     total=False,
 )
 
+BoundingBoxTypeDef = TypedDict(
+    "BoundingBoxTypeDef",
+    {
+        "Width": float,
+        "Height": float,
+        "Left": float,
+        "Top": float,
+    },
+    total=False,
+)
+
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
+    {
+        "Bucket": str,
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 BeardTypeDef = TypedDict(
     "BeardTypeDef",
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
@@ -338,44 +448,22 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
-BoundingBoxTypeDef = TypedDict(
-    "BoundingBoxTypeDef",
-    {
-        "Width": float,
-        "Height": float,
-        "Left": float,
-        "Top": float,
-    },
-    total=False,
-)
-
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
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
 EmotionTypeDef = TypedDict(
     "EmotionTypeDef",
     {
         "Type": EmotionNameType,
         "Confidence": float,
     },
     total=False,
@@ -438,21 +526,19 @@
     "_OptionalConnectedHomeSettingsTypeDef",
     {
         "MinConfidence": float,
     },
     total=False,
 )
 
-
 class ConnectedHomeSettingsTypeDef(
     _RequiredConnectedHomeSettingsTypeDef, _OptionalConnectedHomeSettingsTypeDef
 ):
     pass
 
-
 ModerationLabelTypeDef = TypedDict(
     "ModerationLabelTypeDef",
     {
         "Confidence": float,
         "Name": str,
         "ParentName": str,
     },
@@ -464,14 +550,22 @@
     {
         "S3Bucket": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+CopyProjectVersionResponseTypeDef = TypedDict(
+    "CopyProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CoversBodyPartTypeDef = TypedDict(
     "CoversBodyPartTypeDef",
     {
         "Confidence": float,
         "Value": bool,
     },
     total=False,
@@ -487,42 +581,129 @@
     "_OptionalCreateCollectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
+CreateCollectionResponseTypeDef = TypedDict(
+    "CreateCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "CollectionArn": str,
+        "FaceModelVersion": str,
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
+_RequiredLivenessOutputConfigTypeDef = TypedDict(
+    "_RequiredLivenessOutputConfigTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalLivenessOutputConfigTypeDef = TypedDict(
+    "_OptionalLivenessOutputConfigTypeDef",
+    {
+        "S3KeyPrefix": str,
+    },
+    total=False,
+)
+
+class LivenessOutputConfigTypeDef(
+    _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
+):
+    pass
+
+CreateFaceLivenessSessionResponseTypeDef = TypedDict(
+    "CreateFaceLivenessSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProjectVersionResponseTypeDef = TypedDict(
+    "CreateProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StreamProcessorDataSharingPreferenceTypeDef = TypedDict(
     "StreamProcessorDataSharingPreferenceTypeDef",
     {
         "OptIn": bool,
     },
 )
 
 StreamProcessorNotificationChannelTypeDef = TypedDict(
     "StreamProcessorNotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
     },
 )
 
+CreateStreamProcessorResponseTypeDef = TypedDict(
+    "CreateStreamProcessorResponseTypeDef",
+    {
+        "StreamProcessorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateUserRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+    },
+)
+_OptionalCreateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateUserRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class CreateUserRequestRequestTypeDef(
+    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
+):
+    pass
+
 DatasetChangesTypeDef = TypedDict(
     "DatasetChangesTypeDef",
     {
         "GroundTruth": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
@@ -562,14 +743,22 @@
 DeleteCollectionRequestRequestTypeDef = TypedDict(
     "DeleteCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
+DeleteCollectionResponseTypeDef = TypedDict(
+    "DeleteCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -577,14 +766,24 @@
     "DeleteFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
         "FaceIds": Sequence[str],
     },
 )
 
+UnsuccessfulFaceDeletionTypeDef = TypedDict(
+    "UnsuccessfulFaceDeletionTypeDef",
+    {
+        "FaceId": str,
+        "UserId": str,
+        "Reasons": List[UnsuccessfulFaceDeletionReasonType],
+    },
+    total=False,
+)
+
 _RequiredDeleteProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
     },
 )
@@ -592,67 +791,124 @@
     "_OptionalDeleteProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteProjectPolicyRequestRequestTypeDef(
     _RequiredDeleteProjectPolicyRequestRequestTypeDef,
     _OptionalDeleteProjectPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Status": ProjectStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProjectVersionRequestRequestTypeDef = TypedDict(
     "DeleteProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
     },
 )
 
+DeleteProjectVersionResponseTypeDef = TypedDict(
+    "DeleteProjectVersionResponseTypeDef",
+    {
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteStreamProcessorRequestRequestTypeDef = TypedDict(
     "DeleteStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredDeleteUserRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteUserRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+    },
+)
+_OptionalDeleteUserRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteUserRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class DeleteUserRequestRequestTypeDef(
+    _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
+):
+    pass
+
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
+DescribeCollectionResponseTypeDef = TypedDict(
+    "DescribeCollectionResponseTypeDef",
+    {
+        "FaceCount": int,
+        "FaceModelVersion": str,
+        "CollectionARN": str,
+        "CreationTimestamp": datetime,
+        "UserCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProjectArn": str,
+    },
+)
+_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "VersionNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
+    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+):
+    pass
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -670,21 +926,28 @@
         "VersionNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
+DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    {
+        "ProjectNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
@@ -776,21 +1039,70 @@
         "MinConfidence": float,
         "MinBoundingBoxHeight": float,
         "MinBoundingBoxWidth": float,
     },
     total=False,
 )
 
+_RequiredDisassociateFacesRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateFacesRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+        "FaceIds": Sequence[str],
+    },
+)
+_OptionalDisassociateFacesRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateFacesRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class DisassociateFacesRequestRequestTypeDef(
+    _RequiredDisassociateFacesRequestRequestTypeDef, _OptionalDisassociateFacesRequestRequestTypeDef
+):
+    pass
+
+DisassociatedFaceTypeDef = TypedDict(
+    "DisassociatedFaceTypeDef",
+    {
+        "FaceId": str,
+    },
+    total=False,
+)
+
+UnsuccessfulFaceDisassociationTypeDef = TypedDict(
+    "UnsuccessfulFaceDisassociationTypeDef",
+    {
+        "FaceId": str,
+        "UserId": str,
+        "Reasons": List[UnsuccessfulFaceDisassociationReasonType],
+    },
+    total=False,
+)
+
 DistributeDatasetTypeDef = TypedDict(
     "DistributeDatasetTypeDef",
     {
         "Arn": str,
     },
 )
 
+EyeDirectionTypeDef = TypedDict(
+    "EyeDirectionTypeDef",
+    {
+        "Yaw": float,
+        "Pitch": float,
+        "Confidence": float,
+    },
+    total=False,
+)
+
 EyeOpenTypeDef = TypedDict(
     "EyeOpenTypeDef",
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
@@ -801,14 +1113,23 @@
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
 )
 
+FaceOccludedTypeDef = TypedDict(
+    "FaceOccludedTypeDef",
+    {
+        "Value": bool,
+        "Confidence": float,
+    },
+    total=False,
+)
+
 GenderTypeDef = TypedDict(
     "GenderTypeDef",
     {
         "Value": GenderTypeType,
         "Confidence": float,
     },
     total=False,
@@ -878,60 +1199,66 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": CelebrityRecognitionSortByType,
     },
     total=False,
 )
 
-
 class GetCelebrityRecognitionRequestRequestTypeDef(
     _RequiredGetCelebrityRecognitionRequestRequestTypeDef,
     _OptionalGetCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
-
 VideoMetadataTypeDef = TypedDict(
     "VideoMetadataTypeDef",
     {
         "Codec": str,
         "DurationMillis": int,
         "Format": str,
         "FrameRate": float,
         "FrameHeight": int,
         "FrameWidth": int,
         "ColorRange": VideoColorRangeType,
     },
     total=False,
 )
 
+GetContentModerationRequestMetadataTypeDef = TypedDict(
+    "GetContentModerationRequestMetadataTypeDef",
+    {
+        "SortBy": ContentModerationSortByType,
+        "AggregateBy": ContentModerationAggregateByType,
+    },
+    total=False,
+)
+
 _RequiredGetContentModerationRequestRequestTypeDef = TypedDict(
     "_RequiredGetContentModerationRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetContentModerationRequestRequestTypeDef = TypedDict(
     "_OptionalGetContentModerationRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": ContentModerationSortByType,
+        "AggregateBy": ContentModerationAggregateByType,
     },
     total=False,
 )
 
-
 class GetContentModerationRequestRequestTypeDef(
     _RequiredGetContentModerationRequestRequestTypeDef,
     _OptionalGetContentModerationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFaceDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -939,20 +1266,25 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetFaceDetectionRequestRequestTypeDef(
     _RequiredGetFaceDetectionRequestRequestTypeDef, _OptionalGetFaceDetectionRequestRequestTypeDef
 ):
     pass
 
+GetFaceLivenessSessionResultsRequestRequestTypeDef = TypedDict(
+    "GetFaceLivenessSessionResultsRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
 
 _RequiredGetFaceSearchRequestRequestTypeDef = TypedDict(
     "_RequiredGetFaceSearchRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
@@ -962,44 +1294,50 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": FaceSearchSortByType,
     },
     total=False,
 )
 
-
 class GetFaceSearchRequestRequestTypeDef(
     _RequiredGetFaceSearchRequestRequestTypeDef, _OptionalGetFaceSearchRequestRequestTypeDef
 ):
     pass
 
+GetLabelDetectionRequestMetadataTypeDef = TypedDict(
+    "GetLabelDetectionRequestMetadataTypeDef",
+    {
+        "SortBy": LabelDetectionSortByType,
+        "AggregateBy": LabelDetectionAggregateByType,
+    },
+    total=False,
+)
 
 _RequiredGetLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetLabelDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetLabelDetectionRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": LabelDetectionSortByType,
+        "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
 )
 
-
 class GetLabelDetectionRequestRequestTypeDef(
     _RequiredGetLabelDetectionRequestRequestTypeDef, _OptionalGetLabelDetectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPersonTrackingRequestRequestTypeDef = TypedDict(
     "_RequiredGetPersonTrackingRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetPersonTrackingRequestRequestTypeDef = TypedDict(
@@ -1008,21 +1346,19 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": PersonTrackingSortByType,
     },
     total=False,
 )
 
-
 class GetPersonTrackingRequestRequestTypeDef(
     _RequiredGetPersonTrackingRequestRequestTypeDef, _OptionalGetPersonTrackingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetSegmentDetectionRequestRequestTypeDef = TypedDict(
@@ -1030,22 +1366,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetSegmentDetectionRequestRequestTypeDef(
     _RequiredGetSegmentDetectionRequestRequestTypeDef,
     _OptionalGetSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
-
 SegmentTypeInfoTypeDef = TypedDict(
     "SegmentTypeInfoTypeDef",
     {
         "Type": SegmentTypeType,
         "ModelVersion": str,
     },
     total=False,
@@ -1062,31 +1396,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
-
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
-    {
-        "Bucket": str,
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1136,23 +1458,65 @@
     "ParentTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListCollectionsResponseTypeDef = TypedDict(
+    "ListCollectionsResponseTypeDef",
+    {
+        "CollectionIds": List[str],
+        "NextToken": str,
+        "FaceModelVersions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ContainsLabels": Sequence[str],
+        "Labeled": bool,
+        "SourceRefContains": str,
+        "HasErrors": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
@@ -1164,21 +1528,48 @@
         "HasErrors": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
+    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+):
+    pass
 
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
@@ -1187,42 +1578,82 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_RequiredListFacesRequestListFacesPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_OptionalListFacesRequestListFacesPaginateTypeDef",
+    {
+        "UserId": str,
+        "FaceIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFacesRequestListFacesPaginateTypeDef(
+    _RequiredListFacesRequestListFacesPaginateTypeDef,
+    _OptionalListFacesRequestListFacesPaginateTypeDef,
+):
+    pass
 
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
     "_OptionalListFacesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
+        "UserId": str,
+        "FaceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
+_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
+    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+):
+    pass
 
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
@@ -1231,35 +1662,41 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListProjectPoliciesRequestRequestTypeDef(
     _RequiredListProjectPoliciesRequestRequestTypeDef,
     _OptionalListProjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 ProjectPolicyTypeDef = TypedDict(
     "ProjectPolicyTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyRevisionId": str,
         "PolicyDocument": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStreamProcessorsRequestRequestTypeDef = TypedDict(
     "ListStreamProcessorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1277,22 +1714,98 @@
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
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
+):
+    pass
+
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "UserId": str,
+        "UserStatus": UserStatusType,
+    },
+    total=False,
+)
+
+MatchedUserTypeDef = TypedDict(
+    "MatchedUserTypeDef",
+    {
+        "UserId": str,
+        "UserStatus": UserStatusType,
+    },
+    total=False,
+)
+
 NotificationChannelTypeDef = TypedDict(
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
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
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyDocument": str,
     },
@@ -1301,20 +1814,37 @@
     "_OptionalPutProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
+PutProjectPolicyResponseTypeDef = TypedDict(
+    "PutProjectPolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
@@ -1333,362 +1863,322 @@
     {
         "MaxFaces": int,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
-
 class SearchFacesRequestRequestTypeDef(
     _RequiredSearchFacesRequestRequestTypeDef, _OptionalSearchFacesRequestRequestTypeDef
 ):
     pass
 
-
-ShotSegmentTypeDef = TypedDict(
-    "ShotSegmentTypeDef",
-    {
-        "Index": int,
-        "Confidence": float,
-    },
-    total=False,
-)
-
-TechnicalCueSegmentTypeDef = TypedDict(
-    "TechnicalCueSegmentTypeDef",
-    {
-        "Type": TechnicalCueTypeType,
-        "Confidence": float,
-    },
-    total=False,
-)
-
-_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartProjectVersionRequestRequestTypeDef",
+_RequiredSearchUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchUsersRequestRequestTypeDef",
     {
-        "ProjectVersionArn": str,
-        "MinInferenceUnits": int,
+        "CollectionId": str,
     },
 )
-_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartProjectVersionRequestRequestTypeDef",
+_OptionalSearchUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchUsersRequestRequestTypeDef",
     {
-        "MaxInferenceUnits": int,
+        "UserId": str,
+        "FaceId": str,
+        "UserMatchThreshold": float,
+        "MaxUsers": int,
     },
     total=False,
 )
 
-
-class StartProjectVersionRequestRequestTypeDef(
-    _RequiredStartProjectVersionRequestRequestTypeDef,
-    _OptionalStartProjectVersionRequestRequestTypeDef,
+class SearchUsersRequestRequestTypeDef(
+    _RequiredSearchUsersRequestRequestTypeDef, _OptionalSearchUsersRequestRequestTypeDef
 ):
     pass
 
-
-StartShotDetectionFilterTypeDef = TypedDict(
-    "StartShotDetectionFilterTypeDef",
+SearchedFaceTypeDef = TypedDict(
+    "SearchedFaceTypeDef",
     {
-        "MinSegmentConfidence": float,
+        "FaceId": str,
     },
     total=False,
 )
 
-StreamProcessingStopSelectorTypeDef = TypedDict(
-    "StreamProcessingStopSelectorTypeDef",
+SearchedUserTypeDef = TypedDict(
+    "SearchedUserTypeDef",
     {
-        "MaxDurationInSeconds": int,
+        "UserId": str,
     },
     total=False,
 )
 
-StopProjectVersionRequestRequestTypeDef = TypedDict(
-    "StopProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectVersionArn": str,
-    },
-)
-
-StopStreamProcessorRequestRequestTypeDef = TypedDict(
-    "StopStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ShotSegmentTypeDef = TypedDict(
+    "ShotSegmentTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "Index": int,
+        "Confidence": float,
     },
+    total=False,
 )
 
-StartTechnicalCueDetectionFilterTypeDef = TypedDict(
-    "StartTechnicalCueDetectionFilterTypeDef",
+TechnicalCueSegmentTypeDef = TypedDict(
+    "TechnicalCueSegmentTypeDef",
     {
-        "MinSegmentConfidence": float,
-        "BlackFrame": BlackFrameTypeDef,
+        "Type": TechnicalCueTypeType,
+        "Confidence": float,
     },
     total=False,
 )
 
-ComparedSourceImageFaceTypeDef = TypedDict(
-    "ComparedSourceImageFaceTypeDef",
+StartCelebrityRecognitionResponseTypeDef = TypedDict(
+    "StartCelebrityRecognitionResponseTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Confidence": float,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-FaceTypeDef = TypedDict(
-    "FaceTypeDef",
+StartContentModerationResponseTypeDef = TypedDict(
+    "StartContentModerationResponseTypeDef",
     {
-        "FaceId": str,
-        "BoundingBox": BoundingBoxTypeDef,
-        "ImageId": str,
-        "ExternalImageId": str,
-        "Confidence": float,
-        "IndexFacesModelVersion": str,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CopyProjectVersionResponseTypeDef = TypedDict(
-    "CopyProjectVersionResponseTypeDef",
+StartFaceDetectionResponseTypeDef = TypedDict(
+    "StartFaceDetectionResponseTypeDef",
     {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCollectionResponseTypeDef = TypedDict(
-    "CreateCollectionResponseTypeDef",
+StartFaceSearchResponseTypeDef = TypedDict(
+    "StartFaceSearchResponseTypeDef",
     {
-        "StatusCode": int,
-        "CollectionArn": str,
-        "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
+StartLabelDetectionResponseTypeDef = TypedDict(
+    "StartLabelDetectionResponseTypeDef",
     {
-        "DatasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
+StartPersonTrackingResponseTypeDef = TypedDict(
+    "StartPersonTrackingResponseTypeDef",
     {
-        "ProjectArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProjectVersionResponseTypeDef = TypedDict(
-    "CreateProjectVersionResponseTypeDef",
+_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MinInferenceUnits": int,
     },
 )
-
-CreateStreamProcessorResponseTypeDef = TypedDict(
-    "CreateStreamProcessorResponseTypeDef",
+_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartProjectVersionRequestRequestTypeDef",
     {
-        "StreamProcessorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxInferenceUnits": int,
     },
+    total=False,
 )
 
-DeleteCollectionResponseTypeDef = TypedDict(
-    "DeleteCollectionResponseTypeDef",
+class StartProjectVersionRequestRequestTypeDef(
+    _RequiredStartProjectVersionRequestRequestTypeDef,
+    _OptionalStartProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+StartProjectVersionResponseTypeDef = TypedDict(
+    "StartProjectVersionResponseTypeDef",
     {
-        "StatusCode": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteFacesResponseTypeDef = TypedDict(
-    "DeleteFacesResponseTypeDef",
+StartShotDetectionFilterTypeDef = TypedDict(
+    "StartShotDetectionFilterTypeDef",
     {
-        "DeletedFaces": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MinSegmentConfidence": float,
     },
+    total=False,
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
+StartSegmentDetectionResponseTypeDef = TypedDict(
+    "StartSegmentDetectionResponseTypeDef",
     {
-        "Status": ProjectStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteProjectVersionResponseTypeDef = TypedDict(
-    "DeleteProjectVersionResponseTypeDef",
+StreamProcessingStopSelectorTypeDef = TypedDict(
+    "StreamProcessingStopSelectorTypeDef",
     {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxDurationInSeconds": int,
     },
+    total=False,
 )
 
-DescribeCollectionResponseTypeDef = TypedDict(
-    "DescribeCollectionResponseTypeDef",
+StartStreamProcessorResponseTypeDef = TypedDict(
+    "StartStreamProcessorResponseTypeDef",
     {
-        "FaceCount": int,
-        "FaceModelVersion": str,
-        "CollectionARN": str,
-        "CreationTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetCelebrityInfoResponseTypeDef = TypedDict(
-    "GetCelebrityInfoResponseTypeDef",
+StartTextDetectionResponseTypeDef = TypedDict(
+    "StartTextDetectionResponseTypeDef",
     {
-        "Urls": List[str],
-        "Name": str,
-        "KnownGender": KnownGenderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListCollectionsResponseTypeDef = TypedDict(
-    "ListCollectionsResponseTypeDef",
+StopProjectVersionRequestRequestTypeDef = TypedDict(
+    "StopProjectVersionRequestRequestTypeDef",
     {
-        "CollectionIds": List[str],
-        "NextToken": str,
-        "FaceModelVersions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProjectVersionArn": str,
     },
 )
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
+StopProjectVersionResponseTypeDef = TypedDict(
+    "StopProjectVersionResponseTypeDef",
     {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+StopStreamProcessorRequestRequestTypeDef = TypedDict(
+    "StopStreamProcessorRequestRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
     },
 )
 
-PutProjectPolicyResponseTypeDef = TypedDict(
-    "PutProjectPolicyResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-StartCelebrityRecognitionResponseTypeDef = TypedDict(
-    "StartCelebrityRecognitionResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-StartContentModerationResponseTypeDef = TypedDict(
-    "StartContentModerationResponseTypeDef",
+AssociateFacesResponseTypeDef = TypedDict(
+    "AssociateFacesResponseTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AssociatedFaces": List[AssociatedFaceTypeDef],
+        "UnsuccessfulFaceAssociations": List[UnsuccessfulFaceAssociationTypeDef],
+        "UserStatus": UserStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartFaceDetectionResponseTypeDef = TypedDict(
-    "StartFaceDetectionResponseTypeDef",
+ComparedSourceImageFaceTypeDef = TypedDict(
+    "ComparedSourceImageFaceTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Confidence": float,
     },
+    total=False,
 )
 
-StartFaceSearchResponseTypeDef = TypedDict(
-    "StartFaceSearchResponseTypeDef",
+FaceTypeDef = TypedDict(
+    "FaceTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FaceId": str,
+        "BoundingBox": BoundingBoxTypeDef,
+        "ImageId": str,
+        "ExternalImageId": str,
+        "Confidence": float,
+        "IndexFacesModelVersion": str,
+        "UserId": str,
     },
+    total=False,
 )
 
-StartLabelDetectionResponseTypeDef = TypedDict(
-    "StartLabelDetectionResponseTypeDef",
+AuditImageTypeDef = TypedDict(
+    "AuditImageTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Bytes": bytes,
+        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
     },
+    total=False,
 )
 
-StartPersonTrackingResponseTypeDef = TypedDict(
-    "StartPersonTrackingResponseTypeDef",
+GroundTruthManifestTypeDef = TypedDict(
+    "GroundTruthManifestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartProjectVersionResponseTypeDef = TypedDict(
-    "StartProjectVersionResponseTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartSegmentDetectionResponseTypeDef = TypedDict(
-    "StartSegmentDetectionResponseTypeDef",
+SummaryTypeDef = TypedDict(
+    "SummaryTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartStreamProcessorResponseTypeDef = TypedDict(
-    "StartStreamProcessorResponseTypeDef",
+VideoTypeDef = TypedDict(
+    "VideoTypeDef",
     {
-        "SessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartTextDetectionResponseTypeDef = TypedDict(
-    "StartTextDetectionResponseTypeDef",
+StartTechnicalCueDetectionFilterTypeDef = TypedDict(
+    "StartTechnicalCueDetectionFilterTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MinSegmentConfidence": float,
+        "BlackFrame": BlackFrameTypeDef,
     },
+    total=False,
 )
 
-StopProjectVersionResponseTypeDef = TypedDict(
-    "StopProjectVersionResponseTypeDef",
+GetCelebrityInfoResponseTypeDef = TypedDict(
+    "GetCelebrityInfoResponseTypeDef",
     {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Urls": List[str],
+        "Name": str,
+        "KnownGender": KnownGenderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
@@ -1711,14 +2201,17 @@
 )
 
 ContentModerationDetectionTypeDef = TypedDict(
     "ContentModerationDetectionTypeDef",
     {
         "Timestamp": int,
         "ModerationLabel": ModerationLabelTypeDef,
+        "StartTimestampMillis": int,
+        "EndTimestampMillis": int,
+        "DurationMillis": int,
     },
     total=False,
 )
 
 _RequiredCopyProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyProjectVersionRequestRequestTypeDef",
     {
@@ -1734,33 +2227,40 @@
     {
         "Tags": Mapping[str, str],
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class CopyProjectVersionRequestRequestTypeDef(
     _RequiredCopyProjectVersionRequestRequestTypeDef,
     _OptionalCopyProjectVersionRequestRequestTypeDef,
 ):
     pass
 
-
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
     },
     total=False,
 )
 
+CreateFaceLivenessSessionRequestSettingsTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestSettingsTypeDef",
+    {
+        "OutputConfig": LivenessOutputConfigTypeDef,
+        "AuditImagesLimit": int,
+    },
+    total=False,
+)
+
 UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
     "UpdateDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
         "Changes": DatasetChangesTypeDef,
     },
 )
@@ -1794,152 +2294,21 @@
         "CreationTimestamp": datetime,
         "Status": ProjectStatusType,
         "Datasets": List[DatasetMetadataTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "VersionNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
-    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-):
-    pass
-
-
-DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    {
-        "ProjectNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ContainsLabels": Sequence[str],
-        "Labeled": bool,
-        "SourceRefContains": str,
-        "HasErrors": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
-    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_RequiredListFacesRequestListFacesPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_OptionalListFacesRequestListFacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFacesRequestListFacesPaginateTypeDef(
-    _RequiredListFacesRequestListFacesPaginateTypeDef,
-    _OptionalListFacesRequestListFacesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
-    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-):
-    pass
-
-
-ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+DeleteFacesResponseTypeDef = TypedDict(
+    "DeleteFacesResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DeletedFaces": List[str],
+        "UnsuccessfulFaceDeletions": List[UnsuccessfulFaceDeletionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
@@ -1951,22 +2320,20 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
@@ -1976,22 +2343,20 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
 ):
     pass
 
-
 DetectLabelsImageBackgroundTypeDef = TypedDict(
     "DetectLabelsImageBackgroundTypeDef",
     {
         "Quality": DetectLabelsImageQualityTypeDef,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
@@ -2021,21 +2386,39 @@
     {
         "GeneralLabels": GeneralLabelsSettingsTypeDef,
         "ImageProperties": DetectLabelsImagePropertiesSettingsTypeDef,
     },
     total=False,
 )
 
+LabelDetectionSettingsTypeDef = TypedDict(
+    "LabelDetectionSettingsTypeDef",
+    {
+        "GeneralLabels": GeneralLabelsSettingsTypeDef,
+    },
+    total=False,
+)
+
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateFacesResponseTypeDef = TypedDict(
+    "DisassociateFacesResponseTypeDef",
+    {
+        "DisassociatedFaces": List[DisassociatedFaceTypeDef],
+        "UnsuccessfulFaceDisassociations": List[UnsuccessfulFaceDisassociationTypeDef],
+        "UserStatus": UserStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DistributeDatasetEntriesRequestRequestTypeDef = TypedDict(
     "DistributeDatasetEntriesRequestRequestTypeDef",
     {
         "Datasets": Sequence[DistributeDatasetTypeDef],
@@ -2056,14 +2439,16 @@
         "EyesOpen": EyeOpenTypeDef,
         "MouthOpen": MouthOpenTypeDef,
         "Emotions": List[EmotionTypeDef],
         "Landmarks": List[LandmarkTypeDef],
         "Pose": PoseTypeDef,
         "Quality": ImageQualityTypeDef,
         "Confidence": float,
+        "FaceOccluded": FaceOccludedTypeDef,
+        "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
@@ -2087,47 +2472,14 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
 )
 
-GroundTruthManifestTypeDef = TypedDict(
-    "GroundTruthManifestTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-SummaryTypeDef = TypedDict(
-    "SummaryTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-VideoTypeDef = TypedDict(
-    "VideoTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
         "HumanLoopName": str,
         "FlowDefinitionArn": str,
     },
 )
@@ -2135,19 +2487,17 @@
     "_OptionalHumanLoopConfigTypeDef",
     {
         "DataAttributes": HumanLoopDataAttributesTypeDef,
     },
     total=False,
 )
 
-
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
-
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2161,25 +2511,43 @@
 )
 
 ListProjectPoliciesResponseTypeDef = TypedDict(
     "ListProjectPoliciesResponseTypeDef",
     {
         "ProjectPolicies": List[ProjectPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamProcessorsResponseTypeDef = TypedDict(
     "ListStreamProcessorsResponseTypeDef",
     {
         "NextToken": str,
         "StreamProcessors": List[StreamProcessorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
+    {
+        "Users": List[UserTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UserMatchTypeDef = TypedDict(
+    "UserMatchTypeDef",
+    {
+        "Similarity": float,
+        "User": MatchedUserTypeDef,
     },
+    total=False,
 )
 
 StreamProcessorOutputTypeDef = TypedDict(
     "StreamProcessorOutputTypeDef",
     {
         "KinesisDataStream": KinesisDataStreamTypeDef,
         "S3Destination": S3DestinationTypeDef,
@@ -2202,23 +2570,14 @@
         "StartFrameNumber": int,
         "EndFrameNumber": int,
         "DurationFrames": int,
     },
     total=False,
 )
 
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
 FaceMatchTypeDef = TypedDict(
     "FaceMatchTypeDef",
     {
         "Similarity": float,
         "Face": FaceTypeDef,
     },
     total=False,
@@ -2226,239 +2585,30 @@
 
 ListFacesResponseTypeDef = TypedDict(
     "ListFacesResponseTypeDef",
     {
         "Faces": List[FaceTypeDef],
         "NextToken": str,
         "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CelebrityTypeDef = TypedDict(
-    "CelebrityTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Face": ComparedFaceTypeDef,
-        "MatchConfidence": float,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-CompareFacesMatchTypeDef = TypedDict(
-    "CompareFacesMatchTypeDef",
-    {
-        "Similarity": float,
-        "Face": ComparedFaceTypeDef,
-    },
-    total=False,
-)
-
-GetContentModerationResponseTypeDef = TypedDict(
-    "GetContentModerationResponseTypeDef",
-    {
-        "JobStatus": VideoJobStatusType,
-        "StatusMessage": str,
-        "VideoMetadata": VideoMetadataTypeDef,
-        "ModerationLabels": List[ContentModerationDetectionTypeDef],
-        "NextToken": str,
-        "ModerationModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ProtectiveEquipmentBodyPartTypeDef = TypedDict(
-    "ProtectiveEquipmentBodyPartTypeDef",
-    {
-        "Name": BodyPartType,
-        "Confidence": float,
-        "EquipmentDetections": List[EquipmentDetectionTypeDef],
-    },
-    total=False,
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatasetLabelsResponseTypeDef = TypedDict(
-    "ListDatasetLabelsResponseTypeDef",
+GetFaceLivenessSessionResultsResponseTypeDef = TypedDict(
+    "GetFaceLivenessSessionResultsResponseTypeDef",
     {
-        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeProjectsResponseTypeDef = TypedDict(
-    "DescribeProjectsResponseTypeDef",
-    {
-        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectLabelsImagePropertiesTypeDef = TypedDict(
-    "DetectLabelsImagePropertiesTypeDef",
-    {
-        "Quality": DetectLabelsImageQualityTypeDef,
-        "DominantColors": List[DominantColorTypeDef],
-        "Foreground": DetectLabelsImageForegroundTypeDef,
-        "Background": DetectLabelsImageBackgroundTypeDef,
-    },
-    total=False,
-)
-
-LabelTypeDef = TypedDict(
-    "LabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Instances": List[InstanceTypeDef],
-        "Parents": List[ParentTypeDef],
-        "Aliases": List[LabelAliasTypeDef],
-        "Categories": List[LabelCategoryTypeDef],
-    },
-    total=False,
-)
-
-CelebrityDetailTypeDef = TypedDict(
-    "CelebrityDetailTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Confidence": float,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-DetectFacesResponseTypeDef = TypedDict(
-    "DetectFacesResponseTypeDef",
-    {
-        "FaceDetails": List[FaceDetailTypeDef],
-        "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-FaceDetectionTypeDef = TypedDict(
-    "FaceDetectionTypeDef",
-    {
-        "Timestamp": int,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-FaceRecordTypeDef = TypedDict(
-    "FaceRecordTypeDef",
-    {
-        "Face": FaceTypeDef,
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-PersonDetailTypeDef = TypedDict(
-    "PersonDetailTypeDef",
-    {
-        "Index": int,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-UnindexedFaceTypeDef = TypedDict(
-    "UnindexedFaceTypeDef",
-    {
-        "Reasons": List[ReasonType],
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-CustomLabelTypeDef = TypedDict(
-    "CustomLabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-TextDetectionTypeDef = TypedDict(
-    "TextDetectionTypeDef",
-    {
-        "DetectedText": str,
-        "Type": TextTypesType,
-        "Id": int,
-        "ParentId": int,
+        "SessionId": str,
+        "Status": LivenessSessionStatusType,
         "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-DetectTextFiltersTypeDef = TypedDict(
-    "DetectTextFiltersTypeDef",
-    {
-        "WordFilter": DetectionFilterTypeDef,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
-    },
-    total=False,
-)
-
-StartTextDetectionFiltersTypeDef = TypedDict(
-    "StartTextDetectionFiltersTypeDef",
-    {
-        "WordFilter": DetectionFilterTypeDef,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
-    },
-    total=False,
-)
-
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+        "ReferenceImage": AuditImageTypeDef,
+        "AuditImages": List[AuditImageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
     },
     total=False,
 )
@@ -2484,21 +2634,19 @@
     {
         "SimilarityThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class CompareFacesRequestRequestTypeDef(
     _RequiredCompareFacesRequestRequestTypeDef, _OptionalCompareFacesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDetectCustomLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectCustomLabelsRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2507,89 +2655,59 @@
     {
         "MaxResults": int,
         "MinConfidence": float,
     },
     total=False,
 )
 
-
 class DetectCustomLabelsRequestRequestTypeDef(
     _RequiredDetectCustomLabelsRequestRequestTypeDef,
     _OptionalDetectCustomLabelsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDetectFacesRequestRequestTypeDef = TypedDict(
     "_RequiredDetectFacesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectFacesRequestRequestTypeDef = TypedDict(
     "_OptionalDetectFacesRequestRequestTypeDef",
     {
         "Attributes": Sequence[AttributeType],
     },
     total=False,
 )
 
-
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectLabelsRequestRequestTypeDef",
-    {
-        "MaxLabels": int,
-        "MinConfidence": float,
-        "Features": Sequence[DetectLabelsFeatureNameType],
-        "Settings": DetectLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class DetectLabelsRequestRequestTypeDef(
-    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_OptionalDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "SummarizationAttributes": ProtectiveEquipmentSummarizationAttributesTypeDef,
     },
     total=False,
 )
 
-
 class DetectProtectiveEquipmentRequestRequestTypeDef(
     _RequiredDetectProtectiveEquipmentRequestRequestTypeDef,
     _OptionalDetectProtectiveEquipmentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredIndexFacesRequestRequestTypeDef = TypedDict(
     "_RequiredIndexFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2600,21 +2718,19 @@
         "DetectionAttributes": Sequence[AttributeType],
         "MaxFaces": int,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class IndexFacesRequestRequestTypeDef(
     _RequiredIndexFacesRequestRequestTypeDef, _OptionalIndexFacesRequestRequestTypeDef
 ):
     pass
 
-
 RecognizeCelebritiesRequestRequestTypeDef = TypedDict(
     "RecognizeCelebritiesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 
@@ -2631,21 +2747,42 @@
         "MaxFaces": int,
         "FaceMatchThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class SearchFacesByImageRequestRequestTypeDef(
     _RequiredSearchFacesByImageRequestRequestTypeDef,
     _OptionalSearchFacesByImageRequestRequestTypeDef,
 ):
     pass
 
+_RequiredSearchUsersByImageRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchUsersByImageRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalSearchUsersByImageRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchUsersByImageRequestRequestTypeDef",
+    {
+        "UserMatchThreshold": float,
+        "MaxUsers": int,
+        "QualityFilter": QualityFilterType,
+    },
+    total=False,
+)
+
+class SearchUsersByImageRequestRequestTypeDef(
+    _RequiredSearchUsersByImageRequestRequestTypeDef,
+    _OptionalSearchUsersByImageRequestRequestTypeDef,
+):
+    pass
 
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "F1Score": float,
         "Summary": SummaryTypeDef,
     },
@@ -2664,22 +2801,20 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartCelebrityRecognitionRequestRequestTypeDef(
     _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
     _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartContentModerationRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
@@ -2689,22 +2824,20 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartContentModerationRequestRequestTypeDef(
     _RequiredStartContentModerationRequestRequestTypeDef,
     _OptionalStartContentModerationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -2714,22 +2847,20 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "FaceAttributes": FaceAttributesType,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartFaceDetectionRequestRequestTypeDef(
     _RequiredStartFaceDetectionRequestRequestTypeDef,
     _OptionalStartFaceDetectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceSearchRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "CollectionId": str,
     },
 )
@@ -2740,70 +2871,347 @@
         "FaceMatchThreshold": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+CelebrityTypeDef = TypedDict(
+    "CelebrityTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Face": ComparedFaceTypeDef,
+        "MatchConfidence": float,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+CompareFacesMatchTypeDef = TypedDict(
+    "CompareFacesMatchTypeDef",
+    {
+        "Similarity": float,
+        "Face": ComparedFaceTypeDef,
+    },
+    total=False,
+)
+
+GetContentModerationResponseTypeDef = TypedDict(
+    "GetContentModerationResponseTypeDef",
+    {
+        "JobStatus": VideoJobStatusType,
+        "StatusMessage": str,
+        "VideoMetadata": VideoMetadataTypeDef,
+        "ModerationLabels": List[ContentModerationDetectionTypeDef],
+        "NextToken": str,
+        "ModerationModelVersion": str,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProtectiveEquipmentBodyPartTypeDef = TypedDict(
+    "ProtectiveEquipmentBodyPartTypeDef",
+    {
+        "Name": BodyPartType,
+        "Confidence": float,
+        "EquipmentDetections": List[EquipmentDetectionTypeDef],
+    },
+    total=False,
+)
+
+CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
+    {
+        "KmsKeyId": str,
+        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetDescription": DatasetDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDatasetLabelsResponseTypeDef = TypedDict(
+    "ListDatasetLabelsResponseTypeDef",
+    {
+        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeProjectsResponseTypeDef = TypedDict(
+    "DescribeProjectsResponseTypeDef",
+    {
+        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DetectLabelsImagePropertiesTypeDef = TypedDict(
+    "DetectLabelsImagePropertiesTypeDef",
+    {
+        "Quality": DetectLabelsImageQualityTypeDef,
+        "DominantColors": List[DominantColorTypeDef],
+        "Foreground": DetectLabelsImageForegroundTypeDef,
+        "Background": DetectLabelsImageBackgroundTypeDef,
+    },
+    total=False,
+)
+
+LabelTypeDef = TypedDict(
+    "LabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Instances": List[InstanceTypeDef],
+        "Parents": List[ParentTypeDef],
+        "Aliases": List[LabelAliasTypeDef],
+        "Categories": List[LabelCategoryTypeDef],
+    },
+    total=False,
+)
+
+_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectLabelsRequestRequestTypeDef",
+    {
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectLabelsRequestRequestTypeDef",
+    {
+        "MaxLabels": int,
+        "MinConfidence": float,
+        "Features": Sequence[DetectLabelsFeatureNameType],
+        "Settings": DetectLabelsSettingsTypeDef,
+    },
+    total=False,
+)
+
+class DetectLabelsRequestRequestTypeDef(
+    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
+):
+    pass
 
 _RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
+        "Features": Sequence[Literal["GENERAL_LABELS"]],
+        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
     _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
+CelebrityDetailTypeDef = TypedDict(
+    "CelebrityDetailTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Confidence": float,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+DetectFacesResponseTypeDef = TypedDict(
+    "DetectFacesResponseTypeDef",
+    {
+        "FaceDetails": List[FaceDetailTypeDef],
+        "OrientationCorrection": OrientationCorrectionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+FaceDetectionTypeDef = TypedDict(
+    "FaceDetectionTypeDef",
     {
-        "Video": VideoTypeDef,
+        "Timestamp": int,
+        "Face": FaceDetailTypeDef,
     },
+    total=False,
 )
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+
+FaceRecordTypeDef = TypedDict(
+    "FaceRecordTypeDef",
     {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
+        "Face": FaceTypeDef,
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+PersonDetailTypeDef = TypedDict(
+    "PersonDetailTypeDef",
+    {
+        "Index": int,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
     },
     total=False,
 )
 
+SearchedFaceDetailsTypeDef = TypedDict(
+    "SearchedFaceDetailsTypeDef",
+    {
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
 
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
+UnindexedFaceTypeDef = TypedDict(
+    "UnindexedFaceTypeDef",
+    {
+        "Reasons": List[ReasonType],
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnsearchedFaceTypeDef = TypedDict(
+    "UnsearchedFaceTypeDef",
+    {
+        "FaceDetails": FaceDetailTypeDef,
+        "Reasons": List[UnsearchedFaceReasonType],
+    },
+    total=False,
+)
+
+CustomLabelTypeDef = TypedDict(
+    "CustomLabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+TextDetectionTypeDef = TypedDict(
+    "TextDetectionTypeDef",
+    {
+        "DetectedText": str,
+        "Type": TextTypesType,
+        "Id": int,
+        "ParentId": int,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+DetectTextFiltersTypeDef = TypedDict(
+    "DetectTextFiltersTypeDef",
+    {
+        "WordFilter": DetectionFilterTypeDef,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+    },
+    total=False,
+)
+
+StartTextDetectionFiltersTypeDef = TypedDict(
+    "StartTextDetectionFiltersTypeDef",
+    {
+        "WordFilter": DetectionFilterTypeDef,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+    },
+    total=False,
+)
+
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -2811,22 +3219,20 @@
     {
         "MinConfidence": float,
         "HumanLoopConfig": HumanLoopConfigTypeDef,
     },
     total=False,
 )
 
-
 class DetectModerationLabelsRequestRequestTypeDef(
     _RequiredDetectModerationLabelsRequestRequestTypeDef,
     _OptionalDetectModerationLabelsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredStartStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
@@ -2834,21 +3240,30 @@
     {
         "StartSelector": StreamProcessingStartSelectorTypeDef,
         "StopSelector": StreamProcessingStopSelectorTypeDef,
     },
     total=False,
 )
 
-
 class StartStreamProcessorRequestRequestTypeDef(
     _RequiredStartStreamProcessorRequestRequestTypeDef,
     _OptionalStartStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
+    {
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceTypeDef,
+        "SearchedUser": SearchedUserTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamProcessorRequestRequestTypeDef",
     {
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "Name": str,
@@ -2864,22 +3279,20 @@
         "KmsKeyId": str,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
     },
     total=False,
 )
 
-
 class CreateStreamProcessorRequestRequestTypeDef(
     _RequiredCreateStreamProcessorRequestRequestTypeDef,
     _OptionalCreateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
@@ -2889,32 +3302,101 @@
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
         "Settings": StreamProcessorSettingsTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
         "RegionsOfInterest": List[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": List[VideoMetadataTypeDef],
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchFacesByImageResponseTypeDef = TypedDict(
+    "SearchFacesByImageResponseTypeDef",
+    {
+        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
+        "SearchedFaceConfidence": float,
+        "FaceMatches": List[FaceMatchTypeDef],
+        "FaceModelVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchFacesResponseTypeDef = TypedDict(
+    "SearchFacesResponseTypeDef",
+    {
+        "SearchedFaceId": str,
+        "FaceMatches": List[FaceMatchTypeDef],
+        "FaceModelVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TestingDataTypeDef = TypedDict(
+    "TestingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+        "AutoCreate": bool,
+    },
+    total=False,
+)
+
+TrainingDataTypeDef = TypedDict(
+    "TrainingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+    },
+    total=False,
+)
+
+ValidationDataTypeDef = TypedDict(
+    "ValidationDataTypeDef",
+    {
+        "Assets": List[AssetTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "ProjectArn": str,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetSource": DatasetSourceTypeDef,
     },
+    total=False,
 )
 
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -2925,62 +3407,39 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartSegmentDetectionFiltersTypeDef,
     },
     total=False,
 )
 
-
 class StartSegmentDetectionRequestRequestTypeDef(
     _RequiredStartSegmentDetectionRequestRequestTypeDef,
     _OptionalStartSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
-
-SearchFacesByImageResponseTypeDef = TypedDict(
-    "SearchFacesByImageResponseTypeDef",
-    {
-        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
-        "SearchedFaceConfidence": float,
-        "FaceMatches": List[FaceMatchTypeDef],
-        "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchFacesResponseTypeDef = TypedDict(
-    "SearchFacesResponseTypeDef",
-    {
-        "SearchedFaceId": str,
-        "FaceMatches": List[FaceMatchTypeDef],
-        "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompareFacesResponseTypeDef = TypedDict(
     "CompareFacesResponseTypeDef",
     {
         "SourceImageFace": ComparedSourceImageFaceTypeDef,
         "FaceMatches": List[CompareFacesMatchTypeDef],
         "UnmatchedFaces": List[ComparedFaceTypeDef],
         "SourceImageOrientationCorrection": OrientationCorrectionType,
         "TargetImageOrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
@@ -2994,23 +3453,26 @@
 DetectLabelsResponseTypeDef = TypedDict(
     "DetectLabelsResponseTypeDef",
     {
         "Labels": List[LabelTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "LabelModelVersion": str,
         "ImageProperties": DetectLabelsImagePropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
         "Label": LabelTypeDef,
+        "StartTimestampMillis": int,
+        "EndTimestampMillis": int,
+        "DurationMillis": int,
     },
     total=False,
 )
 
 CelebrityRecognitionTypeDef = TypedDict(
     "CelebrityRecognitionTypeDef",
     {
@@ -3024,15 +3486,18 @@
     "GetFaceDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3054,32 +3519,43 @@
 IndexFacesResponseTypeDef = TypedDict(
     "IndexFacesResponseTypeDef",
     {
         "FaceRecords": List[FaceRecordTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "FaceModelVersion": str,
         "UnindexedFaces": List[UnindexedFaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchUsersByImageResponseTypeDef = TypedDict(
+    "SearchUsersByImageResponseTypeDef",
+    {
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceDetailsTypeDef,
+        "UnsearchedFaces": List[UnsearchedFaceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectCustomLabelsResponseTypeDef = TypedDict(
     "DetectCustomLabelsResponseTypeDef",
     {
         "CustomLabels": List[CustomLabelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectTextResponseTypeDef = TypedDict(
     "DetectTextResponseTypeDef",
     {
         "TextDetections": List[TextDetectionTypeDef],
         "TextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TextDetectionResultTypeDef = TypedDict(
     "TextDetectionResultTypeDef",
     {
         "Timestamp": int,
@@ -3098,21 +3574,19 @@
     "_OptionalDetectTextRequestRequestTypeDef",
     {
         "Filters": DetectTextFiltersTypeDef,
     },
     total=False,
 )
 
-
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3122,186 +3596,151 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartTextDetectionFiltersTypeDef,
     },
     total=False,
 )
 
-
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
-
-TestingDataTypeDef = TypedDict(
-    "TestingDataTypeDef",
+_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
-        "AutoCreate": bool,
+        "ProjectArn": str,
+        "VersionName": str,
+        "OutputConfig": OutputConfigTypeDef,
     },
-    total=False,
 )
-
-TrainingDataTypeDef = TypedDict(
-    "TrainingDataTypeDef",
+_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectVersionRequestRequestTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
+        "TrainingData": TrainingDataTypeDef,
+        "TestingData": TestingDataTypeDef,
+        "Tags": Mapping[str, str],
+        "KmsKeyId": str,
     },
     total=False,
 )
 
-ValidationDataTypeDef = TypedDict(
-    "ValidationDataTypeDef",
+class CreateProjectVersionRequestRequestTypeDef(
+    _RequiredCreateProjectVersionRequestRequestTypeDef,
+    _OptionalCreateProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+TestingDataResultTypeDef = TypedDict(
+    "TestingDataResultTypeDef",
     {
-        "Assets": List[AssetTypeDef],
+        "Input": TestingDataTypeDef,
+        "Output": TestingDataTypeDef,
+        "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "ProjectArn": str,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
+TrainingDataResultTypeDef = TypedDict(
+    "TrainingDataResultTypeDef",
     {
-        "DatasetSource": DatasetSourceTypeDef,
+        "Input": TrainingDataTypeDef,
+        "Output": TrainingDataTypeDef,
+        "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
     {
         "ProtectiveEquipmentModelVersion": str,
         "Persons": List[ProtectiveEquipmentPersonTypeDef],
         "Summary": ProtectiveEquipmentSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLabelDetectionResponseTypeDef = TypedDict(
     "GetLabelDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
     "GetCelebrityRecognitionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectArn": str,
-        "VersionName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectVersionRequestRequestTypeDef",
-    {
-        "TrainingData": TrainingDataTypeDef,
-        "TestingData": TestingDataTypeDef,
-        "Tags": Mapping[str, str],
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class CreateProjectVersionRequestRequestTypeDef(
-    _RequiredCreateProjectVersionRequestRequestTypeDef,
-    _OptionalCreateProjectVersionRequestRequestTypeDef,
-):
-    pass
-
-
-TestingDataResultTypeDef = TypedDict(
-    "TestingDataResultTypeDef",
-    {
-        "Input": TestingDataTypeDef,
-        "Output": TestingDataTypeDef,
-        "Validation": ValidationDataTypeDef,
-    },
-    total=False,
-)
-
-TrainingDataResultTypeDef = TypedDict(
-    "TrainingDataResultTypeDef",
-    {
-        "Input": TrainingDataTypeDef,
-        "Output": TrainingDataTypeDef,
-        "Validation": ValidationDataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
         "CreationTimestamp": datetime,
@@ -3323,10 +3762,10 @@
 )
 
 DescribeProjectVersionsResponseTypeDef = TypedDict(
     "DescribeProjectVersionsResponseTypeDef",
     {
         "ProjectVersionDescriptions": List[ProjectVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,315 +18,429 @@
 from botocore.response import StreamingBody
 
 from .literals import (
     AttributeType,
     BodyPartType,
     CelebrityRecognitionSortByType,
     ContentClassifierType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetStatusMessageCodeType,
     DatasetStatusType,
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
+    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     LandmarkTypeType,
+    LivenessSessionStatusType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionStatusType,
     ProtectiveEquipmentTypeType,
     QualityFilterType,
     ReasonType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
     StreamProcessorStatusType,
     TechnicalCueTypeType,
     TextTypesType,
+    UnsearchedFaceReasonType,
+    UnsuccessfulFaceAssociationReasonType,
+    UnsuccessfulFaceDeletionReasonType,
+    UnsuccessfulFaceDisassociationReasonType,
+    UserStatusType,
     VideoColorRangeType,
     VideoJobStatusType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AgeRangeTypeDef",
+    "AssociateFacesRequestRequestTypeDef",
+    "AssociatedFaceTypeDef",
+    "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
+    "BoundingBoxTypeDef",
+    "S3ObjectTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
-    "BoundingBoxTypeDef",
     "KnownGenderTypeDef",
-    "ResponseMetadataTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
+    "CopyProjectVersionResponseTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
+    "CreateCollectionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "LivenessOutputConfigTypeDef",
+    "CreateFaceLivenessSessionResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateProjectVersionResponseTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
+    "CreateStreamProcessorResponseTypeDef",
+    "CreateUserRequestRequestTypeDef",
     "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
+    "DeleteCollectionResponseTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
+    "UnsuccessfulFaceDeletionTypeDef",
     "DeleteProjectPolicyRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResponseTypeDef",
     "DeleteProjectVersionRequestRequestTypeDef",
+    "DeleteProjectVersionResponseTypeDef",
     "DeleteStreamProcessorRequestRequestTypeDef",
+    "DeleteUserRequestRequestTypeDef",
     "DescribeCollectionRequestRequestTypeDef",
+    "DescribeCollectionResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ProtectiveEquipmentSummarizationAttributesTypeDef",
     "ProtectiveEquipmentSummaryTypeDef",
     "DetectionFilterTypeDef",
+    "DisassociateFacesRequestRequestTypeDef",
+    "DisassociatedFaceTypeDef",
+    "UnsuccessfulFaceDisassociationTypeDef",
     "DistributeDatasetTypeDef",
+    "EyeDirectionTypeDef",
     "EyeOpenTypeDef",
     "EyeglassesTypeDef",
+    "FaceOccludedTypeDef",
     "GenderTypeDef",
     "MouthOpenTypeDef",
     "MustacheTypeDef",
     "SunglassesTypeDef",
     "FaceSearchSettingsTypeDef",
     "PointTypeDef",
     "GetCelebrityInfoRequestRequestTypeDef",
     "GetCelebrityRecognitionRequestRequestTypeDef",
     "VideoMetadataTypeDef",
+    "GetContentModerationRequestMetadataTypeDef",
     "GetContentModerationRequestRequestTypeDef",
     "GetFaceDetectionRequestRequestTypeDef",
+    "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     "GetFaceSearchRequestRequestTypeDef",
+    "GetLabelDetectionRequestMetadataTypeDef",
     "GetLabelDetectionRequestRequestTypeDef",
     "GetPersonTrackingRequestRequestTypeDef",
     "GetSegmentDetectionRequestRequestTypeDef",
     "SegmentTypeInfoTypeDef",
     "GetTextDetectionRequestRequestTypeDef",
-    "S3ObjectTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
     "ListCollectionsRequestRequestTypeDef",
+    "ListCollectionsResponseTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     "ListDatasetLabelsRequestRequestTypeDef",
+    "ListFacesRequestListFacesPaginateTypeDef",
     "ListFacesRequestRequestTypeDef",
+    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     "ListProjectPoliciesRequestRequestTypeDef",
     "ProjectPolicyTypeDef",
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListUsersRequestRequestTypeDef",
+    "UserTypeDef",
+    "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
+    "PaginatorConfigTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
+    "PutProjectPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
+    "SearchUsersRequestRequestTypeDef",
+    "SearchedFaceTypeDef",
+    "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
     "TechnicalCueSegmentTypeDef",
-    "StartProjectVersionRequestRequestTypeDef",
-    "StartShotDetectionFilterTypeDef",
-    "StreamProcessingStopSelectorTypeDef",
-    "StopProjectVersionRequestRequestTypeDef",
-    "StopStreamProcessorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "StartTechnicalCueDetectionFilterTypeDef",
-    "ComparedSourceImageFaceTypeDef",
-    "FaceTypeDef",
-    "CopyProjectVersionResponseTypeDef",
-    "CreateCollectionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateProjectVersionResponseTypeDef",
-    "CreateStreamProcessorResponseTypeDef",
-    "DeleteCollectionResponseTypeDef",
-    "DeleteFacesResponseTypeDef",
-    "DeleteProjectResponseTypeDef",
-    "DeleteProjectVersionResponseTypeDef",
-    "DescribeCollectionResponseTypeDef",
-    "GetCelebrityInfoResponseTypeDef",
-    "ListCollectionsResponseTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutProjectPolicyResponseTypeDef",
     "StartCelebrityRecognitionResponseTypeDef",
     "StartContentModerationResponseTypeDef",
     "StartFaceDetectionResponseTypeDef",
     "StartFaceSearchResponseTypeDef",
     "StartLabelDetectionResponseTypeDef",
     "StartPersonTrackingResponseTypeDef",
+    "StartProjectVersionRequestRequestTypeDef",
     "StartProjectVersionResponseTypeDef",
+    "StartShotDetectionFilterTypeDef",
     "StartSegmentDetectionResponseTypeDef",
+    "StreamProcessingStopSelectorTypeDef",
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
+    "StopProjectVersionRequestRequestTypeDef",
     "StopProjectVersionResponseTypeDef",
+    "StopStreamProcessorRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "AssociateFacesResponseTypeDef",
+    "ComparedSourceImageFaceTypeDef",
+    "FaceTypeDef",
+    "AuditImageTypeDef",
+    "GroundTruthManifestTypeDef",
+    "ImageTypeDef",
+    "SummaryTypeDef",
+    "VideoTypeDef",
+    "StartTechnicalCueDetectionFilterTypeDef",
+    "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
+    "CreateFaceLivenessSessionRequestSettingsTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
-    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    "ListFacesRequestListFacesPaginateTypeDef",
-    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    "DeleteFacesResponseTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
+    "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
+    "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
     "RegionOfInterestTypeDef",
-    "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
-    "SummaryTypeDef",
-    "VideoTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "UserMatchTypeDef",
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
-    "StartSegmentDetectionFiltersTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
+    "GetFaceLivenessSessionResultsResponseTypeDef",
+    "AssetTypeDef",
+    "DatasetSourceTypeDef",
+    "CompareFacesRequestRequestTypeDef",
+    "DetectCustomLabelsRequestRequestTypeDef",
+    "DetectFacesRequestRequestTypeDef",
+    "DetectProtectiveEquipmentRequestRequestTypeDef",
+    "IndexFacesRequestRequestTypeDef",
+    "RecognizeCelebritiesRequestRequestTypeDef",
+    "SearchFacesByImageRequestRequestTypeDef",
+    "SearchUsersByImageRequestRequestTypeDef",
+    "EvaluationResultTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
+    "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
     "DescribeProjectsResponseTypeDef",
     "DetectLabelsImagePropertiesTypeDef",
     "LabelTypeDef",
+    "DetectLabelsRequestRequestTypeDef",
+    "StartLabelDetectionRequestRequestTypeDef",
     "CelebrityDetailTypeDef",
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
+    "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
+    "UnsearchedFaceTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
     "StartTextDetectionFiltersTypeDef",
     "UpdateStreamProcessorRequestRequestTypeDef",
-    "AssetTypeDef",
-    "DatasetSourceTypeDef",
-    "CompareFacesRequestRequestTypeDef",
-    "DetectCustomLabelsRequestRequestTypeDef",
-    "DetectFacesRequestRequestTypeDef",
-    "DetectLabelsRequestRequestTypeDef",
-    "DetectProtectiveEquipmentRequestRequestTypeDef",
-    "IndexFacesRequestRequestTypeDef",
-    "RecognizeCelebritiesRequestRequestTypeDef",
-    "SearchFacesByImageRequestRequestTypeDef",
-    "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartLabelDetectionRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
+    "SearchUsersResponseTypeDef",
     "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
-    "StartSegmentDetectionRequestRequestTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
+    "TestingDataTypeDef",
+    "TrainingDataTypeDef",
+    "ValidationDataTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
     "DetectLabelsResponseTypeDef",
     "LabelDetectionTypeDef",
     "CelebrityRecognitionTypeDef",
     "GetFaceDetectionResponseTypeDef",
     "PersonDetectionTypeDef",
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
+    "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "TestingDataTypeDef",
-    "TrainingDataTypeDef",
-    "ValidationDataTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
+    "CreateProjectVersionRequestRequestTypeDef",
+    "TestingDataResultTypeDef",
+    "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
     "GetTextDetectionResponseTypeDef",
-    "CreateProjectVersionRequestRequestTypeDef",
-    "TestingDataResultTypeDef",
-    "TrainingDataResultTypeDef",
     "ProjectVersionDescriptionTypeDef",
     "DescribeProjectVersionsResponseTypeDef",
 )
 
 AgeRangeTypeDef = TypedDict(
     "AgeRangeTypeDef",
     {
         "Low": int,
         "High": int,
     },
     total=False,
 )
 
+_RequiredAssociateFacesRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateFacesRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+        "FaceIds": Sequence[str],
+    },
+)
+_OptionalAssociateFacesRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateFacesRequestRequestTypeDef",
+    {
+        "UserMatchThreshold": float,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class AssociateFacesRequestRequestTypeDef(
+    _RequiredAssociateFacesRequestRequestTypeDef, _OptionalAssociateFacesRequestRequestTypeDef
+):
+    pass
+
+
+AssociatedFaceTypeDef = TypedDict(
+    "AssociatedFaceTypeDef",
+    {
+        "FaceId": str,
+    },
+    total=False,
+)
+
+UnsuccessfulFaceAssociationTypeDef = TypedDict(
+    "UnsuccessfulFaceAssociationTypeDef",
+    {
+        "FaceId": str,
+        "UserId": str,
+        "Confidence": float,
+        "Reasons": List[UnsuccessfulFaceAssociationReasonType],
+    },
+    total=False,
+)
+
 AudioMetadataTypeDef = TypedDict(
     "AudioMetadataTypeDef",
     {
         "Codec": str,
         "DurationMillis": int,
         "SampleRate": int,
         "NumberOfChannels": int,
     },
     total=False,
 )
 
+BoundingBoxTypeDef = TypedDict(
+    "BoundingBoxTypeDef",
+    {
+        "Width": float,
+        "Height": float,
+        "Left": float,
+        "Top": float,
+    },
+    total=False,
+)
+
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
+    {
+        "Bucket": str,
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 BeardTypeDef = TypedDict(
     "BeardTypeDef",
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
@@ -337,44 +451,22 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
-BoundingBoxTypeDef = TypedDict(
-    "BoundingBoxTypeDef",
-    {
-        "Width": float,
-        "Height": float,
-        "Left": float,
-        "Top": float,
-    },
-    total=False,
-)
-
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
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
 EmotionTypeDef = TypedDict(
     "EmotionTypeDef",
     {
         "Type": EmotionNameType,
         "Confidence": float,
     },
     total=False,
@@ -437,19 +529,21 @@
     "_OptionalConnectedHomeSettingsTypeDef",
     {
         "MinConfidence": float,
     },
     total=False,
 )
 
+
 class ConnectedHomeSettingsTypeDef(
     _RequiredConnectedHomeSettingsTypeDef, _OptionalConnectedHomeSettingsTypeDef
 ):
     pass
 
+
 ModerationLabelTypeDef = TypedDict(
     "ModerationLabelTypeDef",
     {
         "Confidence": float,
         "Name": str,
         "ParentName": str,
     },
@@ -461,14 +555,22 @@
     {
         "S3Bucket": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+CopyProjectVersionResponseTypeDef = TypedDict(
+    "CopyProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CoversBodyPartTypeDef = TypedDict(
     "CoversBodyPartTypeDef",
     {
         "Confidence": float,
         "Value": bool,
     },
     total=False,
@@ -484,40 +586,135 @@
     "_OptionalCreateCollectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
+
+CreateCollectionResponseTypeDef = TypedDict(
+    "CreateCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "CollectionArn": str,
+        "FaceModelVersion": str,
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
+_RequiredLivenessOutputConfigTypeDef = TypedDict(
+    "_RequiredLivenessOutputConfigTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalLivenessOutputConfigTypeDef = TypedDict(
+    "_OptionalLivenessOutputConfigTypeDef",
+    {
+        "S3KeyPrefix": str,
+    },
+    total=False,
+)
+
+
+class LivenessOutputConfigTypeDef(
+    _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
+):
+    pass
+
+
+CreateFaceLivenessSessionResponseTypeDef = TypedDict(
+    "CreateFaceLivenessSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProjectVersionResponseTypeDef = TypedDict(
+    "CreateProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StreamProcessorDataSharingPreferenceTypeDef = TypedDict(
     "StreamProcessorDataSharingPreferenceTypeDef",
     {
         "OptIn": bool,
     },
 )
 
 StreamProcessorNotificationChannelTypeDef = TypedDict(
     "StreamProcessorNotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
     },
 )
 
+CreateStreamProcessorResponseTypeDef = TypedDict(
+    "CreateStreamProcessorResponseTypeDef",
+    {
+        "StreamProcessorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateUserRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+    },
+)
+_OptionalCreateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateUserRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class CreateUserRequestRequestTypeDef(
+    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
+):
+    pass
+
+
 DatasetChangesTypeDef = TypedDict(
     "DatasetChangesTypeDef",
     {
         "GroundTruth": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
@@ -557,14 +754,22 @@
 DeleteCollectionRequestRequestTypeDef = TypedDict(
     "DeleteCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
+DeleteCollectionResponseTypeDef = TypedDict(
+    "DeleteCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -572,14 +777,24 @@
     "DeleteFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
         "FaceIds": Sequence[str],
     },
 )
 
+UnsuccessfulFaceDeletionTypeDef = TypedDict(
+    "UnsuccessfulFaceDeletionTypeDef",
+    {
+        "FaceId": str,
+        "UserId": str,
+        "Reasons": List[UnsuccessfulFaceDeletionReasonType],
+    },
+    total=False,
+)
+
 _RequiredDeleteProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
     },
 )
@@ -587,65 +802,130 @@
     "_OptionalDeleteProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteProjectPolicyRequestRequestTypeDef(
     _RequiredDeleteProjectPolicyRequestRequestTypeDef,
     _OptionalDeleteProjectPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Status": ProjectStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProjectVersionRequestRequestTypeDef = TypedDict(
     "DeleteProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
     },
 )
 
+DeleteProjectVersionResponseTypeDef = TypedDict(
+    "DeleteProjectVersionResponseTypeDef",
+    {
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteStreamProcessorRequestRequestTypeDef = TypedDict(
     "DeleteStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredDeleteUserRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteUserRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+    },
+)
+_OptionalDeleteUserRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteUserRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class DeleteUserRequestRequestTypeDef(
+    _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
+):
+    pass
+
+
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
+DescribeCollectionResponseTypeDef = TypedDict(
+    "DescribeCollectionResponseTypeDef",
+    {
+        "FaceCount": int,
+        "FaceModelVersion": str,
+        "CollectionARN": str,
+        "CreationTimestamp": datetime,
+        "UserCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProjectArn": str,
+    },
+)
+_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "VersionNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
+    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+):
+    pass
+
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -663,20 +943,31 @@
         "VersionNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    {
+        "ProjectNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -767,21 +1058,72 @@
         "MinConfidence": float,
         "MinBoundingBoxHeight": float,
         "MinBoundingBoxWidth": float,
     },
     total=False,
 )
 
+_RequiredDisassociateFacesRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateFacesRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "UserId": str,
+        "FaceIds": Sequence[str],
+    },
+)
+_OptionalDisassociateFacesRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateFacesRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class DisassociateFacesRequestRequestTypeDef(
+    _RequiredDisassociateFacesRequestRequestTypeDef, _OptionalDisassociateFacesRequestRequestTypeDef
+):
+    pass
+
+
+DisassociatedFaceTypeDef = TypedDict(
+    "DisassociatedFaceTypeDef",
+    {
+        "FaceId": str,
+    },
+    total=False,
+)
+
+UnsuccessfulFaceDisassociationTypeDef = TypedDict(
+    "UnsuccessfulFaceDisassociationTypeDef",
+    {
+        "FaceId": str,
+        "UserId": str,
+        "Reasons": List[UnsuccessfulFaceDisassociationReasonType],
+    },
+    total=False,
+)
+
 DistributeDatasetTypeDef = TypedDict(
     "DistributeDatasetTypeDef",
     {
         "Arn": str,
     },
 )
 
+EyeDirectionTypeDef = TypedDict(
+    "EyeDirectionTypeDef",
+    {
+        "Yaw": float,
+        "Pitch": float,
+        "Confidence": float,
+    },
+    total=False,
+)
+
 EyeOpenTypeDef = TypedDict(
     "EyeOpenTypeDef",
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
@@ -792,14 +1134,23 @@
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
 )
 
+FaceOccludedTypeDef = TypedDict(
+    "FaceOccludedTypeDef",
+    {
+        "Value": bool,
+        "Confidence": float,
+    },
+    total=False,
+)
+
 GenderTypeDef = TypedDict(
     "GenderTypeDef",
     {
         "Value": GenderTypeType,
         "Confidence": float,
     },
     total=False,
@@ -869,56 +1220,70 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": CelebrityRecognitionSortByType,
     },
     total=False,
 )
 
+
 class GetCelebrityRecognitionRequestRequestTypeDef(
     _RequiredGetCelebrityRecognitionRequestRequestTypeDef,
     _OptionalGetCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
+
 VideoMetadataTypeDef = TypedDict(
     "VideoMetadataTypeDef",
     {
         "Codec": str,
         "DurationMillis": int,
         "Format": str,
         "FrameRate": float,
         "FrameHeight": int,
         "FrameWidth": int,
         "ColorRange": VideoColorRangeType,
     },
     total=False,
 )
 
+GetContentModerationRequestMetadataTypeDef = TypedDict(
+    "GetContentModerationRequestMetadataTypeDef",
+    {
+        "SortBy": ContentModerationSortByType,
+        "AggregateBy": ContentModerationAggregateByType,
+    },
+    total=False,
+)
+
 _RequiredGetContentModerationRequestRequestTypeDef = TypedDict(
     "_RequiredGetContentModerationRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetContentModerationRequestRequestTypeDef = TypedDict(
     "_OptionalGetContentModerationRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": ContentModerationSortByType,
+        "AggregateBy": ContentModerationAggregateByType,
     },
     total=False,
 )
 
+
 class GetContentModerationRequestRequestTypeDef(
     _RequiredGetContentModerationRequestRequestTypeDef,
     _OptionalGetContentModerationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFaceDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -926,19 +1291,28 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetFaceDetectionRequestRequestTypeDef(
     _RequiredGetFaceDetectionRequestRequestTypeDef, _OptionalGetFaceDetectionRequestRequestTypeDef
 ):
     pass
 
+
+GetFaceLivenessSessionResultsRequestRequestTypeDef = TypedDict(
+    "GetFaceLivenessSessionResultsRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
 _RequiredGetFaceSearchRequestRequestTypeDef = TypedDict(
     "_RequiredGetFaceSearchRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetFaceSearchRequestRequestTypeDef = TypedDict(
@@ -947,40 +1321,54 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": FaceSearchSortByType,
     },
     total=False,
 )
 
+
 class GetFaceSearchRequestRequestTypeDef(
     _RequiredGetFaceSearchRequestRequestTypeDef, _OptionalGetFaceSearchRequestRequestTypeDef
 ):
     pass
 
+
+GetLabelDetectionRequestMetadataTypeDef = TypedDict(
+    "GetLabelDetectionRequestMetadataTypeDef",
+    {
+        "SortBy": LabelDetectionSortByType,
+        "AggregateBy": LabelDetectionAggregateByType,
+    },
+    total=False,
+)
+
 _RequiredGetLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetLabelDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetLabelDetectionRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": LabelDetectionSortByType,
+        "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
 )
 
+
 class GetLabelDetectionRequestRequestTypeDef(
     _RequiredGetLabelDetectionRequestRequestTypeDef, _OptionalGetLabelDetectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPersonTrackingRequestRequestTypeDef = TypedDict(
     "_RequiredGetPersonTrackingRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetPersonTrackingRequestRequestTypeDef = TypedDict(
@@ -989,19 +1377,21 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": PersonTrackingSortByType,
     },
     total=False,
 )
 
+
 class GetPersonTrackingRequestRequestTypeDef(
     _RequiredGetPersonTrackingRequestRequestTypeDef, _OptionalGetPersonTrackingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetSegmentDetectionRequestRequestTypeDef = TypedDict(
@@ -1009,20 +1399,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetSegmentDetectionRequestRequestTypeDef(
     _RequiredGetSegmentDetectionRequestRequestTypeDef,
     _OptionalGetSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
+
 SegmentTypeInfoTypeDef = TypedDict(
     "SegmentTypeInfoTypeDef",
     {
         "Type": SegmentTypeType,
         "ModelVersion": str,
     },
     total=False,
@@ -1039,28 +1431,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
-    {
-        "Bucket": str,
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
 
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
@@ -1111,23 +1495,67 @@
     "ParentTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListCollectionsResponseTypeDef = TypedDict(
+    "ListCollectionsResponseTypeDef",
+    {
+        "CollectionIds": List[str],
+        "NextToken": str,
+        "FaceModelVersions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ContainsLabels": Sequence[str],
+        "Labeled": bool,
+        "SourceRefContains": str,
+        "HasErrors": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
@@ -1139,20 +1567,53 @@
         "HasErrors": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
+    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1160,39 +1621,91 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_RequiredListFacesRequestListFacesPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_OptionalListFacesRequestListFacesPaginateTypeDef",
+    {
+        "UserId": str,
+        "FaceIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFacesRequestListFacesPaginateTypeDef(
+    _RequiredListFacesRequestListFacesPaginateTypeDef,
+    _OptionalListFacesRequestListFacesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
     "_OptionalListFacesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
+        "UserId": str,
+        "FaceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
+    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1200,33 +1713,43 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListProjectPoliciesRequestRequestTypeDef(
     _RequiredListProjectPoliciesRequestRequestTypeDef,
     _OptionalListProjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 ProjectPolicyTypeDef = TypedDict(
     "ProjectPolicyTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyRevisionId": str,
         "PolicyDocument": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStreamProcessorsRequestRequestTypeDef = TypedDict(
     "ListStreamProcessorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1244,22 +1767,102 @@
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
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
+):
+    pass
+
+
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "UserId": str,
+        "UserStatus": UserStatusType,
+    },
+    total=False,
+)
+
+MatchedUserTypeDef = TypedDict(
+    "MatchedUserTypeDef",
+    {
+        "UserId": str,
+        "UserStatus": UserStatusType,
+    },
+    total=False,
+)
+
 NotificationChannelTypeDef = TypedDict(
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
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
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyDocument": str,
     },
@@ -1268,19 +1871,40 @@
     "_OptionalPutProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
+
+PutProjectPolicyResponseTypeDef = TypedDict(
+    "PutProjectPolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1298,358 +1922,328 @@
     {
         "MaxFaces": int,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
+
 class SearchFacesRequestRequestTypeDef(
     _RequiredSearchFacesRequestRequestTypeDef, _OptionalSearchFacesRequestRequestTypeDef
 ):
     pass
 
-ShotSegmentTypeDef = TypedDict(
-    "ShotSegmentTypeDef",
-    {
-        "Index": int,
-        "Confidence": float,
-    },
-    total=False,
-)
-
-TechnicalCueSegmentTypeDef = TypedDict(
-    "TechnicalCueSegmentTypeDef",
-    {
-        "Type": TechnicalCueTypeType,
-        "Confidence": float,
-    },
-    total=False,
-)
 
-_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartProjectVersionRequestRequestTypeDef",
+_RequiredSearchUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchUsersRequestRequestTypeDef",
     {
-        "ProjectVersionArn": str,
-        "MinInferenceUnits": int,
+        "CollectionId": str,
     },
 )
-_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartProjectVersionRequestRequestTypeDef",
+_OptionalSearchUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchUsersRequestRequestTypeDef",
     {
-        "MaxInferenceUnits": int,
+        "UserId": str,
+        "FaceId": str,
+        "UserMatchThreshold": float,
+        "MaxUsers": int,
     },
     total=False,
 )
 
-class StartProjectVersionRequestRequestTypeDef(
-    _RequiredStartProjectVersionRequestRequestTypeDef,
-    _OptionalStartProjectVersionRequestRequestTypeDef,
+
+class SearchUsersRequestRequestTypeDef(
+    _RequiredSearchUsersRequestRequestTypeDef, _OptionalSearchUsersRequestRequestTypeDef
 ):
     pass
 
-StartShotDetectionFilterTypeDef = TypedDict(
-    "StartShotDetectionFilterTypeDef",
+
+SearchedFaceTypeDef = TypedDict(
+    "SearchedFaceTypeDef",
     {
-        "MinSegmentConfidence": float,
+        "FaceId": str,
     },
     total=False,
 )
 
-StreamProcessingStopSelectorTypeDef = TypedDict(
-    "StreamProcessingStopSelectorTypeDef",
+SearchedUserTypeDef = TypedDict(
+    "SearchedUserTypeDef",
     {
-        "MaxDurationInSeconds": int,
+        "UserId": str,
     },
     total=False,
 )
 
-StopProjectVersionRequestRequestTypeDef = TypedDict(
-    "StopProjectVersionRequestRequestTypeDef",
+ShotSegmentTypeDef = TypedDict(
+    "ShotSegmentTypeDef",
     {
-        "ProjectVersionArn": str,
+        "Index": int,
+        "Confidence": float,
     },
+    total=False,
 )
 
-StopStreamProcessorRequestRequestTypeDef = TypedDict(
-    "StopStreamProcessorRequestRequestTypeDef",
+TechnicalCueSegmentTypeDef = TypedDict(
+    "TechnicalCueSegmentTypeDef",
     {
-        "Name": str,
+        "Type": TechnicalCueTypeType,
+        "Confidence": float,
     },
+    total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartCelebrityRecognitionResponseTypeDef = TypedDict(
+    "StartCelebrityRecognitionResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartContentModerationResponseTypeDef = TypedDict(
+    "StartContentModerationResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTechnicalCueDetectionFilterTypeDef = TypedDict(
-    "StartTechnicalCueDetectionFilterTypeDef",
+StartFaceDetectionResponseTypeDef = TypedDict(
+    "StartFaceDetectionResponseTypeDef",
     {
-        "MinSegmentConfidence": float,
-        "BlackFrame": BlackFrameTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ComparedSourceImageFaceTypeDef = TypedDict(
-    "ComparedSourceImageFaceTypeDef",
+StartFaceSearchResponseTypeDef = TypedDict(
+    "StartFaceSearchResponseTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Confidence": float,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-FaceTypeDef = TypedDict(
-    "FaceTypeDef",
+StartLabelDetectionResponseTypeDef = TypedDict(
+    "StartLabelDetectionResponseTypeDef",
     {
-        "FaceId": str,
-        "BoundingBox": BoundingBoxTypeDef,
-        "ImageId": str,
-        "ExternalImageId": str,
-        "Confidence": float,
-        "IndexFacesModelVersion": str,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CopyProjectVersionResponseTypeDef = TypedDict(
-    "CopyProjectVersionResponseTypeDef",
+StartPersonTrackingResponseTypeDef = TypedDict(
+    "StartPersonTrackingResponseTypeDef",
     {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCollectionResponseTypeDef = TypedDict(
-    "CreateCollectionResponseTypeDef",
+_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartProjectVersionRequestRequestTypeDef",
     {
-        "StatusCode": int,
-        "CollectionArn": str,
-        "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProjectVersionArn": str,
+        "MinInferenceUnits": int,
     },
 )
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
+_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartProjectVersionRequestRequestTypeDef",
     {
-        "DatasetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxInferenceUnits": int,
     },
+    total=False,
 )
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-CreateProjectVersionResponseTypeDef = TypedDict(
-    "CreateProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class StartProjectVersionRequestRequestTypeDef(
+    _RequiredStartProjectVersionRequestRequestTypeDef,
+    _OptionalStartProjectVersionRequestRequestTypeDef,
+):
+    pass
 
-CreateStreamProcessorResponseTypeDef = TypedDict(
-    "CreateStreamProcessorResponseTypeDef",
-    {
-        "StreamProcessorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-DeleteCollectionResponseTypeDef = TypedDict(
-    "DeleteCollectionResponseTypeDef",
+StartProjectVersionResponseTypeDef = TypedDict(
+    "StartProjectVersionResponseTypeDef",
     {
-        "StatusCode": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteFacesResponseTypeDef = TypedDict(
-    "DeleteFacesResponseTypeDef",
+StartShotDetectionFilterTypeDef = TypedDict(
+    "StartShotDetectionFilterTypeDef",
     {
-        "DeletedFaces": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MinSegmentConfidence": float,
     },
+    total=False,
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
+StartSegmentDetectionResponseTypeDef = TypedDict(
+    "StartSegmentDetectionResponseTypeDef",
     {
-        "Status": ProjectStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteProjectVersionResponseTypeDef = TypedDict(
-    "DeleteProjectVersionResponseTypeDef",
+StreamProcessingStopSelectorTypeDef = TypedDict(
+    "StreamProcessingStopSelectorTypeDef",
     {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxDurationInSeconds": int,
     },
+    total=False,
 )
 
-DescribeCollectionResponseTypeDef = TypedDict(
-    "DescribeCollectionResponseTypeDef",
+StartStreamProcessorResponseTypeDef = TypedDict(
+    "StartStreamProcessorResponseTypeDef",
     {
-        "FaceCount": int,
-        "FaceModelVersion": str,
-        "CollectionARN": str,
-        "CreationTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetCelebrityInfoResponseTypeDef = TypedDict(
-    "GetCelebrityInfoResponseTypeDef",
+StartTextDetectionResponseTypeDef = TypedDict(
+    "StartTextDetectionResponseTypeDef",
     {
-        "Urls": List[str],
-        "Name": str,
-        "KnownGender": KnownGenderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListCollectionsResponseTypeDef = TypedDict(
-    "ListCollectionsResponseTypeDef",
+StopProjectVersionRequestRequestTypeDef = TypedDict(
+    "StopProjectVersionRequestRequestTypeDef",
     {
-        "CollectionIds": List[str],
-        "NextToken": str,
-        "FaceModelVersions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProjectVersionArn": str,
     },
 )
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
+StopProjectVersionResponseTypeDef = TypedDict(
+    "StopProjectVersionResponseTypeDef",
     {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+StopStreamProcessorRequestRequestTypeDef = TypedDict(
+    "StopStreamProcessorRequestRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
     },
 )
 
-PutProjectPolicyResponseTypeDef = TypedDict(
-    "PutProjectPolicyResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-StartCelebrityRecognitionResponseTypeDef = TypedDict(
-    "StartCelebrityRecognitionResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-StartContentModerationResponseTypeDef = TypedDict(
-    "StartContentModerationResponseTypeDef",
+AssociateFacesResponseTypeDef = TypedDict(
+    "AssociateFacesResponseTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AssociatedFaces": List[AssociatedFaceTypeDef],
+        "UnsuccessfulFaceAssociations": List[UnsuccessfulFaceAssociationTypeDef],
+        "UserStatus": UserStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartFaceDetectionResponseTypeDef = TypedDict(
-    "StartFaceDetectionResponseTypeDef",
+ComparedSourceImageFaceTypeDef = TypedDict(
+    "ComparedSourceImageFaceTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Confidence": float,
     },
+    total=False,
 )
 
-StartFaceSearchResponseTypeDef = TypedDict(
-    "StartFaceSearchResponseTypeDef",
+FaceTypeDef = TypedDict(
+    "FaceTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FaceId": str,
+        "BoundingBox": BoundingBoxTypeDef,
+        "ImageId": str,
+        "ExternalImageId": str,
+        "Confidence": float,
+        "IndexFacesModelVersion": str,
+        "UserId": str,
     },
+    total=False,
 )
 
-StartLabelDetectionResponseTypeDef = TypedDict(
-    "StartLabelDetectionResponseTypeDef",
+AuditImageTypeDef = TypedDict(
+    "AuditImageTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Bytes": bytes,
+        "S3Object": S3ObjectTypeDef,
+        "BoundingBox": BoundingBoxTypeDef,
     },
+    total=False,
 )
 
-StartPersonTrackingResponseTypeDef = TypedDict(
-    "StartPersonTrackingResponseTypeDef",
+GroundTruthManifestTypeDef = TypedDict(
+    "GroundTruthManifestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartProjectVersionResponseTypeDef = TypedDict(
-    "StartProjectVersionResponseTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartSegmentDetectionResponseTypeDef = TypedDict(
-    "StartSegmentDetectionResponseTypeDef",
+SummaryTypeDef = TypedDict(
+    "SummaryTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartStreamProcessorResponseTypeDef = TypedDict(
-    "StartStreamProcessorResponseTypeDef",
+VideoTypeDef = TypedDict(
+    "VideoTypeDef",
     {
-        "SessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Object": S3ObjectTypeDef,
     },
+    total=False,
 )
 
-StartTextDetectionResponseTypeDef = TypedDict(
-    "StartTextDetectionResponseTypeDef",
+StartTechnicalCueDetectionFilterTypeDef = TypedDict(
+    "StartTechnicalCueDetectionFilterTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MinSegmentConfidence": float,
+        "BlackFrame": BlackFrameTypeDef,
     },
+    total=False,
 )
 
-StopProjectVersionResponseTypeDef = TypedDict(
-    "StopProjectVersionResponseTypeDef",
+GetCelebrityInfoResponseTypeDef = TypedDict(
+    "GetCelebrityInfoResponseTypeDef",
     {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Urls": List[str],
+        "Name": str,
+        "KnownGender": KnownGenderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
@@ -1672,14 +2266,17 @@
 )
 
 ContentModerationDetectionTypeDef = TypedDict(
     "ContentModerationDetectionTypeDef",
     {
         "Timestamp": int,
         "ModerationLabel": ModerationLabelTypeDef,
+        "StartTimestampMillis": int,
+        "EndTimestampMillis": int,
+        "DurationMillis": int,
     },
     total=False,
 )
 
 _RequiredCopyProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyProjectVersionRequestRequestTypeDef",
     {
@@ -1695,31 +2292,42 @@
     {
         "Tags": Mapping[str, str],
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class CopyProjectVersionRequestRequestTypeDef(
     _RequiredCopyProjectVersionRequestRequestTypeDef,
     _OptionalCopyProjectVersionRequestRequestTypeDef,
 ):
     pass
 
+
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
     },
     total=False,
 )
 
+CreateFaceLivenessSessionRequestSettingsTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestSettingsTypeDef",
+    {
+        "OutputConfig": LivenessOutputConfigTypeDef,
+        "AuditImagesLimit": int,
+    },
+    total=False,
+)
+
 UpdateDatasetEntriesRequestRequestTypeDef = TypedDict(
     "UpdateDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
         "Changes": DatasetChangesTypeDef,
     },
 )
@@ -1753,142 +2361,21 @@
         "CreationTimestamp": datetime,
         "Status": ProjectStatusType,
         "Datasets": List[DatasetMetadataTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "VersionNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
-    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-):
-    pass
-
-DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    {
-        "ProjectNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ContainsLabels": Sequence[str],
-        "Labeled": bool,
-        "SourceRefContains": str,
-        "HasErrors": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
-    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_RequiredListFacesRequestListFacesPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_OptionalListFacesRequestListFacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFacesRequestListFacesPaginateTypeDef(
-    _RequiredListFacesRequestListFacesPaginateTypeDef,
-    _OptionalListFacesRequestListFacesPaginateTypeDef,
-):
-    pass
-
-_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
-    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-):
-    pass
-
-ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+DeleteFacesResponseTypeDef = TypedDict(
+    "DeleteFacesResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "DeletedFaces": List[str],
+        "UnsuccessfulFaceDeletions": List[UnsuccessfulFaceDeletionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
@@ -1900,20 +2387,22 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
@@ -1923,20 +2412,22 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
 ):
     pass
 
+
 DetectLabelsImageBackgroundTypeDef = TypedDict(
     "DetectLabelsImageBackgroundTypeDef",
     {
         "Quality": DetectLabelsImageQualityTypeDef,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
@@ -1966,21 +2457,39 @@
     {
         "GeneralLabels": GeneralLabelsSettingsTypeDef,
         "ImageProperties": DetectLabelsImagePropertiesSettingsTypeDef,
     },
     total=False,
 )
 
+LabelDetectionSettingsTypeDef = TypedDict(
+    "LabelDetectionSettingsTypeDef",
+    {
+        "GeneralLabels": GeneralLabelsSettingsTypeDef,
+    },
+    total=False,
+)
+
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateFacesResponseTypeDef = TypedDict(
+    "DisassociateFacesResponseTypeDef",
+    {
+        "DisassociatedFaces": List[DisassociatedFaceTypeDef],
+        "UnsuccessfulFaceDisassociations": List[UnsuccessfulFaceDisassociationTypeDef],
+        "UserStatus": UserStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DistributeDatasetEntriesRequestRequestTypeDef = TypedDict(
     "DistributeDatasetEntriesRequestRequestTypeDef",
     {
         "Datasets": Sequence[DistributeDatasetTypeDef],
@@ -2001,14 +2510,16 @@
         "EyesOpen": EyeOpenTypeDef,
         "MouthOpen": MouthOpenTypeDef,
         "Emotions": List[EmotionTypeDef],
         "Landmarks": List[LandmarkTypeDef],
         "Pose": PoseTypeDef,
         "Quality": ImageQualityTypeDef,
         "Confidence": float,
+        "FaceOccluded": FaceOccludedTypeDef,
+        "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
@@ -2032,47 +2543,14 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
 )
 
-GroundTruthManifestTypeDef = TypedDict(
-    "GroundTruthManifestTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-SummaryTypeDef = TypedDict(
-    "SummaryTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-VideoTypeDef = TypedDict(
-    "VideoTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
         "HumanLoopName": str,
         "FlowDefinitionArn": str,
     },
 )
@@ -2080,17 +2558,19 @@
     "_OptionalHumanLoopConfigTypeDef",
     {
         "DataAttributes": HumanLoopDataAttributesTypeDef,
     },
     total=False,
 )
 
+
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
+
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2104,25 +2584,43 @@
 )
 
 ListProjectPoliciesResponseTypeDef = TypedDict(
     "ListProjectPoliciesResponseTypeDef",
     {
         "ProjectPolicies": List[ProjectPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamProcessorsResponseTypeDef = TypedDict(
     "ListStreamProcessorsResponseTypeDef",
     {
         "NextToken": str,
         "StreamProcessors": List[StreamProcessorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
+    {
+        "Users": List[UserTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UserMatchTypeDef = TypedDict(
+    "UserMatchTypeDef",
+    {
+        "Similarity": float,
+        "User": MatchedUserTypeDef,
     },
+    total=False,
 )
 
 StreamProcessorOutputTypeDef = TypedDict(
     "StreamProcessorOutputTypeDef",
     {
         "KinesisDataStream": KinesisDataStreamTypeDef,
         "S3Destination": S3DestinationTypeDef,
@@ -2145,23 +2643,14 @@
         "StartFrameNumber": int,
         "EndFrameNumber": int,
         "DurationFrames": int,
     },
     total=False,
 )
 
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
 FaceMatchTypeDef = TypedDict(
     "FaceMatchTypeDef",
     {
         "Similarity": float,
         "Face": FaceTypeDef,
     },
     total=False,
@@ -2169,237 +2658,30 @@
 
 ListFacesResponseTypeDef = TypedDict(
     "ListFacesResponseTypeDef",
     {
         "Faces": List[FaceTypeDef],
         "NextToken": str,
         "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CelebrityTypeDef = TypedDict(
-    "CelebrityTypeDef",
+GetFaceLivenessSessionResultsResponseTypeDef = TypedDict(
+    "GetFaceLivenessSessionResultsResponseTypeDef",
     {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Face": ComparedFaceTypeDef,
-        "MatchConfidence": float,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-CompareFacesMatchTypeDef = TypedDict(
-    "CompareFacesMatchTypeDef",
-    {
-        "Similarity": float,
-        "Face": ComparedFaceTypeDef,
-    },
-    total=False,
-)
-
-GetContentModerationResponseTypeDef = TypedDict(
-    "GetContentModerationResponseTypeDef",
-    {
-        "JobStatus": VideoJobStatusType,
-        "StatusMessage": str,
-        "VideoMetadata": VideoMetadataTypeDef,
-        "ModerationLabels": List[ContentModerationDetectionTypeDef],
-        "NextToken": str,
-        "ModerationModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProtectiveEquipmentBodyPartTypeDef = TypedDict(
-    "ProtectiveEquipmentBodyPartTypeDef",
-    {
-        "Name": BodyPartType,
-        "Confidence": float,
-        "EquipmentDetections": List[EquipmentDetectionTypeDef],
-    },
-    total=False,
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatasetLabelsResponseTypeDef = TypedDict(
-    "ListDatasetLabelsResponseTypeDef",
-    {
-        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeProjectsResponseTypeDef = TypedDict(
-    "DescribeProjectsResponseTypeDef",
-    {
-        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectLabelsImagePropertiesTypeDef = TypedDict(
-    "DetectLabelsImagePropertiesTypeDef",
-    {
-        "Quality": DetectLabelsImageQualityTypeDef,
-        "DominantColors": List[DominantColorTypeDef],
-        "Foreground": DetectLabelsImageForegroundTypeDef,
-        "Background": DetectLabelsImageBackgroundTypeDef,
-    },
-    total=False,
-)
-
-LabelTypeDef = TypedDict(
-    "LabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Instances": List[InstanceTypeDef],
-        "Parents": List[ParentTypeDef],
-        "Aliases": List[LabelAliasTypeDef],
-        "Categories": List[LabelCategoryTypeDef],
-    },
-    total=False,
-)
-
-CelebrityDetailTypeDef = TypedDict(
-    "CelebrityDetailTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Confidence": float,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-DetectFacesResponseTypeDef = TypedDict(
-    "DetectFacesResponseTypeDef",
-    {
-        "FaceDetails": List[FaceDetailTypeDef],
-        "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-FaceDetectionTypeDef = TypedDict(
-    "FaceDetectionTypeDef",
-    {
-        "Timestamp": int,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-FaceRecordTypeDef = TypedDict(
-    "FaceRecordTypeDef",
-    {
-        "Face": FaceTypeDef,
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-PersonDetailTypeDef = TypedDict(
-    "PersonDetailTypeDef",
-    {
-        "Index": int,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-UnindexedFaceTypeDef = TypedDict(
-    "UnindexedFaceTypeDef",
-    {
-        "Reasons": List[ReasonType],
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-CustomLabelTypeDef = TypedDict(
-    "CustomLabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-TextDetectionTypeDef = TypedDict(
-    "TextDetectionTypeDef",
-    {
-        "DetectedText": str,
-        "Type": TextTypesType,
-        "Id": int,
-        "ParentId": int,
+        "SessionId": str,
+        "Status": LivenessSessionStatusType,
         "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-DetectTextFiltersTypeDef = TypedDict(
-    "DetectTextFiltersTypeDef",
-    {
-        "WordFilter": DetectionFilterTypeDef,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
-    },
-    total=False,
-)
-
-StartTextDetectionFiltersTypeDef = TypedDict(
-    "StartTextDetectionFiltersTypeDef",
-    {
-        "WordFilter": DetectionFilterTypeDef,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "ReferenceImage": AuditImageTypeDef,
+        "AuditImages": List[AuditImageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
     },
     total=False,
 )
@@ -2425,19 +2707,21 @@
     {
         "SimilarityThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class CompareFacesRequestRequestTypeDef(
     _RequiredCompareFacesRequestRequestTypeDef, _OptionalCompareFacesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDetectCustomLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectCustomLabelsRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2446,60 +2730,42 @@
     {
         "MaxResults": int,
         "MinConfidence": float,
     },
     total=False,
 )
 
+
 class DetectCustomLabelsRequestRequestTypeDef(
     _RequiredDetectCustomLabelsRequestRequestTypeDef,
     _OptionalDetectCustomLabelsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDetectFacesRequestRequestTypeDef = TypedDict(
     "_RequiredDetectFacesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectFacesRequestRequestTypeDef = TypedDict(
     "_OptionalDetectFacesRequestRequestTypeDef",
     {
         "Attributes": Sequence[AttributeType],
     },
     total=False,
 )
 
+
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
-_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectLabelsRequestRequestTypeDef",
-    {
-        "MaxLabels": int,
-        "MinConfidence": float,
-        "Features": Sequence[DetectLabelsFeatureNameType],
-        "Settings": DetectLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
-class DetectLabelsRequestRequestTypeDef(
-    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
-):
-    pass
 
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
@@ -2507,20 +2773,22 @@
     "_OptionalDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "SummarizationAttributes": ProtectiveEquipmentSummarizationAttributesTypeDef,
     },
     total=False,
 )
 
+
 class DetectProtectiveEquipmentRequestRequestTypeDef(
     _RequiredDetectProtectiveEquipmentRequestRequestTypeDef,
     _OptionalDetectProtectiveEquipmentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredIndexFacesRequestRequestTypeDef = TypedDict(
     "_RequiredIndexFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2531,19 +2799,21 @@
         "DetectionAttributes": Sequence[AttributeType],
         "MaxFaces": int,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class IndexFacesRequestRequestTypeDef(
     _RequiredIndexFacesRequestRequestTypeDef, _OptionalIndexFacesRequestRequestTypeDef
 ):
     pass
 
+
 RecognizeCelebritiesRequestRequestTypeDef = TypedDict(
     "RecognizeCelebritiesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 
@@ -2560,20 +2830,47 @@
         "MaxFaces": int,
         "FaceMatchThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class SearchFacesByImageRequestRequestTypeDef(
     _RequiredSearchFacesByImageRequestRequestTypeDef,
     _OptionalSearchFacesByImageRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredSearchUsersByImageRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchUsersByImageRequestRequestTypeDef",
+    {
+        "CollectionId": str,
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalSearchUsersByImageRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchUsersByImageRequestRequestTypeDef",
+    {
+        "UserMatchThreshold": float,
+        "MaxUsers": int,
+        "QualityFilter": QualityFilterType,
+    },
+    total=False,
+)
+
+
+class SearchUsersByImageRequestRequestTypeDef(
+    _RequiredSearchUsersByImageRequestRequestTypeDef,
+    _OptionalSearchUsersByImageRequestRequestTypeDef,
+):
+    pass
+
+
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "F1Score": float,
         "Summary": SummaryTypeDef,
     },
     total=False,
@@ -2591,20 +2888,22 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartCelebrityRecognitionRequestRequestTypeDef(
     _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
     _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartContentModerationRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
@@ -2614,20 +2913,22 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartContentModerationRequestRequestTypeDef(
     _RequiredStartContentModerationRequestRequestTypeDef,
     _OptionalStartContentModerationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -2637,20 +2938,22 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "FaceAttributes": FaceAttributesType,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartFaceDetectionRequestRequestTypeDef(
     _RequiredStartFaceDetectionRequestRequestTypeDef,
     _OptionalStartFaceDetectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceSearchRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "CollectionId": str,
     },
 )
@@ -2661,64 +2964,357 @@
         "FaceMatchThreshold": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+    {
+        "Video": VideoTypeDef,
+    },
+)
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
+    },
+    total=False,
+)
+
+
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
+
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+CelebrityTypeDef = TypedDict(
+    "CelebrityTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Face": ComparedFaceTypeDef,
+        "MatchConfidence": float,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+CompareFacesMatchTypeDef = TypedDict(
+    "CompareFacesMatchTypeDef",
+    {
+        "Similarity": float,
+        "Face": ComparedFaceTypeDef,
+    },
+    total=False,
+)
+
+GetContentModerationResponseTypeDef = TypedDict(
+    "GetContentModerationResponseTypeDef",
+    {
+        "JobStatus": VideoJobStatusType,
+        "StatusMessage": str,
+        "VideoMetadata": VideoMetadataTypeDef,
+        "ModerationLabels": List[ContentModerationDetectionTypeDef],
+        "NextToken": str,
+        "ModerationModelVersion": str,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProtectiveEquipmentBodyPartTypeDef = TypedDict(
+    "ProtectiveEquipmentBodyPartTypeDef",
+    {
+        "Name": BodyPartType,
+        "Confidence": float,
+        "EquipmentDetections": List[EquipmentDetectionTypeDef],
+    },
+    total=False,
+)
+
+CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
+    {
+        "KmsKeyId": str,
+        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetDescription": DatasetDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDatasetLabelsResponseTypeDef = TypedDict(
+    "ListDatasetLabelsResponseTypeDef",
+    {
+        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeProjectsResponseTypeDef = TypedDict(
+    "DescribeProjectsResponseTypeDef",
+    {
+        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DetectLabelsImagePropertiesTypeDef = TypedDict(
+    "DetectLabelsImagePropertiesTypeDef",
+    {
+        "Quality": DetectLabelsImageQualityTypeDef,
+        "DominantColors": List[DominantColorTypeDef],
+        "Foreground": DetectLabelsImageForegroundTypeDef,
+        "Background": DetectLabelsImageBackgroundTypeDef,
+    },
+    total=False,
+)
+
+LabelTypeDef = TypedDict(
+    "LabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Instances": List[InstanceTypeDef],
+        "Parents": List[ParentTypeDef],
+        "Aliases": List[LabelAliasTypeDef],
+        "Categories": List[LabelCategoryTypeDef],
+    },
+    total=False,
+)
+
+_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectLabelsRequestRequestTypeDef",
+    {
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectLabelsRequestRequestTypeDef",
+    {
+        "MaxLabels": int,
+        "MinConfidence": float,
+        "Features": Sequence[DetectLabelsFeatureNameType],
+        "Settings": DetectLabelsSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class DetectLabelsRequestRequestTypeDef(
+    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
+        "Features": Sequence[Literal["GENERAL_LABELS"]],
+        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
     _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+
+CelebrityDetailTypeDef = TypedDict(
+    "CelebrityDetailTypeDef",
     {
-        "Video": VideoTypeDef,
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Confidence": float,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+        "KnownGender": KnownGenderTypeDef,
     },
+    total=False,
 )
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+
+DetectFacesResponseTypeDef = TypedDict(
+    "DetectFacesResponseTypeDef",
     {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
+        "FaceDetails": List[FaceDetailTypeDef],
+        "OrientationCorrection": OrientationCorrectionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FaceDetectionTypeDef = TypedDict(
+    "FaceDetectionTypeDef",
+    {
+        "Timestamp": int,
+        "Face": FaceDetailTypeDef,
     },
     total=False,
 )
 
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
+FaceRecordTypeDef = TypedDict(
+    "FaceRecordTypeDef",
+    {
+        "Face": FaceTypeDef,
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+PersonDetailTypeDef = TypedDict(
+    "PersonDetailTypeDef",
+    {
+        "Index": int,
+        "BoundingBox": BoundingBoxTypeDef,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+SearchedFaceDetailsTypeDef = TypedDict(
+    "SearchedFaceDetailsTypeDef",
+    {
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnindexedFaceTypeDef = TypedDict(
+    "UnindexedFaceTypeDef",
+    {
+        "Reasons": List[ReasonType],
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnsearchedFaceTypeDef = TypedDict(
+    "UnsearchedFaceTypeDef",
+    {
+        "FaceDetails": FaceDetailTypeDef,
+        "Reasons": List[UnsearchedFaceReasonType],
+    },
+    total=False,
+)
+
+CustomLabelTypeDef = TypedDict(
+    "CustomLabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+TextDetectionTypeDef = TypedDict(
+    "TextDetectionTypeDef",
+    {
+        "DetectedText": str,
+        "Type": TextTypesType,
+        "Id": int,
+        "ParentId": int,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+DetectTextFiltersTypeDef = TypedDict(
+    "DetectTextFiltersTypeDef",
+    {
+        "WordFilter": DetectionFilterTypeDef,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+    },
+    total=False,
+)
+
+StartTextDetectionFiltersTypeDef = TypedDict(
+    "StartTextDetectionFiltersTypeDef",
+    {
+        "WordFilter": DetectionFilterTypeDef,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+    },
+    total=False,
+)
+
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -2726,20 +3322,22 @@
     {
         "MinConfidence": float,
         "HumanLoopConfig": HumanLoopConfigTypeDef,
     },
     total=False,
 )
 
+
 class DetectModerationLabelsRequestRequestTypeDef(
     _RequiredDetectModerationLabelsRequestRequestTypeDef,
     _OptionalDetectModerationLabelsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredStartStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
@@ -2747,20 +3345,33 @@
     {
         "StartSelector": StreamProcessingStartSelectorTypeDef,
         "StopSelector": StreamProcessingStopSelectorTypeDef,
     },
     total=False,
 )
 
+
 class StartStreamProcessorRequestRequestTypeDef(
     _RequiredStartStreamProcessorRequestRequestTypeDef,
     _OptionalStartStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
+
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
+    {
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceTypeDef,
+        "SearchedUser": SearchedUserTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamProcessorRequestRequestTypeDef",
     {
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "Name": str,
         "Settings": StreamProcessorSettingsTypeDef,
@@ -2775,20 +3386,22 @@
         "KmsKeyId": str,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
     },
     total=False,
 )
 
+
 class CreateStreamProcessorRequestRequestTypeDef(
     _RequiredCreateStreamProcessorRequestRequestTypeDef,
     _OptionalCreateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
@@ -2798,32 +3411,103 @@
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
         "Settings": StreamProcessorSettingsTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
         "RegionsOfInterest": List[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": List[VideoMetadataTypeDef],
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchFacesByImageResponseTypeDef = TypedDict(
+    "SearchFacesByImageResponseTypeDef",
+    {
+        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
+        "SearchedFaceConfidence": float,
+        "FaceMatches": List[FaceMatchTypeDef],
+        "FaceModelVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchFacesResponseTypeDef = TypedDict(
+    "SearchFacesResponseTypeDef",
+    {
+        "SearchedFaceId": str,
+        "FaceMatches": List[FaceMatchTypeDef],
+        "FaceModelVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TestingDataTypeDef = TypedDict(
+    "TestingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+        "AutoCreate": bool,
+    },
+    total=False,
+)
+
+TrainingDataTypeDef = TypedDict(
+    "TrainingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+    },
+    total=False,
+)
+
+ValidationDataTypeDef = TypedDict(
+    "ValidationDataTypeDef",
+    {
+        "Assets": List[AssetTypeDef],
     },
+    total=False,
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "ProjectArn": str,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetSource": DatasetSourceTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -2834,60 +3518,41 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartSegmentDetectionFiltersTypeDef,
     },
     total=False,
 )
 
+
 class StartSegmentDetectionRequestRequestTypeDef(
     _RequiredStartSegmentDetectionRequestRequestTypeDef,
     _OptionalStartSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
-SearchFacesByImageResponseTypeDef = TypedDict(
-    "SearchFacesByImageResponseTypeDef",
-    {
-        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
-        "SearchedFaceConfidence": float,
-        "FaceMatches": List[FaceMatchTypeDef],
-        "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchFacesResponseTypeDef = TypedDict(
-    "SearchFacesResponseTypeDef",
-    {
-        "SearchedFaceId": str,
-        "FaceMatches": List[FaceMatchTypeDef],
-        "FaceModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompareFacesResponseTypeDef = TypedDict(
     "CompareFacesResponseTypeDef",
     {
         "SourceImageFace": ComparedSourceImageFaceTypeDef,
         "FaceMatches": List[CompareFacesMatchTypeDef],
         "UnmatchedFaces": List[ComparedFaceTypeDef],
         "SourceImageOrientationCorrection": OrientationCorrectionType,
         "TargetImageOrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
@@ -2901,23 +3566,26 @@
 DetectLabelsResponseTypeDef = TypedDict(
     "DetectLabelsResponseTypeDef",
     {
         "Labels": List[LabelTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "LabelModelVersion": str,
         "ImageProperties": DetectLabelsImagePropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
         "Label": LabelTypeDef,
+        "StartTimestampMillis": int,
+        "EndTimestampMillis": int,
+        "DurationMillis": int,
     },
     total=False,
 )
 
 CelebrityRecognitionTypeDef = TypedDict(
     "CelebrityRecognitionTypeDef",
     {
@@ -2931,15 +3599,18 @@
     "GetFaceDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
     {
         "Timestamp": int,
@@ -2961,32 +3632,43 @@
 IndexFacesResponseTypeDef = TypedDict(
     "IndexFacesResponseTypeDef",
     {
         "FaceRecords": List[FaceRecordTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "FaceModelVersion": str,
         "UnindexedFaces": List[UnindexedFaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchUsersByImageResponseTypeDef = TypedDict(
+    "SearchUsersByImageResponseTypeDef",
+    {
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceDetailsTypeDef,
+        "UnsearchedFaces": List[UnsearchedFaceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectCustomLabelsResponseTypeDef = TypedDict(
     "DetectCustomLabelsResponseTypeDef",
     {
         "CustomLabels": List[CustomLabelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectTextResponseTypeDef = TypedDict(
     "DetectTextResponseTypeDef",
     {
         "TextDetections": List[TextDetectionTypeDef],
         "TextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TextDetectionResultTypeDef = TypedDict(
     "TextDetectionResultTypeDef",
     {
         "Timestamp": int,
@@ -3005,19 +3687,21 @@
     "_OptionalDetectTextRequestRequestTypeDef",
     {
         "Filters": DetectTextFiltersTypeDef,
     },
     total=False,
 )
 
+
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3027,180 +3711,155 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartTextDetectionFiltersTypeDef,
     },
     total=False,
 )
 
+
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
-TestingDataTypeDef = TypedDict(
-    "TestingDataTypeDef",
+
+_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
-        "AutoCreate": bool,
+        "ProjectArn": str,
+        "VersionName": str,
+        "OutputConfig": OutputConfigTypeDef,
     },
-    total=False,
 )
-
-TrainingDataTypeDef = TypedDict(
-    "TrainingDataTypeDef",
+_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectVersionRequestRequestTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
+        "TrainingData": TrainingDataTypeDef,
+        "TestingData": TestingDataTypeDef,
+        "Tags": Mapping[str, str],
+        "KmsKeyId": str,
     },
     total=False,
 )
 
-ValidationDataTypeDef = TypedDict(
-    "ValidationDataTypeDef",
+
+class CreateProjectVersionRequestRequestTypeDef(
+    _RequiredCreateProjectVersionRequestRequestTypeDef,
+    _OptionalCreateProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+
+TestingDataResultTypeDef = TypedDict(
+    "TestingDataResultTypeDef",
     {
-        "Assets": List[AssetTypeDef],
+        "Input": TestingDataTypeDef,
+        "Output": TestingDataTypeDef,
+        "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "ProjectArn": str,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
+TrainingDataResultTypeDef = TypedDict(
+    "TrainingDataResultTypeDef",
     {
-        "DatasetSource": DatasetSourceTypeDef,
+        "Input": TrainingDataTypeDef,
+        "Output": TrainingDataTypeDef,
+        "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
     {
         "ProtectiveEquipmentModelVersion": str,
         "Persons": List[ProtectiveEquipmentPersonTypeDef],
         "Summary": ProtectiveEquipmentSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLabelDetectionResponseTypeDef = TypedDict(
     "GetLabelDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
     "GetCelebrityRecognitionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectArn": str,
-        "VersionName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectVersionRequestRequestTypeDef",
-    {
-        "TrainingData": TrainingDataTypeDef,
-        "TestingData": TestingDataTypeDef,
-        "Tags": Mapping[str, str],
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class CreateProjectVersionRequestRequestTypeDef(
-    _RequiredCreateProjectVersionRequestRequestTypeDef,
-    _OptionalCreateProjectVersionRequestRequestTypeDef,
-):
-    pass
-
-TestingDataResultTypeDef = TypedDict(
-    "TestingDataResultTypeDef",
-    {
-        "Input": TestingDataTypeDef,
-        "Output": TestingDataTypeDef,
-        "Validation": ValidationDataTypeDef,
-    },
-    total=False,
-)
-
-TrainingDataResultTypeDef = TypedDict(
-    "TrainingDataResultTypeDef",
-    {
-        "Input": TrainingDataTypeDef,
-        "Output": TrainingDataTypeDef,
-        "Validation": ValidationDataTypeDef,
+        "JobId": str,
+        "Video": VideoTypeDef,
+        "JobTag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
         "CreationTimestamp": datetime,
@@ -3222,10 +3881,10 @@
 )
 
 DescribeProjectVersionsResponseTypeDef = TypedDict(
     "DescribeProjectVersionsResponseTypeDef",
     {
         "ProjectVersionDescriptions": List[ProjectVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.27.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-rekognition
-Version: 1.26.8
-Summary: Type annotations for boto3.Rekognition 1.26.8 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-rekognition"></a>
 
 # mypy-boto3-rekognition
 
 [![PyPI - mypy-boto3-rekognition](https://img.shields.io/pypi/v/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,14 +256,15 @@
     DescribeProjectsPaginator,
     ListCollectionsPaginator,
     ListDatasetEntriesPaginator,
     ListDatasetLabelsPaginator,
     ListFacesPaginator,
     ListProjectPoliciesPaginator,
     ListStreamProcessorsPaginator,
+    ListUsersPaginator,
 )
 
 client: RekognitionClient = Session().client("rekognition")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_project_versions_paginator: DescribeProjectVersionsPaginator = client.get_paginator(
@@ -311,14 +281,15 @@
 list_faces_paginator: ListFacesPaginator = client.get_paginator("list_faces")
 list_project_policies_paginator: ListProjectPoliciesPaginator = client.get_paginator(
     "list_project_policies"
 )
 list_stream_processors_paginator: ListStreamProcessorsPaginator = client.get_paginator(
     "list_stream_processors"
 )
+list_users_paginator: ListUsersPaginator = client.get_paginator("list_users")
 ```
 
 <a id="waiters-annotations"></a>
 
 ### Waiters annotations
 
 `mypy_boto3_rekognition.waiter` module contains type annotations for all
@@ -354,48 +325,58 @@
 
 ```python
 from mypy_boto3_rekognition.literals import (
     AttributeType,
     BodyPartType,
     CelebrityRecognitionSortByType,
     ContentClassifierType,
+    ContentModerationAggregateByType,
     ContentModerationSortByType,
     DatasetStatusMessageCodeType,
     DatasetStatusType,
     DatasetTypeType,
     DescribeProjectVersionsPaginatorName,
     DescribeProjectsPaginatorName,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
+    LabelDetectionAggregateByType,
+    LabelDetectionFeatureNameType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     ListCollectionsPaginatorName,
     ListDatasetEntriesPaginatorName,
     ListDatasetLabelsPaginatorName,
     ListFacesPaginatorName,
     ListProjectPoliciesPaginatorName,
     ListStreamProcessorsPaginatorName,
+    ListUsersPaginatorName,
+    LivenessSessionStatusType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionRunningWaiterName,
     ProjectVersionStatusType,
     ProjectVersionTrainingCompletedWaiterName,
     ProtectiveEquipmentTypeType,
     QualityFilterType,
     ReasonType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
     StreamProcessorStatusType,
     TechnicalCueTypeType,
     TextTypesType,
+    UnsearchedFaceReasonType,
+    UnsuccessfulFaceAssociationReasonType,
+    UnsuccessfulFaceDeletionReasonType,
+    UnsuccessfulFaceDisassociationReasonType,
+    UserStatusType,
     VideoColorRangeType,
     VideoJobStatusType,
     RekognitionServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
@@ -413,256 +394,293 @@
 
 `mypy_boto3_rekognition.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
+    AssociateFacesRequestRequestTypeDef,
+    AssociatedFaceTypeDef,
+    UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
+    BoundingBoxTypeDef,
+    S3ObjectTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
-    BoundingBoxTypeDef,
     KnownGenderTypeDef,
-    ResponseMetadataTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
+    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    LivenessOutputConfigTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    CreateUserRequestRequestTypeDef,
     DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
+    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
+    UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
+    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
+    DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
+    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
     DetectionFilterTypeDef,
+    DisassociateFacesRequestRequestTypeDef,
+    DisassociatedFaceTypeDef,
+    UnsuccessfulFaceDisassociationTypeDef,
     DistributeDatasetTypeDef,
+    EyeDirectionTypeDef,
     EyeOpenTypeDef,
     EyeglassesTypeDef,
+    FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
     FaceSearchSettingsTypeDef,
     PointTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
+    GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
+    GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
+    GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
-    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListUsersRequestRequestTypeDef,
+    UserTypeDef,
+    MatchedUserTypeDef,
     NotificationChannelTypeDef,
+    PaginatorConfigTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
+    PutProjectPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
+    SearchUsersRequestRequestTypeDef,
+    SearchedFaceTypeDef,
+    SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
-    StartShotDetectionFilterTypeDef,
-    StreamProcessingStopSelectorTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    StartTechnicalCueDetectionFilterTypeDef,
-    ComparedSourceImageFaceTypeDef,
-    FaceTypeDef,
-    CopyProjectVersionResponseTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
-    CreateStreamProcessorResponseTypeDef,
-    DeleteCollectionResponseTypeDef,
-    DeleteFacesResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    DeleteProjectVersionResponseTypeDef,
-    DescribeCollectionResponseTypeDef,
-    GetCelebrityInfoResponseTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
+    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
+    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    AssociateFacesResponseTypeDef,
+    ComparedSourceImageFaceTypeDef,
+    FaceTypeDef,
+    AuditImageTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
+    SummaryTypeDef,
+    VideoTypeDef,
+    StartTechnicalCueDetectionFilterTypeDef,
+    GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
+    CreateFaceLivenessSessionRequestSettingsTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    DeleteFacesResponseTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
+    LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
+    DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
-    SummaryTypeDef,
-    VideoTypeDef,
     HumanLoopConfigTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
+    ListUsersResponseTypeDef,
+    UserMatchTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
-    StartSegmentDetectionFiltersTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
+    GetFaceLivenessSessionResultsResponseTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
+    EvaluationResultTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
+    StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
+    CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
+    SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
+    UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
     DetectTextFiltersTypeDef,
     StartTextDetectionFiltersTypeDef,
     UpdateStreamProcessorRequestRequestTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
+    SearchUsersResponseTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
-    StartSegmentDetectionRequestRequestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
+    ValidationDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
     GetFaceDetectionResponseTypeDef,
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
+    SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
-    ValidationDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
+    TestingDataResultTypeDef,
+    TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
-    TestingDataResultTypeDef,
-    TrainingDataResultTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
@@ -671,42 +689,42 @@
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

### Comparing `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.27.0/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.8/setup.py` & `mypy-boto3-rekognition-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-rekognition.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.26.8",
+    version="1.27.0",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Rekognition 1.26.8 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Rekognition 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_rekognition": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_rekognition": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/",
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


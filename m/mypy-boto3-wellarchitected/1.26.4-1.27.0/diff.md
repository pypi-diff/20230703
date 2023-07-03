# Comparing `tmp/mypy-boto3-wellarchitected-1.26.4.tar.gz` & `tmp/mypy-boto3-wellarchitected-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wellarchitected-1.26.4.tar", last modified: Mon Nov  7 20:50:37 2022, max compression
+gzip compressed data, was "mypy-boto3-wellarchitected-1.27.0.tar", last modified: Mon Jul  3 19:51:36 2023, max compression
```

## Comparing `mypy-boto3-wellarchitected-1.26.4.tar` & `mypy-boto3-wellarchitected-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16502 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15035 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.072346 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29412 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    29364 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9627 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    39740 2022-11-07 20:50:24.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    39695 2022-11-07 20:50:24.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16502 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.172143 mypy-boto3-wellarchitected-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-07-03 19:51:36.172143 mypy-boto3-wellarchitected-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.172143 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38027 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37965 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53113 2023-07-03 19:49:43.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53056 2023-07-03 19:49:42.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.172143 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-07-03 19:51:36.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 19:51:36.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:36.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:36.000000 mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:36.172143 mypy-boto3-wellarchitected-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-03 19:49:41.000000 mypy-boto3-wellarchitected-1.27.0/setup.py
```

### Comparing `mypy-boto3-wellarchitected-1.26.4/LICENSE` & `mypy-boto3-wellarchitected-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-wellarchitected-1.26.4/PKG-INFO` & `mypy-boto3-wellarchitected-1.27.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.26.4
-Summary: Type annotations for boto3.WellArchitected 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.WellArchitected 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
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
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,22 +284,30 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
+    DefinitionTypeType,
     DifferenceStatusType,
+    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
+    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileNotificationTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    QuestionTypeType,
+    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -322,161 +331,199 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
+    AssociateProfilesInputRequestTypeDef,
+    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLensShareOutputTypeDef,
     CreateLensVersionInputRequestTypeDef,
+    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
+    CreateMilestoneOutputTypeDef,
+    ProfileQuestionUpdateTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareInputRequestTypeDef,
+    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
+    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
+    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
+    DeleteProfileInputRequestTypeDef,
+    DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
+    DisassociateProfilesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
+    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
+    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
+    GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    LensReviewSummaryTypeDef,
+    ImportLensOutputTypeDef,
+    WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
     ListCheckSummariesInputRequestTypeDef,
     ListLensReviewImprovementsInputRequestTypeDef,
     ListLensReviewsInputRequestTypeDef,
     ListLensSharesInputRequestTypeDef,
     ListLensesInputRequestTypeDef,
     ListMilestonesInputRequestTypeDef,
     ListNotificationsInputRequestTypeDef,
+    ListProfileNotificationsInputRequestTypeDef,
+    ProfileNotificationSummaryTypeDef,
+    ListProfileSharesInputRequestTypeDef,
+    ProfileShareSummaryTypeDef,
+    ListProfilesInputRequestTypeDef,
+    ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
-    WorkloadSummaryTypeDef,
     QuestionDifferenceTypeDef,
+    ProfileChoiceTypeDef,
+    ProfileTemplateChoiceTypeDef,
+    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
+    UpgradeProfileVersionInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    ImprovementSummaryTypeDef,
-    UpdateAnswerInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
-    CreateLensVersionOutputTypeDef,
-    CreateMilestoneOutputTypeDef,
-    CreateWorkloadOutputTypeDef,
-    CreateWorkloadShareOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportLensOutputTypeDef,
-    ImportLensOutputTypeDef,
+    QuestionMetricTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ImprovementSummaryTypeDef,
+    UpdateAnswerInputRequestTypeDef,
+    CreateProfileInputRequestTypeDef,
+    UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
-    WorkloadTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
-    ListLensReviewsOutputTypeDef,
+    LensReviewSummaryTypeDef,
+    WorkloadSummaryTypeDef,
+    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
+    ListProfileNotificationsOutputTypeDef,
+    ListProfileSharesOutputTypeDef,
+    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
-    ListWorkloadsOutputTypeDef,
-    MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
+    ProfileQuestionTypeDef,
+    ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
+    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
+    ListLensReviewsOutputTypeDef,
+    ListWorkloadsOutputTypeDef,
+    MilestoneSummaryTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
-    ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
+    ProfileTypeDef,
+    ProfileTemplateTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
+    LensMetricTypeDef,
+    ListMilestonesOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
+    GetProfileOutputTypeDef,
+    UpdateProfileOutputTypeDef,
+    GetProfileTemplateOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
+    ConsolidatedReportMetricTypeDef,
+    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-wellarchitected-1.26.4/README.md` & `mypy-boto3-wellarchitected-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -252,22 +252,30 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
+    DefinitionTypeType,
     DifferenceStatusType,
+    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
+    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileNotificationTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    QuestionTypeType,
+    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -291,161 +299,199 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
+    AssociateProfilesInputRequestTypeDef,
+    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLensShareOutputTypeDef,
     CreateLensVersionInputRequestTypeDef,
+    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
+    CreateMilestoneOutputTypeDef,
+    ProfileQuestionUpdateTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareInputRequestTypeDef,
+    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
+    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
+    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
+    DeleteProfileInputRequestTypeDef,
+    DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
+    DisassociateProfilesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
+    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
+    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
+    GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    LensReviewSummaryTypeDef,
+    ImportLensOutputTypeDef,
+    WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
     ListCheckSummariesInputRequestTypeDef,
     ListLensReviewImprovementsInputRequestTypeDef,
     ListLensReviewsInputRequestTypeDef,
     ListLensSharesInputRequestTypeDef,
     ListLensesInputRequestTypeDef,
     ListMilestonesInputRequestTypeDef,
     ListNotificationsInputRequestTypeDef,
+    ListProfileNotificationsInputRequestTypeDef,
+    ProfileNotificationSummaryTypeDef,
+    ListProfileSharesInputRequestTypeDef,
+    ProfileShareSummaryTypeDef,
+    ListProfilesInputRequestTypeDef,
+    ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
-    WorkloadSummaryTypeDef,
     QuestionDifferenceTypeDef,
+    ProfileChoiceTypeDef,
+    ProfileTemplateChoiceTypeDef,
+    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
+    UpgradeProfileVersionInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    ImprovementSummaryTypeDef,
-    UpdateAnswerInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
-    CreateLensVersionOutputTypeDef,
-    CreateMilestoneOutputTypeDef,
-    CreateWorkloadOutputTypeDef,
-    CreateWorkloadShareOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportLensOutputTypeDef,
-    ImportLensOutputTypeDef,
+    QuestionMetricTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ImprovementSummaryTypeDef,
+    UpdateAnswerInputRequestTypeDef,
+    CreateProfileInputRequestTypeDef,
+    UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
-    WorkloadTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
-    ListLensReviewsOutputTypeDef,
+    LensReviewSummaryTypeDef,
+    WorkloadSummaryTypeDef,
+    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
+    ListProfileNotificationsOutputTypeDef,
+    ListProfileSharesOutputTypeDef,
+    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
-    ListWorkloadsOutputTypeDef,
-    MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
+    ProfileQuestionTypeDef,
+    ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
+    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
+    ListLensReviewsOutputTypeDef,
+    ListWorkloadsOutputTypeDef,
+    MilestoneSummaryTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
-    ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
+    ProfileTypeDef,
+    ProfileTemplateTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
+    LensMetricTypeDef,
+    ListMilestonesOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
+    GetProfileOutputTypeDef,
+    UpdateProfileOutputTypeDef,
+    GetProfileTemplateOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
+    ConsolidatedReportMetricTypeDef,
+    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__main__.py` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WellArchitected 1.26.4\nVersion:         1.26.4\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.WellArchitected 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.4")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.py` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,56 +15,70 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
+    DiscoveryIntegrationStatusType,
     LensStatusTypeType,
     LensTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    ReportFormatType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
     ChoiceUpdateTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
+    GetConsolidatedReportOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
+    GetProfileOutputTypeDef,
+    GetProfileTemplateOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
     ListAnswersOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListLensesOutputTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListLensSharesOutputTypeDef,
     ListMilestonesOutputTypeDef,
     ListNotificationsOutputTypeDef,
+    ListProfileNotificationsOutputTypeDef,
+    ListProfileSharesOutputTypeDef,
+    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
+    ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
+    UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
@@ -112,14 +126,24 @@
         """
         Associate a lens to a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_lenses)
         """
 
+    def associate_profiles(
+        self, *, WorkloadId: str, ProfileArns: Sequence[str]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Associate a profile with a workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_profiles)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#can_paginate)
         """
@@ -163,14 +187,40 @@
         """
         Create a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_milestone)
         """
 
+    def create_profile(
+        self,
+        *,
+        ProfileName: str,
+        ProfileDescription: str,
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
+        ClientRequestToken: str,
+        Tags: Mapping[str, str] = ...
+    ) -> CreateProfileOutputTypeDef:
+        """
+        Create a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile)
+        """
+
+    def create_profile_share(
+        self, *, ProfileArn: str, SharedWith: str, ClientRequestToken: str
+    ) -> CreateProfileShareOutputTypeDef:
+        """
+        Create a profile share.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile_share)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile_share)
+        """
+
     def create_workload(
         self,
         *,
         WorkloadName: str,
         Description: str,
         Environment: WorkloadEnvironmentType,
         Lenses: Sequence[str],
@@ -182,15 +232,16 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...
+        Applications: Sequence[str] = ...,
+        ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload)
         """
@@ -226,14 +277,34 @@
         """
         Delete a lens share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_lens_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_lens_share)
         """
 
+    def delete_profile(
+        self, *, ProfileArn: str, ClientRequestToken: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Delete a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile)
+        """
+
+    def delete_profile_share(
+        self, *, ShareId: str, ProfileArn: str, ClientRequestToken: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Delete a profile share.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile_share)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile_share)
+        """
+
     def delete_workload(
         self, *, WorkloadId: str, ClientRequestToken: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_workload)
@@ -256,14 +327,24 @@
         """
         Disassociate a lens from a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_lenses)
         """
 
+    def disassociate_profiles(
+        self, *, WorkloadId: str, ProfileArns: Sequence[str]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Disassociate a profile from a workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_profiles)
+        """
+
     def export_lens(self, *, LensAlias: str, LensVersion: str = ...) -> ExportLensOutputTypeDef:
         """
         Export an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.export_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#export_lens)
         """
@@ -288,14 +369,29 @@
         """
         Get the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_answer)
         """
 
+    def get_consolidated_report(
+        self,
+        *,
+        Format: ReportFormatType,
+        IncludeSharedResources: bool = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetConsolidatedReportOutputTypeDef:
+        """
+        Get a consolidated report of your workloads.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
+        """
+
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -334,14 +430,30 @@
         """
         Get a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_milestone)
         """
 
+    def get_profile(self, *, ProfileArn: str, ProfileVersion: str = ...) -> GetProfileOutputTypeDef:
+        """
+        Get profile information.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile)
+        """
+
+    def get_profile_template(self) -> GetProfileTemplateOutputTypeDef:
+        """
+        Get profile template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile_template)
+        """
+
     def get_workload(self, *, WorkloadId: str) -> GetWorkloadOutputTypeDef:
         """
         Get an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_workload)
         """
@@ -351,32 +463,33 @@
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> ImportLensOutputTypeDef:
         """
-        Import a new lens.
+        Import a new custom lens or update an existing custom lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
 
     def list_answers(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        QuestionPriority: QuestionPriorityType = ...
     ) -> ListAnswersOutputTypeDef:
         """
-        List of answers.
+        List of answers for a particular workload and lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
 
     def list_check_details(
         self,
@@ -419,15 +532,16 @@
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        QuestionPriority: QuestionPriorityType = ...
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
         List lens review improvements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_review_improvements)
         """
@@ -437,15 +551,15 @@
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLensReviewsOutputTypeDef:
         """
-        List lens reviews.
+        List lens reviews for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
 
     def list_lens_shares(
         self,
@@ -495,22 +609,64 @@
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_notifications)
         """
 
+    def list_profile_notifications(
+        self, *, WorkloadId: str = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> ListProfileNotificationsOutputTypeDef:
+        """
+        List profile notifications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_notifications)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_notifications)
+        """
+
+    def list_profile_shares(
+        self,
+        *,
+        ProfileArn: str,
+        SharedWithPrefix: str = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        Status: ShareStatusType = ...
+    ) -> ListProfileSharesOutputTypeDef:
+        """
+        List profile shares.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_shares)
+        """
+
+    def list_profiles(
+        self,
+        *,
+        ProfileNamePrefix: str = ...,
+        ProfileOwnerType: ProfileOwnerTypeType = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListProfilesOutputTypeDef:
+        """
+        List profiles.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profiles)
+        """
+
     def list_share_invitations(
         self,
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        ProfileNamePrefix: str = ...
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the workload invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_share_invitations)
         """
@@ -539,15 +695,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
 
     def list_workloads(
         self, *, WorkloadNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        List workloads.
+        Paginated list of workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workloads)
         """
 
     def tag_resource(self, *, WorkloadArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
@@ -581,39 +737,56 @@
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
 
     def update_global_settings(
-        self, *, OrganizationSharingStatus: OrganizationSharingStatusType = ...
+        self,
+        *,
+        OrganizationSharingStatus: OrganizationSharingStatusType = ...,
+        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
-        sharing features.
+        sharing and discovery integration features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
 
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
         PillarNotes: Mapping[str, str] = ...
     ) -> UpdateLensReviewOutputTypeDef:
         """
-        Update lens review.
+        Update lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
 
+    def update_profile(
+        self,
+        *,
+        ProfileArn: str,
+        ProfileDescription: str = ...,
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
+    ) -> UpdateProfileOutputTypeDef:
+        """
+        Update a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_profile)
+        """
+
     def update_share_invitation(
         self, *, ShareInvitationId: str, ShareInvitationAction: ShareInvitationActionType
     ) -> UpdateShareInvitationOutputTypeDef:
         """
         Update a workload or custom lens share invitation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_share_invitation)
@@ -658,12 +831,27 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload_share)
         """
 
     def upgrade_lens_review(
         self, *, WorkloadId: str, LensAlias: str, MilestoneName: str, ClientRequestToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Upgrade lens review.
+        Upgrade lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_lens_review)
         """
+
+    def upgrade_profile_version(
+        self,
+        *,
+        WorkloadId: str,
+        ProfileArn: str,
+        MilestoneName: str = ...,
+        ClientRequestToken: str = ...
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Upgrade a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_profile_version)
+        """
```

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.pyi` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/client.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -15,56 +15,70 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
+    DiscoveryIntegrationStatusType,
     LensStatusTypeType,
     LensTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    ReportFormatType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
     ChoiceUpdateTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
+    GetConsolidatedReportOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
+    GetProfileOutputTypeDef,
+    GetProfileTemplateOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
     ListAnswersOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListLensesOutputTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListLensSharesOutputTypeDef,
     ListMilestonesOutputTypeDef,
     ListNotificationsOutputTypeDef,
+    ListProfileNotificationsOutputTypeDef,
+    ListProfileSharesOutputTypeDef,
+    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
+    ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
+    UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
@@ -107,14 +121,23 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associate a lens to a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_lenses)
         """
+    def associate_profiles(
+        self, *, WorkloadId: str, ProfileArns: Sequence[str]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Associate a profile with a workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_profiles)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#can_paginate)
         """
@@ -153,14 +176,38 @@
     ) -> CreateMilestoneOutputTypeDef:
         """
         Create a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_milestone)
         """
+    def create_profile(
+        self,
+        *,
+        ProfileName: str,
+        ProfileDescription: str,
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
+        ClientRequestToken: str,
+        Tags: Mapping[str, str] = ...
+    ) -> CreateProfileOutputTypeDef:
+        """
+        Create a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile)
+        """
+    def create_profile_share(
+        self, *, ProfileArn: str, SharedWith: str, ClientRequestToken: str
+    ) -> CreateProfileShareOutputTypeDef:
+        """
+        Create a profile share.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile_share)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile_share)
+        """
     def create_workload(
         self,
         *,
         WorkloadName: str,
         Description: str,
         Environment: WorkloadEnvironmentType,
         Lenses: Sequence[str],
@@ -172,15 +219,16 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...
+        Applications: Sequence[str] = ...,
+        ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload)
         """
@@ -212,14 +260,32 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a lens share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_lens_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_lens_share)
         """
+    def delete_profile(
+        self, *, ProfileArn: str, ClientRequestToken: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Delete a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile)
+        """
+    def delete_profile_share(
+        self, *, ShareId: str, ProfileArn: str, ClientRequestToken: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Delete a profile share.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile_share)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile_share)
+        """
     def delete_workload(
         self, *, WorkloadId: str, ClientRequestToken: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_workload)
@@ -239,14 +305,23 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disassociate a lens from a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_lenses)
         """
+    def disassociate_profiles(
+        self, *, WorkloadId: str, ProfileArns: Sequence[str]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Disassociate a profile from a workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_profiles)
+        """
     def export_lens(self, *, LensAlias: str, LensVersion: str = ...) -> ExportLensOutputTypeDef:
         """
         Export an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.export_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#export_lens)
         """
@@ -268,14 +343,28 @@
     ) -> GetAnswerOutputTypeDef:
         """
         Get the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_answer)
         """
+    def get_consolidated_report(
+        self,
+        *,
+        Format: ReportFormatType,
+        IncludeSharedResources: bool = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetConsolidatedReportOutputTypeDef:
+        """
+        Get a consolidated report of your workloads.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
+        """
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -309,14 +398,28 @@
     def get_milestone(self, *, WorkloadId: str, MilestoneNumber: int) -> GetMilestoneOutputTypeDef:
         """
         Get a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_milestone)
         """
+    def get_profile(self, *, ProfileArn: str, ProfileVersion: str = ...) -> GetProfileOutputTypeDef:
+        """
+        Get profile information.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile)
+        """
+    def get_profile_template(self) -> GetProfileTemplateOutputTypeDef:
+        """
+        Get profile template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile_template)
+        """
     def get_workload(self, *, WorkloadId: str) -> GetWorkloadOutputTypeDef:
         """
         Get an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_workload)
         """
@@ -325,31 +428,32 @@
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> ImportLensOutputTypeDef:
         """
-        Import a new lens.
+        Import a new custom lens or update an existing custom lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
     def list_answers(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        QuestionPriority: QuestionPriorityType = ...
     ) -> ListAnswersOutputTypeDef:
         """
-        List of answers.
+        List of answers for a particular workload and lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
     def list_check_details(
         self,
         *,
@@ -389,15 +493,16 @@
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        QuestionPriority: QuestionPriorityType = ...
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
         List lens review improvements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_review_improvements)
         """
@@ -406,15 +511,15 @@
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLensReviewsOutputTypeDef:
         """
-        List lens reviews.
+        List lens reviews for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
     def list_lens_shares(
         self,
         *,
@@ -459,22 +564,61 @@
     ) -> ListNotificationsOutputTypeDef:
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_notifications)
         """
+    def list_profile_notifications(
+        self, *, WorkloadId: str = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> ListProfileNotificationsOutputTypeDef:
+        """
+        List profile notifications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_notifications)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_notifications)
+        """
+    def list_profile_shares(
+        self,
+        *,
+        ProfileArn: str,
+        SharedWithPrefix: str = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        Status: ShareStatusType = ...
+    ) -> ListProfileSharesOutputTypeDef:
+        """
+        List profile shares.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_shares)
+        """
+    def list_profiles(
+        self,
+        *,
+        ProfileNamePrefix: str = ...,
+        ProfileOwnerType: ProfileOwnerTypeType = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListProfilesOutputTypeDef:
+        """
+        List profiles.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profiles)
+        """
     def list_share_invitations(
         self,
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        ProfileNamePrefix: str = ...
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the workload invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_share_invitations)
         """
@@ -500,15 +644,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
     def list_workloads(
         self, *, WorkloadNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        List workloads.
+        Paginated list of workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workloads)
         """
     def tag_resource(self, *, WorkloadArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to the specified resource.
@@ -538,37 +682,53 @@
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
     def update_global_settings(
-        self, *, OrganizationSharingStatus: OrganizationSharingStatusType = ...
+        self,
+        *,
+        OrganizationSharingStatus: OrganizationSharingStatusType = ...,
+        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
-        sharing features.
+        sharing and discovery integration features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
         PillarNotes: Mapping[str, str] = ...
     ) -> UpdateLensReviewOutputTypeDef:
         """
-        Update lens review.
+        Update lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
+    def update_profile(
+        self,
+        *,
+        ProfileArn: str,
+        ProfileDescription: str = ...,
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
+    ) -> UpdateProfileOutputTypeDef:
+        """
+        Update a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_profile)
+        """
     def update_share_invitation(
         self, *, ShareInvitationId: str, ShareInvitationAction: ShareInvitationActionType
     ) -> UpdateShareInvitationOutputTypeDef:
         """
         Update a workload or custom lens share invitation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_share_invitation)
@@ -610,12 +770,26 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload_share)
         """
     def upgrade_lens_review(
         self, *, WorkloadId: str, LensAlias: str, MilestoneName: str, ClientRequestToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Upgrade lens review.
+        Upgrade lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_lens_review)
         """
+    def upgrade_profile_version(
+        self,
+        *,
+        WorkloadId: str,
+        ProfileArn: str,
+        MilestoneName: str = ...,
+        ClientRequestToken: str = ...
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Upgrade a profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_profile_version)
+        """
```

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.py` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/literals.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -14,69 +14,83 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
+    "DefinitionTypeType",
     "DifferenceStatusType",
+    "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
+    "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
+    "ProfileNotificationTypeType",
+    "ProfileOwnerTypeType",
+    "QuestionPriorityType",
+    "QuestionTypeType",
+    "ReportFormatType",
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
 CheckProviderType = Literal["TRUSTED_ADVISOR"]
 CheckStatusType = Literal["ERROR", "FETCH_FAILED", "NOT_AVAILABLE", "OKAY", "WARNING"]
 ChoiceReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
+DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
+DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
+MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
+ProfileNotificationTypeType = Literal["PROFILE_ANSWERS_UPDATED", "PROFILE_DELETED"]
+ProfileOwnerTypeType = Literal["SELF", "SHARED"]
+QuestionPriorityType = Literal["NONE", "PRIORITIZED"]
+QuestionTypeType = Literal["NON_PRIORITIZED", "PRIORITIZED"]
+ReportFormatType = Literal["JSON", "PDF"]
 RiskType = Literal["HIGH", "MEDIUM", "NONE", "NOT_APPLICABLE", "UNANSWERED"]
 ShareInvitationActionType = Literal["ACCEPT", "REJECT"]
-ShareResourceTypeType = Literal["LENS", "WORKLOAD"]
+ShareResourceTypeType = Literal["LENS", "PROFILE", "WORKLOAD"]
 ShareStatusType = Literal[
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 WorkloadEnvironmentType = Literal["PREPRODUCTION", "PRODUCTION"]
 WorkloadImprovementStatusType = Literal[
     "COMPLETE", "IN_PROGRESS", "NOT_APPLICABLE", "NOT_STARTED", "RISK_ACKNOWLEDGED"
@@ -93,23 +107,25 @@
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
@@ -119,30 +135,35 @@
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
@@ -168,14 +189,15 @@
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
@@ -220,51 +242,57 @@
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
@@ -277,14 +305,15 @@
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
@@ -296,28 +325,35 @@
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
@@ -326,14 +362,15 @@
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
@@ -344,55 +381,64 @@
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

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.pyi` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/literals.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,67 +14,85 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
+    "DefinitionTypeType",
     "DifferenceStatusType",
+    "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
+    "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
+    "ProfileNotificationTypeType",
+    "ProfileOwnerTypeType",
+    "QuestionPriorityType",
+    "QuestionTypeType",
+    "ReportFormatType",
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
 CheckProviderType = Literal["TRUSTED_ADVISOR"]
 CheckStatusType = Literal["ERROR", "FETCH_FAILED", "NOT_AVAILABLE", "OKAY", "WARNING"]
 ChoiceReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
+DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
+DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
+MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
+ProfileNotificationTypeType = Literal["PROFILE_ANSWERS_UPDATED", "PROFILE_DELETED"]
+ProfileOwnerTypeType = Literal["SELF", "SHARED"]
+QuestionPriorityType = Literal["NONE", "PRIORITIZED"]
+QuestionTypeType = Literal["NON_PRIORITIZED", "PRIORITIZED"]
+ReportFormatType = Literal["JSON", "PDF"]
 RiskType = Literal["HIGH", "MEDIUM", "NONE", "NOT_APPLICABLE", "UNANSWERED"]
 ShareInvitationActionType = Literal["ACCEPT", "REJECT"]
-ShareResourceTypeType = Literal["LENS", "WORKLOAD"]
+ShareResourceTypeType = Literal["LENS", "PROFILE", "WORKLOAD"]
 ShareStatusType = Literal[
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 WorkloadEnvironmentType = Literal["PREPRODUCTION", "PRODUCTION"]
 WorkloadImprovementStatusType = Literal[
     "COMPLETE", "IN_PROGRESS", "NOT_APPLICABLE", "NOT_STARTED", "RISK_ACKNOWLEDGED"
@@ -91,23 +109,25 @@
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
@@ -117,30 +137,35 @@
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
@@ -166,14 +191,15 @@
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
@@ -218,51 +244,57 @@
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
@@ -275,14 +307,15 @@
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
@@ -294,28 +327,35 @@
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
@@ -324,14 +364,15 @@
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
@@ -342,55 +383,64 @@
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

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.py` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -18,22 +18,29 @@
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
+    DefinitionTypeType,
     DifferenceStatusType,
+    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileNotificationTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    QuestionTypeType,
+    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -44,125 +51,162 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
+    "AssociateProfilesInputRequestTypeDef",
+    "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateLensShareOutputTypeDef",
     "CreateLensVersionInputRequestTypeDef",
+    "CreateLensVersionOutputTypeDef",
     "CreateMilestoneInputRequestTypeDef",
+    "CreateMilestoneOutputTypeDef",
+    "ProfileQuestionUpdateTypeDef",
+    "CreateProfileOutputTypeDef",
+    "CreateProfileShareInputRequestTypeDef",
+    "CreateProfileShareOutputTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
+    "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
+    "CreateWorkloadShareOutputTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
+    "DeleteProfileInputRequestTypeDef",
+    "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
+    "DisassociateProfilesInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportLensInputRequestTypeDef",
+    "ExportLensOutputTypeDef",
     "GetAnswerInputRequestTypeDef",
+    "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
+    "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "LensReviewSummaryTypeDef",
+    "ImportLensOutputTypeDef",
+    "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
     "ListCheckSummariesInputRequestTypeDef",
     "ListLensReviewImprovementsInputRequestTypeDef",
     "ListLensReviewsInputRequestTypeDef",
     "ListLensSharesInputRequestTypeDef",
     "ListLensesInputRequestTypeDef",
     "ListMilestonesInputRequestTypeDef",
     "ListNotificationsInputRequestTypeDef",
+    "ListProfileNotificationsInputRequestTypeDef",
+    "ProfileNotificationSummaryTypeDef",
+    "ListProfileSharesInputRequestTypeDef",
+    "ProfileShareSummaryTypeDef",
+    "ListProfilesInputRequestTypeDef",
+    "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
-    "WorkloadSummaryTypeDef",
     "QuestionDifferenceTypeDef",
+    "ProfileChoiceTypeDef",
+    "ProfileTemplateChoiceTypeDef",
+    "ResponseMetadataTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
+    "UpgradeProfileVersionInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
-    "ImprovementSummaryTypeDef",
-    "UpdateAnswerInputRequestTypeDef",
-    "CreateLensShareOutputTypeDef",
-    "CreateLensVersionOutputTypeDef",
-    "CreateMilestoneOutputTypeDef",
-    "CreateWorkloadOutputTypeDef",
-    "CreateWorkloadShareOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportLensOutputTypeDef",
-    "ImportLensOutputTypeDef",
+    "QuestionMetricTypeDef",
     "ListCheckDetailsOutputTypeDef",
     "ListCheckSummariesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
+    "ImprovementSummaryTypeDef",
+    "UpdateAnswerInputRequestTypeDef",
+    "CreateProfileInputRequestTypeDef",
+    "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
-    "WorkloadTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
-    "ListLensReviewsOutputTypeDef",
+    "LensReviewSummaryTypeDef",
+    "WorkloadSummaryTypeDef",
+    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
+    "ListProfileNotificationsOutputTypeDef",
+    "ListProfileSharesOutputTypeDef",
+    "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
-    "ListWorkloadsOutputTypeDef",
-    "MilestoneSummaryTypeDef",
     "PillarDifferenceTypeDef",
+    "ProfileQuestionTypeDef",
+    "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
     "ChoiceTypeDef",
+    "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
+    "ListLensReviewsOutputTypeDef",
+    "ListWorkloadsOutputTypeDef",
+    "MilestoneSummaryTypeDef",
     "GetWorkloadOutputTypeDef",
     "MilestoneTypeDef",
     "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
-    "ListMilestonesOutputTypeDef",
     "VersionDifferencesTypeDef",
+    "ProfileTypeDef",
+    "ProfileTemplateTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
+    "LensMetricTypeDef",
+    "ListMilestonesOutputTypeDef",
     "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
+    "GetProfileOutputTypeDef",
+    "UpdateProfileOutputTypeDef",
+    "GetProfileTemplateOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
+    "ConsolidatedReportMetricTypeDef",
+    "GetConsolidatedReportOutputTypeDef",
 )
 
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": str,
         "Url": str,
@@ -195,14 +239,31 @@
     "AssociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
+AssociateProfilesInputRequestTypeDef = TypedDict(
+    "AssociateProfilesInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "ProfileArns": Sequence[str],
+    },
+)
+
+BestPracticeTypeDef = TypedDict(
+    "BestPracticeTypeDef",
+    {
+        "ChoiceId": str,
+        "ChoiceTitle": str,
+    },
+    total=False,
+)
+
 CheckDetailTypeDef = TypedDict(
     "CheckDetailTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Provider": Literal["TRUSTED_ADVISOR"],
@@ -258,36 +319,31 @@
     {
         "Reason": ChoiceReasonType,
         "Notes": str,
     },
     total=False,
 )
 
-
 class ChoiceUpdateTypeDef(_RequiredChoiceUpdateTypeDef, _OptionalChoiceUpdateTypeDef):
     pass
 
-
 CreateLensShareInputRequestTypeDef = TypedDict(
     "CreateLensShareInputRequestTypeDef",
     {
         "LensAlias": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLensShareOutputTypeDef = TypedDict(
+    "CreateLensShareOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ShareId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLensVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
@@ -299,48 +355,119 @@
     "_OptionalCreateLensVersionInputRequestTypeDef",
     {
         "IsMajorVersion": bool,
     },
     total=False,
 )
 
-
 class CreateLensVersionInputRequestTypeDef(
     _RequiredCreateLensVersionInputRequestTypeDef, _OptionalCreateLensVersionInputRequestTypeDef
 ):
     pass
 
+CreateLensVersionOutputTypeDef = TypedDict(
+    "CreateLensVersionOutputTypeDef",
+    {
+        "LensArn": str,
+        "LensVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CreateMilestoneInputRequestTypeDef = TypedDict(
     "CreateMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
+CreateMilestoneOutputTypeDef = TypedDict(
+    "CreateMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProfileQuestionUpdateTypeDef = TypedDict(
+    "ProfileQuestionUpdateTypeDef",
+    {
+        "QuestionId": str,
+        "SelectedChoiceIds": Sequence[str],
+    },
+    total=False,
+)
+
+CreateProfileOutputTypeDef = TypedDict(
+    "CreateProfileOutputTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProfileShareInputRequestTypeDef = TypedDict(
+    "CreateProfileShareInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+        "SharedWith": str,
+        "ClientRequestToken": str,
+    },
+)
+
+CreateProfileShareOutputTypeDef = TypedDict(
+    "CreateProfileShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
+        "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
+CreateWorkloadOutputTypeDef = TypedDict(
+    "CreateWorkloadOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
     },
 )
 
+CreateWorkloadShareOutputTypeDef = TypedDict(
+    "CreateWorkloadShareOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "ShareId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLensInputRequestTypeDef = TypedDict(
     "DeleteLensInputRequestTypeDef",
     {
         "LensAlias": str,
         "ClientRequestToken": str,
         "LensStatus": LensStatusTypeType,
     },
@@ -351,14 +478,31 @@
     {
         "ShareId": str,
         "LensAlias": str,
         "ClientRequestToken": str,
     },
 )
 
+DeleteProfileInputRequestTypeDef = TypedDict(
+    "DeleteProfileInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+        "ClientRequestToken": str,
+    },
+)
+
+DeleteProfileShareInputRequestTypeDef = TypedDict(
+    "DeleteProfileShareInputRequestTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ClientRequestToken": str,
+    },
+)
+
 DeleteWorkloadInputRequestTypeDef = TypedDict(
     "DeleteWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ClientRequestToken": str,
     },
 )
@@ -376,34 +520,55 @@
     "DisassociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
+DisassociateProfilesInputRequestTypeDef = TypedDict(
+    "DisassociateProfilesInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "ProfileArns": Sequence[str],
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
     "_OptionalExportLensInputRequestTypeDef",
     {
         "LensVersion": str,
     },
     total=False,
 )
 
-
 class ExportLensInputRequestTypeDef(
     _RequiredExportLensInputRequestTypeDef, _OptionalExportLensInputRequestTypeDef
 ):
     pass
 
+ExportLensOutputTypeDef = TypedDict(
+    "ExportLensOutputTypeDef",
+    {
+        "LensJSON": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetAnswerInputRequestTypeDef = TypedDict(
     "_RequiredGetAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "QuestionId": str,
@@ -413,20 +578,40 @@
     "_OptionalGetAnswerInputRequestTypeDef",
     {
         "MilestoneNumber": int,
     },
     total=False,
 )
 
-
 class GetAnswerInputRequestTypeDef(
     _RequiredGetAnswerInputRequestTypeDef, _OptionalGetAnswerInputRequestTypeDef
 ):
     pass
 
+_RequiredGetConsolidatedReportInputRequestTypeDef = TypedDict(
+    "_RequiredGetConsolidatedReportInputRequestTypeDef",
+    {
+        "Format": ReportFormatType,
+    },
+)
+_OptionalGetConsolidatedReportInputRequestTypeDef = TypedDict(
+    "_OptionalGetConsolidatedReportInputRequestTypeDef",
+    {
+        "IncludeSharedResources": bool,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetConsolidatedReportInputRequestTypeDef(
+    _RequiredGetConsolidatedReportInputRequestTypeDef,
+    _OptionalGetConsolidatedReportInputRequestTypeDef,
+):
+    pass
 
 _RequiredGetLensInputRequestTypeDef = TypedDict(
     "_RequiredGetLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
@@ -434,21 +619,19 @@
     "_OptionalGetLensInputRequestTypeDef",
     {
         "LensVersion": str,
     },
     total=False,
 )
 
-
 class GetLensInputRequestTypeDef(
     _RequiredGetLensInputRequestTypeDef, _OptionalGetLensInputRequestTypeDef
 ):
     pass
 
-
 LensTypeDef = TypedDict(
     "LensTypeDef",
     {
         "LensArn": str,
         "LensVersion": str,
         "Name": str,
         "Description": str,
@@ -470,21 +653,19 @@
     "_OptionalGetLensReviewInputRequestTypeDef",
     {
         "MilestoneNumber": int,
     },
     total=False,
 )
 
-
 class GetLensReviewInputRequestTypeDef(
     _RequiredGetLensReviewInputRequestTypeDef, _OptionalGetLensReviewInputRequestTypeDef
 ):
     pass
 
-
 _RequiredGetLensReviewReportInputRequestTypeDef = TypedDict(
     "_RequiredGetLensReviewReportInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
     },
 )
@@ -492,21 +673,19 @@
     "_OptionalGetLensReviewReportInputRequestTypeDef",
     {
         "MilestoneNumber": int,
     },
     total=False,
 )
 
-
 class GetLensReviewReportInputRequestTypeDef(
     _RequiredGetLensReviewReportInputRequestTypeDef, _OptionalGetLensReviewReportInputRequestTypeDef
 ):
     pass
 
-
 LensReviewReportTypeDef = TypedDict(
     "LensReviewReportTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "Base64String": str,
     },
@@ -524,30 +703,47 @@
     {
         "BaseLensVersion": str,
         "TargetLensVersion": str,
     },
     total=False,
 )
 
-
 class GetLensVersionDifferenceInputRequestTypeDef(
     _RequiredGetLensVersionDifferenceInputRequestTypeDef,
     _OptionalGetLensVersionDifferenceInputRequestTypeDef,
 ):
     pass
 
-
 GetMilestoneInputRequestTypeDef = TypedDict(
     "GetMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
     },
 )
 
+_RequiredGetProfileInputRequestTypeDef = TypedDict(
+    "_RequiredGetProfileInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+    },
+)
+_OptionalGetProfileInputRequestTypeDef = TypedDict(
+    "_OptionalGetProfileInputRequestTypeDef",
+    {
+        "ProfileVersion": str,
+    },
+    total=False,
+)
+
+class GetProfileInputRequestTypeDef(
+    _RequiredGetProfileInputRequestTypeDef, _OptionalGetProfileInputRequestTypeDef
+):
+    pass
+
 GetWorkloadInputRequestTypeDef = TypedDict(
     "GetWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 
@@ -563,42 +759,45 @@
     {
         "LensAlias": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
-
-LensReviewSummaryTypeDef = TypedDict(
-    "LensReviewSummaryTypeDef",
+ImportLensOutputTypeDef = TypedDict(
+    "ImportLensOutputTypeDef",
     {
-        "LensAlias": str,
         "LensArn": str,
-        "LensVersion": str,
-        "LensName": str,
-        "LensStatus": LensStatusType,
-        "UpdatedAt": datetime,
-        "RiskCounts": Dict[RiskType, int],
+        "Status": ImportLensStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+WorkloadProfileTypeDef = TypedDict(
+    "WorkloadProfileTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
     },
     total=False,
 )
 
 PillarReviewSummaryTypeDef = TypedDict(
     "PillarReviewSummaryTypeDef",
     {
         "PillarId": str,
         "PillarName": str,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 LensShareSummaryTypeDef = TypedDict(
     "LensShareSummaryTypeDef",
     {
@@ -650,25 +849,24 @@
 _OptionalListAnswersInputRequestTypeDef = TypedDict(
     "_OptionalListAnswersInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
+        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
-
 class ListAnswersInputRequestTypeDef(
     _RequiredListAnswersInputRequestTypeDef, _OptionalListAnswersInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListCheckDetailsInputRequestTypeDef = TypedDict(
     "_RequiredListCheckDetailsInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensArn": str,
         "PillarId": str,
         "QuestionId": str,
@@ -680,21 +878,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListCheckDetailsInputRequestTypeDef(
     _RequiredListCheckDetailsInputRequestTypeDef, _OptionalListCheckDetailsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListCheckSummariesInputRequestTypeDef = TypedDict(
     "_RequiredListCheckSummariesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensArn": str,
         "PillarId": str,
         "QuestionId": str,
@@ -706,47 +902,44 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListCheckSummariesInputRequestTypeDef(
     _RequiredListCheckSummariesInputRequestTypeDef, _OptionalListCheckSummariesInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListLensReviewImprovementsInputRequestTypeDef = TypedDict(
     "_RequiredListLensReviewImprovementsInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
     },
 )
 _OptionalListLensReviewImprovementsInputRequestTypeDef = TypedDict(
     "_OptionalListLensReviewImprovementsInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
+        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
-
 class ListLensReviewImprovementsInputRequestTypeDef(
     _RequiredListLensReviewImprovementsInputRequestTypeDef,
     _OptionalListLensReviewImprovementsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLensReviewsInputRequestTypeDef = TypedDict(
     "_RequiredListLensReviewsInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListLensReviewsInputRequestTypeDef = TypedDict(
@@ -755,21 +948,19 @@
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLensReviewsInputRequestTypeDef(
     _RequiredListLensReviewsInputRequestTypeDef, _OptionalListLensReviewsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListLensSharesInputRequestTypeDef = TypedDict(
     "_RequiredListLensSharesInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalListLensSharesInputRequestTypeDef = TypedDict(
@@ -779,21 +970,19 @@
         "NextToken": str,
         "MaxResults": int,
         "Status": ShareStatusType,
     },
     total=False,
 )
 
-
 class ListLensSharesInputRequestTypeDef(
     _RequiredListLensSharesInputRequestTypeDef, _OptionalListLensSharesInputRequestTypeDef
 ):
     pass
 
-
 ListLensesInputRequestTypeDef = TypedDict(
     "ListLensesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "LensType": LensTypeType,
         "LensStatus": LensStatusTypeType,
@@ -813,39 +1002,120 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMilestonesInputRequestTypeDef(
     _RequiredListMilestonesInputRequestTypeDef, _OptionalListMilestonesInputRequestTypeDef
 ):
     pass
 
-
 ListNotificationsInputRequestTypeDef = TypedDict(
     "ListNotificationsInputRequestTypeDef",
     {
         "WorkloadId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListProfileNotificationsInputRequestTypeDef = TypedDict(
+    "ListProfileNotificationsInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ProfileNotificationSummaryTypeDef = TypedDict(
+    "ProfileNotificationSummaryTypeDef",
+    {
+        "CurrentProfileVersion": str,
+        "LatestProfileVersion": str,
+        "Type": ProfileNotificationTypeType,
+        "ProfileArn": str,
+        "ProfileName": str,
+        "WorkloadId": str,
+        "WorkloadName": str,
+    },
+    total=False,
+)
+
+_RequiredListProfileSharesInputRequestTypeDef = TypedDict(
+    "_RequiredListProfileSharesInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+    },
+)
+_OptionalListProfileSharesInputRequestTypeDef = TypedDict(
+    "_OptionalListProfileSharesInputRequestTypeDef",
+    {
+        "SharedWithPrefix": str,
+        "NextToken": str,
+        "MaxResults": int,
+        "Status": ShareStatusType,
+    },
+    total=False,
+)
+
+class ListProfileSharesInputRequestTypeDef(
+    _RequiredListProfileSharesInputRequestTypeDef, _OptionalListProfileSharesInputRequestTypeDef
+):
+    pass
+
+ProfileShareSummaryTypeDef = TypedDict(
+    "ProfileShareSummaryTypeDef",
+    {
+        "ShareId": str,
+        "SharedWith": str,
+        "Status": ShareStatusType,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
+ListProfilesInputRequestTypeDef = TypedDict(
+    "ListProfilesInputRequestTypeDef",
+    {
+        "ProfileNamePrefix": str,
+        "ProfileOwnerType": ProfileOwnerTypeType,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ProfileSummaryTypeDef = TypedDict(
+    "ProfileSummaryTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ProfileName": str,
+        "ProfileDescription": str,
+        "Owner": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+    },
+    total=False,
+)
+
 ListShareInvitationsInputRequestTypeDef = TypedDict(
     "ListShareInvitationsInputRequestTypeDef",
     {
         "WorkloadNamePrefix": str,
         "LensNamePrefix": str,
         "ShareResourceType": ShareResourceTypeType,
         "NextToken": str,
         "MaxResults": int,
+        "ProfileNamePrefix": str,
     },
     total=False,
 )
 
 ShareInvitationSummaryTypeDef = TypedDict(
     "ShareInvitationSummaryTypeDef",
     {
@@ -854,25 +1124,35 @@
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadName": str,
         "WorkloadId": str,
         "LensName": str,
         "LensArn": str,
+        "ProfileName": str,
+        "ProfileArn": str,
     },
     total=False,
 )
 
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListWorkloadSharesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkloadSharesInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListWorkloadSharesInputRequestTypeDef = TypedDict(
@@ -882,21 +1162,19 @@
         "NextToken": str,
         "MaxResults": int,
         "Status": ShareStatusType,
     },
     total=False,
 )
 
-
 class ListWorkloadSharesInputRequestTypeDef(
     _RequiredListWorkloadSharesInputRequestTypeDef, _OptionalListWorkloadSharesInputRequestTypeDef
 ):
     pass
 
-
 WorkloadShareSummaryTypeDef = TypedDict(
     "WorkloadShareSummaryTypeDef",
     {
         "ShareId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "Status": ShareStatusType,
@@ -911,47 +1189,64 @@
         "WorkloadNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-WorkloadSummaryTypeDef = TypedDict(
-    "WorkloadSummaryTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Owner": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[str],
-        "RiskCounts": Dict[RiskType, int],
-        "ImprovementStatus": WorkloadImprovementStatusType,
-    },
-    total=False,
-)
-
 QuestionDifferenceTypeDef = TypedDict(
     "QuestionDifferenceTypeDef",
     {
         "QuestionId": str,
         "QuestionTitle": str,
         "DifferenceStatus": DifferenceStatusType,
     },
     total=False,
 )
 
+ProfileChoiceTypeDef = TypedDict(
+    "ProfileChoiceTypeDef",
+    {
+        "ChoiceId": str,
+        "ChoiceTitle": str,
+        "ChoiceDescription": str,
+    },
+    total=False,
+)
+
+ProfileTemplateChoiceTypeDef = TypedDict(
+    "ProfileTemplateChoiceTypeDef",
+    {
+        "ChoiceId": str,
+        "ChoiceTitle": str,
+        "ChoiceDescription": str,
+    },
+    total=False,
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
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
+        "ProfileArn": str,
     },
     total=False,
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
@@ -968,14 +1263,15 @@
     },
 )
 
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "OrganizationSharingStatus": OrganizationSharingStatusType,
+        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
     },
     total=False,
 )
 
 _RequiredUpdateLensReviewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateLensReviewInputRequestTypeDef",
     {
@@ -988,21 +1284,19 @@
     {
         "LensNotes": str,
         "PillarNotes": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdateLensReviewInputRequestTypeDef(
     _RequiredUpdateLensReviewInputRequestTypeDef, _OptionalUpdateLensReviewInputRequestTypeDef
 ):
     pass
 
-
 UpdateShareInvitationInputRequestTypeDef = TypedDict(
     "UpdateShareInvitationInputRequestTypeDef",
     {
         "ShareInvitationId": str,
         "ShareInvitationAction": ShareInvitationActionType,
     },
 )
@@ -1042,30 +1336,78 @@
     "_OptionalUpgradeLensReviewInputRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpgradeLensReviewInputRequestTypeDef(
     _RequiredUpgradeLensReviewInputRequestTypeDef, _OptionalUpgradeLensReviewInputRequestTypeDef
 ):
     pass
 
+_RequiredUpgradeProfileVersionInputRequestTypeDef = TypedDict(
+    "_RequiredUpgradeProfileVersionInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "ProfileArn": str,
+    },
+)
+_OptionalUpgradeProfileVersionInputRequestTypeDef = TypedDict(
+    "_OptionalUpgradeProfileVersionInputRequestTypeDef",
+    {
+        "MilestoneName": str,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class UpgradeProfileVersionInputRequestTypeDef(
+    _RequiredUpgradeProfileVersionInputRequestTypeDef,
+    _OptionalUpgradeProfileVersionInputRequestTypeDef,
+):
+    pass
 
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
 )
 
+QuestionMetricTypeDef = TypedDict(
+    "QuestionMetricTypeDef",
+    {
+        "QuestionId": str,
+        "Risk": RiskType,
+        "BestPractices": List[BestPracticeTypeDef],
+    },
+    total=False,
+)
+
+ListCheckDetailsOutputTypeDef = TypedDict(
+    "ListCheckDetailsOutputTypeDef",
+    {
+        "CheckDetails": List[CheckDetailTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCheckSummariesOutputTypeDef = TypedDict(
+    "ListCheckSummariesOutputTypeDef",
+    {
+        "CheckSummaries": List[CheckSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1091,114 +1433,60 @@
         "Notes": str,
         "IsApplicable": bool,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
-
 class UpdateAnswerInputRequestTypeDef(
     _RequiredUpdateAnswerInputRequestTypeDef, _OptionalUpdateAnswerInputRequestTypeDef
 ):
     pass
 
-
-CreateLensShareOutputTypeDef = TypedDict(
-    "CreateLensShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLensVersionOutputTypeDef = TypedDict(
-    "CreateLensVersionOutputTypeDef",
+_RequiredCreateProfileInputRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileInputRequestTypeDef",
     {
-        "LensArn": str,
-        "LensVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMilestoneOutputTypeDef = TypedDict(
-    "CreateMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkloadOutputTypeDef = TypedDict(
-    "CreateWorkloadOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkloadShareOutputTypeDef = TypedDict(
-    "CreateWorkloadShareOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "ShareId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProfileName": str,
+        "ProfileDescription": str,
+        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
+        "ClientRequestToken": str,
     },
 )
-
-ExportLensOutputTypeDef = TypedDict(
-    "ExportLensOutputTypeDef",
+_OptionalCreateProfileInputRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileInputRequestTypeDef",
     {
-        "LensJSON": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
-ImportLensOutputTypeDef = TypedDict(
-    "ImportLensOutputTypeDef",
-    {
-        "LensArn": str,
-        "Status": ImportLensStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class CreateProfileInputRequestTypeDef(
+    _RequiredCreateProfileInputRequestTypeDef, _OptionalCreateProfileInputRequestTypeDef
+):
+    pass
 
-ListCheckDetailsOutputTypeDef = TypedDict(
-    "ListCheckDetailsOutputTypeDef",
+_RequiredUpdateProfileInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateProfileInputRequestTypeDef",
     {
-        "CheckDetails": List[CheckDetailTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProfileArn": str,
     },
 )
-
-ListCheckSummariesOutputTypeDef = TypedDict(
-    "ListCheckSummariesOutputTypeDef",
+_OptionalUpdateProfileInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateProfileInputRequestTypeDef",
     {
-        "CheckSummaries": List[CheckSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProfileDescription": str,
+        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
     },
+    total=False,
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateProfileInputRequestTypeDef(
+    _RequiredUpdateProfileInputRequestTypeDef, _OptionalUpdateProfileInputRequestTypeDef
+):
+    pass
 
 _RequiredCreateWorkloadInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkloadInputRequestTypeDef",
     {
         "WorkloadName": str,
         "Description": str,
         "Environment": WorkloadEnvironmentType,
@@ -1217,25 +1505,24 @@
         "ReviewOwner": str,
         "IndustryType": str,
         "Industry": str,
         "Notes": str,
         "Tags": Mapping[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": Sequence[str],
+        "ProfileArns": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateWorkloadInputRequestTypeDef(
     _RequiredCreateWorkloadInputRequestTypeDef, _OptionalCreateWorkloadInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateWorkloadInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalUpdateWorkloadInputRequestTypeDef = TypedDict(
@@ -1257,20 +1544,69 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateWorkloadInputRequestTypeDef(
     _RequiredUpdateWorkloadInputRequestTypeDef, _OptionalUpdateWorkloadInputRequestTypeDef
 ):
     pass
 
+GetLensOutputTypeDef = TypedDict(
+    "GetLensOutputTypeDef",
+    {
+        "Lens": LensTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLensReviewReportOutputTypeDef = TypedDict(
+    "GetLensReviewReportOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewReport": LensReviewReportTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+LensReviewSummaryTypeDef = TypedDict(
+    "LensReviewSummaryTypeDef",
+    {
+        "LensAlias": str,
+        "LensArn": str,
+        "LensVersion": str,
+        "LensName": str,
+        "LensStatus": LensStatusType,
+        "UpdatedAt": datetime,
+        "RiskCounts": Dict[RiskType, int],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
+WorkloadSummaryTypeDef = TypedDict(
+    "WorkloadSummaryTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Owner": str,
+        "UpdatedAt": datetime,
+        "Lenses": List[str],
+        "RiskCounts": Dict[RiskType, int],
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
 
 WorkloadTypeDef = TypedDict(
     "WorkloadTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "WorkloadName": str,
@@ -1292,155 +1628,164 @@
         "PillarPriorities": List[str],
         "Lenses": List[str],
         "Owner": str,
         "ShareInvitationId": str,
         "Tags": Dict[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
-GetLensOutputTypeDef = TypedDict(
-    "GetLensOutputTypeDef",
-    {
-        "Lens": LensTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLensReviewReportOutputTypeDef = TypedDict(
-    "GetLensReviewReportOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListLensReviewsOutputTypeDef = TypedDict(
-    "ListLensReviewsOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
         "LensStatus": LensStatusType,
         "PillarReviewSummaries": List[PillarReviewSummaryTypeDef],
         "UpdatedAt": datetime,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
         "NextToken": str,
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLensesOutputTypeDef = TypedDict(
     "ListLensesOutputTypeDef",
     {
         "LensSummaries": List[LensSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationSummaryTypeDef = TypedDict(
     "NotificationSummaryTypeDef",
     {
         "Type": NotificationTypeType,
         "LensUpgradeSummary": LensUpgradeSummaryTypeDef,
     },
     total=False,
 )
 
+ListProfileNotificationsOutputTypeDef = TypedDict(
+    "ListProfileNotificationsOutputTypeDef",
+    {
+        "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProfileSharesOutputTypeDef = TypedDict(
+    "ListProfileSharesOutputTypeDef",
+    {
+        "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProfilesOutputTypeDef = TypedDict(
+    "ListProfilesOutputTypeDef",
+    {
+        "ProfileSummaries": List[ProfileSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkloadSharesOutputTypeDef = TypedDict(
     "ListWorkloadSharesOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListWorkloadsOutputTypeDef = TypedDict(
-    "ListWorkloadsOutputTypeDef",
+PillarDifferenceTypeDef = TypedDict(
+    "PillarDifferenceTypeDef",
     {
-        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PillarId": str,
+        "PillarName": str,
+        "DifferenceStatus": DifferenceStatusType,
+        "QuestionDifferences": List[QuestionDifferenceTypeDef],
     },
+    total=False,
 )
 
-MilestoneSummaryTypeDef = TypedDict(
-    "MilestoneSummaryTypeDef",
+ProfileQuestionTypeDef = TypedDict(
+    "ProfileQuestionTypeDef",
     {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "WorkloadSummary": WorkloadSummaryTypeDef,
+        "QuestionId": str,
+        "QuestionTitle": str,
+        "QuestionDescription": str,
+        "QuestionChoices": List[ProfileChoiceTypeDef],
+        "SelectedChoiceIds": List[str],
+        "MinSelectedChoices": int,
+        "MaxSelectedChoices": int,
     },
     total=False,
 )
 
-PillarDifferenceTypeDef = TypedDict(
-    "PillarDifferenceTypeDef",
+ProfileTemplateQuestionTypeDef = TypedDict(
+    "ProfileTemplateQuestionTypeDef",
     {
-        "PillarId": str,
-        "PillarName": str,
-        "DifferenceStatus": DifferenceStatusType,
-        "QuestionDifferences": List[QuestionDifferenceTypeDef],
+        "QuestionId": str,
+        "QuestionTitle": str,
+        "QuestionDescription": str,
+        "QuestionChoices": List[ProfileTemplateChoiceTypeDef],
+        "MinSelectedChoices": int,
+        "MaxSelectedChoices": int,
     },
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
         "ShareInvitation": ShareInvitationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWorkloadShareOutputTypeDef = TypedDict(
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
@@ -1449,32 +1794,73 @@
         "HelpfulResource": ChoiceContentTypeDef,
         "ImprovementPlan": ChoiceContentTypeDef,
         "AdditionalResources": List[AdditionalResourcesTypeDef],
     },
     total=False,
 )
 
+PillarMetricTypeDef = TypedDict(
+    "PillarMetricTypeDef",
+    {
+        "PillarId": str,
+        "RiskCounts": Dict[RiskType, int],
+        "Questions": List[QuestionMetricTypeDef],
+    },
+    total=False,
+)
+
 ListLensReviewImprovementsOutputTypeDef = TypedDict(
     "ListLensReviewImprovementsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListLensReviewsOutputTypeDef = TypedDict(
+    "ListLensReviewsOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListWorkloadsOutputTypeDef = TypedDict(
+    "ListWorkloadsOutputTypeDef",
+    {
+        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+MilestoneSummaryTypeDef = TypedDict(
+    "MilestoneSummaryTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "WorkloadSummary": WorkloadSummaryTypeDef,
+    },
+    total=False,
+)
+
 GetWorkloadOutputTypeDef = TypedDict(
     "GetWorkloadOutputTypeDef",
     {
         "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MilestoneTypeDef = TypedDict(
     "MilestoneTypeDef",
     {
         "MilestoneNumber": int,
@@ -1485,60 +1871,78 @@
     total=False,
 )
 
 UpdateWorkloadOutputTypeDef = TypedDict(
     "UpdateWorkloadOutputTypeDef",
     {
         "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLensReviewOutputTypeDef = TypedDict(
     "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMilestonesOutputTypeDef = TypedDict(
-    "ListMilestonesOutputTypeDef",
+VersionDifferencesTypeDef = TypedDict(
+    "VersionDifferencesTypeDef",
     {
-        "WorkloadId": str,
-        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PillarDifferences": List[PillarDifferenceTypeDef],
     },
+    total=False,
 )
 
-VersionDifferencesTypeDef = TypedDict(
-    "VersionDifferencesTypeDef",
+ProfileTypeDef = TypedDict(
+    "ProfileTypeDef",
     {
-        "PillarDifferences": List[PillarDifferenceTypeDef],
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ProfileName": str,
+        "ProfileDescription": str,
+        "ProfileQuestions": List[ProfileQuestionTypeDef],
+        "Owner": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+ProfileTemplateTypeDef = TypedDict(
+    "ProfileTemplateTypeDef",
+    {
+        "TemplateName": str,
+        "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
     },
     total=False,
 )
 
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
@@ -1547,14 +1951,15 @@
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
         "SelectedChoices": List[str],
         "ChoiceAnswerSummaries": List[ChoiceAnswerSummaryTypeDef],
         "IsApplicable": bool,
         "Risk": RiskType,
         "Reason": AnswerReasonType,
+        "QuestionType": QuestionTypeType,
     },
     total=False,
 )
 
 AnswerTypeDef = TypedDict(
     "AnswerTypeDef",
     {
@@ -1572,64 +1977,133 @@
         "Risk": RiskType,
         "Notes": str,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
+LensMetricTypeDef = TypedDict(
+    "LensMetricTypeDef",
+    {
+        "LensArn": str,
+        "Pillars": List[PillarMetricTypeDef],
+        "RiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
+ListMilestonesOutputTypeDef = TypedDict(
+    "ListMilestonesOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMilestoneOutputTypeDef = TypedDict(
     "GetMilestoneOutputTypeDef",
     {
         "WorkloadId": str,
         "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProfileOutputTypeDef = TypedDict(
+    "GetProfileOutputTypeDef",
+    {
+        "Profile": ProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateProfileOutputTypeDef = TypedDict(
+    "UpdateProfileOutputTypeDef",
+    {
+        "Profile": ProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProfileTemplateOutputTypeDef = TypedDict(
+    "GetProfileTemplateOutputTypeDef",
+    {
+        "ProfileTemplate": ProfileTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "AnswerSummaries": List[AnswerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAnswerOutputTypeDef = TypedDict(
     "GetAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAnswerOutputTypeDef = TypedDict(
     "UpdateAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ConsolidatedReportMetricTypeDef = TypedDict(
+    "ConsolidatedReportMetricTypeDef",
+    {
+        "MetricType": Literal["WORKLOAD"],
+        "RiskCounts": Dict[RiskType, int],
+        "WorkloadId": str,
+        "WorkloadName": str,
+        "WorkloadArn": str,
+        "UpdatedAt": datetime,
+        "Lenses": List[LensMetricTypeDef],
+        "LensesAppliedCount": int,
+    },
+    total=False,
+)
+
+GetConsolidatedReportOutputTypeDef = TypedDict(
+    "GetConsolidatedReportOutputTypeDef",
+    {
+        "Metrics": List[ConsolidatedReportMetricTypeDef],
+        "NextToken": str,
+        "Base64String": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.pyi` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,22 +18,29 @@
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
+    DefinitionTypeType,
     DifferenceStatusType,
+    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileNotificationTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    QuestionTypeType,
+    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -44,124 +51,163 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
+    "AssociateProfilesInputRequestTypeDef",
+    "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateLensShareOutputTypeDef",
     "CreateLensVersionInputRequestTypeDef",
+    "CreateLensVersionOutputTypeDef",
     "CreateMilestoneInputRequestTypeDef",
+    "CreateMilestoneOutputTypeDef",
+    "ProfileQuestionUpdateTypeDef",
+    "CreateProfileOutputTypeDef",
+    "CreateProfileShareInputRequestTypeDef",
+    "CreateProfileShareOutputTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
+    "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
+    "CreateWorkloadShareOutputTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
+    "DeleteProfileInputRequestTypeDef",
+    "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
+    "DisassociateProfilesInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportLensInputRequestTypeDef",
+    "ExportLensOutputTypeDef",
     "GetAnswerInputRequestTypeDef",
+    "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
+    "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "LensReviewSummaryTypeDef",
+    "ImportLensOutputTypeDef",
+    "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
     "ListCheckSummariesInputRequestTypeDef",
     "ListLensReviewImprovementsInputRequestTypeDef",
     "ListLensReviewsInputRequestTypeDef",
     "ListLensSharesInputRequestTypeDef",
     "ListLensesInputRequestTypeDef",
     "ListMilestonesInputRequestTypeDef",
     "ListNotificationsInputRequestTypeDef",
+    "ListProfileNotificationsInputRequestTypeDef",
+    "ProfileNotificationSummaryTypeDef",
+    "ListProfileSharesInputRequestTypeDef",
+    "ProfileShareSummaryTypeDef",
+    "ListProfilesInputRequestTypeDef",
+    "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
-    "WorkloadSummaryTypeDef",
     "QuestionDifferenceTypeDef",
+    "ProfileChoiceTypeDef",
+    "ProfileTemplateChoiceTypeDef",
+    "ResponseMetadataTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
+    "UpgradeProfileVersionInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
-    "ImprovementSummaryTypeDef",
-    "UpdateAnswerInputRequestTypeDef",
-    "CreateLensShareOutputTypeDef",
-    "CreateLensVersionOutputTypeDef",
-    "CreateMilestoneOutputTypeDef",
-    "CreateWorkloadOutputTypeDef",
-    "CreateWorkloadShareOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportLensOutputTypeDef",
-    "ImportLensOutputTypeDef",
+    "QuestionMetricTypeDef",
     "ListCheckDetailsOutputTypeDef",
     "ListCheckSummariesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
+    "ImprovementSummaryTypeDef",
+    "UpdateAnswerInputRequestTypeDef",
+    "CreateProfileInputRequestTypeDef",
+    "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
-    "WorkloadTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
-    "ListLensReviewsOutputTypeDef",
+    "LensReviewSummaryTypeDef",
+    "WorkloadSummaryTypeDef",
+    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
+    "ListProfileNotificationsOutputTypeDef",
+    "ListProfileSharesOutputTypeDef",
+    "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
-    "ListWorkloadsOutputTypeDef",
-    "MilestoneSummaryTypeDef",
     "PillarDifferenceTypeDef",
+    "ProfileQuestionTypeDef",
+    "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
     "ChoiceTypeDef",
+    "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
+    "ListLensReviewsOutputTypeDef",
+    "ListWorkloadsOutputTypeDef",
+    "MilestoneSummaryTypeDef",
     "GetWorkloadOutputTypeDef",
     "MilestoneTypeDef",
     "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
-    "ListMilestonesOutputTypeDef",
     "VersionDifferencesTypeDef",
+    "ProfileTypeDef",
+    "ProfileTemplateTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
+    "LensMetricTypeDef",
+    "ListMilestonesOutputTypeDef",
     "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
+    "GetProfileOutputTypeDef",
+    "UpdateProfileOutputTypeDef",
+    "GetProfileTemplateOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
+    "ConsolidatedReportMetricTypeDef",
+    "GetConsolidatedReportOutputTypeDef",
 )
 
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": str,
         "Url": str,
@@ -194,14 +240,31 @@
     "AssociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
+AssociateProfilesInputRequestTypeDef = TypedDict(
+    "AssociateProfilesInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "ProfileArns": Sequence[str],
+    },
+)
+
+BestPracticeTypeDef = TypedDict(
+    "BestPracticeTypeDef",
+    {
+        "ChoiceId": str,
+        "ChoiceTitle": str,
+    },
+    total=False,
+)
+
 CheckDetailTypeDef = TypedDict(
     "CheckDetailTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Provider": Literal["TRUSTED_ADVISOR"],
@@ -257,34 +320,33 @@
     {
         "Reason": ChoiceReasonType,
         "Notes": str,
     },
     total=False,
 )
 
+
 class ChoiceUpdateTypeDef(_RequiredChoiceUpdateTypeDef, _OptionalChoiceUpdateTypeDef):
     pass
 
+
 CreateLensShareInputRequestTypeDef = TypedDict(
     "CreateLensShareInputRequestTypeDef",
     {
         "LensAlias": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLensShareOutputTypeDef = TypedDict(
+    "CreateLensShareOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ShareId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLensVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
@@ -296,46 +358,121 @@
     "_OptionalCreateLensVersionInputRequestTypeDef",
     {
         "IsMajorVersion": bool,
     },
     total=False,
 )
 
+
 class CreateLensVersionInputRequestTypeDef(
     _RequiredCreateLensVersionInputRequestTypeDef, _OptionalCreateLensVersionInputRequestTypeDef
 ):
     pass
 
+
+CreateLensVersionOutputTypeDef = TypedDict(
+    "CreateLensVersionOutputTypeDef",
+    {
+        "LensArn": str,
+        "LensVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateMilestoneInputRequestTypeDef = TypedDict(
     "CreateMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
+CreateMilestoneOutputTypeDef = TypedDict(
+    "CreateMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProfileQuestionUpdateTypeDef = TypedDict(
+    "ProfileQuestionUpdateTypeDef",
+    {
+        "QuestionId": str,
+        "SelectedChoiceIds": Sequence[str],
+    },
+    total=False,
+)
+
+CreateProfileOutputTypeDef = TypedDict(
+    "CreateProfileOutputTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProfileShareInputRequestTypeDef = TypedDict(
+    "CreateProfileShareInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+        "SharedWith": str,
+        "ClientRequestToken": str,
+    },
+)
+
+CreateProfileShareOutputTypeDef = TypedDict(
+    "CreateProfileShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
+        "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
+CreateWorkloadOutputTypeDef = TypedDict(
+    "CreateWorkloadOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
     },
 )
 
+CreateWorkloadShareOutputTypeDef = TypedDict(
+    "CreateWorkloadShareOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "ShareId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLensInputRequestTypeDef = TypedDict(
     "DeleteLensInputRequestTypeDef",
     {
         "LensAlias": str,
         "ClientRequestToken": str,
         "LensStatus": LensStatusTypeType,
     },
@@ -346,14 +483,31 @@
     {
         "ShareId": str,
         "LensAlias": str,
         "ClientRequestToken": str,
     },
 )
 
+DeleteProfileInputRequestTypeDef = TypedDict(
+    "DeleteProfileInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+        "ClientRequestToken": str,
+    },
+)
+
+DeleteProfileShareInputRequestTypeDef = TypedDict(
+    "DeleteProfileShareInputRequestTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ClientRequestToken": str,
+    },
+)
+
 DeleteWorkloadInputRequestTypeDef = TypedDict(
     "DeleteWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ClientRequestToken": str,
     },
 )
@@ -371,33 +525,58 @@
     "DisassociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
+DisassociateProfilesInputRequestTypeDef = TypedDict(
+    "DisassociateProfilesInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "ProfileArns": Sequence[str],
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
     "_OptionalExportLensInputRequestTypeDef",
     {
         "LensVersion": str,
     },
     total=False,
 )
 
+
 class ExportLensInputRequestTypeDef(
     _RequiredExportLensInputRequestTypeDef, _OptionalExportLensInputRequestTypeDef
 ):
     pass
 
+
+ExportLensOutputTypeDef = TypedDict(
+    "ExportLensOutputTypeDef",
+    {
+        "LensJSON": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetAnswerInputRequestTypeDef = TypedDict(
     "_RequiredGetAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "QuestionId": str,
     },
@@ -406,38 +585,66 @@
     "_OptionalGetAnswerInputRequestTypeDef",
     {
         "MilestoneNumber": int,
     },
     total=False,
 )
 
+
 class GetAnswerInputRequestTypeDef(
     _RequiredGetAnswerInputRequestTypeDef, _OptionalGetAnswerInputRequestTypeDef
 ):
     pass
 
+
+_RequiredGetConsolidatedReportInputRequestTypeDef = TypedDict(
+    "_RequiredGetConsolidatedReportInputRequestTypeDef",
+    {
+        "Format": ReportFormatType,
+    },
+)
+_OptionalGetConsolidatedReportInputRequestTypeDef = TypedDict(
+    "_OptionalGetConsolidatedReportInputRequestTypeDef",
+    {
+        "IncludeSharedResources": bool,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetConsolidatedReportInputRequestTypeDef(
+    _RequiredGetConsolidatedReportInputRequestTypeDef,
+    _OptionalGetConsolidatedReportInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetLensInputRequestTypeDef = TypedDict(
     "_RequiredGetLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalGetLensInputRequestTypeDef = TypedDict(
     "_OptionalGetLensInputRequestTypeDef",
     {
         "LensVersion": str,
     },
     total=False,
 )
 
+
 class GetLensInputRequestTypeDef(
     _RequiredGetLensInputRequestTypeDef, _OptionalGetLensInputRequestTypeDef
 ):
     pass
 
+
 LensTypeDef = TypedDict(
     "LensTypeDef",
     {
         "LensArn": str,
         "LensVersion": str,
         "Name": str,
         "Description": str,
@@ -459,19 +666,21 @@
     "_OptionalGetLensReviewInputRequestTypeDef",
     {
         "MilestoneNumber": int,
     },
     total=False,
 )
 
+
 class GetLensReviewInputRequestTypeDef(
     _RequiredGetLensReviewInputRequestTypeDef, _OptionalGetLensReviewInputRequestTypeDef
 ):
     pass
 
+
 _RequiredGetLensReviewReportInputRequestTypeDef = TypedDict(
     "_RequiredGetLensReviewReportInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
     },
 )
@@ -479,19 +688,21 @@
     "_OptionalGetLensReviewReportInputRequestTypeDef",
     {
         "MilestoneNumber": int,
     },
     total=False,
 )
 
+
 class GetLensReviewReportInputRequestTypeDef(
     _RequiredGetLensReviewReportInputRequestTypeDef, _OptionalGetLensReviewReportInputRequestTypeDef
 ):
     pass
 
+
 LensReviewReportTypeDef = TypedDict(
     "LensReviewReportTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "Base64String": str,
     },
@@ -509,28 +720,51 @@
     {
         "BaseLensVersion": str,
         "TargetLensVersion": str,
     },
     total=False,
 )
 
+
 class GetLensVersionDifferenceInputRequestTypeDef(
     _RequiredGetLensVersionDifferenceInputRequestTypeDef,
     _OptionalGetLensVersionDifferenceInputRequestTypeDef,
 ):
     pass
 
+
 GetMilestoneInputRequestTypeDef = TypedDict(
     "GetMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
     },
 )
 
+_RequiredGetProfileInputRequestTypeDef = TypedDict(
+    "_RequiredGetProfileInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+    },
+)
+_OptionalGetProfileInputRequestTypeDef = TypedDict(
+    "_OptionalGetProfileInputRequestTypeDef",
+    {
+        "ProfileVersion": str,
+    },
+    total=False,
+)
+
+
+class GetProfileInputRequestTypeDef(
+    _RequiredGetProfileInputRequestTypeDef, _OptionalGetProfileInputRequestTypeDef
+):
+    pass
+
+
 GetWorkloadInputRequestTypeDef = TypedDict(
     "GetWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 
@@ -546,40 +780,47 @@
     {
         "LensAlias": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
-LensReviewSummaryTypeDef = TypedDict(
-    "LensReviewSummaryTypeDef",
+
+ImportLensOutputTypeDef = TypedDict(
+    "ImportLensOutputTypeDef",
     {
-        "LensAlias": str,
         "LensArn": str,
-        "LensVersion": str,
-        "LensName": str,
-        "LensStatus": LensStatusType,
-        "UpdatedAt": datetime,
-        "RiskCounts": Dict[RiskType, int],
+        "Status": ImportLensStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+WorkloadProfileTypeDef = TypedDict(
+    "WorkloadProfileTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
     },
     total=False,
 )
 
 PillarReviewSummaryTypeDef = TypedDict(
     "PillarReviewSummaryTypeDef",
     {
         "PillarId": str,
         "PillarName": str,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 LensShareSummaryTypeDef = TypedDict(
     "LensShareSummaryTypeDef",
     {
@@ -631,23 +872,26 @@
 _OptionalListAnswersInputRequestTypeDef = TypedDict(
     "_OptionalListAnswersInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
+        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
+
 class ListAnswersInputRequestTypeDef(
     _RequiredListAnswersInputRequestTypeDef, _OptionalListAnswersInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListCheckDetailsInputRequestTypeDef = TypedDict(
     "_RequiredListCheckDetailsInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensArn": str,
         "PillarId": str,
         "QuestionId": str,
@@ -659,19 +903,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListCheckDetailsInputRequestTypeDef(
     _RequiredListCheckDetailsInputRequestTypeDef, _OptionalListCheckDetailsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListCheckSummariesInputRequestTypeDef = TypedDict(
     "_RequiredListCheckSummariesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensArn": str,
         "PillarId": str,
         "QuestionId": str,
@@ -683,43 +929,48 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListCheckSummariesInputRequestTypeDef(
     _RequiredListCheckSummariesInputRequestTypeDef, _OptionalListCheckSummariesInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListLensReviewImprovementsInputRequestTypeDef = TypedDict(
     "_RequiredListLensReviewImprovementsInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
     },
 )
 _OptionalListLensReviewImprovementsInputRequestTypeDef = TypedDict(
     "_OptionalListLensReviewImprovementsInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
+        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
+
 class ListLensReviewImprovementsInputRequestTypeDef(
     _RequiredListLensReviewImprovementsInputRequestTypeDef,
     _OptionalListLensReviewImprovementsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLensReviewsInputRequestTypeDef = TypedDict(
     "_RequiredListLensReviewsInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListLensReviewsInputRequestTypeDef = TypedDict(
@@ -728,19 +979,21 @@
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLensReviewsInputRequestTypeDef(
     _RequiredListLensReviewsInputRequestTypeDef, _OptionalListLensReviewsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListLensSharesInputRequestTypeDef = TypedDict(
     "_RequiredListLensSharesInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalListLensSharesInputRequestTypeDef = TypedDict(
@@ -750,19 +1003,21 @@
         "NextToken": str,
         "MaxResults": int,
         "Status": ShareStatusType,
     },
     total=False,
 )
 
+
 class ListLensSharesInputRequestTypeDef(
     _RequiredListLensSharesInputRequestTypeDef, _OptionalListLensSharesInputRequestTypeDef
 ):
     pass
 
+
 ListLensesInputRequestTypeDef = TypedDict(
     "ListLensesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "LensType": LensTypeType,
         "LensStatus": LensStatusTypeType,
@@ -782,37 +1037,124 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMilestonesInputRequestTypeDef(
     _RequiredListMilestonesInputRequestTypeDef, _OptionalListMilestonesInputRequestTypeDef
 ):
     pass
 
+
 ListNotificationsInputRequestTypeDef = TypedDict(
     "ListNotificationsInputRequestTypeDef",
     {
         "WorkloadId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListProfileNotificationsInputRequestTypeDef = TypedDict(
+    "ListProfileNotificationsInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ProfileNotificationSummaryTypeDef = TypedDict(
+    "ProfileNotificationSummaryTypeDef",
+    {
+        "CurrentProfileVersion": str,
+        "LatestProfileVersion": str,
+        "Type": ProfileNotificationTypeType,
+        "ProfileArn": str,
+        "ProfileName": str,
+        "WorkloadId": str,
+        "WorkloadName": str,
+    },
+    total=False,
+)
+
+_RequiredListProfileSharesInputRequestTypeDef = TypedDict(
+    "_RequiredListProfileSharesInputRequestTypeDef",
+    {
+        "ProfileArn": str,
+    },
+)
+_OptionalListProfileSharesInputRequestTypeDef = TypedDict(
+    "_OptionalListProfileSharesInputRequestTypeDef",
+    {
+        "SharedWithPrefix": str,
+        "NextToken": str,
+        "MaxResults": int,
+        "Status": ShareStatusType,
+    },
+    total=False,
+)
+
+
+class ListProfileSharesInputRequestTypeDef(
+    _RequiredListProfileSharesInputRequestTypeDef, _OptionalListProfileSharesInputRequestTypeDef
+):
+    pass
+
+
+ProfileShareSummaryTypeDef = TypedDict(
+    "ProfileShareSummaryTypeDef",
+    {
+        "ShareId": str,
+        "SharedWith": str,
+        "Status": ShareStatusType,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
+ListProfilesInputRequestTypeDef = TypedDict(
+    "ListProfilesInputRequestTypeDef",
+    {
+        "ProfileNamePrefix": str,
+        "ProfileOwnerType": ProfileOwnerTypeType,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ProfileSummaryTypeDef = TypedDict(
+    "ProfileSummaryTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ProfileName": str,
+        "ProfileDescription": str,
+        "Owner": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+    },
+    total=False,
+)
+
 ListShareInvitationsInputRequestTypeDef = TypedDict(
     "ListShareInvitationsInputRequestTypeDef",
     {
         "WorkloadNamePrefix": str,
         "LensNamePrefix": str,
         "ShareResourceType": ShareResourceTypeType,
         "NextToken": str,
         "MaxResults": int,
+        "ProfileNamePrefix": str,
     },
     total=False,
 )
 
 ShareInvitationSummaryTypeDef = TypedDict(
     "ShareInvitationSummaryTypeDef",
     {
@@ -821,25 +1163,35 @@
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadName": str,
         "WorkloadId": str,
         "LensName": str,
         "LensArn": str,
+        "ProfileName": str,
+        "ProfileArn": str,
     },
     total=False,
 )
 
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListWorkloadSharesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkloadSharesInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListWorkloadSharesInputRequestTypeDef = TypedDict(
@@ -849,19 +1201,21 @@
         "NextToken": str,
         "MaxResults": int,
         "Status": ShareStatusType,
     },
     total=False,
 )
 
+
 class ListWorkloadSharesInputRequestTypeDef(
     _RequiredListWorkloadSharesInputRequestTypeDef, _OptionalListWorkloadSharesInputRequestTypeDef
 ):
     pass
 
+
 WorkloadShareSummaryTypeDef = TypedDict(
     "WorkloadShareSummaryTypeDef",
     {
         "ShareId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "Status": ShareStatusType,
@@ -876,47 +1230,64 @@
         "WorkloadNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-WorkloadSummaryTypeDef = TypedDict(
-    "WorkloadSummaryTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Owner": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[str],
-        "RiskCounts": Dict[RiskType, int],
-        "ImprovementStatus": WorkloadImprovementStatusType,
-    },
-    total=False,
-)
-
 QuestionDifferenceTypeDef = TypedDict(
     "QuestionDifferenceTypeDef",
     {
         "QuestionId": str,
         "QuestionTitle": str,
         "DifferenceStatus": DifferenceStatusType,
     },
     total=False,
 )
 
+ProfileChoiceTypeDef = TypedDict(
+    "ProfileChoiceTypeDef",
+    {
+        "ChoiceId": str,
+        "ChoiceTitle": str,
+        "ChoiceDescription": str,
+    },
+    total=False,
+)
+
+ProfileTemplateChoiceTypeDef = TypedDict(
+    "ProfileTemplateChoiceTypeDef",
+    {
+        "ChoiceId": str,
+        "ChoiceTitle": str,
+        "ChoiceDescription": str,
+    },
+    total=False,
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
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
+        "ProfileArn": str,
     },
     total=False,
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
@@ -933,14 +1304,15 @@
     },
 )
 
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "OrganizationSharingStatus": OrganizationSharingStatusType,
+        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
     },
     total=False,
 )
 
 _RequiredUpdateLensReviewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateLensReviewInputRequestTypeDef",
     {
@@ -953,19 +1325,21 @@
     {
         "LensNotes": str,
         "PillarNotes": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdateLensReviewInputRequestTypeDef(
     _RequiredUpdateLensReviewInputRequestTypeDef, _OptionalUpdateLensReviewInputRequestTypeDef
 ):
     pass
 
+
 UpdateShareInvitationInputRequestTypeDef = TypedDict(
     "UpdateShareInvitationInputRequestTypeDef",
     {
         "ShareInvitationId": str,
         "ShareInvitationAction": ShareInvitationActionType,
     },
 )
@@ -1005,28 +1379,82 @@
     "_OptionalUpgradeLensReviewInputRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpgradeLensReviewInputRequestTypeDef(
     _RequiredUpgradeLensReviewInputRequestTypeDef, _OptionalUpgradeLensReviewInputRequestTypeDef
 ):
     pass
 
+
+_RequiredUpgradeProfileVersionInputRequestTypeDef = TypedDict(
+    "_RequiredUpgradeProfileVersionInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "ProfileArn": str,
+    },
+)
+_OptionalUpgradeProfileVersionInputRequestTypeDef = TypedDict(
+    "_OptionalUpgradeProfileVersionInputRequestTypeDef",
+    {
+        "MilestoneName": str,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class UpgradeProfileVersionInputRequestTypeDef(
+    _RequiredUpgradeProfileVersionInputRequestTypeDef,
+    _OptionalUpgradeProfileVersionInputRequestTypeDef,
+):
+    pass
+
+
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
 )
 
+QuestionMetricTypeDef = TypedDict(
+    "QuestionMetricTypeDef",
+    {
+        "QuestionId": str,
+        "Risk": RiskType,
+        "BestPractices": List[BestPracticeTypeDef],
+    },
+    total=False,
+)
+
+ListCheckDetailsOutputTypeDef = TypedDict(
+    "ListCheckDetailsOutputTypeDef",
+    {
+        "CheckDetails": List[CheckDetailTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCheckSummariesOutputTypeDef = TypedDict(
+    "ListCheckSummariesOutputTypeDef",
+    {
+        "CheckSummaries": List[CheckSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1052,112 +1480,66 @@
         "Notes": str,
         "IsApplicable": bool,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
+
 class UpdateAnswerInputRequestTypeDef(
     _RequiredUpdateAnswerInputRequestTypeDef, _OptionalUpdateAnswerInputRequestTypeDef
 ):
     pass
 
-CreateLensShareOutputTypeDef = TypedDict(
-    "CreateLensShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-CreateLensVersionOutputTypeDef = TypedDict(
-    "CreateLensVersionOutputTypeDef",
+_RequiredCreateProfileInputRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileInputRequestTypeDef",
     {
-        "LensArn": str,
-        "LensVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProfileName": str,
+        "ProfileDescription": str,
+        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
+        "ClientRequestToken": str,
     },
 )
-
-CreateMilestoneOutputTypeDef = TypedDict(
-    "CreateMilestoneOutputTypeDef",
+_OptionalCreateProfileInputRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileInputRequestTypeDef",
     {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
-CreateWorkloadOutputTypeDef = TypedDict(
-    "CreateWorkloadOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-CreateWorkloadShareOutputTypeDef = TypedDict(
-    "CreateWorkloadShareOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "ShareId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class CreateProfileInputRequestTypeDef(
+    _RequiredCreateProfileInputRequestTypeDef, _OptionalCreateProfileInputRequestTypeDef
+):
+    pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ExportLensOutputTypeDef = TypedDict(
-    "ExportLensOutputTypeDef",
+_RequiredUpdateProfileInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateProfileInputRequestTypeDef",
     {
-        "LensJSON": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProfileArn": str,
     },
 )
-
-ImportLensOutputTypeDef = TypedDict(
-    "ImportLensOutputTypeDef",
+_OptionalUpdateProfileInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateProfileInputRequestTypeDef",
     {
-        "LensArn": str,
-        "Status": ImportLensStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProfileDescription": str,
+        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
     },
+    total=False,
 )
 
-ListCheckDetailsOutputTypeDef = TypedDict(
-    "ListCheckDetailsOutputTypeDef",
-    {
-        "CheckDetails": List[CheckDetailTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ListCheckSummariesOutputTypeDef = TypedDict(
-    "ListCheckSummariesOutputTypeDef",
-    {
-        "CheckSummaries": List[CheckSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateProfileInputRequestTypeDef(
+    _RequiredUpdateProfileInputRequestTypeDef, _OptionalUpdateProfileInputRequestTypeDef
+):
+    pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateWorkloadInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkloadInputRequestTypeDef",
     {
         "WorkloadName": str,
         "Description": str,
         "Environment": WorkloadEnvironmentType,
@@ -1176,23 +1558,26 @@
         "ReviewOwner": str,
         "IndustryType": str,
         "Industry": str,
         "Notes": str,
         "Tags": Mapping[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": Sequence[str],
+        "ProfileArns": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateWorkloadInputRequestTypeDef(
     _RequiredCreateWorkloadInputRequestTypeDef, _OptionalCreateWorkloadInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateWorkloadInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalUpdateWorkloadInputRequestTypeDef = TypedDict(
@@ -1214,19 +1599,72 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateWorkloadInputRequestTypeDef(
     _RequiredUpdateWorkloadInputRequestTypeDef, _OptionalUpdateWorkloadInputRequestTypeDef
 ):
     pass
 
+
+GetLensOutputTypeDef = TypedDict(
+    "GetLensOutputTypeDef",
+    {
+        "Lens": LensTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLensReviewReportOutputTypeDef = TypedDict(
+    "GetLensReviewReportOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewReport": LensReviewReportTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+LensReviewSummaryTypeDef = TypedDict(
+    "LensReviewSummaryTypeDef",
+    {
+        "LensAlias": str,
+        "LensArn": str,
+        "LensVersion": str,
+        "LensName": str,
+        "LensStatus": LensStatusType,
+        "UpdatedAt": datetime,
+        "RiskCounts": Dict[RiskType, int],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
+WorkloadSummaryTypeDef = TypedDict(
+    "WorkloadSummaryTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Owner": str,
+        "UpdatedAt": datetime,
+        "Lenses": List[str],
+        "RiskCounts": Dict[RiskType, int],
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
 WorkloadTypeDef = TypedDict(
     "WorkloadTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "WorkloadName": str,
         "Description": str,
@@ -1247,155 +1685,164 @@
         "PillarPriorities": List[str],
         "Lenses": List[str],
         "Owner": str,
         "ShareInvitationId": str,
         "Tags": Dict[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
-GetLensOutputTypeDef = TypedDict(
-    "GetLensOutputTypeDef",
-    {
-        "Lens": LensTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLensReviewReportOutputTypeDef = TypedDict(
-    "GetLensReviewReportOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListLensReviewsOutputTypeDef = TypedDict(
-    "ListLensReviewsOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
         "LensStatus": LensStatusType,
         "PillarReviewSummaries": List[PillarReviewSummaryTypeDef],
         "UpdatedAt": datetime,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
         "NextToken": str,
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLensesOutputTypeDef = TypedDict(
     "ListLensesOutputTypeDef",
     {
         "LensSummaries": List[LensSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationSummaryTypeDef = TypedDict(
     "NotificationSummaryTypeDef",
     {
         "Type": NotificationTypeType,
         "LensUpgradeSummary": LensUpgradeSummaryTypeDef,
     },
     total=False,
 )
 
+ListProfileNotificationsOutputTypeDef = TypedDict(
+    "ListProfileNotificationsOutputTypeDef",
+    {
+        "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProfileSharesOutputTypeDef = TypedDict(
+    "ListProfileSharesOutputTypeDef",
+    {
+        "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProfilesOutputTypeDef = TypedDict(
+    "ListProfilesOutputTypeDef",
+    {
+        "ProfileSummaries": List[ProfileSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkloadSharesOutputTypeDef = TypedDict(
     "ListWorkloadSharesOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListWorkloadsOutputTypeDef = TypedDict(
-    "ListWorkloadsOutputTypeDef",
+PillarDifferenceTypeDef = TypedDict(
+    "PillarDifferenceTypeDef",
     {
-        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PillarId": str,
+        "PillarName": str,
+        "DifferenceStatus": DifferenceStatusType,
+        "QuestionDifferences": List[QuestionDifferenceTypeDef],
     },
+    total=False,
 )
 
-MilestoneSummaryTypeDef = TypedDict(
-    "MilestoneSummaryTypeDef",
+ProfileQuestionTypeDef = TypedDict(
+    "ProfileQuestionTypeDef",
     {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "WorkloadSummary": WorkloadSummaryTypeDef,
+        "QuestionId": str,
+        "QuestionTitle": str,
+        "QuestionDescription": str,
+        "QuestionChoices": List[ProfileChoiceTypeDef],
+        "SelectedChoiceIds": List[str],
+        "MinSelectedChoices": int,
+        "MaxSelectedChoices": int,
     },
     total=False,
 )
 
-PillarDifferenceTypeDef = TypedDict(
-    "PillarDifferenceTypeDef",
+ProfileTemplateQuestionTypeDef = TypedDict(
+    "ProfileTemplateQuestionTypeDef",
     {
-        "PillarId": str,
-        "PillarName": str,
-        "DifferenceStatus": DifferenceStatusType,
-        "QuestionDifferences": List[QuestionDifferenceTypeDef],
+        "QuestionId": str,
+        "QuestionTitle": str,
+        "QuestionDescription": str,
+        "QuestionChoices": List[ProfileTemplateChoiceTypeDef],
+        "MinSelectedChoices": int,
+        "MaxSelectedChoices": int,
     },
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
         "ShareInvitation": ShareInvitationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWorkloadShareOutputTypeDef = TypedDict(
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
@@ -1404,32 +1851,73 @@
         "HelpfulResource": ChoiceContentTypeDef,
         "ImprovementPlan": ChoiceContentTypeDef,
         "AdditionalResources": List[AdditionalResourcesTypeDef],
     },
     total=False,
 )
 
+PillarMetricTypeDef = TypedDict(
+    "PillarMetricTypeDef",
+    {
+        "PillarId": str,
+        "RiskCounts": Dict[RiskType, int],
+        "Questions": List[QuestionMetricTypeDef],
+    },
+    total=False,
+)
+
 ListLensReviewImprovementsOutputTypeDef = TypedDict(
     "ListLensReviewImprovementsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListLensReviewsOutputTypeDef = TypedDict(
+    "ListLensReviewsOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListWorkloadsOutputTypeDef = TypedDict(
+    "ListWorkloadsOutputTypeDef",
+    {
+        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MilestoneSummaryTypeDef = TypedDict(
+    "MilestoneSummaryTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "WorkloadSummary": WorkloadSummaryTypeDef,
+    },
+    total=False,
+)
+
 GetWorkloadOutputTypeDef = TypedDict(
     "GetWorkloadOutputTypeDef",
     {
         "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MilestoneTypeDef = TypedDict(
     "MilestoneTypeDef",
     {
         "MilestoneNumber": int,
@@ -1440,60 +1928,78 @@
     total=False,
 )
 
 UpdateWorkloadOutputTypeDef = TypedDict(
     "UpdateWorkloadOutputTypeDef",
     {
         "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLensReviewOutputTypeDef = TypedDict(
     "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMilestonesOutputTypeDef = TypedDict(
-    "ListMilestonesOutputTypeDef",
+VersionDifferencesTypeDef = TypedDict(
+    "VersionDifferencesTypeDef",
     {
-        "WorkloadId": str,
-        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PillarDifferences": List[PillarDifferenceTypeDef],
     },
+    total=False,
 )
 
-VersionDifferencesTypeDef = TypedDict(
-    "VersionDifferencesTypeDef",
+ProfileTypeDef = TypedDict(
+    "ProfileTypeDef",
     {
-        "PillarDifferences": List[PillarDifferenceTypeDef],
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ProfileName": str,
+        "ProfileDescription": str,
+        "ProfileQuestions": List[ProfileQuestionTypeDef],
+        "Owner": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+ProfileTemplateTypeDef = TypedDict(
+    "ProfileTemplateTypeDef",
+    {
+        "TemplateName": str,
+        "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
     },
     total=False,
 )
 
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
@@ -1502,14 +2008,15 @@
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
         "SelectedChoices": List[str],
         "ChoiceAnswerSummaries": List[ChoiceAnswerSummaryTypeDef],
         "IsApplicable": bool,
         "Risk": RiskType,
         "Reason": AnswerReasonType,
+        "QuestionType": QuestionTypeType,
     },
     total=False,
 )
 
 AnswerTypeDef = TypedDict(
     "AnswerTypeDef",
     {
@@ -1527,64 +2034,133 @@
         "Risk": RiskType,
         "Notes": str,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
+LensMetricTypeDef = TypedDict(
+    "LensMetricTypeDef",
+    {
+        "LensArn": str,
+        "Pillars": List[PillarMetricTypeDef],
+        "RiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
+ListMilestonesOutputTypeDef = TypedDict(
+    "ListMilestonesOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMilestoneOutputTypeDef = TypedDict(
     "GetMilestoneOutputTypeDef",
     {
         "WorkloadId": str,
         "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProfileOutputTypeDef = TypedDict(
+    "GetProfileOutputTypeDef",
+    {
+        "Profile": ProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateProfileOutputTypeDef = TypedDict(
+    "UpdateProfileOutputTypeDef",
+    {
+        "Profile": ProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProfileTemplateOutputTypeDef = TypedDict(
+    "GetProfileTemplateOutputTypeDef",
+    {
+        "ProfileTemplate": ProfileTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "AnswerSummaries": List[AnswerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAnswerOutputTypeDef = TypedDict(
     "GetAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAnswerOutputTypeDef = TypedDict(
     "UpdateAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ConsolidatedReportMetricTypeDef = TypedDict(
+    "ConsolidatedReportMetricTypeDef",
+    {
+        "MetricType": Literal["WORKLOAD"],
+        "RiskCounts": Dict[RiskType, int],
+        "WorkloadId": str,
+        "WorkloadName": str,
+        "WorkloadArn": str,
+        "UpdatedAt": datetime,
+        "Lenses": List[LensMetricTypeDef],
+        "LensesAppliedCount": int,
+    },
+    total=False,
+)
+
+GetConsolidatedReportOutputTypeDef = TypedDict(
+    "GetConsolidatedReportOutputTypeDef",
+    {
+        "Metrics": List[ConsolidatedReportMetricTypeDef],
+        "NextToken": str,
+        "Base64String": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/PKG-INFO` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.26.4
-Summary: Type annotations for boto3.WellArchitected 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.WellArchitected 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
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
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,22 +284,30 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
+    DefinitionTypeType,
     DifferenceStatusType,
+    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
+    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
+    ProfileNotificationTypeType,
+    ProfileOwnerTypeType,
+    QuestionPriorityType,
+    QuestionTypeType,
+    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -322,161 +331,199 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
+    AssociateProfilesInputRequestTypeDef,
+    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLensShareOutputTypeDef,
     CreateLensVersionInputRequestTypeDef,
+    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
+    CreateMilestoneOutputTypeDef,
+    ProfileQuestionUpdateTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareInputRequestTypeDef,
+    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
+    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
+    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
+    DeleteProfileInputRequestTypeDef,
+    DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
+    DisassociateProfilesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
+    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
+    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
+    GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    LensReviewSummaryTypeDef,
+    ImportLensOutputTypeDef,
+    WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
     ListCheckSummariesInputRequestTypeDef,
     ListLensReviewImprovementsInputRequestTypeDef,
     ListLensReviewsInputRequestTypeDef,
     ListLensSharesInputRequestTypeDef,
     ListLensesInputRequestTypeDef,
     ListMilestonesInputRequestTypeDef,
     ListNotificationsInputRequestTypeDef,
+    ListProfileNotificationsInputRequestTypeDef,
+    ProfileNotificationSummaryTypeDef,
+    ListProfileSharesInputRequestTypeDef,
+    ProfileShareSummaryTypeDef,
+    ListProfilesInputRequestTypeDef,
+    ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
-    WorkloadSummaryTypeDef,
     QuestionDifferenceTypeDef,
+    ProfileChoiceTypeDef,
+    ProfileTemplateChoiceTypeDef,
+    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
+    UpgradeProfileVersionInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    ImprovementSummaryTypeDef,
-    UpdateAnswerInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
-    CreateLensVersionOutputTypeDef,
-    CreateMilestoneOutputTypeDef,
-    CreateWorkloadOutputTypeDef,
-    CreateWorkloadShareOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportLensOutputTypeDef,
-    ImportLensOutputTypeDef,
+    QuestionMetricTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ImprovementSummaryTypeDef,
+    UpdateAnswerInputRequestTypeDef,
+    CreateProfileInputRequestTypeDef,
+    UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
-    WorkloadTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
-    ListLensReviewsOutputTypeDef,
+    LensReviewSummaryTypeDef,
+    WorkloadSummaryTypeDef,
+    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
+    ListProfileNotificationsOutputTypeDef,
+    ListProfileSharesOutputTypeDef,
+    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
-    ListWorkloadsOutputTypeDef,
-    MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
+    ProfileQuestionTypeDef,
+    ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
+    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
+    ListLensReviewsOutputTypeDef,
+    ListWorkloadsOutputTypeDef,
+    MilestoneSummaryTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
-    ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
+    ProfileTypeDef,
+    ProfileTemplateTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
+    LensMetricTypeDef,
+    ListMilestonesOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
+    GetProfileOutputTypeDef,
+    UpdateProfileOutputTypeDef,
+    GetProfileTemplateOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
+    ConsolidatedReportMetricTypeDef,
+    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/SOURCES.txt` & `mypy-boto3-wellarchitected-1.27.0/mypy_boto3_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.26.4/setup.py` & `mypy-boto3-wellarchitected-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-wellarchitected.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wellarchitected",
-    version="1.26.4",
+    version="1.27.0",
     packages=["mypy_boto3_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WellArchitected 1.26.4 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.WellArchitected 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/",
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


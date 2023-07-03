# Comparing `tmp/mypy-boto3-codepipeline-1.26.141.tar.gz` & `tmp/mypy-boto3-codepipeline-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codepipeline-1.26.141.tar", last modified: Thu May 25 19:32:48 2023, max compression
+gzip compressed data, was "mypy-boto3-codepipeline-1.27.0.tar", last modified: Mon Jul  3 19:50:33 2023, max compression
```

## Comparing `mypy-boto3-codepipeline-1.26.141.tar` & `mypy-boto3-codepipeline-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-05-25 19:31:55.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46118 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:33.583017 mypy-boto3-codepipeline-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-03 19:50:33.575017 mypy-boto3-codepipeline-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17645 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:33.571017 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46243 2023-07-03 19:34:27.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46182 2023-07-03 19:34:27.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:33.575017 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-03 19:50:33.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:33.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:33.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:33.000000 mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:33.583017 mypy-boto3-codepipeline-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:34:26.000000 mypy-boto3-codepipeline-1.27.0/setup.py
```

### Comparing `mypy-boto3-codepipeline-1.26.141/LICENSE` & `mypy-boto3-codepipeline-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.141/PKG-INFO` & `mypy-boto3-codepipeline-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.26.141
-Summary: Type annotations for boto3.CodePipeline 1.26.141 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CodePipeline 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -362,16 +362,17 @@
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
@@ -394,58 +395,63 @@
     TagTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
     JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
     ListActionTypesInputRequestTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
+    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
+    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     WebhookAuthConfigurationTypeDef,
     WebhookFilterRuleTypeDef,
-    AcknowledgeJobOutputTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
-    RetryStageExecutionOutputTypeDef,
-    StartPipelineExecutionOutputTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
@@ -455,20 +461,14 @@
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.26.141/README.md` & `mypy-boto3-codepipeline-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -330,16 +330,17 @@
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
@@ -362,58 +363,63 @@
     TagTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
     JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
     ListActionTypesInputRequestTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
+    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
+    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     WebhookAuthConfigurationTypeDef,
     WebhookFilterRuleTypeDef,
-    AcknowledgeJobOutputTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
-    RetryStageExecutionOutputTypeDef,
-    StartPipelineExecutionOutputTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
@@ -423,20 +429,14 @@
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.py` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.pyi` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__main__.py` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodePipeline 1.26.141\nVersion:         1.26.141\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodePipeline 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.141")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.py` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.pyi` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.py` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -334,14 +336,16 @@
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
@@ -425,14 +429,15 @@
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

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.pyi` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -332,14 +334,16 @@
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
@@ -423,14 +427,15 @@
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

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.py` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
 
@@ -91,73 +91,73 @@
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactiontypespaginator)
         """
 
 
 class ListPipelineExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pipelineName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListWebhooksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWebhooksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
         """
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.pyi` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
 class ListActionTypesPaginator(Paginator):
@@ -87,69 +87,69 @@
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactiontypespaginator)
         """
 
 class ListPipelineExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, pipelineName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
         """
 
 class ListWebhooksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWebhooksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
         """
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.py` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -36,20 +36,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AcknowledgeJobOutputTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
+    "AcknowledgeThirdPartyJobOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
@@ -72,58 +72,63 @@
     "TagTypeDef",
     "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
     "JobWorkerExecutorConfigurationTypeDef",
     "LambdaExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
     "ListActionTypesInputRequestTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelineExecutionsInputRequestTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListWebhooksInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "StageContextTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ThirdPartyJobTypeDef",
+    "PutActionRevisionOutputTypeDef",
+    "PutApprovalResultOutputTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
+    "RetryStageExecutionOutputTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
+    "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
+    "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WebhookAuthConfigurationTypeDef",
     "WebhookFilterRuleTypeDef",
-    "AcknowledgeJobOutputTypeDef",
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "PutActionRevisionOutputTypeDef",
-    "PutApprovalResultOutputTypeDef",
-    "RetryStageExecutionOutputTypeDef",
-    "StartPipelineExecutionOutputTypeDef",
-    "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
     "ActionDeclarationTypeDef",
+    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
     "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
@@ -133,20 +138,14 @@
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "PutJobSuccessResultInputRequestTypeDef",
     "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
-    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "WebhookDefinitionTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
@@ -198,34 +197,39 @@
     "AcknowledgeJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AcknowledgeJobOutputTypeDef = TypedDict(
+    "AcknowledgeJobOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "status": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
         "clientToken": str,
     },
 )
 
+AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    {
+        "status": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -237,21 +241,19 @@
         "queryable": bool,
         "description": str,
         "type": ActionConfigurationPropertyTypeType,
     },
     total=False,
 )
 
-
 class ActionConfigurationPropertyTypeDef(
     _RequiredActionConfigurationPropertyTypeDef, _OptionalActionConfigurationPropertyTypeDef
 ):
     pass
 
-
 ActionConfigurationTypeDef = TypedDict(
     "ActionConfigurationTypeDef",
     {
         "configuration": Dict[str, str],
     },
     total=False,
 )
@@ -364,21 +366,19 @@
     {
         "queryable": bool,
         "description": str,
     },
     total=False,
 )
 
-
 class ActionTypePropertyTypeDef(
     _RequiredActionTypePropertyTypeDef, _OptionalActionTypePropertyTypeDef
 ):
     pass
 
-
 ActionTypeUrlsTypeDef = TypedDict(
     "ActionTypeUrlsTypeDef",
     {
         "configurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
@@ -479,19 +479,17 @@
     {
         "created": Union[datetime, str],
         "revisionSummary": str,
     },
     total=False,
 )
 
-
 class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
     pass
 
-
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -525,14 +523,21 @@
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
         "reason": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnableStageTransitionInputRequestTypeDef = TypedDict(
     "EnableStageTransitionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
     },
@@ -584,19 +589,17 @@
     "_OptionalFailureDetailsTypeDef",
     {
         "externalExecutionId": str,
     },
     total=False,
 )
 
-
 class FailureDetailsTypeDef(_RequiredFailureDetailsTypeDef, _OptionalFailureDetailsTypeDef):
     pass
 
-
 GetActionTypeInputRequestTypeDef = TypedDict(
     "GetActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
@@ -628,21 +631,19 @@
     "_OptionalGetPipelineInputRequestTypeDef",
     {
         "version": int,
     },
     total=False,
 )
 
-
 class GetPipelineInputRequestTypeDef(
     _RequiredGetPipelineInputRequestTypeDef, _OptionalGetPipelineInputRequestTypeDef
 ):
     pass
 
-
 PipelineMetadataTypeDef = TypedDict(
     "PipelineMetadataTypeDef",
     {
         "pipelineArn": str,
         "created": datetime,
         "updated": datetime,
         "pollingDisabledAt": datetime,
@@ -661,34 +662,54 @@
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "actionOwnerFilter": ActionOwnerType,
+        "regionFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListActionTypesInputRequestTypeDef = TypedDict(
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": ActionOwnerType,
         "nextToken": str,
         "regionFilter": str,
     },
     total=False,
 )
 
+_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
+    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPipelineExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListPipelineExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListPipelineExecutionsInputRequestTypeDef = TypedDict(
@@ -696,21 +717,27 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListPipelineExecutionsInputRequestTypeDef(
     _RequiredListPipelineExecutionsInputRequestTypeDef,
     _OptionalListPipelineExecutionsInputRequestTypeDef,
 ):
     pass
 
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
@@ -724,14 +751,34 @@
         "version": int,
         "created": datetime,
         "updated": datetime,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -739,30 +786,46 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListWebhooksInputRequestTypeDef = TypedDict(
     "ListWebhooksInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
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
 StageContextTypeDef = TypedDict(
     "StageContextTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -779,19 +842,17 @@
         "revisionId": str,
         "revisionSummary": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
-
 class SourceRevisionTypeDef(_RequiredSourceRevisionTypeDef, _OptionalSourceRevisionTypeDef):
     pass
 
-
 StopExecutionTriggerTypeDef = TypedDict(
     "StopExecutionTriggerTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
@@ -801,32 +862,68 @@
     {
         "clientId": str,
         "jobId": str,
     },
     total=False,
 )
 
+PutActionRevisionOutputTypeDef = TypedDict(
+    "PutActionRevisionOutputTypeDef",
+    {
+        "newRevision": bool,
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutApprovalResultOutputTypeDef = TypedDict(
+    "PutApprovalResultOutputTypeDef",
+    {
+        "approvedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterWebhookWithThirdPartyInputRequestTypeDef = TypedDict(
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     {
         "webhookName": str,
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
 RetryStageExecutionInputRequestTypeDef = TypedDict(
     "RetryStageExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": Literal["FAILED_ACTIONS"],
     },
 )
 
+RetryStageExecutionOutputTypeDef = TypedDict(
+    "RetryStageExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
     },
 )
@@ -852,21 +949,27 @@
     "_OptionalStartPipelineExecutionInputRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartPipelineExecutionInputRequestTypeDef(
     _RequiredStartPipelineExecutionInputRequestTypeDef,
     _OptionalStartPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
+StartPipelineExecutionOutputTypeDef = TypedDict(
+    "StartPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredStopPipelineExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopPipelineExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineExecutionId": str,
     },
@@ -876,21 +979,27 @@
     {
         "abandon": bool,
         "reason": str,
     },
     total=False,
 )
 
-
 class StopPipelineExecutionInputRequestTypeDef(
     _RequiredStopPipelineExecutionInputRequestTypeDef,
     _OptionalStopPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
+StopPipelineExecutionOutputTypeDef = TypedDict(
+    "StopPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -915,85 +1024,19 @@
     "_OptionalWebhookFilterRuleTypeDef",
     {
         "matchEquals": str,
     },
     total=False,
 )
 
-
 class WebhookFilterRuleTypeDef(
     _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
-
-AcknowledgeJobOutputTypeDef = TypedDict(
-    "AcknowledgeJobOutputTypeDef",
-    {
-        "status": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    {
-        "status": JobStatusType,
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
-PutActionRevisionOutputTypeDef = TypedDict(
-    "PutActionRevisionOutputTypeDef",
-    {
-        "newRevision": bool,
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutApprovalResultOutputTypeDef = TypedDict(
-    "PutApprovalResultOutputTypeDef",
-    {
-        "approvedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RetryStageExecutionOutputTypeDef = TypedDict(
-    "RetryStageExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartPipelineExecutionOutputTypeDef = TypedDict(
-    "StartPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopPipelineExecutionOutputTypeDef = TypedDict(
-    "StopPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForJobsInputRequestTypeDef = TypedDict(
@@ -1001,43 +1044,39 @@
     {
         "maxBatchSize": int,
         "queryParam": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PollForJobsInputRequestTypeDef(
     _RequiredPollForJobsInputRequestTypeDef, _OptionalPollForJobsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForThirdPartyJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_OptionalPollForThirdPartyJobsInputRequestTypeDef",
     {
         "maxBatchSize": int,
     },
     total=False,
 )
 
-
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredActionDeclarationTypeDef = TypedDict(
     "_RequiredActionDeclarationTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -1051,20 +1090,39 @@
         "roleArn": str,
         "region": str,
         "namespace": str,
     },
     total=False,
 )
 
-
 class ActionDeclarationTypeDef(
     _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
 ):
     pass
 
+_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "filter": ActionExecutionFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
+    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+):
+    pass
 
 _RequiredListActionExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListActionExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
@@ -1074,22 +1132,20 @@
         "filter": ActionExecutionFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListActionExecutionsInputRequestTypeDef(
     _RequiredListActionExecutionsInputRequestTypeDef,
     _OptionalListActionExecutionsInputRequestTypeDef,
 ):
     pass
 
-
 ActionExecutionTypeDef = TypedDict(
     "ActionExecutionTypeDef",
     {
         "actionExecutionId": str,
         "status": ActionExecutionStatusType,
         "summary": str,
         "lastStatusChange": datetime,
@@ -1126,19 +1182,17 @@
     {
         "settings": ActionTypeSettingsTypeDef,
         "actionConfigurationProperties": List[ActionConfigurationPropertyTypeDef],
     },
     total=False,
 )
 
-
 class ActionTypeTypeDef(_RequiredActionTypeTypeDef, _OptionalActionTypeTypeDef):
     pass
 
-
 PutApprovalResultInputRequestTypeDef = TypedDict(
     "PutApprovalResultInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "actionName": str,
         "result": ApprovalResultTypeDef,
@@ -1188,19 +1242,17 @@
     "_OptionalArtifactStoreTypeDef",
     {
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-
 class ArtifactStoreTypeDef(_RequiredArtifactStoreTypeDef, _OptionalArtifactStoreTypeDef):
     pass
 
-
 _RequiredCreateCustomActionTypeInputRequestTypeDef = TypedDict(
     "_RequiredCreateCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
@@ -1213,28 +1265,26 @@
         "settings": ActionTypeSettingsTypeDef,
         "configurationProperties": Sequence[ActionConfigurationPropertyTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCustomActionTypeInputRequestTypeDef(
     _RequiredCreateCustomActionTypeInputRequestTypeDef,
     _OptionalCreateCustomActionTypeInputRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
@@ -1255,21 +1305,19 @@
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
         "outputVariables": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PutJobSuccessResultInputRequestTypeDef(
     _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
@@ -1279,22 +1327,20 @@
         "currentRevision": CurrentRevisionTypeDef,
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
     },
     total=False,
 )
 
-
 class PutThirdPartyJobSuccessResultInputRequestTypeDef(
     _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
     _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
-
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
     },
     total=False,
@@ -1313,113 +1359,20 @@
     {
         "jobId": str,
         "clientToken": str,
         "failureDetails": FailureDetailsTypeDef,
     },
 )
 
-_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
-    {
-        "filter": ActionExecutionFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
-    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-):
-    pass
-
-
-ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
-    {
-        "actionOwnerFilter": ActionOwnerType,
-        "regionFilter": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
-    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-):
-    pass
-
-
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
-ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelines": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PipelineContextTypeDef = TypedDict(
     "PipelineContextTypeDef",
     {
         "pipelineName": str,
@@ -1445,15 +1398,15 @@
     total=False,
 )
 
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
@@ -1476,19 +1429,17 @@
     "_OptionalStageDeclarationTypeDef",
     {
         "blockers": Sequence[BlockerDeclarationTypeDef],
     },
     total=False,
 )
 
-
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
-
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
         "currentRevision": ActionRevisionTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
@@ -1498,24 +1449,24 @@
 )
 
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
         "actionTypes": List[ActionTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
@@ -1549,15 +1500,15 @@
     total=False,
 )
 
 GetPipelineExecutionOutputTypeDef = TypedDict(
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
@@ -1569,27 +1520,25 @@
     {
         "policyStatementsTemplate": str,
         "jobTimeout": int,
     },
     total=False,
 )
 
-
 class ActionTypeExecutorTypeDef(
     _RequiredActionTypeExecutorTypeDef, _OptionalActionTypeExecutorTypeDef
 ):
     pass
 
-
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
         "definition": WebhookDefinitionTypeDef,
@@ -1604,40 +1553,36 @@
         "lastTriggered": datetime,
         "arn": str,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class ListWebhookItemTypeDef(_RequiredListWebhookItemTypeDef, _OptionalListWebhookItemTypeDef):
     pass
 
-
 _RequiredPutWebhookInputRequestTypeDef = TypedDict(
     "_RequiredPutWebhookInputRequestTypeDef",
     {
         "webhook": WebhookDefinitionTypeDef,
     },
 )
 _OptionalPutWebhookInputRequestTypeDef = TypedDict(
     "_OptionalPutWebhookInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1648,21 +1593,19 @@
         "artifactStore": ArtifactStoreTypeDef,
         "artifactStores": Mapping[str, ArtifactStoreTypeDef],
         "version": int,
     },
     total=False,
 )
 
-
 class PipelineDeclarationTypeDef(
     _RequiredPipelineDeclarationTypeDef, _OptionalPipelineDeclarationTypeDef
 ):
     pass
 
-
 StageStateTypeDef = TypedDict(
     "StageStateTypeDef",
     {
         "stageName": str,
         "inboundExecution": StageExecutionTypeDef,
         "inboundTransitionState": TransitionStateTypeDef,
         "actionStates": List[ActionStateTypeDef],
@@ -1734,35 +1677,33 @@
         "permissions": ActionTypePermissionsTypeDef,
         "properties": List[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
-
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
 ):
     pass
 
-
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
@@ -1772,72 +1713,70 @@
     "_OptionalCreatePipelineInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineOutputTypeDef = TypedDict(
     "GetPipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
         "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
 UpdatePipelineOutputTypeDef = TypedDict(
     "UpdatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
         "updated": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListActionExecutionsOutputTypeDef = TypedDict(
     "ListActionExecutionsOutputTypeDef",
     {
         "actionExecutionDetails": List[ActionExecutionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "id": str,
@@ -1868,41 +1807,41 @@
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
 
 GetJobDetailsOutputTypeDef = TypedDict(
     "GetJobDetailsOutputTypeDef",
     {
         "jobDetails": JobDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PollForJobsOutputTypeDef = TypedDict(
     "PollForJobsOutputTypeDef",
     {
         "jobs": List[JobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.pyi` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AcknowledgeJobOutputTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
+    "AcknowledgeThirdPartyJobOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
@@ -71,58 +73,63 @@
     "TagTypeDef",
     "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
     "JobWorkerExecutorConfigurationTypeDef",
     "LambdaExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
     "ListActionTypesInputRequestTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelineExecutionsInputRequestTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListWebhooksInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "StageContextTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ThirdPartyJobTypeDef",
+    "PutActionRevisionOutputTypeDef",
+    "PutApprovalResultOutputTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
+    "RetryStageExecutionOutputTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
+    "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
+    "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WebhookAuthConfigurationTypeDef",
     "WebhookFilterRuleTypeDef",
-    "AcknowledgeJobOutputTypeDef",
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "PutActionRevisionOutputTypeDef",
-    "PutApprovalResultOutputTypeDef",
-    "RetryStageExecutionOutputTypeDef",
-    "StartPipelineExecutionOutputTypeDef",
-    "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
     "ActionDeclarationTypeDef",
+    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
     "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
@@ -132,20 +139,14 @@
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "PutJobSuccessResultInputRequestTypeDef",
     "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
-    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "WebhookDefinitionTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
@@ -197,34 +198,39 @@
     "AcknowledgeJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AcknowledgeJobOutputTypeDef = TypedDict(
+    "AcknowledgeJobOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "status": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
         "clientToken": str,
     },
 )
 
+AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    {
+        "status": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -236,19 +242,21 @@
         "queryable": bool,
         "description": str,
         "type": ActionConfigurationPropertyTypeType,
     },
     total=False,
 )
 
+
 class ActionConfigurationPropertyTypeDef(
     _RequiredActionConfigurationPropertyTypeDef, _OptionalActionConfigurationPropertyTypeDef
 ):
     pass
 
+
 ActionConfigurationTypeDef = TypedDict(
     "ActionConfigurationTypeDef",
     {
         "configuration": Dict[str, str],
     },
     total=False,
 )
@@ -361,19 +369,21 @@
     {
         "queryable": bool,
         "description": str,
     },
     total=False,
 )
 
+
 class ActionTypePropertyTypeDef(
     _RequiredActionTypePropertyTypeDef, _OptionalActionTypePropertyTypeDef
 ):
     pass
 
+
 ActionTypeUrlsTypeDef = TypedDict(
     "ActionTypeUrlsTypeDef",
     {
         "configurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
@@ -474,17 +484,19 @@
     {
         "created": Union[datetime, str],
         "revisionSummary": str,
     },
     total=False,
 )
 
+
 class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
     pass
 
+
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -518,14 +530,21 @@
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
         "reason": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnableStageTransitionInputRequestTypeDef = TypedDict(
     "EnableStageTransitionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
     },
@@ -577,17 +596,19 @@
     "_OptionalFailureDetailsTypeDef",
     {
         "externalExecutionId": str,
     },
     total=False,
 )
 
+
 class FailureDetailsTypeDef(_RequiredFailureDetailsTypeDef, _OptionalFailureDetailsTypeDef):
     pass
 
+
 GetActionTypeInputRequestTypeDef = TypedDict(
     "GetActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
@@ -619,19 +640,21 @@
     "_OptionalGetPipelineInputRequestTypeDef",
     {
         "version": int,
     },
     total=False,
 )
 
+
 class GetPipelineInputRequestTypeDef(
     _RequiredGetPipelineInputRequestTypeDef, _OptionalGetPipelineInputRequestTypeDef
 ):
     pass
 
+
 PipelineMetadataTypeDef = TypedDict(
     "PipelineMetadataTypeDef",
     {
         "pipelineArn": str,
         "created": datetime,
         "updated": datetime,
         "pollingDisabledAt": datetime,
@@ -650,34 +673,56 @@
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "actionOwnerFilter": ActionOwnerType,
+        "regionFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListActionTypesInputRequestTypeDef = TypedDict(
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": ActionOwnerType,
         "nextToken": str,
         "regionFilter": str,
     },
     total=False,
 )
 
+_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
+    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPipelineExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListPipelineExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListPipelineExecutionsInputRequestTypeDef = TypedDict(
@@ -685,20 +730,30 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListPipelineExecutionsInputRequestTypeDef(
     _RequiredListPipelineExecutionsInputRequestTypeDef,
     _OptionalListPipelineExecutionsInputRequestTypeDef,
 ):
     pass
 
+
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -711,14 +766,36 @@
         "version": int,
         "created": datetime,
         "updated": datetime,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -726,28 +803,48 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+
+ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWebhooksInputRequestTypeDef = TypedDict(
     "ListWebhooksInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
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
 StageContextTypeDef = TypedDict(
     "StageContextTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -764,17 +861,19 @@
         "revisionId": str,
         "revisionSummary": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
+
 class SourceRevisionTypeDef(_RequiredSourceRevisionTypeDef, _OptionalSourceRevisionTypeDef):
     pass
 
+
 StopExecutionTriggerTypeDef = TypedDict(
     "StopExecutionTriggerTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
@@ -784,32 +883,68 @@
     {
         "clientId": str,
         "jobId": str,
     },
     total=False,
 )
 
+PutActionRevisionOutputTypeDef = TypedDict(
+    "PutActionRevisionOutputTypeDef",
+    {
+        "newRevision": bool,
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutApprovalResultOutputTypeDef = TypedDict(
+    "PutApprovalResultOutputTypeDef",
+    {
+        "approvedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterWebhookWithThirdPartyInputRequestTypeDef = TypedDict(
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     {
         "webhookName": str,
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
 RetryStageExecutionInputRequestTypeDef = TypedDict(
     "RetryStageExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": Literal["FAILED_ACTIONS"],
     },
 )
 
+RetryStageExecutionOutputTypeDef = TypedDict(
+    "RetryStageExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
     },
 )
@@ -835,20 +970,30 @@
     "_OptionalStartPipelineExecutionInputRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartPipelineExecutionInputRequestTypeDef(
     _RequiredStartPipelineExecutionInputRequestTypeDef,
     _OptionalStartPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
+
+StartPipelineExecutionOutputTypeDef = TypedDict(
+    "StartPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopPipelineExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopPipelineExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineExecutionId": str,
     },
 )
@@ -857,20 +1002,30 @@
     {
         "abandon": bool,
         "reason": str,
     },
     total=False,
 )
 
+
 class StopPipelineExecutionInputRequestTypeDef(
     _RequiredStopPipelineExecutionInputRequestTypeDef,
     _OptionalStopPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
+
+StopPipelineExecutionOutputTypeDef = TypedDict(
+    "StopPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -894,82 +1049,20 @@
     "_OptionalWebhookFilterRuleTypeDef",
     {
         "matchEquals": str,
     },
     total=False,
 )
 
+
 class WebhookFilterRuleTypeDef(
     _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
-AcknowledgeJobOutputTypeDef = TypedDict(
-    "AcknowledgeJobOutputTypeDef",
-    {
-        "status": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    {
-        "status": JobStatusType,
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
-PutActionRevisionOutputTypeDef = TypedDict(
-    "PutActionRevisionOutputTypeDef",
-    {
-        "newRevision": bool,
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutApprovalResultOutputTypeDef = TypedDict(
-    "PutApprovalResultOutputTypeDef",
-    {
-        "approvedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RetryStageExecutionOutputTypeDef = TypedDict(
-    "RetryStageExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartPipelineExecutionOutputTypeDef = TypedDict(
-    "StartPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopPipelineExecutionOutputTypeDef = TypedDict(
-    "StopPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -978,39 +1071,43 @@
     {
         "maxBatchSize": int,
         "queryParam": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PollForJobsInputRequestTypeDef(
     _RequiredPollForJobsInputRequestTypeDef, _OptionalPollForJobsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForThirdPartyJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_OptionalPollForThirdPartyJobsInputRequestTypeDef",
     {
         "maxBatchSize": int,
     },
     total=False,
 )
 
+
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredActionDeclarationTypeDef = TypedDict(
     "_RequiredActionDeclarationTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -1024,19 +1121,44 @@
         "roleArn": str,
         "region": str,
         "namespace": str,
     },
     total=False,
 )
 
+
 class ActionDeclarationTypeDef(
     _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
 ):
     pass
 
+
+_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "filter": ActionExecutionFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
+    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListActionExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListActionExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListActionExecutionsInputRequestTypeDef = TypedDict(
@@ -1045,20 +1167,22 @@
         "filter": ActionExecutionFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListActionExecutionsInputRequestTypeDef(
     _RequiredListActionExecutionsInputRequestTypeDef,
     _OptionalListActionExecutionsInputRequestTypeDef,
 ):
     pass
 
+
 ActionExecutionTypeDef = TypedDict(
     "ActionExecutionTypeDef",
     {
         "actionExecutionId": str,
         "status": ActionExecutionStatusType,
         "summary": str,
         "lastStatusChange": datetime,
@@ -1095,17 +1219,19 @@
     {
         "settings": ActionTypeSettingsTypeDef,
         "actionConfigurationProperties": List[ActionConfigurationPropertyTypeDef],
     },
     total=False,
 )
 
+
 class ActionTypeTypeDef(_RequiredActionTypeTypeDef, _OptionalActionTypeTypeDef):
     pass
 
+
 PutApprovalResultInputRequestTypeDef = TypedDict(
     "PutApprovalResultInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "actionName": str,
         "result": ApprovalResultTypeDef,
@@ -1155,17 +1281,19 @@
     "_OptionalArtifactStoreTypeDef",
     {
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+
 class ArtifactStoreTypeDef(_RequiredArtifactStoreTypeDef, _OptionalArtifactStoreTypeDef):
     pass
 
+
 _RequiredCreateCustomActionTypeInputRequestTypeDef = TypedDict(
     "_RequiredCreateCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
@@ -1178,26 +1306,28 @@
         "settings": ActionTypeSettingsTypeDef,
         "configurationProperties": Sequence[ActionConfigurationPropertyTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCustomActionTypeInputRequestTypeDef(
     _RequiredCreateCustomActionTypeInputRequestTypeDef,
     _OptionalCreateCustomActionTypeInputRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
@@ -1218,19 +1348,21 @@
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
         "outputVariables": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PutJobSuccessResultInputRequestTypeDef(
     _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
@@ -1240,20 +1372,22 @@
         "currentRevision": CurrentRevisionTypeDef,
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
     },
     total=False,
 )
 
+
 class PutThirdPartyJobSuccessResultInputRequestTypeDef(
     _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
     _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
+
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
     },
     total=False,
@@ -1272,107 +1406,20 @@
     {
         "jobId": str,
         "clientToken": str,
         "failureDetails": FailureDetailsTypeDef,
     },
 )
 
-_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
-    {
-        "filter": ActionExecutionFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
-    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-):
-    pass
-
-ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
-    {
-        "actionOwnerFilter": ActionOwnerType,
-        "regionFilter": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
-    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-):
-    pass
-
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelines": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PipelineContextTypeDef = TypedDict(
     "PipelineContextTypeDef",
     {
         "pipelineName": str,
@@ -1398,15 +1445,15 @@
     total=False,
 )
 
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
@@ -1429,17 +1476,19 @@
     "_OptionalStageDeclarationTypeDef",
     {
         "blockers": Sequence[BlockerDeclarationTypeDef],
     },
     total=False,
 )
 
+
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
+
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
         "currentRevision": ActionRevisionTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
@@ -1449,24 +1498,24 @@
 )
 
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
         "actionTypes": List[ActionTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
@@ -1500,15 +1549,15 @@
     total=False,
 )
 
 GetPipelineExecutionOutputTypeDef = TypedDict(
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
@@ -1520,25 +1569,27 @@
     {
         "policyStatementsTemplate": str,
         "jobTimeout": int,
     },
     total=False,
 )
 
+
 class ActionTypeExecutorTypeDef(
     _RequiredActionTypeExecutorTypeDef, _OptionalActionTypeExecutorTypeDef
 ):
     pass
 
+
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
         "definition": WebhookDefinitionTypeDef,
@@ -1553,36 +1604,40 @@
         "lastTriggered": datetime,
         "arn": str,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class ListWebhookItemTypeDef(_RequiredListWebhookItemTypeDef, _OptionalListWebhookItemTypeDef):
     pass
 
+
 _RequiredPutWebhookInputRequestTypeDef = TypedDict(
     "_RequiredPutWebhookInputRequestTypeDef",
     {
         "webhook": WebhookDefinitionTypeDef,
     },
 )
 _OptionalPutWebhookInputRequestTypeDef = TypedDict(
     "_OptionalPutWebhookInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1593,19 +1648,21 @@
         "artifactStore": ArtifactStoreTypeDef,
         "artifactStores": Mapping[str, ArtifactStoreTypeDef],
         "version": int,
     },
     total=False,
 )
 
+
 class PipelineDeclarationTypeDef(
     _RequiredPipelineDeclarationTypeDef, _OptionalPipelineDeclarationTypeDef
 ):
     pass
 
+
 StageStateTypeDef = TypedDict(
     "StageStateTypeDef",
     {
         "stageName": str,
         "inboundExecution": StageExecutionTypeDef,
         "inboundTransitionState": TransitionStateTypeDef,
         "actionStates": List[ActionStateTypeDef],
@@ -1677,33 +1734,35 @@
         "permissions": ActionTypePermissionsTypeDef,
         "properties": List[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
+
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
 ):
     pass
 
+
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
@@ -1713,70 +1772,72 @@
     "_OptionalCreatePipelineInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineOutputTypeDef = TypedDict(
     "GetPipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
         "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
 UpdatePipelineOutputTypeDef = TypedDict(
     "UpdatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
         "updated": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListActionExecutionsOutputTypeDef = TypedDict(
     "ListActionExecutionsOutputTypeDef",
     {
         "actionExecutionDetails": List[ActionExecutionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "id": str,
@@ -1807,41 +1868,41 @@
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
 
 GetJobDetailsOutputTypeDef = TypedDict(
     "GetJobDetailsOutputTypeDef",
     {
         "jobDetails": JobDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PollForJobsOutputTypeDef = TypedDict(
     "PollForJobsOutputTypeDef",
     {
         "jobs": List[JobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/PKG-INFO` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.26.141
-Summary: Type annotations for boto3.CodePipeline 1.26.141 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CodePipeline 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -362,16 +362,17 @@
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
@@ -394,58 +395,63 @@
     TagTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
     JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
     ListActionTypesInputRequestTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
+    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
+    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     WebhookAuthConfigurationTypeDef,
     WebhookFilterRuleTypeDef,
-    AcknowledgeJobOutputTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
-    RetryStageExecutionOutputTypeDef,
-    StartPipelineExecutionOutputTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
@@ -455,20 +461,14 @@
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/SOURCES.txt` & `mypy-boto3-codepipeline-1.27.0/mypy_boto3_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.141/setup.py` & `mypy-boto3-codepipeline-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codepipeline",
-    version="1.26.141",
+    version="1.27.0",
     packages=["mypy_boto3_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodePipeline 1.26.141 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.CodePipeline 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


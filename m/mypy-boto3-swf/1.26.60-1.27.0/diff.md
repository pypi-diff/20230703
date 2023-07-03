# Comparing `tmp/mypy-boto3-swf-1.26.60.tar.gz` & `tmp/mypy-boto3-swf-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-swf-1.26.60.tar", last modified: Mon Jan 30 21:06:25 2023, max compression
+gzip compressed data, was "mypy-boto3-swf-1.27.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
```

## Comparing `mypy-boto3-swf-1.26.60.tar` & `mypy-boto3-swf-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:25.158480 mypy-boto3-swf-1.26.60/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-01-30 21:06:25.158480 mypy-boto3-swf-1.26.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:25.158480 mypy-boto3-swf-1.26.60/mypy_boto3_swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30973 2023-01-30 21:06:12.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-01-30 21:06:12.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-01-30 21:06:12.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-01-30 21:06:12.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-01-30 21:06:12.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-01-30 21:06:12.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    83006 2023-01-30 21:06:14.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    82849 2023-01-30 21:06:13.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:25.158480 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-01-30 21:06:25.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-30 21:06:25.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:25.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:25.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 21:06:25.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-30 21:06:25.000000 mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:06:25.158480 mypy-boto3-swf-1.26.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-30 21:06:11.000000 mypy-boto3-swf-1.26.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.152092 mypy-boto3-swf-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-07-03 19:51:33.144091 mypy-boto3-swf-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.144091 mypy-boto3-swf-1.27.0/mypy_boto3_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    83936 2023-07-03 19:49:01.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83779 2023-07-03 19:48:58.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.144091 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-07-03 19:51:32.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:33.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:32.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:32.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:32.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:32.000000 mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:33.152092 mypy-boto3-swf-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:48:57.000000 mypy-boto3-swf-1.27.0/setup.py
```

### Comparing `mypy-boto3-swf-1.26.60/LICENSE` & `mypy-boto3-swf-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-swf-1.26.60/PKG-INFO` & `mypy-boto3-swf-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.26.60
-Summary: Type annotations for boto3.SWF 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SWF 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-swf"></a>
 
 # mypy-boto3-swf
 
 [![PyPI - mypy-boto3-swf](https://img.shields.io/pypi/v/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-swf?color=blue)](https://pypistats.org/packages/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,15 +382,15 @@
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
     ActivityTypeTypeDef,
     TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ResponseMetadataTypeDef,
+    ActivityTaskStatusTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
     WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
@@ -412,16 +412,16 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
-    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -437,56 +437,61 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResourceTagTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
+    ResponseMetadataTypeDef,
+    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
     DeprecateActivityTypeInputRequestTypeDef,
     DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
     UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
     ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
     CountPendingActivityTasksInputRequestTypeDef,
     CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
     PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     PollForDecisionTaskInputRequestTypeDef,
     RegisterActivityTypeInputRequestTypeDef,
     RegisterWorkflowTypeInputRequestTypeDef,
     ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
-    ActivityTaskStatusTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PendingTaskCountTypeDef,
-    RunTypeDef,
-    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
     DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
@@ -501,25 +506,20 @@
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
@@ -540,42 +540,42 @@
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

### Comparing `mypy-boto3-swf-1.26.60/README.md` & `mypy-boto3-swf-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-swf"></a>
 
 # mypy-boto3-swf
 
 [![PyPI - mypy-boto3-swf](https://img.shields.io/pypi/v/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-swf?color=blue)](https://pypistats.org/packages/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,15 +350,15 @@
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
     ActivityTypeTypeDef,
     TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ResponseMetadataTypeDef,
+    ActivityTaskStatusTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
     WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
@@ -380,16 +380,16 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
-    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -405,56 +405,61 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResourceTagTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
+    ResponseMetadataTypeDef,
+    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
     DeprecateActivityTypeInputRequestTypeDef,
     DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
     UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
     ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
     CountPendingActivityTasksInputRequestTypeDef,
     CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
     PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     PollForDecisionTaskInputRequestTypeDef,
     RegisterActivityTypeInputRequestTypeDef,
     RegisterWorkflowTypeInputRequestTypeDef,
     ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
-    ActivityTaskStatusTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PendingTaskCountTypeDef,
-    RunTypeDef,
-    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
     DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
@@ -469,25 +474,20 @@
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
@@ -508,42 +508,42 @@
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

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/__init__.py` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/__init__.pyi` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/__main__.py` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SWF 1.26.60\nVersion:         1.26.60\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.SWF 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.60")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/client.py` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,16 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
+        startAtPreviousStartedEvent: bool = ...
     ) -> DecisionTaskTypeDef:
         """
         Used by deciders to get a  DecisionTask from the specified decision `taskList`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.poll_for_decision_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/client/#poll_for_decision_task)
         """
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/client.pyi` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,16 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
+        startAtPreviousStartedEvent: bool = ...
     ) -> DecisionTaskTypeDef:
         """
         Used by deciders to get a  DecisionTask from the specified decision `taskList`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.poll_for_decision_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/client/#poll_for_decision_task)
         """
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/literals.py` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,15 @@
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
@@ -272,21 +273,23 @@
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
@@ -365,14 +368,15 @@
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
@@ -383,14 +387,15 @@
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
@@ -426,14 +431,15 @@
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
@@ -452,16 +458,19 @@
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
@@ -541,18 +550,21 @@
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

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/literals.pyi` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
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
@@ -270,21 +271,23 @@
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
@@ -363,14 +366,15 @@
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
@@ -381,14 +385,15 @@
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
@@ -424,14 +429,15 @@
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
@@ -450,16 +456,19 @@
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
@@ -539,18 +548,21 @@
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

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/paginator.py` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 
@@ -103,15 +103,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listactivitytypespaginator)
         """
 
 
@@ -128,15 +128,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listdomainspaginator)
         """
 
 
@@ -170,15 +170,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 
@@ -191,15 +191,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listworkflowtypespaginator)
         """
 
 
@@ -212,13 +212,14 @@
     def paginate(
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        startAtPreviousStartedEvent: bool = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/paginator.pyi` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 class ListActivityTypesPaginator(Paginator):
@@ -99,15 +99,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listactivitytypespaginator)
         """
 
 class ListClosedWorkflowExecutionsPaginator(Paginator):
@@ -123,15 +123,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 class ListDomainsPaginator(Paginator):
@@ -141,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listdomainspaginator)
         """
 
 class ListOpenWorkflowExecutionsPaginator(Paginator):
@@ -163,15 +163,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 class ListWorkflowTypesPaginator(Paginator):
@@ -183,15 +183,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listworkflowtypespaginator)
         """
 
 class PollForDecisionTaskPaginator(Paginator):
@@ -203,13 +203,14 @@
     def paginate(
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        startAtPreviousStartedEvent: bool = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/type_defs.py` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
     "ActivityTypeTypeDef",
     "TaskListTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActivityTaskStatusTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
     "WorkflowExecutionTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowTypeTypeDef",
@@ -82,16 +82,16 @@
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
     "DescribeDomainInputRequestTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
-    "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
     "MarkerRecordedEventAttributesTypeDef",
     "RecordMarkerFailedEventAttributesTypeDef",
@@ -107,56 +107,61 @@
     "TimerFiredEventAttributesTypeDef",
     "TimerStartedEventAttributesTypeDef",
     "WorkflowExecutionCanceledEventAttributesTypeDef",
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
+    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListActivityTypesInputRequestTypeDef",
+    "ListDomainsInputListDomainsPaginateTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResourceTagTypeDef",
+    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "PendingTaskCountTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "RunTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "WorkflowExecutionCountTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
     "DeprecateActivityTypeInputRequestTypeDef",
     "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
     "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
     "CountPendingActivityTasksInputRequestTypeDef",
     "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
     "PollForActivityTaskInputRequestTypeDef",
+    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "PollForDecisionTaskInputRequestTypeDef",
     "RegisterActivityTypeInputRequestTypeDef",
     "RegisterWorkflowTypeInputRequestTypeDef",
     "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
-    "ActivityTaskStatusTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "PendingTaskCountTypeDef",
-    "RunTypeDef",
-    "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
     "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
+    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
@@ -171,25 +176,20 @@
     "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
     "CountClosedWorkflowExecutionsInputRequestTypeDef",
     "CountOpenWorkflowExecutionsInputRequestTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListClosedWorkflowExecutionsInputRequestTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
-    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    "ListDomainsInputListDomainsPaginateTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
     "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
@@ -314,22 +314,19 @@
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ActivityTaskStatusTypeDef = TypedDict(
+    "ActivityTaskStatusTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "cancelRequested": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActivityTaskTimedOutEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": ActivityTaskTimeoutTypeType,
@@ -712,30 +709,27 @@
 )
 
 
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
 
-FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
-    "FailWorkflowExecutionFailedEventAttributesTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "cause": FailWorkflowExecutionFailedCauseType,
-        "decisionTaskCompletedEventId": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
+    "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "cause": FailWorkflowExecutionFailedCauseType,
+        "decisionTaskCompletedEventId": int,
     },
-    total=False,
 )
 
 _RequiredLambdaFunctionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
@@ -1143,14 +1137,39 @@
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
 
+_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "domain": str,
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "name": str,
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListActivityTypesInputListActivityTypesPaginateTypeDef(
+    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
+    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListActivityTypesInputRequestTypeDef = TypedDict(
     "_RequiredListActivityTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1168,14 +1187,37 @@
 
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDomainsInputListDomainsPaginateTypeDef(
+    _RequiredListDomainsInputListDomainsPaginateTypeDef,
+    _OptionalListDomainsInputListDomainsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1217,14 +1259,39 @@
 )
 
 
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
 
+_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    {
+        "domain": str,
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    {
+        "name": str,
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
+    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1242,14 +1309,33 @@
 
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
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
+PendingTaskCountTypeDef = TypedDict(
+    "PendingTaskCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
@@ -1354,14 +1440,33 @@
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
 ):
     pass
 
 
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
+RunTypeDef = TypedDict(
+    "RunTypeDef",
+    {
+        "runId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1420,14 +1525,23 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkflowExecutionCountTypeDef = TypedDict(
+    "WorkflowExecutionCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredWorkflowExecutionOpenCountsTypeDef = TypedDict(
     "_RequiredWorkflowExecutionOpenCountsTypeDef",
     {
         "openActivityTasks": int,
         "openDecisionTasks": int,
         "openTimers": int,
         "openChildWorkflowExecutions": int,
@@ -1621,28 +1735,55 @@
 
 class PollForActivityTaskInputRequestTypeDef(
     _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
 ):
     pass
 
 
+_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+    {
+        "identity": str,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
+    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+):
+    pass
+
+
 _RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForDecisionTaskInputRequestTypeDef",
     {
         "domain": str,
         "taskList": TaskListTypeDef,
     },
 )
 _OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
     "_OptionalPollForDecisionTaskInputRequestTypeDef",
     {
         "identity": str,
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
     },
     total=False,
 )
 
 
 class PollForDecisionTaskInputRequestTypeDef(
     _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
@@ -1774,65 +1915,24 @@
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
-ActivityTaskStatusTypeDef = TypedDict(
-    "ActivityTaskStatusTypeDef",
-    {
-        "cancelRequested": bool,
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
-PendingTaskCountTypeDef = TypedDict(
-    "PendingTaskCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunTypeDef = TypedDict(
-    "RunTypeDef",
-    {
-        "runId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-WorkflowExecutionCountTypeDef = TypedDict(
-    "WorkflowExecutionCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "activityType": ActivityTypeTypeDef,
         "input": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
     "DescribeWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
@@ -1852,14 +1952,38 @@
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
+_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
     {
         "domain": str,
         "execution": WorkflowExecutionTypeDef,
     },
 )
@@ -2326,139 +2450,14 @@
 class CountOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-    },
-    total=False,
-)
-
-
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-    },
-)
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
-    {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
-    {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
-    {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListActivityTypesInputListActivityTypesPaginateTypeDef(
-    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
-    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
@@ -2467,46 +2466,53 @@
         "startTimeFilter": ExecutionTimeFilterTypeDef,
         "closeTimeFilter": ExecutionTimeFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
     _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
     {
-        "registrationStatus": RegistrationStatusType,
+        "domain": str,
     },
 )
-_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
     {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
         "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListDomainsInputListDomainsPaginateTypeDef(
-    _RequiredListDomainsInputListDomainsPaginateTypeDef,
-    _OptionalListDomainsInputListDomainsPaginateTypeDef,
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
 
 _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
@@ -2517,82 +2523,78 @@
 _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
     _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
-        "registrationStatus": RegistrationStatusType,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
-_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
     {
-        "name": str,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
         "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
-    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
     {
-        "domain": str,
-        "taskList": TaskListTypeDef,
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
     {
-        "identity": str,
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "domainInfos": List[DomainInfoTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
-    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-):
-    pass
-
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[ResourceTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
         "name": str,
@@ -2624,48 +2626,62 @@
 )
 
 ActivityTypeInfosTypeDef = TypedDict(
     "ActivityTypeInfosTypeDef",
     {
         "typeInfos": List[ActivityTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivityTypeDetailTypeDef = TypedDict(
     "ActivityTypeDetailTypeDef",
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDecisionTypeDef = TypedDict(
     "_RequiredDecisionTypeDef",
     {
         "decisionType": DecisionTypeType,
     },
 )
 _OptionalDecisionTypeDef = TypedDict(
     "_OptionalDecisionTypeDef",
     {
         "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
-        "requestCancelActivityTaskDecisionAttributes": RequestCancelActivityTaskDecisionAttributesTypeDef,
-        "completeWorkflowExecutionDecisionAttributes": CompleteWorkflowExecutionDecisionAttributesTypeDef,
+        "requestCancelActivityTaskDecisionAttributes": (
+            RequestCancelActivityTaskDecisionAttributesTypeDef
+        ),
+        "completeWorkflowExecutionDecisionAttributes": (
+            CompleteWorkflowExecutionDecisionAttributesTypeDef
+        ),
         "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
-        "cancelWorkflowExecutionDecisionAttributes": CancelWorkflowExecutionDecisionAttributesTypeDef,
-        "continueAsNewWorkflowExecutionDecisionAttributes": ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+        "cancelWorkflowExecutionDecisionAttributes": (
+            CancelWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionDecisionAttributes": (
+            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
+        ),
         "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
         "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
         "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
-        "signalExternalWorkflowExecutionDecisionAttributes": SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
-        "requestCancelExternalWorkflowExecutionDecisionAttributes": RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
-        "startChildWorkflowExecutionDecisionAttributes": StartChildWorkflowExecutionDecisionAttributesTypeDef,
+        "signalExternalWorkflowExecutionDecisionAttributes": (
+            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
+            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "startChildWorkflowExecutionDecisionAttributes": (
+            StartChildWorkflowExecutionDecisionAttributesTypeDef
+        ),
         "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
     },
     total=False,
 )
 
 
 class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
@@ -2676,24 +2692,24 @@
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
         "latestExecutionContext": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkflowExecutionInfosTypeDef = TypedDict(
     "WorkflowExecutionInfosTypeDef",
     {
         "executionInfos": List[WorkflowExecutionInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHistoryEventTypeDef = TypedDict(
     "_RequiredHistoryEventTypeDef",
     {
         "eventTimestamp": datetime,
@@ -2701,66 +2717,118 @@
         "eventId": int,
     },
 )
 _OptionalHistoryEventTypeDef = TypedDict(
     "_OptionalHistoryEventTypeDef",
     {
         "workflowExecutionStartedEventAttributes": WorkflowExecutionStartedEventAttributesTypeDef,
-        "workflowExecutionCompletedEventAttributes": WorkflowExecutionCompletedEventAttributesTypeDef,
-        "completeWorkflowExecutionFailedEventAttributes": CompleteWorkflowExecutionFailedEventAttributesTypeDef,
+        "workflowExecutionCompletedEventAttributes": (
+            WorkflowExecutionCompletedEventAttributesTypeDef
+        ),
+        "completeWorkflowExecutionFailedEventAttributes": (
+            CompleteWorkflowExecutionFailedEventAttributesTypeDef
+        ),
         "workflowExecutionFailedEventAttributes": WorkflowExecutionFailedEventAttributesTypeDef,
-        "failWorkflowExecutionFailedEventAttributes": FailWorkflowExecutionFailedEventAttributesTypeDef,
+        "failWorkflowExecutionFailedEventAttributes": (
+            FailWorkflowExecutionFailedEventAttributesTypeDef
+        ),
         "workflowExecutionTimedOutEventAttributes": WorkflowExecutionTimedOutEventAttributesTypeDef,
         "workflowExecutionCanceledEventAttributes": WorkflowExecutionCanceledEventAttributesTypeDef,
-        "cancelWorkflowExecutionFailedEventAttributes": CancelWorkflowExecutionFailedEventAttributesTypeDef,
-        "workflowExecutionContinuedAsNewEventAttributes": WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
-        "continueAsNewWorkflowExecutionFailedEventAttributes": ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-        "workflowExecutionTerminatedEventAttributes": WorkflowExecutionTerminatedEventAttributesTypeDef,
-        "workflowExecutionCancelRequestedEventAttributes": WorkflowExecutionCancelRequestedEventAttributesTypeDef,
+        "cancelWorkflowExecutionFailedEventAttributes": (
+            CancelWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "workflowExecutionContinuedAsNewEventAttributes": (
+            WorkflowExecutionContinuedAsNewEventAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionFailedEventAttributes": (
+            ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "workflowExecutionTerminatedEventAttributes": (
+            WorkflowExecutionTerminatedEventAttributesTypeDef
+        ),
+        "workflowExecutionCancelRequestedEventAttributes": (
+            WorkflowExecutionCancelRequestedEventAttributesTypeDef
+        ),
         "decisionTaskScheduledEventAttributes": DecisionTaskScheduledEventAttributesTypeDef,
         "decisionTaskStartedEventAttributes": DecisionTaskStartedEventAttributesTypeDef,
         "decisionTaskCompletedEventAttributes": DecisionTaskCompletedEventAttributesTypeDef,
         "decisionTaskTimedOutEventAttributes": DecisionTaskTimedOutEventAttributesTypeDef,
         "activityTaskScheduledEventAttributes": ActivityTaskScheduledEventAttributesTypeDef,
         "activityTaskStartedEventAttributes": ActivityTaskStartedEventAttributesTypeDef,
         "activityTaskCompletedEventAttributes": ActivityTaskCompletedEventAttributesTypeDef,
         "activityTaskFailedEventAttributes": ActivityTaskFailedEventAttributesTypeDef,
         "activityTaskTimedOutEventAttributes": ActivityTaskTimedOutEventAttributesTypeDef,
         "activityTaskCanceledEventAttributes": ActivityTaskCanceledEventAttributesTypeDef,
-        "activityTaskCancelRequestedEventAttributes": ActivityTaskCancelRequestedEventAttributesTypeDef,
+        "activityTaskCancelRequestedEventAttributes": (
+            ActivityTaskCancelRequestedEventAttributesTypeDef
+        ),
         "workflowExecutionSignaledEventAttributes": WorkflowExecutionSignaledEventAttributesTypeDef,
         "markerRecordedEventAttributes": MarkerRecordedEventAttributesTypeDef,
         "recordMarkerFailedEventAttributes": RecordMarkerFailedEventAttributesTypeDef,
         "timerStartedEventAttributes": TimerStartedEventAttributesTypeDef,
         "timerFiredEventAttributes": TimerFiredEventAttributesTypeDef,
         "timerCanceledEventAttributes": TimerCanceledEventAttributesTypeDef,
-        "startChildWorkflowExecutionInitiatedEventAttributes": StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
-        "childWorkflowExecutionStartedEventAttributes": ChildWorkflowExecutionStartedEventAttributesTypeDef,
-        "childWorkflowExecutionCompletedEventAttributes": ChildWorkflowExecutionCompletedEventAttributesTypeDef,
-        "childWorkflowExecutionFailedEventAttributes": ChildWorkflowExecutionFailedEventAttributesTypeDef,
-        "childWorkflowExecutionTimedOutEventAttributes": ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
-        "childWorkflowExecutionCanceledEventAttributes": ChildWorkflowExecutionCanceledEventAttributesTypeDef,
-        "childWorkflowExecutionTerminatedEventAttributes": ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
-        "signalExternalWorkflowExecutionInitiatedEventAttributes": SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
-        "externalWorkflowExecutionSignaledEventAttributes": ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-        "signalExternalWorkflowExecutionFailedEventAttributes": SignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
-        "externalWorkflowExecutionCancelRequestedEventAttributes": ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
-        "requestCancelExternalWorkflowExecutionInitiatedEventAttributes": RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
-        "requestCancelExternalWorkflowExecutionFailedEventAttributes": RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
-        "scheduleActivityTaskFailedEventAttributes": ScheduleActivityTaskFailedEventAttributesTypeDef,
-        "requestCancelActivityTaskFailedEventAttributes": RequestCancelActivityTaskFailedEventAttributesTypeDef,
+        "startChildWorkflowExecutionInitiatedEventAttributes": (
+            StartChildWorkflowExecutionInitiatedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionStartedEventAttributes": (
+            ChildWorkflowExecutionStartedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionCompletedEventAttributes": (
+            ChildWorkflowExecutionCompletedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionFailedEventAttributes": (
+            ChildWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionTimedOutEventAttributes": (
+            ChildWorkflowExecutionTimedOutEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionCanceledEventAttributes": (
+            ChildWorkflowExecutionCanceledEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionTerminatedEventAttributes": (
+            ChildWorkflowExecutionTerminatedEventAttributesTypeDef
+        ),
+        "signalExternalWorkflowExecutionInitiatedEventAttributes": (
+            SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef
+        ),
+        "externalWorkflowExecutionSignaledEventAttributes": (
+            ExternalWorkflowExecutionSignaledEventAttributesTypeDef
+        ),
+        "signalExternalWorkflowExecutionFailedEventAttributes": (
+            SignalExternalWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "externalWorkflowExecutionCancelRequestedEventAttributes": (
+            ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionInitiatedEventAttributes": (
+            RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionFailedEventAttributes": (
+            RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "scheduleActivityTaskFailedEventAttributes": (
+            ScheduleActivityTaskFailedEventAttributesTypeDef
+        ),
+        "requestCancelActivityTaskFailedEventAttributes": (
+            RequestCancelActivityTaskFailedEventAttributesTypeDef
+        ),
         "startTimerFailedEventAttributes": StartTimerFailedEventAttributesTypeDef,
         "cancelTimerFailedEventAttributes": CancelTimerFailedEventAttributesTypeDef,
-        "startChildWorkflowExecutionFailedEventAttributes": StartChildWorkflowExecutionFailedEventAttributesTypeDef,
+        "startChildWorkflowExecutionFailedEventAttributes": (
+            StartChildWorkflowExecutionFailedEventAttributesTypeDef
+        ),
         "lambdaFunctionScheduledEventAttributes": LambdaFunctionScheduledEventAttributesTypeDef,
         "lambdaFunctionStartedEventAttributes": LambdaFunctionStartedEventAttributesTypeDef,
         "lambdaFunctionCompletedEventAttributes": LambdaFunctionCompletedEventAttributesTypeDef,
         "lambdaFunctionFailedEventAttributes": LambdaFunctionFailedEventAttributesTypeDef,
         "lambdaFunctionTimedOutEventAttributes": LambdaFunctionTimedOutEventAttributesTypeDef,
-        "scheduleLambdaFunctionFailedEventAttributes": ScheduleLambdaFunctionFailedEventAttributesTypeDef,
+        "scheduleLambdaFunctionFailedEventAttributes": (
+            ScheduleLambdaFunctionFailedEventAttributesTypeDef
+        ),
         "startLambdaFunctionFailedEventAttributes": StartLambdaFunctionFailedEventAttributesTypeDef,
     },
     total=False,
 )
 
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
@@ -2768,24 +2836,24 @@
 
 
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkflowTypeInfosTypeDef = TypedDict(
     "WorkflowTypeInfosTypeDef",
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
@@ -2814,19 +2882,19 @@
         "taskToken": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "workflowType": WorkflowTypeTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HistoryTypeDef = TypedDict(
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf/type_defs.pyi` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
     "ActivityTypeTypeDef",
     "TaskListTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActivityTaskStatusTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
     "WorkflowExecutionTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowTypeTypeDef",
@@ -81,16 +81,16 @@
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
     "DescribeDomainInputRequestTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
-    "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
     "MarkerRecordedEventAttributesTypeDef",
     "RecordMarkerFailedEventAttributesTypeDef",
@@ -106,56 +106,61 @@
     "TimerFiredEventAttributesTypeDef",
     "TimerStartedEventAttributesTypeDef",
     "WorkflowExecutionCanceledEventAttributesTypeDef",
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
+    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListActivityTypesInputRequestTypeDef",
+    "ListDomainsInputListDomainsPaginateTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResourceTagTypeDef",
+    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "PendingTaskCountTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "RunTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "WorkflowExecutionCountTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
     "DeprecateActivityTypeInputRequestTypeDef",
     "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
     "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
     "CountPendingActivityTasksInputRequestTypeDef",
     "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
     "PollForActivityTaskInputRequestTypeDef",
+    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "PollForDecisionTaskInputRequestTypeDef",
     "RegisterActivityTypeInputRequestTypeDef",
     "RegisterWorkflowTypeInputRequestTypeDef",
     "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
-    "ActivityTaskStatusTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "PendingTaskCountTypeDef",
-    "RunTypeDef",
-    "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
     "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
+    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
@@ -170,25 +175,20 @@
     "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
     "CountClosedWorkflowExecutionsInputRequestTypeDef",
     "CountOpenWorkflowExecutionsInputRequestTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListClosedWorkflowExecutionsInputRequestTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
-    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    "ListDomainsInputListDomainsPaginateTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
     "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
@@ -305,22 +305,19 @@
 
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ActivityTaskStatusTypeDef = TypedDict(
+    "ActivityTaskStatusTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "cancelRequested": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActivityTaskTimedOutEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": ActivityTaskTimeoutTypeType,
@@ -681,30 +678,27 @@
     },
     total=False,
 )
 
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
-FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
-    "FailWorkflowExecutionFailedEventAttributesTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "cause": FailWorkflowExecutionFailedCauseType,
-        "decisionTaskCompletedEventId": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
+    "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "cause": FailWorkflowExecutionFailedCauseType,
+        "decisionTaskCompletedEventId": int,
     },
-    total=False,
 )
 
 _RequiredLambdaFunctionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
@@ -1084,14 +1078,37 @@
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
 
+_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "domain": str,
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "name": str,
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListActivityTypesInputListActivityTypesPaginateTypeDef(
+    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
+    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
+):
+    pass
+
 _RequiredListActivityTypesInputRequestTypeDef = TypedDict(
     "_RequiredListActivityTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1107,14 +1124,35 @@
 )
 
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
+_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDomainsInputListDomainsPaginateTypeDef(
+    _RequiredListDomainsInputListDomainsPaginateTypeDef,
+    _OptionalListDomainsInputListDomainsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1152,14 +1190,37 @@
     },
     total=False,
 )
 
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    {
+        "domain": str,
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    {
+        "name": str,
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
+    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+):
+    pass
+
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1175,14 +1236,33 @@
 )
 
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
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
+PendingTaskCountTypeDef = TypedDict(
+    "PendingTaskCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
@@ -1277,14 +1357,33 @@
 
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
 ):
     pass
 
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
+RunTypeDef = TypedDict(
+    "RunTypeDef",
+    {
+        "runId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1339,14 +1438,23 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkflowExecutionCountTypeDef = TypedDict(
+    "WorkflowExecutionCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredWorkflowExecutionOpenCountsTypeDef = TypedDict(
     "_RequiredWorkflowExecutionOpenCountsTypeDef",
     {
         "openActivityTasks": int,
         "openDecisionTasks": int,
         "openTimers": int,
         "openChildWorkflowExecutions": int,
@@ -1530,28 +1638,53 @@
 )
 
 class PollForActivityTaskInputRequestTypeDef(
     _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
 ):
     pass
 
+_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+    {
+        "identity": str,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
+    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+):
+    pass
+
 _RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForDecisionTaskInputRequestTypeDef",
     {
         "domain": str,
         "taskList": TaskListTypeDef,
     },
 )
 _OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
     "_OptionalPollForDecisionTaskInputRequestTypeDef",
     {
         "identity": str,
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
     },
     total=False,
 )
 
 class PollForDecisionTaskInputRequestTypeDef(
     _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
 ):
@@ -1673,65 +1806,24 @@
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
-ActivityTaskStatusTypeDef = TypedDict(
-    "ActivityTaskStatusTypeDef",
-    {
-        "cancelRequested": bool,
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
-PendingTaskCountTypeDef = TypedDict(
-    "PendingTaskCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunTypeDef = TypedDict(
-    "RunTypeDef",
-    {
-        "runId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-WorkflowExecutionCountTypeDef = TypedDict(
-    "WorkflowExecutionCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "activityType": ActivityTypeTypeDef,
         "input": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
     "DescribeWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
@@ -1751,14 +1843,36 @@
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
+_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
     {
         "domain": str,
         "execution": WorkflowExecutionTypeDef,
     },
 )
@@ -2195,131 +2309,14 @@
 
 class CountOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-    },
-    total=False,
-)
-
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-    },
-)
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
-    {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
-    {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
-    {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListActivityTypesInputListActivityTypesPaginateTypeDef(
-    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
-    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
@@ -2328,43 +2325,50 @@
         "startTimeFilter": ExecutionTimeFilterTypeDef,
         "closeTimeFilter": ExecutionTimeFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
     _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
-_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
     {
-        "registrationStatus": RegistrationStatusType,
+        "domain": str,
     },
 )
-_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
     {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
         "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListDomainsInputListDomainsPaginateTypeDef(
-    _RequiredListDomainsInputListDomainsPaginateTypeDef,
-    _OptionalListDomainsInputListDomainsPaginateTypeDef,
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
 _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
@@ -2374,76 +2378,74 @@
 _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
     _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
-_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
-        "registrationStatus": RegistrationStatusType,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
-_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
     {
-        "name": str,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
         "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
-class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
-    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
     {
-        "domain": str,
-        "taskList": TaskListTypeDef,
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
     {
-        "identity": str,
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "domainInfos": List[DomainInfoTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
-    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-):
-    pass
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[ResourceTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
         "name": str,
@@ -2473,48 +2475,62 @@
 )
 
 ActivityTypeInfosTypeDef = TypedDict(
     "ActivityTypeInfosTypeDef",
     {
         "typeInfos": List[ActivityTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivityTypeDetailTypeDef = TypedDict(
     "ActivityTypeDetailTypeDef",
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDecisionTypeDef = TypedDict(
     "_RequiredDecisionTypeDef",
     {
         "decisionType": DecisionTypeType,
     },
 )
 _OptionalDecisionTypeDef = TypedDict(
     "_OptionalDecisionTypeDef",
     {
         "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
-        "requestCancelActivityTaskDecisionAttributes": RequestCancelActivityTaskDecisionAttributesTypeDef,
-        "completeWorkflowExecutionDecisionAttributes": CompleteWorkflowExecutionDecisionAttributesTypeDef,
+        "requestCancelActivityTaskDecisionAttributes": (
+            RequestCancelActivityTaskDecisionAttributesTypeDef
+        ),
+        "completeWorkflowExecutionDecisionAttributes": (
+            CompleteWorkflowExecutionDecisionAttributesTypeDef
+        ),
         "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
-        "cancelWorkflowExecutionDecisionAttributes": CancelWorkflowExecutionDecisionAttributesTypeDef,
-        "continueAsNewWorkflowExecutionDecisionAttributes": ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+        "cancelWorkflowExecutionDecisionAttributes": (
+            CancelWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionDecisionAttributes": (
+            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
+        ),
         "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
         "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
         "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
-        "signalExternalWorkflowExecutionDecisionAttributes": SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
-        "requestCancelExternalWorkflowExecutionDecisionAttributes": RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
-        "startChildWorkflowExecutionDecisionAttributes": StartChildWorkflowExecutionDecisionAttributesTypeDef,
+        "signalExternalWorkflowExecutionDecisionAttributes": (
+            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
+            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "startChildWorkflowExecutionDecisionAttributes": (
+            StartChildWorkflowExecutionDecisionAttributesTypeDef
+        ),
         "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
     },
     total=False,
 )
 
 class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
     pass
@@ -2523,24 +2539,24 @@
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
         "latestExecutionContext": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkflowExecutionInfosTypeDef = TypedDict(
     "WorkflowExecutionInfosTypeDef",
     {
         "executionInfos": List[WorkflowExecutionInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHistoryEventTypeDef = TypedDict(
     "_RequiredHistoryEventTypeDef",
     {
         "eventTimestamp": datetime,
@@ -2548,89 +2564,141 @@
         "eventId": int,
     },
 )
 _OptionalHistoryEventTypeDef = TypedDict(
     "_OptionalHistoryEventTypeDef",
     {
         "workflowExecutionStartedEventAttributes": WorkflowExecutionStartedEventAttributesTypeDef,
-        "workflowExecutionCompletedEventAttributes": WorkflowExecutionCompletedEventAttributesTypeDef,
-        "completeWorkflowExecutionFailedEventAttributes": CompleteWorkflowExecutionFailedEventAttributesTypeDef,
+        "workflowExecutionCompletedEventAttributes": (
+            WorkflowExecutionCompletedEventAttributesTypeDef
+        ),
+        "completeWorkflowExecutionFailedEventAttributes": (
+            CompleteWorkflowExecutionFailedEventAttributesTypeDef
+        ),
         "workflowExecutionFailedEventAttributes": WorkflowExecutionFailedEventAttributesTypeDef,
-        "failWorkflowExecutionFailedEventAttributes": FailWorkflowExecutionFailedEventAttributesTypeDef,
+        "failWorkflowExecutionFailedEventAttributes": (
+            FailWorkflowExecutionFailedEventAttributesTypeDef
+        ),
         "workflowExecutionTimedOutEventAttributes": WorkflowExecutionTimedOutEventAttributesTypeDef,
         "workflowExecutionCanceledEventAttributes": WorkflowExecutionCanceledEventAttributesTypeDef,
-        "cancelWorkflowExecutionFailedEventAttributes": CancelWorkflowExecutionFailedEventAttributesTypeDef,
-        "workflowExecutionContinuedAsNewEventAttributes": WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
-        "continueAsNewWorkflowExecutionFailedEventAttributes": ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-        "workflowExecutionTerminatedEventAttributes": WorkflowExecutionTerminatedEventAttributesTypeDef,
-        "workflowExecutionCancelRequestedEventAttributes": WorkflowExecutionCancelRequestedEventAttributesTypeDef,
+        "cancelWorkflowExecutionFailedEventAttributes": (
+            CancelWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "workflowExecutionContinuedAsNewEventAttributes": (
+            WorkflowExecutionContinuedAsNewEventAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionFailedEventAttributes": (
+            ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "workflowExecutionTerminatedEventAttributes": (
+            WorkflowExecutionTerminatedEventAttributesTypeDef
+        ),
+        "workflowExecutionCancelRequestedEventAttributes": (
+            WorkflowExecutionCancelRequestedEventAttributesTypeDef
+        ),
         "decisionTaskScheduledEventAttributes": DecisionTaskScheduledEventAttributesTypeDef,
         "decisionTaskStartedEventAttributes": DecisionTaskStartedEventAttributesTypeDef,
         "decisionTaskCompletedEventAttributes": DecisionTaskCompletedEventAttributesTypeDef,
         "decisionTaskTimedOutEventAttributes": DecisionTaskTimedOutEventAttributesTypeDef,
         "activityTaskScheduledEventAttributes": ActivityTaskScheduledEventAttributesTypeDef,
         "activityTaskStartedEventAttributes": ActivityTaskStartedEventAttributesTypeDef,
         "activityTaskCompletedEventAttributes": ActivityTaskCompletedEventAttributesTypeDef,
         "activityTaskFailedEventAttributes": ActivityTaskFailedEventAttributesTypeDef,
         "activityTaskTimedOutEventAttributes": ActivityTaskTimedOutEventAttributesTypeDef,
         "activityTaskCanceledEventAttributes": ActivityTaskCanceledEventAttributesTypeDef,
-        "activityTaskCancelRequestedEventAttributes": ActivityTaskCancelRequestedEventAttributesTypeDef,
+        "activityTaskCancelRequestedEventAttributes": (
+            ActivityTaskCancelRequestedEventAttributesTypeDef
+        ),
         "workflowExecutionSignaledEventAttributes": WorkflowExecutionSignaledEventAttributesTypeDef,
         "markerRecordedEventAttributes": MarkerRecordedEventAttributesTypeDef,
         "recordMarkerFailedEventAttributes": RecordMarkerFailedEventAttributesTypeDef,
         "timerStartedEventAttributes": TimerStartedEventAttributesTypeDef,
         "timerFiredEventAttributes": TimerFiredEventAttributesTypeDef,
         "timerCanceledEventAttributes": TimerCanceledEventAttributesTypeDef,
-        "startChildWorkflowExecutionInitiatedEventAttributes": StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
-        "childWorkflowExecutionStartedEventAttributes": ChildWorkflowExecutionStartedEventAttributesTypeDef,
-        "childWorkflowExecutionCompletedEventAttributes": ChildWorkflowExecutionCompletedEventAttributesTypeDef,
-        "childWorkflowExecutionFailedEventAttributes": ChildWorkflowExecutionFailedEventAttributesTypeDef,
-        "childWorkflowExecutionTimedOutEventAttributes": ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
-        "childWorkflowExecutionCanceledEventAttributes": ChildWorkflowExecutionCanceledEventAttributesTypeDef,
-        "childWorkflowExecutionTerminatedEventAttributes": ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
-        "signalExternalWorkflowExecutionInitiatedEventAttributes": SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
-        "externalWorkflowExecutionSignaledEventAttributes": ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-        "signalExternalWorkflowExecutionFailedEventAttributes": SignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
-        "externalWorkflowExecutionCancelRequestedEventAttributes": ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
-        "requestCancelExternalWorkflowExecutionInitiatedEventAttributes": RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
-        "requestCancelExternalWorkflowExecutionFailedEventAttributes": RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
-        "scheduleActivityTaskFailedEventAttributes": ScheduleActivityTaskFailedEventAttributesTypeDef,
-        "requestCancelActivityTaskFailedEventAttributes": RequestCancelActivityTaskFailedEventAttributesTypeDef,
+        "startChildWorkflowExecutionInitiatedEventAttributes": (
+            StartChildWorkflowExecutionInitiatedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionStartedEventAttributes": (
+            ChildWorkflowExecutionStartedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionCompletedEventAttributes": (
+            ChildWorkflowExecutionCompletedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionFailedEventAttributes": (
+            ChildWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionTimedOutEventAttributes": (
+            ChildWorkflowExecutionTimedOutEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionCanceledEventAttributes": (
+            ChildWorkflowExecutionCanceledEventAttributesTypeDef
+        ),
+        "childWorkflowExecutionTerminatedEventAttributes": (
+            ChildWorkflowExecutionTerminatedEventAttributesTypeDef
+        ),
+        "signalExternalWorkflowExecutionInitiatedEventAttributes": (
+            SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef
+        ),
+        "externalWorkflowExecutionSignaledEventAttributes": (
+            ExternalWorkflowExecutionSignaledEventAttributesTypeDef
+        ),
+        "signalExternalWorkflowExecutionFailedEventAttributes": (
+            SignalExternalWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "externalWorkflowExecutionCancelRequestedEventAttributes": (
+            ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionInitiatedEventAttributes": (
+            RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionFailedEventAttributes": (
+            RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef
+        ),
+        "scheduleActivityTaskFailedEventAttributes": (
+            ScheduleActivityTaskFailedEventAttributesTypeDef
+        ),
+        "requestCancelActivityTaskFailedEventAttributes": (
+            RequestCancelActivityTaskFailedEventAttributesTypeDef
+        ),
         "startTimerFailedEventAttributes": StartTimerFailedEventAttributesTypeDef,
         "cancelTimerFailedEventAttributes": CancelTimerFailedEventAttributesTypeDef,
-        "startChildWorkflowExecutionFailedEventAttributes": StartChildWorkflowExecutionFailedEventAttributesTypeDef,
+        "startChildWorkflowExecutionFailedEventAttributes": (
+            StartChildWorkflowExecutionFailedEventAttributesTypeDef
+        ),
         "lambdaFunctionScheduledEventAttributes": LambdaFunctionScheduledEventAttributesTypeDef,
         "lambdaFunctionStartedEventAttributes": LambdaFunctionStartedEventAttributesTypeDef,
         "lambdaFunctionCompletedEventAttributes": LambdaFunctionCompletedEventAttributesTypeDef,
         "lambdaFunctionFailedEventAttributes": LambdaFunctionFailedEventAttributesTypeDef,
         "lambdaFunctionTimedOutEventAttributes": LambdaFunctionTimedOutEventAttributesTypeDef,
-        "scheduleLambdaFunctionFailedEventAttributes": ScheduleLambdaFunctionFailedEventAttributesTypeDef,
+        "scheduleLambdaFunctionFailedEventAttributes": (
+            ScheduleLambdaFunctionFailedEventAttributesTypeDef
+        ),
         "startLambdaFunctionFailedEventAttributes": StartLambdaFunctionFailedEventAttributesTypeDef,
     },
     total=False,
 )
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkflowTypeInfosTypeDef = TypedDict(
     "WorkflowTypeInfosTypeDef",
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
@@ -2657,19 +2725,19 @@
         "taskToken": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "workflowType": WorkflowTypeTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HistoryTypeDef = TypedDict(
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/PKG-INFO` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.26.60
-Summary: Type annotations for boto3.SWF 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SWF 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-swf"></a>
 
 # mypy-boto3-swf
 
 [![PyPI - mypy-boto3-swf](https://img.shields.io/pypi/v/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-swf?color=blue)](https://pypistats.org/packages/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,15 +382,15 @@
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
     ActivityTypeTypeDef,
     TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ResponseMetadataTypeDef,
+    ActivityTaskStatusTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
     WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
@@ -412,16 +412,16 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
-    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -437,56 +437,61 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResourceTagTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
+    ResponseMetadataTypeDef,
+    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
     DeprecateActivityTypeInputRequestTypeDef,
     DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
     UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
     ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
     CountPendingActivityTasksInputRequestTypeDef,
     CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
     PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     PollForDecisionTaskInputRequestTypeDef,
     RegisterActivityTypeInputRequestTypeDef,
     RegisterWorkflowTypeInputRequestTypeDef,
     ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
-    ActivityTaskStatusTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PendingTaskCountTypeDef,
-    RunTypeDef,
-    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
     DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
@@ -501,25 +506,20 @@
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
@@ -540,42 +540,42 @@
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

### Comparing `mypy-boto3-swf-1.26.60/mypy_boto3_swf.egg-info/SOURCES.txt` & `mypy-boto3-swf-1.27.0/mypy_boto3_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.26.60/setup.py` & `mypy-boto3-swf-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-swf.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-swf",
-    version="1.26.60",
+    version="1.27.0",
     packages=["mypy_boto3_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SWF 1.26.60 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.SWF 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/",
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


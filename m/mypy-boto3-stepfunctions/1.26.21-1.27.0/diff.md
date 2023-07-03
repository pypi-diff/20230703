# Comparing `tmp/mypy-boto3-stepfunctions-1.26.21.tar.gz` & `tmp/mypy-boto3-stepfunctions-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.26.21.tar", last modified: Thu Dec  1 20:25:43 2022, max compression
+gzip compressed data, was "mypy-boto3-stepfunctions-1.27.0.tar", last modified: Mon Jul  3 19:51:31 2023, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.26.21.tar` & `mypy-boto3-stepfunctions-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.830803 mypy-boto3-stepfunctions-1.26.21/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    17347 2022-12-01 20:25:43.822803 mypy-boto3-stepfunctions-1.26.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    15896 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.818803 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      912 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    22232 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10402 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10400 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6337 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    37018 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    36963 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.822803 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17347 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      794 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 20:25:43.830803 mypy-boto3-stepfunctions-1.26.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.760069 mypy-boto3-stepfunctions-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18147 2023-07-03 19:51:31.760069 mypy-boto3-stepfunctions-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.756069 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43945 2023-07-03 19:48:48.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43880 2023-07-03 19:48:47.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.760069 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18147 2023-07-03 19:51:31.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:51:31.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:31.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:31.000000 mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:31.760069 mypy-boto3-stepfunctions-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:48:46.000000 mypy-boto3-stepfunctions-1.27.0/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/LICENSE` & `mypy-boto3-stepfunctions-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-stepfunctions-1.26.21/PKG-INFO` & `mypy-boto3-stepfunctions-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.26.21
-Summary: Type annotations for boto3.SFN 1.26.21 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.SFN 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
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
 
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,31 +354,39 @@
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateActivityOutputTypeDef,
+    RoutingConfigurationListItemTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
+    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
+    DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
+    DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
+    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
+    DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetActivityTaskOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -385,62 +394,71 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
+    ListStateMachineAliasesInputRequestTypeDef,
+    StateMachineAliasListItemTypeDef,
+    ListStateMachineVersionsInputRequestTypeDef,
+    StateMachineVersionListItemTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PublishStateMachineVersionInputRequestTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
+    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
+    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
+    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
+    DescribeExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateActivityOutputTypeDef,
-    CreateStateMachineOutputTypeDef,
-    DescribeActivityOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    GetActivityTaskOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    StartExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
-    StopExecutionOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
+    TagResourceInputRequestTypeDef,
+    CreateStateMachineAliasInputRequestTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
+    UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
+    ListStateMachineAliasesOutputTypeDef,
+    ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     UpdateStateMachineInputRequestTypeDef,
@@ -455,42 +473,42 @@
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

### Comparing `mypy-boto3-stepfunctions-1.26.21/README.md` & `mypy-boto3-stepfunctions-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,31 +322,39 @@
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateActivityOutputTypeDef,
+    RoutingConfigurationListItemTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
+    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
+    DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
+    DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
+    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
+    DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetActivityTaskOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -354,62 +362,71 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
+    ListStateMachineAliasesInputRequestTypeDef,
+    StateMachineAliasListItemTypeDef,
+    ListStateMachineVersionsInputRequestTypeDef,
+    StateMachineVersionListItemTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PublishStateMachineVersionInputRequestTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
+    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
+    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
+    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
+    DescribeExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateActivityOutputTypeDef,
-    CreateStateMachineOutputTypeDef,
-    DescribeActivityOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    GetActivityTaskOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    StartExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
-    StopExecutionOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
+    TagResourceInputRequestTypeDef,
+    CreateStateMachineAliasInputRequestTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
+    UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
+    ListStateMachineAliasesOutputTypeDef,
+    ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     UpdateStateMachineInputRequestTypeDef,
@@ -424,42 +441,42 @@
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

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.py` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.pyi` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__main__.py` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.26.21\nVersion:         1.26.21\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.SFN 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.21")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.py` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,33 +24,40 @@
     ListActivitiesPaginator,
     ListExecutionsPaginator,
     ListMapRunsPaginator,
     ListStateMachinesPaginator,
 )
 from .type_defs import (
     CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     DescribeMapRunOutputTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     GetExecutionHistoryOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
+    ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -68,27 +75,29 @@
 
 
 class Exceptions:
     ActivityDoesNotExist: Type[BotocoreClientError]
     ActivityLimitExceeded: Type[BotocoreClientError]
     ActivityWorkerLimitExceeded: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     ExecutionAlreadyExists: Type[BotocoreClientError]
     ExecutionDoesNotExist: Type[BotocoreClientError]
     ExecutionLimitExceeded: Type[BotocoreClientError]
     InvalidArn: Type[BotocoreClientError]
     InvalidDefinition: Type[BotocoreClientError]
     InvalidExecutionInput: Type[BotocoreClientError]
     InvalidLoggingConfiguration: Type[BotocoreClientError]
     InvalidName: Type[BotocoreClientError]
     InvalidOutput: Type[BotocoreClientError]
     InvalidToken: Type[BotocoreClientError]
     InvalidTracingConfiguration: Type[BotocoreClientError]
     MissingRequiredParameter: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     StateMachineAlreadyExists: Type[BotocoreClientError]
     StateMachineDeleting: Type[BotocoreClientError]
     StateMachineDoesNotExist: Type[BotocoreClientError]
     StateMachineLimitExceeded: Type[BotocoreClientError]
     StateMachineTypeNotSupported: Type[BotocoreClientError]
     TaskDoesNotExist: Type[BotocoreClientError]
     TaskTimedOut: Type[BotocoreClientError]
@@ -144,23 +153,43 @@
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...,
+        publish: bool = ...,
+        versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine)
         """
 
+    def create_state_machine_alias(
+        self,
+        *,
+        name: str,
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
+        description: str = ...
+    ) -> CreateStateMachineAliasOutputTypeDef:
+        """
+        Creates an [alias](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-alias.html)_ for a state machine that
+        points to one or two [versions](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-version.html)_ of the same state
+        machine.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine_alias)
+        """
+
     def delete_activity(self, *, activityArn: str) -> Dict[str, Any]:
         """
         Deletes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_activity)
         """
@@ -169,27 +198,45 @@
         """
         Deletes a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine)
         """
 
+    def delete_state_machine_alias(self, *, stateMachineAliasArn: str) -> Dict[str, Any]:
+        """
+        Deletes a state machine [alias](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-alias.html)_.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_alias)
+        """
+
+    def delete_state_machine_version(self, *, stateMachineVersionArn: str) -> Dict[str, Any]:
+        """
+        Deletes a state machine [version](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-version.html)_.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_version)
+        """
+
     def describe_activity(self, *, activityArn: str) -> DescribeActivityOutputTypeDef:
         """
         Describes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_activity)
         """
 
     def describe_execution(self, *, executionArn: str) -> DescribeExecutionOutputTypeDef:
         """
-        Provides all information about a state machine execution, such as the state
-        machine associated with the execution, the execution input and output, and
-        relevant execution metadata.
+        Provides information about a state machine execution, such as the state machine
+        associated with the execution, the execution input and output, and relevant
+        execution metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_execution)
         """
 
     def describe_map_run(self, *, mapRunArn: str) -> DescribeMapRunOutputTypeDef:
         """
@@ -204,14 +251,25 @@
         Provides information about a state machine's definition, its IAM role Amazon
         Resource Name (ARN), and configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine)
         """
 
+    def describe_state_machine_alias(
+        self, *, stateMachineAliasArn: str
+    ) -> DescribeStateMachineAliasOutputTypeDef:
+        """
+        Returns details about a state machine [alias](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-alias.html)_.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine_alias)
+        """
+
     def describe_state_machine_for_execution(
         self, *, executionArn: str
     ) -> DescribeStateMachineForExecutionOutputTypeDef:
         """
         Provides information about a state machine's definition, its execution role ARN,
         and configuration.
 
@@ -292,14 +350,37 @@
         """
         Lists all Map Runs that were started by a given state machine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_map_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_map_runs)
         """
 
+    def list_state_machine_aliases(
+        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListStateMachineAliasesOutputTypeDef:
+        """
+        Lists [aliases](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
+        state-machine-alias.html)_ for a specified state machine ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_aliases)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_aliases)
+        """
+
+    def list_state_machine_versions(
+        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListStateMachineVersionsOutputTypeDef:
+        """
+        Lists [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
+        state-machine-version.html)_ for the specified state machine Amazon Resource
+        Name (ARN).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_versions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_versions)
+        """
+
     def list_state_machines(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStateMachinesOutputTypeDef:
         """
         Lists the existing state machines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machines)
@@ -310,14 +391,26 @@
         """
         List tags for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_tags_for_resource)
         """
 
+    def publish_state_machine_version(
+        self, *, stateMachineArn: str, revisionId: str = ..., description: str = ...
+    ) -> PublishStateMachineVersionOutputTypeDef:
+        """
+        Creates a [version](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-version.html)_ from the current
+        revision of a state machine.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.publish_state_machine_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#publish_state_machine_version)
+        """
+
     def send_task_failure(
         self, *, taskToken: str, error: str = ..., cause: str = ...
     ) -> Dict[str, Any]:
         """
         Used by activity workers and task states using the
         [callback](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
         resource.html#connect-wait-token)_ pattern to report that the task identified by
@@ -415,24 +508,42 @@
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...,
+        publish: bool = ...,
+        versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
-        Updates an existing state machine by modifying its `definition` , `roleArn` , or
+        Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine)
         """
 
+    def update_state_machine_alias(
+        self,
+        *,
+        stateMachineAliasArn: str,
+        description: str = ...,
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
+    ) -> UpdateStateMachineAliasOutputTypeDef:
+        """
+        Updates the configuration of an existing state machine
+        [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-
+        machine-alias.html)_ by modifying its `description` or `routingConfiguration`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine_alias)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_execution_history"]
     ) -> GetExecutionHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_paginator)
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.pyi` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -24,33 +24,40 @@
     ListActivitiesPaginator,
     ListExecutionsPaginator,
     ListMapRunsPaginator,
     ListStateMachinesPaginator,
 )
 from .type_defs import (
     CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     DescribeMapRunOutputTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     GetExecutionHistoryOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
+    ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -65,27 +72,29 @@
         self.operation_name: str
 
 class Exceptions:
     ActivityDoesNotExist: Type[BotocoreClientError]
     ActivityLimitExceeded: Type[BotocoreClientError]
     ActivityWorkerLimitExceeded: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     ExecutionAlreadyExists: Type[BotocoreClientError]
     ExecutionDoesNotExist: Type[BotocoreClientError]
     ExecutionLimitExceeded: Type[BotocoreClientError]
     InvalidArn: Type[BotocoreClientError]
     InvalidDefinition: Type[BotocoreClientError]
     InvalidExecutionInput: Type[BotocoreClientError]
     InvalidLoggingConfiguration: Type[BotocoreClientError]
     InvalidName: Type[BotocoreClientError]
     InvalidOutput: Type[BotocoreClientError]
     InvalidToken: Type[BotocoreClientError]
     InvalidTracingConfiguration: Type[BotocoreClientError]
     MissingRequiredParameter: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     StateMachineAlreadyExists: Type[BotocoreClientError]
     StateMachineDeleting: Type[BotocoreClientError]
     StateMachineDoesNotExist: Type[BotocoreClientError]
     StateMachineLimitExceeded: Type[BotocoreClientError]
     StateMachineTypeNotSupported: Type[BotocoreClientError]
     TaskDoesNotExist: Type[BotocoreClientError]
     TaskTimedOut: Type[BotocoreClientError]
@@ -136,48 +145,83 @@
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...,
+        publish: bool = ...,
+        versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine)
         """
+    def create_state_machine_alias(
+        self,
+        *,
+        name: str,
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
+        description: str = ...
+    ) -> CreateStateMachineAliasOutputTypeDef:
+        """
+        Creates an [alias](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-alias.html)_ for a state machine that
+        points to one or two [versions](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-version.html)_ of the same state
+        machine.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine_alias)
+        """
     def delete_activity(self, *, activityArn: str) -> Dict[str, Any]:
         """
         Deletes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_activity)
         """
     def delete_state_machine(self, *, stateMachineArn: str) -> Dict[str, Any]:
         """
         Deletes a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine)
         """
+    def delete_state_machine_alias(self, *, stateMachineAliasArn: str) -> Dict[str, Any]:
+        """
+        Deletes a state machine [alias](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-alias.html)_.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_alias)
+        """
+    def delete_state_machine_version(self, *, stateMachineVersionArn: str) -> Dict[str, Any]:
+        """
+        Deletes a state machine [version](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-version.html)_.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_version)
+        """
     def describe_activity(self, *, activityArn: str) -> DescribeActivityOutputTypeDef:
         """
         Describes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_activity)
         """
     def describe_execution(self, *, executionArn: str) -> DescribeExecutionOutputTypeDef:
         """
-        Provides all information about a state machine execution, such as the state
-        machine associated with the execution, the execution input and output, and
-        relevant execution metadata.
+        Provides information about a state machine execution, such as the state machine
+        associated with the execution, the execution input and output, and relevant
+        execution metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_execution)
         """
     def describe_map_run(self, *, mapRunArn: str) -> DescribeMapRunOutputTypeDef:
         """
         Provides information about a Map Run's configuration, progress, and results.
@@ -189,14 +233,24 @@
         """
         Provides information about a state machine's definition, its IAM role Amazon
         Resource Name (ARN), and configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine)
         """
+    def describe_state_machine_alias(
+        self, *, stateMachineAliasArn: str
+    ) -> DescribeStateMachineAliasOutputTypeDef:
+        """
+        Returns details about a state machine [alias](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-alias.html)_.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine_alias)
+        """
     def describe_state_machine_for_execution(
         self, *, executionArn: str
     ) -> DescribeStateMachineForExecutionOutputTypeDef:
         """
         Provides information about a state machine's definition, its execution role ARN,
         and configuration.
 
@@ -270,14 +324,35 @@
     ) -> ListMapRunsOutputTypeDef:
         """
         Lists all Map Runs that were started by a given state machine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_map_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_map_runs)
         """
+    def list_state_machine_aliases(
+        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListStateMachineAliasesOutputTypeDef:
+        """
+        Lists [aliases](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
+        state-machine-alias.html)_ for a specified state machine ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_aliases)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_aliases)
+        """
+    def list_state_machine_versions(
+        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListStateMachineVersionsOutputTypeDef:
+        """
+        Lists [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
+        state-machine-version.html)_ for the specified state machine Amazon Resource
+        Name (ARN).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_versions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_versions)
+        """
     def list_state_machines(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStateMachinesOutputTypeDef:
         """
         Lists the existing state machines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machines)
@@ -286,14 +361,25 @@
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         List tags for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_tags_for_resource)
         """
+    def publish_state_machine_version(
+        self, *, stateMachineArn: str, revisionId: str = ..., description: str = ...
+    ) -> PublishStateMachineVersionOutputTypeDef:
+        """
+        Creates a [version](https://docs.aws.amazon.com/step-
+        functions/latest/dg/concepts-state-machine-version.html)_ from the current
+        revision of a state machine.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.publish_state_machine_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#publish_state_machine_version)
+        """
     def send_task_failure(
         self, *, taskToken: str, error: str = ..., cause: str = ...
     ) -> Dict[str, Any]:
         """
         Used by activity workers and task states using the
         [callback](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
         resource.html#connect-wait-token)_ pattern to report that the task identified by
@@ -382,23 +468,40 @@
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...,
+        publish: bool = ...,
+        versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
-        Updates an existing state machine by modifying its `definition` , `roleArn` , or
+        Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine)
         """
+    def update_state_machine_alias(
+        self,
+        *,
+        stateMachineAliasArn: str,
+        description: str = ...,
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
+    ) -> UpdateStateMachineAliasOutputTypeDef:
+        """
+        Updates the configuration of an existing state machine
+        [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-
+        machine-alias.html)_ by modifying its `description` or `routingConfiguration`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine_alias)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine_alias)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["get_execution_history"]
     ) -> GetExecutionHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_paginator)
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.py` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,14 +124,15 @@
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
@@ -152,31 +153,34 @@
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
@@ -255,14 +259,15 @@
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
@@ -273,34 +278,38 @@
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
@@ -313,14 +322,15 @@
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
@@ -339,16 +349,19 @@
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
@@ -386,14 +399,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -427,18 +441,21 @@
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
@@ -474,14 +491,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.pyi` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,15 @@
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
@@ -150,31 +151,34 @@
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
@@ -253,14 +257,15 @@
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
@@ -271,34 +276,38 @@
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
@@ -311,14 +320,15 @@
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
@@ -337,16 +347,19 @@
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
@@ -384,14 +397,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -425,18 +439,21 @@
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
@@ -472,14 +489,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.py` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,30 +68,30 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 
 class ListActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
         """
 
 
@@ -103,43 +103,43 @@
 
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listexecutionspaginator)
         """
 
 
 class ListMapRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
     """
 
     def paginate(
-        self, *, executionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, executionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMapRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
         """
 
 
 class ListStateMachinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStateMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
         """
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.pyi` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,29 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 class ListActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
         """
 
 class ListExecutionsPaginator(Paginator):
@@ -98,41 +98,41 @@
 
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listexecutionspaginator)
         """
 
 class ListMapRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
     """
 
     def paginate(
-        self, *, executionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, executionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMapRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
         """
 
 class ListStateMachinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStateMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
         """
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.py` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -26,43 +26,50 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityFailedEventDetailsTypeDef",
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateActivityOutputTypeDef",
+    "RoutingConfigurationListItemTypeDef",
+    "CreateStateMachineAliasOutputTypeDef",
     "TracingConfigurationTypeDef",
+    "CreateStateMachineOutputTypeDef",
     "DeleteActivityInputRequestTypeDef",
+    "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
+    "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
+    "DescribeActivityOutputTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
+    "DescribeStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetActivityTaskOutputTypeDef",
+    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     "GetExecutionHistoryInputRequestTypeDef",
     "LambdaFunctionFailedEventDetailsTypeDef",
     "LambdaFunctionScheduleFailedEventDetailsTypeDef",
     "LambdaFunctionStartFailedEventDetailsTypeDef",
     "LambdaFunctionTimedOutEventDetailsTypeDef",
     "MapIterationEventDetailsTypeDef",
     "MapRunFailedEventDetailsTypeDef",
@@ -70,62 +77,71 @@
     "MapStateStartedEventDetailsTypeDef",
     "TaskFailedEventDetailsTypeDef",
     "TaskStartFailedEventDetailsTypeDef",
     "TaskStartedEventDetailsTypeDef",
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListActivitiesInputRequestTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
+    "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
+    "ListStateMachineAliasesInputRequestTypeDef",
+    "StateMachineAliasListItemTypeDef",
+    "ListStateMachineVersionsInputRequestTypeDef",
+    "StateMachineVersionListItemTypeDef",
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "PublishStateMachineVersionInputRequestTypeDef",
+    "PublishStateMachineVersionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
+    "StartExecutionOutputTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
+    "StopExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
+    "UpdateStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineOutputTypeDef",
+    "ListActivitiesOutputTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "StartSyncExecutionOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
-    "TagResourceInputRequestTypeDef",
-    "CreateActivityOutputTypeDef",
-    "CreateStateMachineOutputTypeDef",
-    "DescribeActivityOutputTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "GetActivityTaskOutputTypeDef",
-    "ListActivitiesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "StartExecutionOutputTypeDef",
-    "StartSyncExecutionOutputTypeDef",
-    "StopExecutionOutputTypeDef",
-    "UpdateStateMachineOutputTypeDef",
+    "TagResourceInputRequestTypeDef",
+    "CreateStateMachineAliasInputRequestTypeDef",
+    "DescribeStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
     "ListExecutionsOutputTypeDef",
-    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    "ListMapRunsInputListMapRunsPaginateTypeDef",
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
+    "ListStateMachineAliasesOutputTypeDef",
+    "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
@@ -214,54 +230,103 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateActivityOutputTypeDef = TypedDict(
+    "CreateActivityOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "activityArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RoutingConfigurationListItemTypeDef = TypedDict(
+    "RoutingConfigurationListItemTypeDef",
+    {
+        "stateMachineVersionArn": str,
+        "weight": int,
+    },
+)
+
+CreateStateMachineAliasOutputTypeDef = TypedDict(
+    "CreateStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
+CreateStateMachineOutputTypeDef = TypedDict(
+    "CreateStateMachineOutputTypeDef",
+    {
+        "stateMachineArn": str,
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
+DeleteStateMachineAliasInputRequestTypeDef = TypedDict(
+    "DeleteStateMachineAliasInputRequestTypeDef",
+    {
+        "stateMachineAliasArn": str,
+    },
+)
+
 DeleteStateMachineInputRequestTypeDef = TypedDict(
     "DeleteStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
+DeleteStateMachineVersionInputRequestTypeDef = TypedDict(
+    "DeleteStateMachineVersionInputRequestTypeDef",
+    {
+        "stateMachineVersionArn": str,
+    },
+)
+
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
+DescribeActivityOutputTypeDef = TypedDict(
+    "DescribeActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "name": str,
+        "creationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeExecutionInputRequestTypeDef = TypedDict(
     "DescribeExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -296,14 +361,21 @@
         "timedOut": int,
         "aborted": int,
         "total": int,
         "resultsWritten": int,
     },
 )
 
+DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
+    "DescribeStateMachineAliasInputRequestTypeDef",
+    {
+        "stateMachineAliasArn": str,
+    },
+)
+
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -344,25 +416,25 @@
 )
 _OptionalExecutionListItemTypeDef = TypedDict(
     "_OptionalExecutionListItemTypeDef",
     {
         "stopDate": datetime,
         "mapRunArn": str,
         "itemCount": int,
+        "stateMachineVersionArn": str,
+        "stateMachineAliasArn": str,
     },
     total=False,
 )
 
-
 class ExecutionListItemTypeDef(
     _RequiredExecutionListItemTypeDef, _OptionalExecutionListItemTypeDef
 ):
     pass
 
-
 ExecutionTimedOutEventDetailsTypeDef = TypedDict(
     "ExecutionTimedOutEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -378,31 +450,50 @@
     "_OptionalGetActivityTaskInputRequestTypeDef",
     {
         "workerName": str,
     },
     total=False,
 )
 
-
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
+GetActivityTaskOutputTypeDef = TypedDict(
+    "GetActivityTaskOutputTypeDef",
+    {
+        "taskToken": str,
+        "input": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "executionArn": str,
+    },
+)
+_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "includeExecutionData": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
+    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetExecutionHistoryInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalGetExecutionHistoryInputRequestTypeDef = TypedDict(
@@ -412,21 +503,19 @@
         "reverseOrder": bool,
         "nextToken": str,
         "includeExecutionData": bool,
     },
     total=False,
 )
 
-
 class GetExecutionHistoryInputRequestTypeDef(
     _RequiredGetExecutionHistoryInputRequestTypeDef, _OptionalGetExecutionHistoryInputRequestTypeDef
 ):
     pass
 
-
 LambdaFunctionFailedEventDetailsTypeDef = TypedDict(
     "LambdaFunctionFailedEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -505,21 +594,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskFailedEventDetailsTypeDef(
     _RequiredTaskFailedEventDetailsTypeDef, _OptionalTaskFailedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskStartFailedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskStartFailedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -528,21 +615,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskStartFailedEventDetailsTypeDef(
     _RequiredTaskStartFailedEventDetailsTypeDef, _OptionalTaskStartFailedEventDetailsTypeDef
 ):
     pass
 
-
 TaskStartedEventDetailsTypeDef = TypedDict(
     "TaskStartedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -559,21 +644,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskSubmitFailedEventDetailsTypeDef(
     _RequiredTaskSubmitFailedEventDetailsTypeDef, _OptionalTaskSubmitFailedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskTimedOutEventDetailsTypeDef = TypedDict(
     "_RequiredTaskTimedOutEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -582,50 +665,87 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskTimedOutEventDetailsTypeDef(
     _RequiredTaskTimedOutEventDetailsTypeDef, _OptionalTaskTimedOutEventDetailsTypeDef
 ):
     pass
 
-
 TaskCredentialsTypeDef = TypedDict(
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
 
+ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListActivitiesInputRequestTypeDef = TypedDict(
     "ListActivitiesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "stateMachineArn": str,
+        "statusFilter": ExecutionStatusType,
+        "mapRunArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListExecutionsInputRequestTypeDef = TypedDict(
     "ListExecutionsInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "statusFilter": ExecutionStatusType,
         "maxResults": int,
         "nextToken": str,
         "mapRunArn": str,
     },
     total=False,
 )
 
+_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListMapRunsInputListMapRunsPaginateTypeDef(
+    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
+    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+):
+    pass
+
 _RequiredListMapRunsInputRequestTypeDef = TypedDict(
     "_RequiredListMapRunsInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalListMapRunsInputRequestTypeDef = TypedDict(
@@ -633,21 +753,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListMapRunsInputRequestTypeDef(
     _RequiredListMapRunsInputRequestTypeDef, _OptionalListMapRunsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredMapRunListItemTypeDef = TypedDict(
     "_RequiredMapRunListItemTypeDef",
     {
         "executionArn": str,
         "mapRunArn": str,
         "stateMachineArn": str,
         "startDate": datetime,
@@ -657,18 +775,82 @@
     "_OptionalMapRunListItemTypeDef",
     {
         "stopDate": datetime,
     },
     total=False,
 )
 
-
 class MapRunListItemTypeDef(_RequiredMapRunListItemTypeDef, _OptionalMapRunListItemTypeDef):
     pass
 
+_RequiredListStateMachineAliasesInputRequestTypeDef = TypedDict(
+    "_RequiredListStateMachineAliasesInputRequestTypeDef",
+    {
+        "stateMachineArn": str,
+    },
+)
+_OptionalListStateMachineAliasesInputRequestTypeDef = TypedDict(
+    "_OptionalListStateMachineAliasesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListStateMachineAliasesInputRequestTypeDef(
+    _RequiredListStateMachineAliasesInputRequestTypeDef,
+    _OptionalListStateMachineAliasesInputRequestTypeDef,
+):
+    pass
+
+StateMachineAliasListItemTypeDef = TypedDict(
+    "StateMachineAliasListItemTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+    },
+)
+
+_RequiredListStateMachineVersionsInputRequestTypeDef = TypedDict(
+    "_RequiredListStateMachineVersionsInputRequestTypeDef",
+    {
+        "stateMachineArn": str,
+    },
+)
+_OptionalListStateMachineVersionsInputRequestTypeDef = TypedDict(
+    "_OptionalListStateMachineVersionsInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListStateMachineVersionsInputRequestTypeDef(
+    _RequiredListStateMachineVersionsInputRequestTypeDef,
+    _OptionalListStateMachineVersionsInputRequestTypeDef,
+):
+    pass
+
+StateMachineVersionListItemTypeDef = TypedDict(
+    "StateMachineVersionListItemTypeDef",
+    {
+        "stateMachineVersionArn": str,
+        "creationDate": datetime,
+    },
+)
+
+ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
@@ -688,14 +870,65 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
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
+_RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
+    "_RequiredPublishStateMachineVersionInputRequestTypeDef",
+    {
+        "stateMachineArn": str,
+    },
+)
+_OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
+    "_OptionalPublishStateMachineVersionInputRequestTypeDef",
+    {
+        "revisionId": str,
+        "description": str,
+    },
+    total=False,
+)
+
+class PublishStateMachineVersionInputRequestTypeDef(
+    _RequiredPublishStateMachineVersionInputRequestTypeDef,
+    _OptionalPublishStateMachineVersionInputRequestTypeDef,
+):
+    pass
+
+PublishStateMachineVersionOutputTypeDef = TypedDict(
+    "PublishStateMachineVersionOutputTypeDef",
+    {
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
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
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -703,21 +936,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class SendTaskFailureInputRequestTypeDef(
     _RequiredSendTaskFailureInputRequestTypeDef, _OptionalSendTaskFailureInputRequestTypeDef
 ):
     pass
 
-
 SendTaskHeartbeatInputRequestTypeDef = TypedDict(
     "SendTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 
@@ -741,20 +972,27 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
-
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
+StartExecutionOutputTypeDef = TypedDict(
+    "StartExecutionOutputTypeDef",
+    {
+        "executionArn": str,
+        "startDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
@@ -764,21 +1002,19 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
-
 class StartSyncExecutionInputRequestTypeDef(
     _RequiredStartSyncExecutionInputRequestTypeDef, _OptionalStartSyncExecutionInputRequestTypeDef
 ):
     pass
 
-
 _RequiredStopExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalStopExecutionInputRequestTypeDef = TypedDict(
@@ -786,20 +1022,26 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
+StopExecutionOutputTypeDef = TypedDict(
+    "StopExecutionOutputTypeDef",
+    {
+        "stopDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -817,20 +1059,45 @@
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
     },
     total=False,
 )
 
-
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
+UpdateStateMachineAliasOutputTypeDef = TypedDict(
+    "UpdateStateMachineAliasOutputTypeDef",
+    {
+        "updateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStateMachineOutputTypeDef = TypedDict(
+    "UpdateStateMachineOutputTypeDef",
+    {
+        "updateDate": datetime,
+        "revisionId": str,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListActivitiesOutputTypeDef = TypedDict(
+    "ListActivitiesOutputTypeDef",
+    {
+        "activities": List[ActivityListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
@@ -841,21 +1108,19 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
     },
     total=False,
 )
 
-
 class ActivityScheduledEventDetailsTypeDef(
     _RequiredActivityScheduledEventDetailsTypeDef, _OptionalActivityScheduledEventDetailsTypeDef
 ):
     pass
 
-
 ActivitySucceededEventDetailsTypeDef = TypedDict(
     "ActivitySucceededEventDetailsTypeDef",
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
@@ -863,14 +1128,16 @@
 
 ExecutionStartedEventDetailsTypeDef = TypedDict(
     "ExecutionStartedEventDetailsTypeDef",
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "roleArn": str,
+        "stateMachineAliasArn": str,
+        "stateMachineVersionArn": str,
     },
     total=False,
 )
 
 ExecutionSucceededEventDetailsTypeDef = TypedDict(
     "ExecutionSucceededEventDetailsTypeDef",
     {
@@ -900,21 +1167,19 @@
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StateEnteredEventDetailsTypeDef(
     _RequiredStateEnteredEventDetailsTypeDef, _OptionalStateEnteredEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredStateExitedEventDetailsTypeDef = TypedDict(
     "_RequiredStateExitedEventDetailsTypeDef",
     {
         "name": str,
     },
 )
 _OptionalStateExitedEventDetailsTypeDef = TypedDict(
@@ -922,21 +1187,19 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StateExitedEventDetailsTypeDef(
     _RequiredStateExitedEventDetailsTypeDef, _OptionalStateExitedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskSubmittedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSubmittedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -945,21 +1208,19 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class TaskSubmittedEventDetailsTypeDef(
     _RequiredTaskSubmittedEventDetailsTypeDef, _OptionalTaskSubmittedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskSucceededEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSucceededEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -968,86 +1229,19 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
-
-LogDestinationTypeDef = TypedDict(
-    "LogDestinationTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateActivityInputRequestTypeDef = TypedDict(
-    "_RequiredCreateActivityInputRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateActivityInputRequestTypeDef = TypedDict(
-    "_OptionalCreateActivityInputRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateActivityInputRequestTypeDef(
-    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
-):
-    pass
-
-
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateActivityOutputTypeDef = TypedDict(
-    "CreateActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStateMachineOutputTypeDef = TypedDict(
-    "CreateStateMachineOutputTypeDef",
-    {
-        "stateMachineArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeActivityOutputTypeDef = TypedDict(
-    "DescribeActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "name": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeExecutionOutputTypeDef = TypedDict(
     "DescribeExecutionOutputTypeDef",
     {
         "executionArn": str,
         "stateMachineArn": str,
         "name": str,
         "status": ExecutionStatusType,
@@ -1057,50 +1251,17 @@
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetActivityTaskOutputTypeDef = TypedDict(
-    "GetActivityTaskOutputTypeDef",
-    {
-        "taskToken": str,
-        "input": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListActivitiesOutputTypeDef = TypedDict(
-    "ListActivitiesOutputTypeDef",
-    {
-        "activities": List[ActivityListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartExecutionOutputTypeDef = TypedDict(
-    "StartExecutionOutputTypeDef",
-    {
-        "executionArn": str,
-        "startDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "stateMachineVersionArn": str,
+        "stateMachineAliasArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSyncExecutionOutputTypeDef = TypedDict(
     "StartSyncExecutionOutputTypeDef",
     {
         "executionArn": str,
@@ -1113,131 +1274,140 @@
         "cause": str,
         "input": str,
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "billingDetails": BillingDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopExecutionOutputTypeDef = TypedDict(
-    "StopExecutionOutputTypeDef",
+LogDestinationTypeDef = TypedDict(
+    "LogDestinationTypeDef",
     {
-        "stopDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
+    total=False,
 )
 
-UpdateStateMachineOutputTypeDef = TypedDict(
-    "UpdateStateMachineOutputTypeDef",
+_RequiredCreateActivityInputRequestTypeDef = TypedDict(
+    "_RequiredCreateActivityInputRequestTypeDef",
     {
-        "updateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
     },
 )
+_OptionalCreateActivityInputRequestTypeDef = TypedDict(
+    "_OptionalCreateActivityInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
 
-DescribeMapRunOutputTypeDef = TypedDict(
-    "DescribeMapRunOutputTypeDef",
+class CreateActivityInputRequestTypeDef(
+    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
+):
+    pass
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
-        "mapRunArn": str,
-        "executionArn": str,
-        "status": MapRunStatusType,
-        "startDate": datetime,
-        "stopDate": datetime,
-        "maxConcurrency": int,
-        "toleratedFailurePercentage": float,
-        "toleratedFailureCount": int,
-        "itemCounts": MapRunItemCountsTypeDef,
-        "executionCounts": MapRunExecutionCountsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListExecutionsOutputTypeDef = TypedDict(
-    "ListExecutionsOutputTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "executions": List[ExecutionListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+_RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineAliasInputRequestTypeDef",
     {
-        "executionArn": str,
+        "name": str,
+        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
     },
 )
-_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+_OptionalCreateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineAliasInputRequestTypeDef",
     {
-        "reverseOrder": bool,
-        "includeExecutionData": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "description": str,
     },
     total=False,
 )
 
-
-class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
-    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+class CreateStateMachineAliasInputRequestTypeDef(
+    _RequiredCreateStateMachineAliasInputRequestTypeDef,
+    _OptionalCreateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
-
-ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
+DescribeStateMachineAliasOutputTypeDef = TypedDict(
+    "DescribeStateMachineAliasOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "stateMachineArn": str,
-        "statusFilter": ExecutionStatusType,
-        "mapRunArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "stateMachineAliasArn": str,
+        "name": str,
+        "description": str,
+        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
+        "creationDate": datetime,
+        "updateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+_RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
-        "executionArn": str,
+        "stateMachineAliasArn": str,
     },
 )
-_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+_OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateStateMachineAliasInputRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "description": str,
+        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
     },
     total=False,
 )
 
-
-class ListMapRunsInputListMapRunsPaginateTypeDef(
-    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
-    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+class UpdateStateMachineAliasInputRequestTypeDef(
+    _RequiredUpdateStateMachineAliasInputRequestTypeDef,
+    _OptionalUpdateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
+DescribeMapRunOutputTypeDef = TypedDict(
+    "DescribeMapRunOutputTypeDef",
+    {
+        "mapRunArn": str,
+        "executionArn": str,
+        "status": MapRunStatusType,
+        "startDate": datetime,
+        "stopDate": datetime,
+        "maxConcurrency": int,
+        "toleratedFailurePercentage": float,
+        "toleratedFailureCount": int,
+        "itemCounts": MapRunItemCountsTypeDef,
+        "executionCounts": MapRunExecutionCountsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+ListExecutionsOutputTypeDef = TypedDict(
+    "ListExecutionsOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "executions": List[ExecutionListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
@@ -1249,22 +1419,20 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class LambdaFunctionScheduledEventDetailsTypeDef(
     _RequiredLambdaFunctionScheduledEventDetailsTypeDef,
     _OptionalLambdaFunctionScheduledEventDetailsTypeDef,
 ):
     pass
 
-
 _RequiredTaskScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredTaskScheduledEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
         "region": str,
         "parameters": str,
@@ -1276,36 +1444,52 @@
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class TaskScheduledEventDetailsTypeDef(
     _RequiredTaskScheduledEventDetailsTypeDef, _OptionalTaskScheduledEventDetailsTypeDef
 ):
     pass
 
-
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStateMachineAliasesOutputTypeDef = TypedDict(
+    "ListStateMachineAliasesOutputTypeDef",
+    {
+        "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStateMachineVersionsOutputTypeDef = TypedDict(
+    "ListStateMachineVersionsOutputTypeDef",
+    {
+        "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
@@ -1361,19 +1545,17 @@
         "stateExitedEventDetails": StateExitedEventDetailsTypeDef,
         "mapRunStartedEventDetails": MapRunStartedEventDetailsTypeDef,
         "mapRunFailedEventDetails": MapRunFailedEventDetailsTypeDef,
     },
     total=False,
 )
 
-
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
-
 _RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineInputRequestTypeDef",
     {
         "name": str,
         "definition": str,
         "roleArn": str,
     },
@@ -1381,38 +1563,39 @@
 _OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalCreateStateMachineInputRequestTypeDef",
     {
         "type": StateMachineTypeType,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
     },
     total=False,
 )
 
-
 class CreateStateMachineInputRequestTypeDef(
     _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
 ):
     pass
 
-
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
@@ -1421,15 +1604,17 @@
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "revisionId": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
@@ -1438,26 +1623,26 @@
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalUpdateStateMachineInputRequestTypeDef",
     {
         "definition": str,
         "roleArn": str,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
     },
     total=False,
 )
 
-
 class UpdateStateMachineInputRequestTypeDef(
     _RequiredUpdateStateMachineInputRequestTypeDef, _OptionalUpdateStateMachineInputRequestTypeDef
 ):
     pass
 
-
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,42 +26,51 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActivityFailedEventDetailsTypeDef",
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateActivityOutputTypeDef",
+    "RoutingConfigurationListItemTypeDef",
+    "CreateStateMachineAliasOutputTypeDef",
     "TracingConfigurationTypeDef",
+    "CreateStateMachineOutputTypeDef",
     "DeleteActivityInputRequestTypeDef",
+    "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
+    "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
+    "DescribeActivityOutputTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
+    "DescribeStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetActivityTaskOutputTypeDef",
+    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     "GetExecutionHistoryInputRequestTypeDef",
     "LambdaFunctionFailedEventDetailsTypeDef",
     "LambdaFunctionScheduleFailedEventDetailsTypeDef",
     "LambdaFunctionStartFailedEventDetailsTypeDef",
     "LambdaFunctionTimedOutEventDetailsTypeDef",
     "MapIterationEventDetailsTypeDef",
     "MapRunFailedEventDetailsTypeDef",
@@ -69,62 +78,71 @@
     "MapStateStartedEventDetailsTypeDef",
     "TaskFailedEventDetailsTypeDef",
     "TaskStartFailedEventDetailsTypeDef",
     "TaskStartedEventDetailsTypeDef",
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListActivitiesInputRequestTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
+    "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
+    "ListStateMachineAliasesInputRequestTypeDef",
+    "StateMachineAliasListItemTypeDef",
+    "ListStateMachineVersionsInputRequestTypeDef",
+    "StateMachineVersionListItemTypeDef",
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "PublishStateMachineVersionInputRequestTypeDef",
+    "PublishStateMachineVersionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
+    "StartExecutionOutputTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
+    "StopExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
+    "UpdateStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineOutputTypeDef",
+    "ListActivitiesOutputTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "StartSyncExecutionOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
-    "TagResourceInputRequestTypeDef",
-    "CreateActivityOutputTypeDef",
-    "CreateStateMachineOutputTypeDef",
-    "DescribeActivityOutputTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "GetActivityTaskOutputTypeDef",
-    "ListActivitiesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "StartExecutionOutputTypeDef",
-    "StartSyncExecutionOutputTypeDef",
-    "StopExecutionOutputTypeDef",
-    "UpdateStateMachineOutputTypeDef",
+    "TagResourceInputRequestTypeDef",
+    "CreateStateMachineAliasInputRequestTypeDef",
+    "DescribeStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
     "ListExecutionsOutputTypeDef",
-    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    "ListMapRunsInputListMapRunsPaginateTypeDef",
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
+    "ListStateMachineAliasesOutputTypeDef",
+    "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
@@ -213,54 +231,103 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateActivityOutputTypeDef = TypedDict(
+    "CreateActivityOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "activityArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RoutingConfigurationListItemTypeDef = TypedDict(
+    "RoutingConfigurationListItemTypeDef",
+    {
+        "stateMachineVersionArn": str,
+        "weight": int,
+    },
+)
+
+CreateStateMachineAliasOutputTypeDef = TypedDict(
+    "CreateStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
+CreateStateMachineOutputTypeDef = TypedDict(
+    "CreateStateMachineOutputTypeDef",
+    {
+        "stateMachineArn": str,
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
+DeleteStateMachineAliasInputRequestTypeDef = TypedDict(
+    "DeleteStateMachineAliasInputRequestTypeDef",
+    {
+        "stateMachineAliasArn": str,
+    },
+)
+
 DeleteStateMachineInputRequestTypeDef = TypedDict(
     "DeleteStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
+DeleteStateMachineVersionInputRequestTypeDef = TypedDict(
+    "DeleteStateMachineVersionInputRequestTypeDef",
+    {
+        "stateMachineVersionArn": str,
+    },
+)
+
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
+DescribeActivityOutputTypeDef = TypedDict(
+    "DescribeActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "name": str,
+        "creationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeExecutionInputRequestTypeDef = TypedDict(
     "DescribeExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -295,14 +362,21 @@
         "timedOut": int,
         "aborted": int,
         "total": int,
         "resultsWritten": int,
     },
 )
 
+DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
+    "DescribeStateMachineAliasInputRequestTypeDef",
+    {
+        "stateMachineAliasArn": str,
+    },
+)
+
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -343,23 +417,27 @@
 )
 _OptionalExecutionListItemTypeDef = TypedDict(
     "_OptionalExecutionListItemTypeDef",
     {
         "stopDate": datetime,
         "mapRunArn": str,
         "itemCount": int,
+        "stateMachineVersionArn": str,
+        "stateMachineAliasArn": str,
     },
     total=False,
 )
 
+
 class ExecutionListItemTypeDef(
     _RequiredExecutionListItemTypeDef, _OptionalExecutionListItemTypeDef
 ):
     pass
 
+
 ExecutionTimedOutEventDetailsTypeDef = TypedDict(
     "ExecutionTimedOutEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -375,29 +453,54 @@
     "_OptionalGetActivityTaskInputRequestTypeDef",
     {
         "workerName": str,
     },
     total=False,
 )
 
+
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+GetActivityTaskOutputTypeDef = TypedDict(
+    "GetActivityTaskOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "taskToken": str,
+        "input": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "includeExecutionData": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
+    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetExecutionHistoryInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalGetExecutionHistoryInputRequestTypeDef = TypedDict(
@@ -407,19 +510,21 @@
         "reverseOrder": bool,
         "nextToken": str,
         "includeExecutionData": bool,
     },
     total=False,
 )
 
+
 class GetExecutionHistoryInputRequestTypeDef(
     _RequiredGetExecutionHistoryInputRequestTypeDef, _OptionalGetExecutionHistoryInputRequestTypeDef
 ):
     pass
 
+
 LambdaFunctionFailedEventDetailsTypeDef = TypedDict(
     "LambdaFunctionFailedEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -498,19 +603,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskFailedEventDetailsTypeDef(
     _RequiredTaskFailedEventDetailsTypeDef, _OptionalTaskFailedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskStartFailedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskStartFailedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -519,19 +626,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskStartFailedEventDetailsTypeDef(
     _RequiredTaskStartFailedEventDetailsTypeDef, _OptionalTaskStartFailedEventDetailsTypeDef
 ):
     pass
 
+
 TaskStartedEventDetailsTypeDef = TypedDict(
     "TaskStartedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -548,19 +657,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskSubmitFailedEventDetailsTypeDef(
     _RequiredTaskSubmitFailedEventDetailsTypeDef, _OptionalTaskSubmitFailedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskTimedOutEventDetailsTypeDef = TypedDict(
     "_RequiredTaskTimedOutEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -569,48 +680,91 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskTimedOutEventDetailsTypeDef(
     _RequiredTaskTimedOutEventDetailsTypeDef, _OptionalTaskTimedOutEventDetailsTypeDef
 ):
     pass
 
+
 TaskCredentialsTypeDef = TypedDict(
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
 
+ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListActivitiesInputRequestTypeDef = TypedDict(
     "ListActivitiesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "stateMachineArn": str,
+        "statusFilter": ExecutionStatusType,
+        "mapRunArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListExecutionsInputRequestTypeDef = TypedDict(
     "ListExecutionsInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "statusFilter": ExecutionStatusType,
         "maxResults": int,
         "nextToken": str,
         "mapRunArn": str,
     },
     total=False,
 )
 
+_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListMapRunsInputListMapRunsPaginateTypeDef(
+    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
+    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListMapRunsInputRequestTypeDef = TypedDict(
     "_RequiredListMapRunsInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalListMapRunsInputRequestTypeDef = TypedDict(
@@ -618,19 +772,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListMapRunsInputRequestTypeDef(
     _RequiredListMapRunsInputRequestTypeDef, _OptionalListMapRunsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredMapRunListItemTypeDef = TypedDict(
     "_RequiredMapRunListItemTypeDef",
     {
         "executionArn": str,
         "mapRunArn": str,
         "stateMachineArn": str,
         "startDate": datetime,
@@ -640,17 +796,89 @@
     "_OptionalMapRunListItemTypeDef",
     {
         "stopDate": datetime,
     },
     total=False,
 )
 
+
 class MapRunListItemTypeDef(_RequiredMapRunListItemTypeDef, _OptionalMapRunListItemTypeDef):
     pass
 
+
+_RequiredListStateMachineAliasesInputRequestTypeDef = TypedDict(
+    "_RequiredListStateMachineAliasesInputRequestTypeDef",
+    {
+        "stateMachineArn": str,
+    },
+)
+_OptionalListStateMachineAliasesInputRequestTypeDef = TypedDict(
+    "_OptionalListStateMachineAliasesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListStateMachineAliasesInputRequestTypeDef(
+    _RequiredListStateMachineAliasesInputRequestTypeDef,
+    _OptionalListStateMachineAliasesInputRequestTypeDef,
+):
+    pass
+
+
+StateMachineAliasListItemTypeDef = TypedDict(
+    "StateMachineAliasListItemTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+    },
+)
+
+_RequiredListStateMachineVersionsInputRequestTypeDef = TypedDict(
+    "_RequiredListStateMachineVersionsInputRequestTypeDef",
+    {
+        "stateMachineArn": str,
+    },
+)
+_OptionalListStateMachineVersionsInputRequestTypeDef = TypedDict(
+    "_OptionalListStateMachineVersionsInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListStateMachineVersionsInputRequestTypeDef(
+    _RequiredListStateMachineVersionsInputRequestTypeDef,
+    _OptionalListStateMachineVersionsInputRequestTypeDef,
+):
+    pass
+
+
+StateMachineVersionListItemTypeDef = TypedDict(
+    "StateMachineVersionListItemTypeDef",
+    {
+        "stateMachineVersionArn": str,
+        "creationDate": datetime,
+    },
+)
+
+ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -669,14 +897,67 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
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
+_RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
+    "_RequiredPublishStateMachineVersionInputRequestTypeDef",
+    {
+        "stateMachineArn": str,
+    },
+)
+_OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
+    "_OptionalPublishStateMachineVersionInputRequestTypeDef",
+    {
+        "revisionId": str,
+        "description": str,
+    },
+    total=False,
+)
+
+
+class PublishStateMachineVersionInputRequestTypeDef(
+    _RequiredPublishStateMachineVersionInputRequestTypeDef,
+    _OptionalPublishStateMachineVersionInputRequestTypeDef,
+):
+    pass
+
+
+PublishStateMachineVersionOutputTypeDef = TypedDict(
+    "PublishStateMachineVersionOutputTypeDef",
+    {
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
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
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -684,19 +965,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class SendTaskFailureInputRequestTypeDef(
     _RequiredSendTaskFailureInputRequestTypeDef, _OptionalSendTaskFailureInputRequestTypeDef
 ):
     pass
 
+
 SendTaskHeartbeatInputRequestTypeDef = TypedDict(
     "SendTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 
@@ -720,19 +1003,30 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
+
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
+
+StartExecutionOutputTypeDef = TypedDict(
+    "StartExecutionOutputTypeDef",
+    {
+        "executionArn": str,
+        "startDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -741,19 +1035,21 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
+
 class StartSyncExecutionInputRequestTypeDef(
     _RequiredStartSyncExecutionInputRequestTypeDef, _OptionalStartSyncExecutionInputRequestTypeDef
 ):
     pass
 
+
 _RequiredStopExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalStopExecutionInputRequestTypeDef = TypedDict(
@@ -761,19 +1057,29 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
+
+StopExecutionOutputTypeDef = TypedDict(
+    "StopExecutionOutputTypeDef",
+    {
+        "stopDate": datetime,
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
@@ -790,19 +1096,48 @@
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
     },
     total=False,
 )
 
+
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
+
+UpdateStateMachineAliasOutputTypeDef = TypedDict(
+    "UpdateStateMachineAliasOutputTypeDef",
+    {
+        "updateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStateMachineOutputTypeDef = TypedDict(
+    "UpdateStateMachineOutputTypeDef",
+    {
+        "updateDate": datetime,
+        "revisionId": str,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListActivitiesOutputTypeDef = TypedDict(
+    "ListActivitiesOutputTypeDef",
+    {
+        "activities": List[ActivityListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -812,19 +1147,21 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
     },
     total=False,
 )
 
+
 class ActivityScheduledEventDetailsTypeDef(
     _RequiredActivityScheduledEventDetailsTypeDef, _OptionalActivityScheduledEventDetailsTypeDef
 ):
     pass
 
+
 ActivitySucceededEventDetailsTypeDef = TypedDict(
     "ActivitySucceededEventDetailsTypeDef",
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
@@ -832,14 +1169,16 @@
 
 ExecutionStartedEventDetailsTypeDef = TypedDict(
     "ExecutionStartedEventDetailsTypeDef",
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "roleArn": str,
+        "stateMachineAliasArn": str,
+        "stateMachineVersionArn": str,
     },
     total=False,
 )
 
 ExecutionSucceededEventDetailsTypeDef = TypedDict(
     "ExecutionSucceededEventDetailsTypeDef",
     {
@@ -869,19 +1208,21 @@
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StateEnteredEventDetailsTypeDef(
     _RequiredStateEnteredEventDetailsTypeDef, _OptionalStateEnteredEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredStateExitedEventDetailsTypeDef = TypedDict(
     "_RequiredStateExitedEventDetailsTypeDef",
     {
         "name": str,
     },
 )
 _OptionalStateExitedEventDetailsTypeDef = TypedDict(
@@ -889,19 +1230,21 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StateExitedEventDetailsTypeDef(
     _RequiredStateExitedEventDetailsTypeDef, _OptionalStateExitedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskSubmittedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSubmittedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -910,19 +1253,21 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class TaskSubmittedEventDetailsTypeDef(
     _RequiredTaskSubmittedEventDetailsTypeDef, _OptionalTaskSubmittedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskSucceededEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSucceededEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -931,81 +1276,20 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
-LogDestinationTypeDef = TypedDict(
-    "LogDestinationTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateActivityInputRequestTypeDef = TypedDict(
-    "_RequiredCreateActivityInputRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateActivityInputRequestTypeDef = TypedDict(
-    "_OptionalCreateActivityInputRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateActivityInputRequestTypeDef(
-    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
-):
-    pass
-
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateActivityOutputTypeDef = TypedDict(
-    "CreateActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStateMachineOutputTypeDef = TypedDict(
-    "CreateStateMachineOutputTypeDef",
-    {
-        "stateMachineArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeActivityOutputTypeDef = TypedDict(
-    "DescribeActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "name": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 DescribeExecutionOutputTypeDef = TypedDict(
     "DescribeExecutionOutputTypeDef",
     {
         "executionArn": str,
         "stateMachineArn": str,
         "name": str,
@@ -1016,50 +1300,17 @@
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetActivityTaskOutputTypeDef = TypedDict(
-    "GetActivityTaskOutputTypeDef",
-    {
-        "taskToken": str,
-        "input": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListActivitiesOutputTypeDef = TypedDict(
-    "ListActivitiesOutputTypeDef",
-    {
-        "activities": List[ActivityListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartExecutionOutputTypeDef = TypedDict(
-    "StartExecutionOutputTypeDef",
-    {
-        "executionArn": str,
-        "startDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "stateMachineVersionArn": str,
+        "stateMachineAliasArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSyncExecutionOutputTypeDef = TypedDict(
     "StartSyncExecutionOutputTypeDef",
     {
         "executionArn": str,
@@ -1072,127 +1323,146 @@
         "cause": str,
         "input": str,
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "billingDetails": BillingDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopExecutionOutputTypeDef = TypedDict(
-    "StopExecutionOutputTypeDef",
+LogDestinationTypeDef = TypedDict(
+    "LogDestinationTypeDef",
     {
-        "stopDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
+    total=False,
 )
 
-UpdateStateMachineOutputTypeDef = TypedDict(
-    "UpdateStateMachineOutputTypeDef",
+_RequiredCreateActivityInputRequestTypeDef = TypedDict(
+    "_RequiredCreateActivityInputRequestTypeDef",
     {
-        "updateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
     },
 )
+_OptionalCreateActivityInputRequestTypeDef = TypedDict(
+    "_OptionalCreateActivityInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
 
-DescribeMapRunOutputTypeDef = TypedDict(
-    "DescribeMapRunOutputTypeDef",
+
+class CreateActivityInputRequestTypeDef(
+    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
+):
+    pass
+
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
-        "mapRunArn": str,
-        "executionArn": str,
-        "status": MapRunStatusType,
-        "startDate": datetime,
-        "stopDate": datetime,
-        "maxConcurrency": int,
-        "toleratedFailurePercentage": float,
-        "toleratedFailureCount": int,
-        "itemCounts": MapRunItemCountsTypeDef,
-        "executionCounts": MapRunExecutionCountsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListExecutionsOutputTypeDef = TypedDict(
-    "ListExecutionsOutputTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "executions": List[ExecutionListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+_RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineAliasInputRequestTypeDef",
     {
-        "executionArn": str,
+        "name": str,
+        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
     },
 )
-_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+_OptionalCreateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineAliasInputRequestTypeDef",
     {
-        "reverseOrder": bool,
-        "includeExecutionData": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "description": str,
     },
     total=False,
 )
 
-class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
-    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+
+class CreateStateMachineAliasInputRequestTypeDef(
+    _RequiredCreateStateMachineAliasInputRequestTypeDef,
+    _OptionalCreateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
-ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
-ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
+DescribeStateMachineAliasOutputTypeDef = TypedDict(
+    "DescribeStateMachineAliasOutputTypeDef",
     {
-        "stateMachineArn": str,
-        "statusFilter": ExecutionStatusType,
-        "mapRunArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "stateMachineAliasArn": str,
+        "name": str,
+        "description": str,
+        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
+        "creationDate": datetime,
+        "updateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+_RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
-        "executionArn": str,
+        "stateMachineAliasArn": str,
     },
 )
-_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+_OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateStateMachineAliasInputRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "description": str,
+        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
     },
     total=False,
 )
 
-class ListMapRunsInputListMapRunsPaginateTypeDef(
-    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
-    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+
+class UpdateStateMachineAliasInputRequestTypeDef(
+    _RequiredUpdateStateMachineAliasInputRequestTypeDef,
+    _OptionalUpdateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
-ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+
+DescribeMapRunOutputTypeDef = TypedDict(
+    "DescribeMapRunOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "mapRunArn": str,
+        "executionArn": str,
+        "status": MapRunStatusType,
+        "startDate": datetime,
+        "stopDate": datetime,
+        "maxConcurrency": int,
+        "toleratedFailurePercentage": float,
+        "toleratedFailureCount": int,
+        "itemCounts": MapRunItemCountsTypeDef,
+        "executionCounts": MapRunExecutionCountsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListExecutionsOutputTypeDef = TypedDict(
+    "ListExecutionsOutputTypeDef",
+    {
+        "executions": List[ExecutionListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
@@ -1204,20 +1474,22 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class LambdaFunctionScheduledEventDetailsTypeDef(
     _RequiredLambdaFunctionScheduledEventDetailsTypeDef,
     _OptionalLambdaFunctionScheduledEventDetailsTypeDef,
 ):
     pass
 
+
 _RequiredTaskScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredTaskScheduledEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
         "region": str,
         "parameters": str,
@@ -1229,34 +1501,54 @@
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class TaskScheduledEventDetailsTypeDef(
     _RequiredTaskScheduledEventDetailsTypeDef, _OptionalTaskScheduledEventDetailsTypeDef
 ):
     pass
 
+
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStateMachineAliasesOutputTypeDef = TypedDict(
+    "ListStateMachineAliasesOutputTypeDef",
+    {
+        "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStateMachineVersionsOutputTypeDef = TypedDict(
+    "ListStateMachineVersionsOutputTypeDef",
+    {
+        "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
@@ -1312,17 +1604,19 @@
         "stateExitedEventDetails": StateExitedEventDetailsTypeDef,
         "mapRunStartedEventDetails": MapRunStartedEventDetailsTypeDef,
         "mapRunFailedEventDetails": MapRunFailedEventDetailsTypeDef,
     },
     total=False,
 )
 
+
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
+
 _RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineInputRequestTypeDef",
     {
         "name": str,
         "definition": str,
         "roleArn": str,
     },
@@ -1330,36 +1624,41 @@
 _OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalCreateStateMachineInputRequestTypeDef",
     {
         "type": StateMachineTypeType,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
     },
     total=False,
 )
 
+
 class CreateStateMachineInputRequestTypeDef(
     _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
 ):
     pass
 
+
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
@@ -1368,15 +1667,17 @@
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "revisionId": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
@@ -1385,24 +1686,28 @@
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalUpdateStateMachineInputRequestTypeDef",
     {
         "definition": str,
         "roleArn": str,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
     },
     total=False,
 )
 
+
 class UpdateStateMachineInputRequestTypeDef(
     _RequiredUpdateStateMachineInputRequestTypeDef, _OptionalUpdateStateMachineInputRequestTypeDef
 ):
     pass
 
+
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.26.21
-Summary: Type annotations for boto3.SFN 1.26.21 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.SFN 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
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
 
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,31 +354,39 @@
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateActivityOutputTypeDef,
+    RoutingConfigurationListItemTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
+    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
+    DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
+    DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
+    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
+    DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetActivityTaskOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -385,62 +394,71 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
+    ListStateMachineAliasesInputRequestTypeDef,
+    StateMachineAliasListItemTypeDef,
+    ListStateMachineVersionsInputRequestTypeDef,
+    StateMachineVersionListItemTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PublishStateMachineVersionInputRequestTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
+    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
+    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
+    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
+    DescribeExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateActivityOutputTypeDef,
-    CreateStateMachineOutputTypeDef,
-    DescribeActivityOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    GetActivityTaskOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    StartExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
-    StopExecutionOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
+    TagResourceInputRequestTypeDef,
+    CreateStateMachineAliasInputRequestTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
+    UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
+    ListStateMachineAliasesOutputTypeDef,
+    ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     UpdateStateMachineInputRequestTypeDef,
@@ -455,42 +473,42 @@
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

### Comparing `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy-boto3-stepfunctions-1.27.0/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.21/setup.py` & `mypy-boto3-stepfunctions-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-stepfunctions.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.26.21",
+    version="1.27.0",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SFN 1.26.21 service generated with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.SFN 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_stepfunctions": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_stepfunctions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/",
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


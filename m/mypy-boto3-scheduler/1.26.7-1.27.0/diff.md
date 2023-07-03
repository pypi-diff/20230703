# Comparing `tmp/mypy-boto3-scheduler-1.26.7.tar.gz` & `tmp/mypy-boto3-scheduler-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-scheduler-1.26.7.tar", last modified: Thu Nov 10 20:32:39 2022, max compression
+gzip compressed data, was "mypy-boto3-scheduler-1.27.0.tar", last modified: Mon Jul  3 19:51:25 2023, max compression
```

## Comparing `mypy-boto3-scheduler-1.26.7.tar` & `mypy-boto3-scheduler-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.517202 mypy-boto3-scheduler-1.26.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14537 2022-11-10 20:32:39.517202 mypy-boto3-scheduler-1.26.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13083 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.513202 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11721 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    11700 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7853 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7851 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    15526 2022-11-10 20:32:30.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    15504 2022-11-10 20:32:30.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.517202 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14537 2022-11-10 20:32:39.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-10 20:32:39.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-10 20:32:39.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 20:32:39.000000 mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 20:32:39.517202 mypy-boto3-scheduler-1.26.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-11-10 20:32:29.000000 mypy-boto3-scheduler-1.26.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.023955 mypy-boto3-scheduler-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-03 19:51:25.023955 mypy-boto3-scheduler-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.023955 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-07-03 19:47:30.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-03 19:47:30.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.023955 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-03 19:51:24.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:24.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:24.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:24.000000 mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:25.023955 mypy-boto3-scheduler-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-03 19:47:29.000000 mypy-boto3-scheduler-1.27.0/setup.py
```

### Comparing `mypy-boto3-scheduler-1.26.7/LICENSE` & `mypy-boto3-scheduler-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-scheduler-1.26.7/PKG-INFO` & `mypy-boto3-scheduler-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.26.7
-Summary: Type annotations for boto3.EventBridgeScheduler 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.EventBridgeScheduler 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
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
 
 <a id="mypy-boto3-scheduler"></a>
 
 # mypy-boto3-scheduler
 
 [![PyPI - mypy-boto3-scheduler](https://img.shields.io/pypi/v/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-scheduler?color=blue)](https://pypistats.org/packages/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,14 +314,15 @@
     PropagateTagsType,
     ScheduleGroupStateType,
     ScheduleStateType,
     EventBridgeSchedulerServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AssignPublicIpType) -> bool:
     ...
 ```
 
@@ -332,45 +334,45 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateScheduleGroupOutputTypeDef,
     FlexibleTimeWindowTypeDef,
+    CreateScheduleOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EventBridgeParametersTypeDef,
     GetScheduleGroupInputRequestTypeDef,
+    GetScheduleGroupOutputTypeDef,
     GetScheduleInputRequestTypeDef,
     KinesisParametersTypeDef,
-    PaginatorConfigTypeDef,
+    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
     ListScheduleGroupsInputRequestTypeDef,
     ScheduleGroupSummaryTypeDef,
+    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListSchedulesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RetryPolicyTypeDef,
     SageMakerPipelineParameterTypeDef,
     TargetSummaryTypeDef,
     SqsParametersTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateScheduleOutputTypeDef,
     NetworkConfigurationTypeDef,
     CreateScheduleGroupInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateScheduleGroupOutputTypeDef,
-    CreateScheduleOutputTypeDef,
-    GetScheduleGroupOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    UpdateScheduleOutputTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
+    TagResourceInputRequestTypeDef,
     ListScheduleGroupsOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     ScheduleSummaryTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
     TargetTypeDef,
     CreateScheduleInputRequestTypeDef,
@@ -386,42 +388,42 @@
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

### Comparing `mypy-boto3-scheduler-1.26.7/README.md` & `mypy-boto3-scheduler-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-scheduler"></a>
 
 # mypy-boto3-scheduler
 
 [![PyPI - mypy-boto3-scheduler](https://img.shields.io/pypi/v/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-scheduler?color=blue)](https://pypistats.org/packages/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,14 +282,15 @@
     PropagateTagsType,
     ScheduleGroupStateType,
     ScheduleStateType,
     EventBridgeSchedulerServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AssignPublicIpType) -> bool:
     ...
 ```
 
@@ -301,45 +302,45 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateScheduleGroupOutputTypeDef,
     FlexibleTimeWindowTypeDef,
+    CreateScheduleOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EventBridgeParametersTypeDef,
     GetScheduleGroupInputRequestTypeDef,
+    GetScheduleGroupOutputTypeDef,
     GetScheduleInputRequestTypeDef,
     KinesisParametersTypeDef,
-    PaginatorConfigTypeDef,
+    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
     ListScheduleGroupsInputRequestTypeDef,
     ScheduleGroupSummaryTypeDef,
+    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListSchedulesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RetryPolicyTypeDef,
     SageMakerPipelineParameterTypeDef,
     TargetSummaryTypeDef,
     SqsParametersTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateScheduleOutputTypeDef,
     NetworkConfigurationTypeDef,
     CreateScheduleGroupInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateScheduleGroupOutputTypeDef,
-    CreateScheduleOutputTypeDef,
-    GetScheduleGroupOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    UpdateScheduleOutputTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
+    TagResourceInputRequestTypeDef,
     ListScheduleGroupsOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     ScheduleSummaryTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
     TargetTypeDef,
     CreateScheduleInputRequestTypeDef,
@@ -355,42 +356,42 @@
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

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/__init__.py` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/__init__.pyi` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/__main__.py` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgeScheduler 1.26.7\nVersion:         1.26.7\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.EventBridgeScheduler 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.7")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/client.py` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
         State: ScheduleStateType = ...
     ) -> CreateScheduleOutputTypeDef:
         """
-        .
+        Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule)
         """
 
     def create_schedule_group(
         self, *, Name: str, ClientToken: str = ..., Tags: Sequence[TagTypeDef] = ...
@@ -158,15 +158,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#generate_presigned_url)
         """
 
     def get_schedule(self, *, Name: str, GroupName: str = ...) -> GetScheduleOutputTypeDef:
         """
-        .
+        Retrieves the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_schedule)
         """
 
     def get_schedule_group(self, *, Name: str) -> GetScheduleGroupOutputTypeDef:
         """
@@ -241,15 +241,15 @@
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
         State: ScheduleStateType = ...
     ) -> UpdateScheduleOutputTypeDef:
         """
-        .
+        Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#update_schedule)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/client.pyi` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
         State: ScheduleStateType = ...
     ) -> CreateScheduleOutputTypeDef:
         """
-        .
+        Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule)
         """
     def create_schedule_group(
         self, *, Name: str, ClientToken: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateScheduleGroupOutputTypeDef:
@@ -146,15 +146,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#generate_presigned_url)
         """
     def get_schedule(self, *, Name: str, GroupName: str = ...) -> GetScheduleOutputTypeDef:
         """
-        .
+        Retrieves the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_schedule)
         """
     def get_schedule_group(self, *, Name: str) -> GetScheduleGroupOutputTypeDef:
         """
         Retrieves the specified schedule group.
@@ -222,15 +222,15 @@
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
         State: ScheduleStateType = ...
     ) -> UpdateScheduleOutputTypeDef:
         """
-        .
+        Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#update_schedule)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_schedule_groups"]
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/literals.py` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
     "PlacementConstraintTypeType",
@@ -30,17 +29,17 @@
     "PropagateTagsType",
     "ScheduleGroupStateType",
     "ScheduleStateType",
     "EventBridgeSchedulerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
-
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
 PlacementStrategyTypeType = Literal["binpack", "random", "spread"]
@@ -59,23 +58,25 @@
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
@@ -85,30 +86,35 @@
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
@@ -134,14 +140,15 @@
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
@@ -186,51 +193,57 @@
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
@@ -243,14 +256,15 @@
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
@@ -262,28 +276,35 @@
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
@@ -311,56 +332,64 @@
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
@@ -379,7 +408,36 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_schedule_groups", "list_schedules"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/literals.pyi` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/literals.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
     "PlacementConstraintTypeType",
@@ -29,16 +30,18 @@
     "PropagateTagsType",
     "ScheduleGroupStateType",
     "ScheduleStateType",
     "EventBridgeSchedulerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
+
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
 PlacementStrategyTypeType = Literal["binpack", "random", "spread"]
@@ -57,23 +60,25 @@
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
@@ -83,30 +88,35 @@
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
@@ -132,14 +142,15 @@
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
@@ -184,51 +195,57 @@
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
@@ -241,14 +258,15 @@
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
@@ -260,28 +278,35 @@
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
@@ -309,56 +334,64 @@
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
@@ -377,7 +410,36 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_schedule_groups", "list_schedules"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/paginator.py` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,51 +30,47 @@
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListScheduleGroupsPaginator", "ListSchedulesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListScheduleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
     """
 
     def paginate(
-        self, *, NamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, NamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScheduleGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
         """
 
-
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
     """
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         NamePrefix: str = ...,
         State: ScheduleStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchedulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/paginator.pyi` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,47 +30,51 @@
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListScheduleGroupsPaginator", "ListSchedulesPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListScheduleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
     """
 
     def paginate(
-        self, *, NamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, NamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScheduleGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
         """
 
+
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
     """
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         NamePrefix: str = ...,
         State: ScheduleStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchedulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/type_defs.py` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,45 +35,45 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateScheduleGroupOutputTypeDef",
     "FlexibleTimeWindowTypeDef",
+    "CreateScheduleOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeleteScheduleGroupInputRequestTypeDef",
     "DeleteScheduleInputRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EventBridgeParametersTypeDef",
     "GetScheduleGroupInputRequestTypeDef",
+    "GetScheduleGroupOutputTypeDef",
     "GetScheduleInputRequestTypeDef",
     "KinesisParametersTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
     "ListScheduleGroupsInputRequestTypeDef",
     "ScheduleGroupSummaryTypeDef",
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListSchedulesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryPolicyTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "TargetSummaryTypeDef",
     "SqsParametersTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateScheduleOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateScheduleGroupInputRequestTypeDef",
-    "TagResourceInputRequestTypeDef",
-    "CreateScheduleGroupOutputTypeDef",
-    "CreateScheduleOutputTypeDef",
-    "GetScheduleGroupOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "UpdateScheduleOutputTypeDef",
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
+    "TagResourceInputRequestTypeDef",
     "ListScheduleGroupsOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "ScheduleSummaryTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
     "TargetTypeDef",
     "CreateScheduleInputRequestTypeDef",
@@ -129,22 +129,19 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateScheduleGroupOutputTypeDef = TypedDict(
+    "CreateScheduleGroupOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScheduleGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlexibleTimeWindowTypeDef = TypedDict(
     "_RequiredFlexibleTimeWindowTypeDef",
     {
         "Mode": FlexibleTimeWindowModeType,
@@ -161,14 +158,22 @@
 
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
 
+CreateScheduleOutputTypeDef = TypedDict(
+    "CreateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -245,14 +250,26 @@
 GetScheduleGroupInputRequestTypeDef = TypedDict(
     "GetScheduleGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetScheduleGroupOutputTypeDef = TypedDict(
+    "GetScheduleGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationDate": datetime,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "State": ScheduleGroupStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetScheduleInputRequestTypeDef = TypedDict(
     "_RequiredGetScheduleInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetScheduleInputRequestTypeDef = TypedDict(
@@ -273,20 +290,19 @@
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "NamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListScheduleGroupsInputRequestTypeDef = TypedDict(
     "ListScheduleGroupsInputRequestTypeDef",
     {
@@ -305,14 +321,25 @@
         "LastModificationDate": datetime,
         "Name": str,
         "State": ScheduleGroupStateType,
     },
     total=False,
 )
 
+ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
+    {
+        "GroupName": str,
+        "NamePrefix": str,
+        "State": ScheduleStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchedulesInputRequestTypeDef = TypedDict(
     "ListSchedulesInputRequestTypeDef",
     {
         "GroupName": str,
         "MaxResults": int,
         "NamePrefix": str,
         "NextToken": str,
@@ -324,14 +351,35 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumEventAgeInSeconds": int,
         "MaximumRetryAttempts": int,
     },
     total=False,
@@ -364,14 +412,22 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateScheduleOutputTypeDef = TypedDict(
+    "UpdateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -394,92 +450,36 @@
 
 class CreateScheduleGroupInputRequestTypeDef(
     _RequiredCreateScheduleGroupInputRequestTypeDef, _OptionalCreateScheduleGroupInputRequestTypeDef
 ):
     pass
 
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateScheduleGroupOutputTypeDef = TypedDict(
-    "CreateScheduleGroupOutputTypeDef",
-    {
-        "ScheduleGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScheduleOutputTypeDef = TypedDict(
-    "CreateScheduleOutputTypeDef",
-    {
-        "ScheduleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetScheduleGroupOutputTypeDef = TypedDict(
-    "GetScheduleGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationDate": datetime,
-        "LastModificationDate": datetime,
-        "Name": str,
-        "State": ScheduleGroupStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateScheduleOutputTypeDef = TypedDict(
-    "UpdateScheduleOutputTypeDef",
-    {
-        "ScheduleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
-    {
-        "NamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "GroupName": str,
-        "NamePrefix": str,
-        "State": ScheduleStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
 ListScheduleGroupsOutputTypeDef = TypedDict(
     "ListScheduleGroupsOutputTypeDef",
     {
         "NextToken": str,
         "ScheduleGroups": List[ScheduleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
         "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
@@ -533,15 +533,15 @@
 
 
 ListSchedulesOutputTypeDef = TypedDict(
     "ListSchedulesOutputTypeDef",
     {
         "NextToken": str,
         "Schedules": List[ScheduleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Arn": str,
@@ -612,15 +612,15 @@
         "LastModificationDate": datetime,
         "Name": str,
         "ScheduleExpression": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": datetime,
         "State": ScheduleStateType,
         "Target": TargetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler/type_defs.pyi` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,45 +34,45 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateScheduleGroupOutputTypeDef",
     "FlexibleTimeWindowTypeDef",
+    "CreateScheduleOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeleteScheduleGroupInputRequestTypeDef",
     "DeleteScheduleInputRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EventBridgeParametersTypeDef",
     "GetScheduleGroupInputRequestTypeDef",
+    "GetScheduleGroupOutputTypeDef",
     "GetScheduleInputRequestTypeDef",
     "KinesisParametersTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
     "ListScheduleGroupsInputRequestTypeDef",
     "ScheduleGroupSummaryTypeDef",
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListSchedulesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryPolicyTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "TargetSummaryTypeDef",
     "SqsParametersTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateScheduleOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateScheduleGroupInputRequestTypeDef",
-    "TagResourceInputRequestTypeDef",
-    "CreateScheduleGroupOutputTypeDef",
-    "CreateScheduleOutputTypeDef",
-    "GetScheduleGroupOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "UpdateScheduleOutputTypeDef",
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
+    "TagResourceInputRequestTypeDef",
     "ListScheduleGroupsOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "ScheduleSummaryTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
     "TargetTypeDef",
     "CreateScheduleInputRequestTypeDef",
@@ -124,22 +124,19 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateScheduleGroupOutputTypeDef = TypedDict(
+    "CreateScheduleGroupOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScheduleGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlexibleTimeWindowTypeDef = TypedDict(
     "_RequiredFlexibleTimeWindowTypeDef",
     {
         "Mode": FlexibleTimeWindowModeType,
@@ -154,14 +151,22 @@
 )
 
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
+CreateScheduleOutputTypeDef = TypedDict(
+    "CreateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -234,14 +239,26 @@
 GetScheduleGroupInputRequestTypeDef = TypedDict(
     "GetScheduleGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetScheduleGroupOutputTypeDef = TypedDict(
+    "GetScheduleGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationDate": datetime,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "State": ScheduleGroupStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetScheduleInputRequestTypeDef = TypedDict(
     "_RequiredGetScheduleInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetScheduleInputRequestTypeDef = TypedDict(
@@ -260,20 +277,19 @@
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "NamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListScheduleGroupsInputRequestTypeDef = TypedDict(
     "ListScheduleGroupsInputRequestTypeDef",
     {
@@ -292,14 +308,25 @@
         "LastModificationDate": datetime,
         "Name": str,
         "State": ScheduleGroupStateType,
     },
     total=False,
 )
 
+ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
+    {
+        "GroupName": str,
+        "NamePrefix": str,
+        "State": ScheduleStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchedulesInputRequestTypeDef = TypedDict(
     "ListSchedulesInputRequestTypeDef",
     {
         "GroupName": str,
         "MaxResults": int,
         "NamePrefix": str,
         "NextToken": str,
@@ -311,14 +338,35 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumEventAgeInSeconds": int,
         "MaximumRetryAttempts": int,
     },
     total=False,
@@ -351,14 +399,22 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateScheduleOutputTypeDef = TypedDict(
+    "UpdateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -379,92 +435,36 @@
 )
 
 class CreateScheduleGroupInputRequestTypeDef(
     _RequiredCreateScheduleGroupInputRequestTypeDef, _OptionalCreateScheduleGroupInputRequestTypeDef
 ):
     pass
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateScheduleGroupOutputTypeDef = TypedDict(
-    "CreateScheduleGroupOutputTypeDef",
-    {
-        "ScheduleGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScheduleOutputTypeDef = TypedDict(
-    "CreateScheduleOutputTypeDef",
-    {
-        "ScheduleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetScheduleGroupOutputTypeDef = TypedDict(
-    "GetScheduleGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationDate": datetime,
-        "LastModificationDate": datetime,
-        "Name": str,
-        "State": ScheduleGroupStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateScheduleOutputTypeDef = TypedDict(
-    "UpdateScheduleOutputTypeDef",
-    {
-        "ScheduleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
-    {
-        "NamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "GroupName": str,
-        "NamePrefix": str,
-        "State": ScheduleStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
 ListScheduleGroupsOutputTypeDef = TypedDict(
     "ListScheduleGroupsOutputTypeDef",
     {
         "NextToken": str,
         "ScheduleGroups": List[ScheduleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
         "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
@@ -516,15 +516,15 @@
     pass
 
 ListSchedulesOutputTypeDef = TypedDict(
     "ListSchedulesOutputTypeDef",
     {
         "NextToken": str,
         "Schedules": List[ScheduleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Arn": str,
@@ -591,15 +591,15 @@
         "LastModificationDate": datetime,
         "Name": str,
         "ScheduleExpression": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": datetime,
         "State": ScheduleStateType,
         "Target": TargetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
```

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/PKG-INFO` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.26.7
-Summary: Type annotations for boto3.EventBridgeScheduler 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.EventBridgeScheduler 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
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
 
 <a id="mypy-boto3-scheduler"></a>
 
 # mypy-boto3-scheduler
 
 [![PyPI - mypy-boto3-scheduler](https://img.shields.io/pypi/v/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-scheduler?color=blue)](https://pypistats.org/packages/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,14 +314,15 @@
     PropagateTagsType,
     ScheduleGroupStateType,
     ScheduleStateType,
     EventBridgeSchedulerServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AssignPublicIpType) -> bool:
     ...
 ```
 
@@ -332,45 +334,45 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateScheduleGroupOutputTypeDef,
     FlexibleTimeWindowTypeDef,
+    CreateScheduleOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EventBridgeParametersTypeDef,
     GetScheduleGroupInputRequestTypeDef,
+    GetScheduleGroupOutputTypeDef,
     GetScheduleInputRequestTypeDef,
     KinesisParametersTypeDef,
-    PaginatorConfigTypeDef,
+    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
     ListScheduleGroupsInputRequestTypeDef,
     ScheduleGroupSummaryTypeDef,
+    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListSchedulesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RetryPolicyTypeDef,
     SageMakerPipelineParameterTypeDef,
     TargetSummaryTypeDef,
     SqsParametersTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateScheduleOutputTypeDef,
     NetworkConfigurationTypeDef,
     CreateScheduleGroupInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateScheduleGroupOutputTypeDef,
-    CreateScheduleOutputTypeDef,
-    GetScheduleGroupOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    UpdateScheduleOutputTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
+    TagResourceInputRequestTypeDef,
     ListScheduleGroupsOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     ScheduleSummaryTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
     TargetTypeDef,
     CreateScheduleInputRequestTypeDef,
@@ -386,42 +388,42 @@
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

### Comparing `mypy-boto3-scheduler-1.26.7/mypy_boto3_scheduler.egg-info/SOURCES.txt` & `mypy-boto3-scheduler-1.27.0/mypy_boto3_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.26.7/setup.py` & `mypy-boto3-scheduler-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-scheduler.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-scheduler",
-    version="1.26.7",
+    version="1.27.0",
     packages=["mypy_boto3_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgeScheduler 1.26.7 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.EventBridgeScheduler 1.27.0 service generated with"
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
     keywords="boto3 scheduler type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_scheduler": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_scheduler": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/",
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


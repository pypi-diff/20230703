# Comparing `tmp/mypy-boto3-codeguruprofiler-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codeguruprofiler-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguruprofiler-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:14 2022, max compression
+gzip compressed data, was "mypy-boto3-codeguruprofiler-1.27.0.tar", last modified: Mon Jul  3 19:50:33 2023, max compression
```

## Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1.tar` & `mypy-boto3-codeguruprofiler-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.116817 mypy-boto3-codeguruprofiler-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15541 2022-11-01 21:43:14.116817 mypy-boto3-codeguruprofiler-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14064 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.112817 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18688 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    18657 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-11-01 21:31:56.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8156 2022-11-01 21:31:56.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    22258 2022-11-01 21:31:56.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22229 2022-11-01 21:31:56.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.116817 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15541 2022-11-01 21:43:13.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-01 21:43:13.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:13.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-01 21:43:13.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:14.116817 mypy-boto3-codeguruprofiler-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-01 21:31:55.000000 mypy-boto3-codeguruprofiler-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:33.495016 mypy-boto3-codeguruprofiler-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-03 19:50:33.495016 mypy-boto3-codeguruprofiler-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:33.495016 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-03 19:34:24.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:33.495016 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-03 19:50:33.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:50:33.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:33.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:50:33.000000 mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:33.495016 mypy-boto3-codeguruprofiler-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 19:34:23.000000 mypy-boto3-codeguruprofiler-1.27.0/setup.py
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/LICENSE` & `mypy-boto3-codeguruprofiler-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeGuruProfiler 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeGuruProfiler 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
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
 
 <a id="mypy-boto3-codeguruprofiler"></a>
 
 # mypy-boto3-codeguruprofiler
 
 [![PyPI - mypy-boto3-codeguruprofiler](https://img.shields.io/pypi/v/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguruprofiler?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,63 +329,63 @@
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
-    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
+    GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     ListFindingsReportsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
+    PaginatorConfigTypeDef,
     PatternTypeDef,
     PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
+    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    RemovePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
     NotificationConfigurationTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutPermissionResponseTypeDef,
-    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
     FrameMetricDatumTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     ProfilingGroupDescriptionTypeDef,
     AnomalyTypeDef,
@@ -404,42 +405,42 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/README.md` & `mypy-boto3-codeguruprofiler-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguruprofiler"></a>
 
 # mypy-boto3-codeguruprofiler
 
 [![PyPI - mypy-boto3-codeguruprofiler](https://img.shields.io/pypi/v/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguruprofiler?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,63 +297,63 @@
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
-    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
+    GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     ListFindingsReportsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
+    PaginatorConfigTypeDef,
     PatternTypeDef,
     PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
+    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    RemovePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
     NotificationConfigurationTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutPermissionResponseTypeDef,
-    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
     FrameMetricDatumTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     ProfilingGroupDescriptionTypeDef,
     AnomalyTypeDef,
@@ -373,42 +373,42 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/__init__.py` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/__init__.pyi` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/__main__.py` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruProfiler 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CodeGuruProfiler 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/client.py` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,15 +144,16 @@
         self,
         *,
         profilingGroupName: str,
         fleetInstanceId: str = ...,
         metadata: Mapping[MetadataFieldType, str] = ...
     ) -> ConfigureAgentResponseTypeDef:
         """
-        .
+        Used by profiler agents to report their current state and to receive remote
+        configuration updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#configure_agent)
         """
 
     def create_profiling_group(
         self,
@@ -160,15 +161,15 @@
         clientToken: str,
         profilingGroupName: str,
         agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateProfilingGroupResponseTypeDef:
         """
-        .
+        Creates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#create_profiling_group)
         """
 
     def delete_profiling_group(self, *, profilingGroupName: str) -> Dict[str, Any]:
         """
@@ -178,15 +179,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#delete_profiling_group)
         """
 
     def describe_profiling_group(
         self, *, profilingGroupName: str
     ) -> DescribeProfilingGroupResponseTypeDef:
         """
-        .
+        Returns a
+        [ProfilingGroupDescription](https://docs.aws.amazon.com/codeguru/latest/profiler-
+        api/API_ProfilingGroupDescription.html)_ object that contains information about
+        the requested profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.describe_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#describe_profiling_group)
         """
 
     def generate_presigned_url(
         self,
@@ -202,15 +206,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#generate_presigned_url)
         """
 
     def get_findings_report_account_summary(
         self, *, dailyReportsOnly: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetFindingsReportAccountSummaryResponseTypeDef:
         """
-        .
+        Returns a list of
+        [FindingsReportSummary](https://docs.aws.amazon.com/codeguru/latest/profiler-
+        api/API_FindingsReportSummary.html)_ objects that contain analysis results for
+        all profiling groups in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_findings_report_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_findings_report_account_summary)
         """
 
     def get_notification_configuration(
         self, *, profilingGroupName: str
@@ -252,15 +259,18 @@
         *,
         endTime: Union[datetime, str],
         profilingGroupName: str,
         startTime: Union[datetime, str],
         locale: str = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
-        .
+        Returns a list of
+        [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-
+        api/API_Recommendation.html)_ objects that contain recommendations for a
+        profiling group for a given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_recommendations)
         """
 
     def list_findings_reports(
         self,
@@ -298,15 +308,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profile_times)
         """
 
     def list_profiling_groups(
         self, *, includeDescription: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListProfilingGroupsResponseTypeDef:
         """
-        .
+        Returns a list of profiling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profiling_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profiling_groups)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -321,15 +331,15 @@
         *,
         agentProfile: Union[str, bytes, IO[Any], StreamingBody],
         contentType: str,
         profilingGroupName: str,
         profileToken: str = ...
     ) -> Dict[str, Any]:
         """
-        .
+        Submits profiling data to an aggregated profile of a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#post_agent_profile)
         """
 
     def put_permission(
         self,
@@ -357,30 +367,32 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_notification_channel)
         """
 
     def remove_permission(
         self, *, actionGroup: Literal["agentPermissions"], profilingGroupName: str, revisionId: str
     ) -> RemovePermissionResponseTypeDef:
         """
-        .
+        Removes permissions from a profiling group's resource-based policy that are
+        provided using an action group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_permission)
         """
 
     def submit_feedback(
         self,
         *,
         anomalyInstanceId: str,
         profilingGroupName: str,
         type: FeedbackTypeType,
         comment: str = ...
     ) -> Dict[str, Any]:
         """
-        .
+        Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
+        analysis is useful or not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#submit_feedback)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
@@ -398,15 +410,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#untag_resource)
         """
 
     def update_profiling_group(
         self, *, agentOrchestrationConfig: AgentOrchestrationConfigTypeDef, profilingGroupName: str
     ) -> UpdateProfilingGroupResponseTypeDef:
         """
-        .
+        Updates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.update_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#update_profiling_group)
         """
 
     def get_paginator(
         self, operation_name: Literal["list_profile_times"]
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/client.pyi` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -135,30 +135,31 @@
         self,
         *,
         profilingGroupName: str,
         fleetInstanceId: str = ...,
         metadata: Mapping[MetadataFieldType, str] = ...
     ) -> ConfigureAgentResponseTypeDef:
         """
-        .
+        Used by profiler agents to report their current state and to receive remote
+        configuration updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#configure_agent)
         """
     def create_profiling_group(
         self,
         *,
         clientToken: str,
         profilingGroupName: str,
         agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateProfilingGroupResponseTypeDef:
         """
-        .
+        Creates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#create_profiling_group)
         """
     def delete_profiling_group(self, *, profilingGroupName: str) -> Dict[str, Any]:
         """
         Deletes a profiling group.
@@ -166,15 +167,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.delete_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#delete_profiling_group)
         """
     def describe_profiling_group(
         self, *, profilingGroupName: str
     ) -> DescribeProfilingGroupResponseTypeDef:
         """
-        .
+        Returns a
+        [ProfilingGroupDescription](https://docs.aws.amazon.com/codeguru/latest/profiler-
+        api/API_ProfilingGroupDescription.html)_ object that contains information about
+        the requested profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.describe_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#describe_profiling_group)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -188,15 +192,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#generate_presigned_url)
         """
     def get_findings_report_account_summary(
         self, *, dailyReportsOnly: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetFindingsReportAccountSummaryResponseTypeDef:
         """
-        .
+        Returns a list of
+        [FindingsReportSummary](https://docs.aws.amazon.com/codeguru/latest/profiler-
+        api/API_FindingsReportSummary.html)_ objects that contain analysis results for
+        all profiling groups in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_findings_report_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_findings_report_account_summary)
         """
     def get_notification_configuration(
         self, *, profilingGroupName: str
     ) -> GetNotificationConfigurationResponseTypeDef:
@@ -234,15 +241,18 @@
         *,
         endTime: Union[datetime, str],
         profilingGroupName: str,
         startTime: Union[datetime, str],
         locale: str = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
-        .
+        Returns a list of
+        [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-
+        api/API_Recommendation.html)_ objects that contain recommendations for a
+        profiling group for a given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#get_recommendations)
         """
     def list_findings_reports(
         self,
         *,
@@ -277,15 +287,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profile_times)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profile_times)
         """
     def list_profiling_groups(
         self, *, includeDescription: bool = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListProfilingGroupsResponseTypeDef:
         """
-        .
+        Returns a list of profiling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profiling_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#list_profiling_groups)
         """
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags that are assigned to a specified resource.
@@ -298,15 +308,15 @@
         *,
         agentProfile: Union[str, bytes, IO[Any], StreamingBody],
         contentType: str,
         profilingGroupName: str,
         profileToken: str = ...
     ) -> Dict[str, Any]:
         """
-        .
+        Submits profiling data to an aggregated profile of a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#post_agent_profile)
         """
     def put_permission(
         self,
         *,
@@ -331,29 +341,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_notification_channel)
         """
     def remove_permission(
         self, *, actionGroup: Literal["agentPermissions"], profilingGroupName: str, revisionId: str
     ) -> RemovePermissionResponseTypeDef:
         """
-        .
+        Removes permissions from a profiling group's resource-based policy that are
+        provided using an action group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#remove_permission)
         """
     def submit_feedback(
         self,
         *,
         anomalyInstanceId: str,
         profilingGroupName: str,
         type: FeedbackTypeType,
         comment: str = ...
     ) -> Dict[str, Any]:
         """
-        .
+        Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
+        analysis is useful or not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#submit_feedback)
         """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Use to assign one or more tags to a resource.
@@ -368,15 +380,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#untag_resource)
         """
     def update_profiling_group(
         self, *, agentOrchestrationConfig: AgentOrchestrationConfigTypeDef, profilingGroupName: str
     ) -> UpdateProfilingGroupResponseTypeDef:
         """
-        .
+        Updates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.update_profiling_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/client/#update_profiling_group)
         """
     def get_paginator(
         self, operation_name: Literal["list_profile_times"]
     ) -> ListProfileTimesPaginator:
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/literals.py` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,23 +75,25 @@
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
@@ -101,30 +103,35 @@
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
@@ -150,14 +157,15 @@
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
@@ -202,51 +210,57 @@
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
@@ -259,14 +273,15 @@
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
@@ -278,28 +293,35 @@
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
@@ -308,14 +330,15 @@
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
@@ -326,55 +349,64 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/literals.pyi` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -73,23 +73,25 @@
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
@@ -99,30 +101,35 @@
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
@@ -148,14 +155,15 @@
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
@@ -200,51 +208,57 @@
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
@@ -257,14 +271,15 @@
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
@@ -276,28 +291,35 @@
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
@@ -306,14 +328,15 @@
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
@@ -324,55 +347,64 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/paginator.py` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,13 +50,13 @@
         self,
         *,
         endTime: Union[datetime, str],
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: Union[datetime, str],
         orderBy: OrderByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/paginator.pyi` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,13 +47,13 @@
         self,
         *,
         endTime: Union[datetime, str],
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: Union[datetime, str],
         orderBy: OrderByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/type_defs.py` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -31,66 +31,65 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChannelTypeDef",
-    "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
     "FrameMetricTypeDef",
     "TimestampStructureTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
+    "GetPolicyResponseTypeDef",
     "GetProfileRequestRequestTypeDef",
+    "GetProfileResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "ListFindingsReportsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesRequestRequestTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MatchTypeDef",
+    "PaginatorConfigTypeDef",
     "PatternTypeDef",
     "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
+    "PutPermissionResponseTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "RemovePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddNotificationChannelsRequestRequestTypeDef",
     "NotificationConfigurationTypeDef",
-    "GetPolicyResponseTypeDef",
-    "GetProfileResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutPermissionResponseTypeDef",
-    "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
     "BatchGetFrameMetricDataRequestRequestTypeDef",
     "FrameMetricDatumTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
-    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
     "ProfilingGroupDescriptionTypeDef",
     "AnomalyTypeDef",
@@ -113,30 +112,17 @@
     "_OptionalChannelTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
-
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
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
 _RequiredAgentConfigurationTypeDef = TypedDict(
     "_RequiredAgentConfigurationTypeDef",
     {
         "periodInSeconds": int,
         "shouldProfile": bool,
     },
 )
@@ -144,21 +130,19 @@
     "_OptionalAgentConfigurationTypeDef",
     {
         "agentParameters": Dict[AgentParameterFieldType, str],
     },
     total=False,
 )
 
-
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
-
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -214,21 +198,19 @@
     {
         "fleetInstanceId": str,
         "metadata": Mapping[MetadataFieldType, str],
     },
     total=False,
 )
 
-
 class ConfigureAgentRequestRequestTypeDef(
     _RequiredConfigureAgentRequestRequestTypeDef, _OptionalConfigureAgentRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProfilingGroupRequestRequestTypeDef = TypedDict(
     "DeleteProfilingGroupRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
@@ -271,14 +253,23 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetProfileRequestRequestTypeDef = TypedDict(
     "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalGetProfileRequestRequestTypeDef = TypedDict(
@@ -289,20 +280,28 @@
         "maxDepth": int,
         "period": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetProfileRequestRequestTypeDef(
     _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
+GetProfileResponseTypeDef = TypedDict(
+    "GetProfileResponseTypeDef",
+    {
+        "contentEncoding": str,
+        "contentType": str,
+        "profile": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
@@ -312,22 +311,20 @@
     "_OptionalGetRecommendationsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
-
 class GetRecommendationsRequestRequestTypeDef(
     _RequiredGetRecommendationsRequestRequestTypeDef,
     _OptionalGetRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsReportsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
     },
@@ -338,32 +335,44 @@
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListFindingsReportsRequestRequestTypeDef(
     _RequiredListFindingsReportsRequestRequestTypeDef,
     _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "endTime": Union[datetime, str],
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "orderBy": OrderByType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
+    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
+):
+    pass
+
 _RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
@@ -375,21 +384,19 @@
         "maxResults": int,
         "nextToken": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-
 class ListProfileTimesRequestRequestTypeDef(
     _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
 ):
     pass
 
-
 ProfileTimeTypeDef = TypedDict(
     "ProfileTimeTypeDef",
     {
         "start": datetime,
     },
     total=False,
 )
@@ -407,24 +414,42 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MatchTypeDef = TypedDict(
     "MatchTypeDef",
     {
         "frameAddress": str,
         "targetFramesIndex": int,
         "thresholdBreachValue": float,
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
 PatternTypeDef = TypedDict(
     "PatternTypeDef",
     {
         "countersToAggregate": List[str],
         "description": str,
         "id": str,
         "name": str,
@@ -447,21 +472,19 @@
     "_OptionalPostAgentProfileRequestRequestTypeDef",
     {
         "profileToken": str,
     },
     total=False,
 )
 
-
 class PostAgentProfileRequestRequestTypeDef(
     _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredPutPermissionRequestRequestTypeDef",
     {
         "actionGroup": Literal["agentPermissions"],
         "principals": Sequence[str],
         "profilingGroupName": str,
     },
@@ -470,20 +493,27 @@
     "_OptionalPutPermissionRequestRequestTypeDef",
     {
         "revisionId": str,
     },
     total=False,
 )
 
-
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
+PutPermissionResponseTypeDef = TypedDict(
+    "PutPermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
@@ -494,14 +524,34 @@
     {
         "actionGroup": Literal["agentPermissions"],
         "profilingGroupName": str,
         "revisionId": str,
     },
 )
 
+RemovePermissionResponseTypeDef = TypedDict(
+    "RemovePermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
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
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "anomalyInstanceId": str,
         "profilingGroupName": str,
         "type": FeedbackTypeType,
     },
@@ -510,21 +560,19 @@
     "_OptionalSubmitFeedbackRequestRequestTypeDef",
     {
         "comment": str,
     },
     total=False,
 )
 
-
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -549,64 +597,19 @@
     "NotificationConfigurationTypeDef",
     {
         "channels": List[ChannelTypeDef],
     },
     total=False,
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProfileResponseTypeDef = TypedDict(
-    "GetProfileResponseTypeDef",
-    {
-        "contentEncoding": str,
-        "contentType": str,
-        "profile": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutPermissionResponseTypeDef = TypedDict(
-    "PutPermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemovePermissionResponseTypeDef = TypedDict(
-    "RemovePermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProfilingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfilingGroupRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -619,22 +622,20 @@
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "computePlatform": ComputePlatformType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProfilingGroupRequestRequestTypeDef(
     _RequiredCreateProfilingGroupRequestRequestTypeDef,
     _OptionalCreateProfilingGroupRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateProfilingGroupRequestRequestTypeDef = TypedDict(
     "UpdateProfilingGroupRequestRequestTypeDef",
     {
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "profilingGroupName": str,
     },
 )
@@ -661,19 +662,17 @@
     {
         "endTime": datetime,
         "userFeedback": UserFeedbackTypeDef,
     },
     total=False,
 )
 
-
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
-
 _RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
@@ -684,80 +683,52 @@
         "period": str,
         "startTime": Union[datetime, str],
         "targetResolution": AggregationPeriodType,
     },
     total=False,
 )
 
-
 class BatchGetFrameMetricDataRequestRequestTypeDef(
     _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
     _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
 ):
     pass
 
-
 FrameMetricDatumTypeDef = TypedDict(
     "FrameMetricDatumTypeDef",
     {
         "frameMetric": FrameMetricTypeDef,
         "values": List[float],
     },
 )
 
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingsReportsResponseTypeDef = TypedDict(
     "ListFindingsReportsResponseTypeDef",
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "orderBy": OrderByType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
-    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
-):
-    pass
-
-
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "allMatchesCount": int,
@@ -769,31 +740,31 @@
     },
 )
 
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNotificationConfigurationResponseTypeDef = TypedDict(
     "GetNotificationConfigurationResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveNotificationChannelResponseTypeDef = TypedDict(
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProfilingGroupDescriptionTypeDef = TypedDict(
     "ProfilingGroupDescriptionTypeDef",
     {
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
@@ -822,56 +793,56 @@
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeProfilingGroupResponseTypeDef = TypedDict(
     "DescribeProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfilingGroupsResponseTypeDef = TypedDict(
     "ListProfilingGroupsResponseTypeDef",
     {
         "nextToken": str,
         "profilingGroupNames": List[str],
         "profilingGroups": List[ProfilingGroupDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProfilingGroupResponseTypeDef = TypedDict(
     "UpdateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "anomalies": List[AnomalyTypeDef],
         "profileEndTime": datetime,
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler/type_defs.pyi` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,65 +31,66 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ChannelTypeDef",
-    "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
     "FrameMetricTypeDef",
     "TimestampStructureTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
+    "GetPolicyResponseTypeDef",
     "GetProfileRequestRequestTypeDef",
+    "GetProfileResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "ListFindingsReportsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesRequestRequestTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MatchTypeDef",
+    "PaginatorConfigTypeDef",
     "PatternTypeDef",
     "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
+    "PutPermissionResponseTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "RemovePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddNotificationChannelsRequestRequestTypeDef",
     "NotificationConfigurationTypeDef",
-    "GetPolicyResponseTypeDef",
-    "GetProfileResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutPermissionResponseTypeDef",
-    "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
     "BatchGetFrameMetricDataRequestRequestTypeDef",
     "FrameMetricDatumTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
-    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
     "ProfilingGroupDescriptionTypeDef",
     "AnomalyTypeDef",
@@ -112,27 +113,18 @@
     "_OptionalChannelTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
+
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
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
 
 _RequiredAgentConfigurationTypeDef = TypedDict(
     "_RequiredAgentConfigurationTypeDef",
     {
         "periodInSeconds": int,
         "shouldProfile": bool,
     },
@@ -141,19 +133,21 @@
     "_OptionalAgentConfigurationTypeDef",
     {
         "agentParameters": Dict[AgentParameterFieldType, str],
     },
     total=False,
 )
 
+
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
+
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -209,19 +203,21 @@
     {
         "fleetInstanceId": str,
         "metadata": Mapping[MetadataFieldType, str],
     },
     total=False,
 )
 
+
 class ConfigureAgentRequestRequestTypeDef(
     _RequiredConfigureAgentRequestRequestTypeDef, _OptionalConfigureAgentRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProfilingGroupRequestRequestTypeDef = TypedDict(
     "DeleteProfilingGroupRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
@@ -264,14 +260,23 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetProfileRequestRequestTypeDef = TypedDict(
     "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalGetProfileRequestRequestTypeDef = TypedDict(
@@ -282,19 +287,31 @@
         "maxDepth": int,
         "period": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetProfileRequestRequestTypeDef(
     _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
+
+GetProfileResponseTypeDef = TypedDict(
+    "GetProfileResponseTypeDef",
+    {
+        "contentEncoding": str,
+        "contentType": str,
+        "profile": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
     },
@@ -303,20 +320,22 @@
     "_OptionalGetRecommendationsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
+
 class GetRecommendationsRequestRequestTypeDef(
     _RequiredGetRecommendationsRequestRequestTypeDef,
     _OptionalGetRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsReportsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
     },
@@ -327,30 +346,48 @@
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListFindingsReportsRequestRequestTypeDef(
     _RequiredListFindingsReportsRequestRequestTypeDef,
     _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "endTime": Union[datetime, str],
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "orderBy": OrderByType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
+    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
@@ -362,19 +399,21 @@
         "maxResults": int,
         "nextToken": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
+
 class ListProfileTimesRequestRequestTypeDef(
     _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
 ):
     pass
 
+
 ProfileTimeTypeDef = TypedDict(
     "ProfileTimeTypeDef",
     {
         "start": datetime,
     },
     total=False,
 )
@@ -392,24 +431,42 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MatchTypeDef = TypedDict(
     "MatchTypeDef",
     {
         "frameAddress": str,
         "targetFramesIndex": int,
         "thresholdBreachValue": float,
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
 PatternTypeDef = TypedDict(
     "PatternTypeDef",
     {
         "countersToAggregate": List[str],
         "description": str,
         "id": str,
         "name": str,
@@ -432,19 +489,21 @@
     "_OptionalPostAgentProfileRequestRequestTypeDef",
     {
         "profileToken": str,
     },
     total=False,
 )
 
+
 class PostAgentProfileRequestRequestTypeDef(
     _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredPutPermissionRequestRequestTypeDef",
     {
         "actionGroup": Literal["agentPermissions"],
         "principals": Sequence[str],
         "profilingGroupName": str,
     },
@@ -453,19 +512,30 @@
     "_OptionalPutPermissionRequestRequestTypeDef",
     {
         "revisionId": str,
     },
     total=False,
 )
 
+
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
+
+PutPermissionResponseTypeDef = TypedDict(
+    "PutPermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -475,14 +545,34 @@
     {
         "actionGroup": Literal["agentPermissions"],
         "profilingGroupName": str,
         "revisionId": str,
     },
 )
 
+RemovePermissionResponseTypeDef = TypedDict(
+    "RemovePermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
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
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "anomalyInstanceId": str,
         "profilingGroupName": str,
         "type": FeedbackTypeType,
     },
@@ -491,19 +581,21 @@
     "_OptionalSubmitFeedbackRequestRequestTypeDef",
     {
         "comment": str,
     },
     total=False,
 )
 
+
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -528,64 +620,19 @@
     "NotificationConfigurationTypeDef",
     {
         "channels": List[ChannelTypeDef],
     },
     total=False,
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProfileResponseTypeDef = TypedDict(
-    "GetProfileResponseTypeDef",
-    {
-        "contentEncoding": str,
-        "contentType": str,
-        "profile": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutPermissionResponseTypeDef = TypedDict(
-    "PutPermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemovePermissionResponseTypeDef = TypedDict(
-    "RemovePermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProfilingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfilingGroupRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -598,20 +645,22 @@
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "computePlatform": ComputePlatformType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProfilingGroupRequestRequestTypeDef(
     _RequiredCreateProfilingGroupRequestRequestTypeDef,
     _OptionalCreateProfilingGroupRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateProfilingGroupRequestRequestTypeDef = TypedDict(
     "UpdateProfilingGroupRequestRequestTypeDef",
     {
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "profilingGroupName": str,
     },
 )
@@ -638,17 +687,19 @@
     {
         "endTime": datetime,
         "userFeedback": UserFeedbackTypeDef,
     },
     total=False,
 )
 
+
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
+
 _RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
@@ -659,76 +710,54 @@
         "period": str,
         "startTime": Union[datetime, str],
         "targetResolution": AggregationPeriodType,
     },
     total=False,
 )
 
+
 class BatchGetFrameMetricDataRequestRequestTypeDef(
     _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
     _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
 ):
     pass
 
+
 FrameMetricDatumTypeDef = TypedDict(
     "FrameMetricDatumTypeDef",
     {
         "frameMetric": FrameMetricTypeDef,
         "values": List[float],
     },
 )
 
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingsReportsResponseTypeDef = TypedDict(
     "ListFindingsReportsResponseTypeDef",
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "orderBy": OrderByType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
-    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
-):
-    pass
-
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "allMatchesCount": int,
@@ -740,31 +769,31 @@
     },
 )
 
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNotificationConfigurationResponseTypeDef = TypedDict(
     "GetNotificationConfigurationResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveNotificationChannelResponseTypeDef = TypedDict(
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProfilingGroupDescriptionTypeDef = TypedDict(
     "ProfilingGroupDescriptionTypeDef",
     {
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
@@ -793,56 +822,56 @@
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeProfilingGroupResponseTypeDef = TypedDict(
     "DescribeProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfilingGroupsResponseTypeDef = TypedDict(
     "ListProfilingGroupsResponseTypeDef",
     {
         "nextToken": str,
         "profilingGroupNames": List[str],
         "profilingGroups": List[ProfilingGroupDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProfilingGroupResponseTypeDef = TypedDict(
     "UpdateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "anomalies": List[AnomalyTypeDef],
         "profileEndTime": datetime,
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeGuruProfiler 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeGuruProfiler 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
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
 
 <a id="mypy-boto3-codeguruprofiler"></a>
 
 # mypy-boto3-codeguruprofiler
 
 [![PyPI - mypy-boto3-codeguruprofiler](https://img.shields.io/pypi/v/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguruprofiler?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,63 +329,63 @@
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
-    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
+    GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     ListFindingsReportsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
+    PaginatorConfigTypeDef,
     PatternTypeDef,
     PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
+    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    RemovePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
     NotificationConfigurationTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutPermissionResponseTypeDef,
-    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
     FrameMetricDatumTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     ProfilingGroupDescriptionTypeDef,
     AnomalyTypeDef,
@@ -404,42 +405,42 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt` & `mypy-boto3-codeguruprofiler-1.27.0/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.26.0.post1/setup.py` & `mypy-boto3-codeguruprofiler-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codeguruprofiler.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguruprofiler",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruProfiler 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CodeGuruProfiler 1.27.0 service generated with"
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
     keywords="boto3 codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codeguruprofiler": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codeguruprofiler": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/",
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


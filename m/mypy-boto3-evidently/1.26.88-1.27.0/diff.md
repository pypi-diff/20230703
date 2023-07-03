# Comparing `tmp/mypy-boto3-evidently-1.26.88.tar.gz` & `tmp/mypy-boto3-evidently-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-evidently-1.26.88.tar", last modified: Thu Mar  9 20:38:41 2023, max compression
+gzip compressed data, was "mypy-boto3-evidently-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
```

## Comparing `mypy-boto3-evidently-1.26.88.tar` & `mypy-boto3-evidently-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.670347 mypy-boto3-evidently-1.26.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-03-09 20:38:41.670347 mypy-boto3-evidently-1.26.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.662347 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-03-09 20:36:10.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-03-09 20:36:10.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-03-09 20:36:10.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-03-09 20:36:10.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-03-09 20:36:10.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45453 2023-03-09 20:36:12.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45368 2023-03-09 20:36:10.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.670347 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-03-09 20:38:41.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-09 20:38:41.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-09 20:38:41.000000 mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:41.670347 mypy-boto3-evidently-1.26.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-09 20:36:09.000000 mypy-boto3-evidently-1.26.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.799239 mypy-boto3-evidently-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-03 19:50:45.799239 mypy-boto3-evidently-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.795239 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45527 2023-07-03 19:37:42.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45442 2023-07-03 19:37:42.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:41.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.799239 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-03 19:50:45.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:45.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:45.000000 mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.799239 mypy-boto3-evidently-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 19:37:39.000000 mypy-boto3-evidently-1.27.0/setup.py
```

### Comparing `mypy-boto3-evidently-1.26.88/LICENSE` & `mypy-boto3-evidently-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-evidently-1.26.88/PKG-INFO` & `mypy-boto3-evidently-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.26.88
-Summary: Type annotations for boto3.CloudWatchEvidently 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchEvidently 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-evidently"></a>
 
 # mypy-boto3-evidently
 
 [![PyPI - mypy-boto3-evidently](https://img.shields.io/pypi/v/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-evidently?color=blue)](https://pypistats.org/packages/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,15 +356,14 @@
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
-    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
@@ -388,61 +387,62 @@
     GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    PaginatorConfigTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
     ListExperimentsRequestRequestTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
+    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
     StartExperimentRequestRequestTypeDef,
+    StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
+    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
+    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartExperimentResponseTypeDef,
-    StopExperimentResponseTypeDef,
-    StopLaunchResponseTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
@@ -492,42 +492,42 @@
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

### Comparing `mypy-boto3-evidently-1.26.88/README.md` & `mypy-boto3-evidently-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-evidently"></a>
 
 # mypy-boto3-evidently
 
 [![PyPI - mypy-boto3-evidently](https://img.shields.io/pypi/v/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-evidently?color=blue)](https://pypistats.org/packages/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,15 +324,14 @@
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
-    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
@@ -356,61 +355,62 @@
     GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    PaginatorConfigTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
     ListExperimentsRequestRequestTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
+    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
     StartExperimentRequestRequestTypeDef,
+    StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
+    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
+    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartExperimentResponseTypeDef,
-    StopExperimentResponseTypeDef,
-    StopLaunchResponseTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
@@ -460,42 +460,42 @@
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

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/__init__.py` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/__init__.pyi` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/__main__.py` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchEvidently 1.26.88\nVersion:         1.26.88\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.CloudWatchEvidently 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.88")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/client.py` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/client.pyi` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/literals.py` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
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
@@ -141,14 +142,15 @@
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
@@ -246,14 +248,15 @@
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
@@ -289,14 +292,15 @@
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
@@ -315,16 +319,19 @@
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
@@ -408,15 +415,17 @@
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

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/literals.pyi` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -139,14 +140,15 @@
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
@@ -244,14 +246,15 @@
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
@@ -287,14 +290,15 @@
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
@@ -313,16 +317,19 @@
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
@@ -406,15 +413,17 @@
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

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/paginator.py` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,30 +71,30 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listexperimentspaginator)
         """
 
 
 class ListFeaturesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
     """
 
     def paginate(
-        self, *, project: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, project: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFeaturesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
         """
 
 
@@ -105,30 +105,30 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLaunchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listlaunchespaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
         """
 
 
@@ -139,28 +139,28 @@
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentreferencespaginator)
         """
 
 
 class ListSegmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSegmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
         """
```

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/paginator.pyi` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,29 +68,29 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listexperimentspaginator)
         """
 
 class ListFeaturesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
     """
 
     def paginate(
-        self, *, project: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, project: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFeaturesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
         """
 
 class ListLaunchesPaginator(Paginator):
@@ -100,29 +100,29 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLaunchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listlaunchespaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
         """
 
 class ListSegmentReferencesPaginator(Paginator):
@@ -132,27 +132,27 @@
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentreferencespaginator)
         """
 
 class ListSegmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSegmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
         """
```

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/type_defs.py` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "EvaluationRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
     "LaunchGroupConfigTypeDef",
     "ProjectAppConfigResourceConfigTypeDef",
     "CreateSegmentRequestRequestTypeDef",
@@ -71,61 +70,62 @@
     "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListExperimentsRequestListExperimentsPaginateTypeDef",
     "ListExperimentsRequestRequestTypeDef",
+    "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListFeaturesRequestRequestTypeDef",
+    "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListLaunchesRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
+    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentReferencesRequestRequestTypeDef",
     "RefResourceTypeDef",
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListSegmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
+    "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
     "StartExperimentRequestRequestTypeDef",
+    "StartExperimentResponseTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
+    "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
+    "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
+    "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartExperimentResponseTypeDef",
-    "StopExperimentResponseTypeDef",
-    "StopLaunchResponseTypeDef",
-    "TestSegmentPatternResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
     "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
     "PutProjectEventsRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
-    "ListExperimentsRequestListExperimentsPaginateTypeDef",
-    "ListFeaturesRequestListFeaturesPaginateTypeDef",
-    "ListLaunchesRequestListLaunchesPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
     "MetricMonitorConfigTypeDef",
     "MetricGoalTypeDef",
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
@@ -185,25 +185,14 @@
 
 class EvaluationRequestTypeDef(
     _RequiredEvaluationRequestTypeDef, _OptionalEvaluationRequestTypeDef
 ):
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
-
 CloudWatchLogsDestinationConfigTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
@@ -588,24 +577,37 @@
 )
 
 
 class LaunchGroupTypeDef(_RequiredLaunchGroupTypeDef, _OptionalLaunchGroupTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "project": str,
+    },
+)
+_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "status": ExperimentStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListExperimentsRequestListExperimentsPaginateTypeDef(
+    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
+    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListExperimentsRequestRequestTypeDef = TypedDict(
     "_RequiredListExperimentsRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListExperimentsRequestRequestTypeDef = TypedDict(
@@ -621,14 +623,36 @@
 
 class ListExperimentsRequestRequestTypeDef(
     _RequiredListExperimentsRequestRequestTypeDef, _OptionalListExperimentsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFeaturesRequestListFeaturesPaginateTypeDef(
+    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
+    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFeaturesRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListFeaturesRequestRequestTypeDef = TypedDict(
@@ -643,14 +667,37 @@
 
 class ListFeaturesRequestRequestTypeDef(
     _RequiredListFeaturesRequestRequestTypeDef, _OptionalListFeaturesRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "status": LaunchStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLaunchesRequestListLaunchesPaginateTypeDef(
+    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
+    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLaunchesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListLaunchesRequestRequestTypeDef = TypedDict(
@@ -666,14 +713,22 @@
 
 class ListLaunchesRequestRequestTypeDef(
     _RequiredListLaunchesRequestRequestTypeDef, _OptionalListLaunchesRequestRequestTypeDef
 ):
     pass
 
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -704,14 +759,37 @@
 )
 
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
 
+_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "segment": str,
+        "type": SegmentReferenceResourceTypeType,
+    },
+)
+_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
+    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSegmentReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListSegmentReferencesRequestRequestTypeDef",
     {
         "segment": str,
         "type": SegmentReferenceResourceTypeType,
     },
 )
@@ -752,14 +830,22 @@
 )
 
 
 class RefResourceTypeDef(_RequiredRefResourceTypeDef, _OptionalRefResourceTypeDef):
     pass
 
 
+ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSegmentsRequestRequestTypeDef = TypedDict(
     "ListSegmentsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -768,14 +854,22 @@
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
 _RequiredMetricDefinitionConfigTypeDef = TypedDict(
     "_RequiredMetricDefinitionConfigTypeDef",
     {
         "entityIdKey": str,
         "name": str,
         "valueKey": str,
     },
@@ -804,14 +898,24 @@
         "name": str,
         "unitLabel": str,
         "valueKey": str,
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
 ProjectAppConfigResourceTypeDef = TypedDict(
     "ProjectAppConfigResourceTypeDef",
     {
         "applicationId": str,
         "configurationProfileId": str,
         "environmentId": str,
     },
@@ -841,14 +945,25 @@
         "errorCode": str,
         "errorMessage": str,
         "eventId": str,
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
 SegmentOverrideTypeDef = TypedDict(
     "SegmentOverrideTypeDef",
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
@@ -859,14 +974,22 @@
     {
         "analysisCompleteTime": Union[datetime, str],
         "experiment": str,
         "project": str,
     },
 )
 
+StartExperimentResponseTypeDef = TypedDict(
+    "StartExperimentResponseTypeDef",
+    {
+        "startedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -890,14 +1013,22 @@
 
 class StopExperimentRequestRequestTypeDef(
     _RequiredStopExperimentRequestRequestTypeDef, _OptionalStopExperimentRequestRequestTypeDef
 ):
     pass
 
 
+StopExperimentResponseTypeDef = TypedDict(
+    "StopExperimentResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredStopLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -913,14 +1044,22 @@
 
 class StopLaunchRequestRequestTypeDef(
     _RequiredStopLaunchRequestRequestTypeDef, _OptionalStopLaunchRequestRequestTypeDef
 ):
     pass
 
 
+StopLaunchResponseTypeDef = TypedDict(
+    "StopLaunchResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -929,14 +1068,22 @@
     "TestSegmentPatternRequestRequestTypeDef",
     {
         "pattern": str,
         "payload": str,
     },
 )
 
+TestSegmentPatternResponseTypeDef = TypedDict(
+    "TestSegmentPatternResponseTypeDef",
+    {
+        "match": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -945,54 +1092,14 @@
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartExperimentResponseTypeDef = TypedDict(
-    "StartExperimentResponseTypeDef",
-    {
-        "startedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopExperimentResponseTypeDef = TypedDict(
-    "StopExperimentResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopLaunchResponseTypeDef = TypedDict(
-    "StopLaunchResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestSegmentPatternResponseTypeDef = TypedDict(
-    "TestSegmentPatternResponseTypeDef",
-    {
-        "match": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1011,43 +1118,43 @@
     pass
 
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSegmentsResponseTypeDef = TypedDict(
     "ListSegmentsResponseTypeDef",
     {
         "nextToken": str,
         "segments": List[SegmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
         "value": VariableValueTypeDef,
         "variation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "entityId": str,
@@ -1126,140 +1233,33 @@
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
         "details": str,
         "reports": List[ExperimentReportTypeDef],
         "resultsData": List[ExperimentResultsDataTypeDef],
         "timestamps": List[datetime],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "status": ExperimentStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-
-class ListExperimentsRequestListExperimentsPaginateTypeDef(
-    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
-    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFeaturesRequestListFeaturesPaginateTypeDef(
-    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
-    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "status": LaunchStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLaunchesRequestListLaunchesPaginateTypeDef(
-    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
-    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
-):
-    pass
-
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "segment": str,
-        "type": SegmentReferenceResourceTypeType,
-    },
-)
-_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
-    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-):
-    pass
-
-
-ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "projects": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSegmentReferencesResponseTypeDef = TypedDict(
     "ListSegmentReferencesResponseTypeDef",
     {
         "nextToken": str,
         "referencedBy": List[RefResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricGoalConfigTypeDef = TypedDict(
     "_RequiredMetricGoalConfigTypeDef",
     {
         "metricDefinition": MetricDefinitionConfigTypeDef,
@@ -1353,15 +1353,15 @@
 )
 
 PutProjectEventsResponseTypeDef = TypedDict(
     "PutProjectEventsResponseTypeDef",
     {
         "eventResults": List[PutProjectEventsResultEntryTypeDef],
         "failedEventCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
@@ -1403,15 +1403,15 @@
     pass
 
 
 BatchEvaluateFeatureResponseTypeDef = TypedDict(
     "BatchEvaluateFeatureResponseTypeDef",
     {
         "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFeatureRequestRequestTypeDef",
     {
         "name": str,
@@ -1497,15 +1497,15 @@
 
 
 ListFeaturesResponseTypeDef = TypedDict(
     "ListFeaturesResponseTypeDef",
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
@@ -1668,96 +1668,96 @@
     total=False,
 )
 
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFeatureResponseTypeDef = TypedDict(
     "GetFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFeatureResponseTypeDef = TypedDict(
     "UpdateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExperimentResponseTypeDef = TypedDict(
     "CreateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateExperimentResponseTypeDef = TypedDict(
     "UpdateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectDataDeliveryResponseTypeDef = TypedDict(
     "UpdateProjectDataDeliveryResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectResponseTypeDef = TypedDict(
     "UpdateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchRequestRequestTypeDef",
     {
         "groups": Sequence[LaunchGroupConfigTypeDef],
@@ -1842,43 +1842,43 @@
     pass
 
 
 CreateLaunchResponseTypeDef = TypedDict(
     "CreateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchResponseTypeDef = TypedDict(
     "GetLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLaunchesResponseTypeDef = TypedDict(
     "ListLaunchesResponseTypeDef",
     {
         "launches": List[LaunchTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartLaunchResponseTypeDef = TypedDict(
     "StartLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLaunchResponseTypeDef = TypedDict(
     "UpdateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently/type_defs.pyi` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "EvaluationRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
     "LaunchGroupConfigTypeDef",
     "ProjectAppConfigResourceConfigTypeDef",
     "CreateSegmentRequestRequestTypeDef",
@@ -70,61 +69,62 @@
     "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListExperimentsRequestListExperimentsPaginateTypeDef",
     "ListExperimentsRequestRequestTypeDef",
+    "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListFeaturesRequestRequestTypeDef",
+    "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListLaunchesRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
+    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentReferencesRequestRequestTypeDef",
     "RefResourceTypeDef",
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListSegmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
+    "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
     "StartExperimentRequestRequestTypeDef",
+    "StartExperimentResponseTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
+    "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
+    "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
+    "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartExperimentResponseTypeDef",
-    "StopExperimentResponseTypeDef",
-    "StopLaunchResponseTypeDef",
-    "TestSegmentPatternResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
     "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
     "PutProjectEventsRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
-    "ListExperimentsRequestListExperimentsPaginateTypeDef",
-    "ListFeaturesRequestListFeaturesPaginateTypeDef",
-    "ListLaunchesRequestListLaunchesPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
     "MetricMonitorConfigTypeDef",
     "MetricGoalTypeDef",
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
@@ -182,25 +182,14 @@
 )
 
 class EvaluationRequestTypeDef(
     _RequiredEvaluationRequestTypeDef, _OptionalEvaluationRequestTypeDef
 ):
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
-
 CloudWatchLogsDestinationConfigTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
@@ -567,24 +556,35 @@
     },
     total=False,
 )
 
 class LaunchGroupTypeDef(_RequiredLaunchGroupTypeDef, _OptionalLaunchGroupTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "project": str,
+    },
+)
+_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "status": ExperimentStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListExperimentsRequestListExperimentsPaginateTypeDef(
+    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
+    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListExperimentsRequestRequestTypeDef = TypedDict(
     "_RequiredListExperimentsRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListExperimentsRequestRequestTypeDef = TypedDict(
@@ -598,14 +598,34 @@
 )
 
 class ListExperimentsRequestRequestTypeDef(
     _RequiredListExperimentsRequestRequestTypeDef, _OptionalListExperimentsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFeaturesRequestListFeaturesPaginateTypeDef(
+    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
+    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
+):
+    pass
+
 _RequiredListFeaturesRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListFeaturesRequestRequestTypeDef = TypedDict(
@@ -618,14 +638,35 @@
 )
 
 class ListFeaturesRequestRequestTypeDef(
     _RequiredListFeaturesRequestRequestTypeDef, _OptionalListFeaturesRequestRequestTypeDef
 ):
     pass
 
+_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "status": LaunchStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLaunchesRequestListLaunchesPaginateTypeDef(
+    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
+    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
+):
+    pass
+
 _RequiredListLaunchesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListLaunchesRequestRequestTypeDef = TypedDict(
@@ -639,14 +680,22 @@
 )
 
 class ListLaunchesRequestRequestTypeDef(
     _RequiredListLaunchesRequestRequestTypeDef, _OptionalListLaunchesRequestRequestTypeDef
 ):
     pass
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -675,14 +724,35 @@
     },
     total=False,
 )
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
+_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "segment": str,
+        "type": SegmentReferenceResourceTypeType,
+    },
+)
+_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
+    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+):
+    pass
+
 _RequiredListSegmentReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListSegmentReferencesRequestRequestTypeDef",
     {
         "segment": str,
         "type": SegmentReferenceResourceTypeType,
     },
 )
@@ -719,14 +789,22 @@
     },
     total=False,
 )
 
 class RefResourceTypeDef(_RequiredRefResourceTypeDef, _OptionalRefResourceTypeDef):
     pass
 
+ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSegmentsRequestRequestTypeDef = TypedDict(
     "ListSegmentsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -735,14 +813,22 @@
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
 _RequiredMetricDefinitionConfigTypeDef = TypedDict(
     "_RequiredMetricDefinitionConfigTypeDef",
     {
         "entityIdKey": str,
         "name": str,
         "valueKey": str,
     },
@@ -769,14 +855,24 @@
         "name": str,
         "unitLabel": str,
         "valueKey": str,
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
 ProjectAppConfigResourceTypeDef = TypedDict(
     "ProjectAppConfigResourceTypeDef",
     {
         "applicationId": str,
         "configurationProfileId": str,
         "environmentId": str,
     },
@@ -806,14 +902,25 @@
         "errorCode": str,
         "errorMessage": str,
         "eventId": str,
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
 SegmentOverrideTypeDef = TypedDict(
     "SegmentOverrideTypeDef",
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
@@ -824,14 +931,22 @@
     {
         "analysisCompleteTime": Union[datetime, str],
         "experiment": str,
         "project": str,
     },
 )
 
+StartExperimentResponseTypeDef = TypedDict(
+    "StartExperimentResponseTypeDef",
+    {
+        "startedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -853,14 +968,22 @@
 )
 
 class StopExperimentRequestRequestTypeDef(
     _RequiredStopExperimentRequestRequestTypeDef, _OptionalStopExperimentRequestRequestTypeDef
 ):
     pass
 
+StopExperimentResponseTypeDef = TypedDict(
+    "StopExperimentResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredStopLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -874,14 +997,22 @@
 )
 
 class StopLaunchRequestRequestTypeDef(
     _RequiredStopLaunchRequestRequestTypeDef, _OptionalStopLaunchRequestRequestTypeDef
 ):
     pass
 
+StopLaunchResponseTypeDef = TypedDict(
+    "StopLaunchResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -890,14 +1021,22 @@
     "TestSegmentPatternRequestRequestTypeDef",
     {
         "pattern": str,
         "payload": str,
     },
 )
 
+TestSegmentPatternResponseTypeDef = TypedDict(
+    "TestSegmentPatternResponseTypeDef",
+    {
+        "match": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -906,54 +1045,14 @@
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartExperimentResponseTypeDef = TypedDict(
-    "StartExperimentResponseTypeDef",
-    {
-        "startedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopExperimentResponseTypeDef = TypedDict(
-    "StopExperimentResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopLaunchResponseTypeDef = TypedDict(
-    "StopLaunchResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestSegmentPatternResponseTypeDef = TypedDict(
-    "TestSegmentPatternResponseTypeDef",
-    {
-        "match": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -970,43 +1069,43 @@
 ):
     pass
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSegmentsResponseTypeDef = TypedDict(
     "ListSegmentsResponseTypeDef",
     {
         "nextToken": str,
         "segments": List[SegmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
         "value": VariableValueTypeDef,
         "variation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "entityId": str,
@@ -1081,132 +1180,33 @@
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
         "details": str,
         "reports": List[ExperimentReportTypeDef],
         "resultsData": List[ExperimentResultsDataTypeDef],
         "timestamps": List[datetime],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "status": ExperimentStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListExperimentsRequestListExperimentsPaginateTypeDef(
-    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
-    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFeaturesRequestListFeaturesPaginateTypeDef(
-    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
-    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
-):
-    pass
-
-_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "status": LaunchStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLaunchesRequestListLaunchesPaginateTypeDef(
-    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
-    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
-):
-    pass
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "segment": str,
-        "type": SegmentReferenceResourceTypeType,
-    },
-)
-_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
-    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-):
-    pass
-
-ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "projects": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSegmentReferencesResponseTypeDef = TypedDict(
     "ListSegmentReferencesResponseTypeDef",
     {
         "nextToken": str,
         "referencedBy": List[RefResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricGoalConfigTypeDef = TypedDict(
     "_RequiredMetricGoalConfigTypeDef",
     {
         "metricDefinition": MetricDefinitionConfigTypeDef,
@@ -1294,15 +1294,15 @@
 )
 
 PutProjectEventsResponseTypeDef = TypedDict(
     "PutProjectEventsResponseTypeDef",
     {
         "eventResults": List[PutProjectEventsResultEntryTypeDef],
         "failedEventCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
@@ -1340,15 +1340,15 @@
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
 BatchEvaluateFeatureResponseTypeDef = TypedDict(
     "BatchEvaluateFeatureResponseTypeDef",
     {
         "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFeatureRequestRequestTypeDef",
     {
         "name": str,
@@ -1428,15 +1428,15 @@
     pass
 
 ListFeaturesResponseTypeDef = TypedDict(
     "ListFeaturesResponseTypeDef",
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
@@ -1589,96 +1589,96 @@
     total=False,
 )
 
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFeatureResponseTypeDef = TypedDict(
     "GetFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFeatureResponseTypeDef = TypedDict(
     "UpdateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExperimentResponseTypeDef = TypedDict(
     "CreateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateExperimentResponseTypeDef = TypedDict(
     "UpdateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectDataDeliveryResponseTypeDef = TypedDict(
     "UpdateProjectDataDeliveryResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectResponseTypeDef = TypedDict(
     "UpdateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchRequestRequestTypeDef",
     {
         "groups": Sequence[LaunchGroupConfigTypeDef],
@@ -1757,43 +1757,43 @@
 class LaunchTypeDef(_RequiredLaunchTypeDef, _OptionalLaunchTypeDef):
     pass
 
 CreateLaunchResponseTypeDef = TypedDict(
     "CreateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchResponseTypeDef = TypedDict(
     "GetLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLaunchesResponseTypeDef = TypedDict(
     "ListLaunchesResponseTypeDef",
     {
         "launches": List[LaunchTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartLaunchResponseTypeDef = TypedDict(
     "StartLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLaunchResponseTypeDef = TypedDict(
     "UpdateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/PKG-INFO` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.26.88
-Summary: Type annotations for boto3.CloudWatchEvidently 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchEvidently 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-evidently"></a>
 
 # mypy-boto3-evidently
 
 [![PyPI - mypy-boto3-evidently](https://img.shields.io/pypi/v/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-evidently?color=blue)](https://pypistats.org/packages/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,15 +356,14 @@
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
-    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
@@ -388,61 +387,62 @@
     GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    PaginatorConfigTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
     ListExperimentsRequestRequestTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
+    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
     StartExperimentRequestRequestTypeDef,
+    StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
+    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
+    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartExperimentResponseTypeDef,
-    StopExperimentResponseTypeDef,
-    StopLaunchResponseTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
@@ -492,42 +492,42 @@
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

### Comparing `mypy-boto3-evidently-1.26.88/mypy_boto3_evidently.egg-info/SOURCES.txt` & `mypy-boto3-evidently-1.27.0/mypy_boto3_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.26.88/setup.py` & `mypy-boto3-evidently-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-evidently.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-evidently",
-    version="1.26.88",
+    version="1.27.0",
     packages=["mypy_boto3_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchEvidently 1.26.88 service generated with"
-        " mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.CloudWatchEvidently 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/",
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


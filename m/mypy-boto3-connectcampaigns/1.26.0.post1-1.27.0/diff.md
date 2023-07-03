# Comparing `tmp/mypy-boto3-connectcampaigns-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-connectcampaigns-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcampaigns-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:17 2022, max compression
+gzip compressed data, was "mypy-boto3-connectcampaigns-1.27.0.tar", last modified: Mon Jul  3 19:50:36 2023, max compression
```

## Comparing `mypy-boto3-connectcampaigns-1.26.0.post1.tar` & `mypy-boto3-connectcampaigns-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:17.740821 mypy-boto3-connectcampaigns-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15342 2022-11-01 21:43:17.740821 mypy-boto3-connectcampaigns-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13859 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:17.740821 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16759 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16729 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8004 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8002 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    15046 2022-11-01 21:32:28.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    15033 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:17.740821 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15342 2022-11-01 21:43:17.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-01 21:43:17.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:17.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:17.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:17.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-01 21:43:17.000000 mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:17.740821 mypy-boto3-connectcampaigns-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-11-01 21:32:27.000000 mypy-boto3-connectcampaigns-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.247066 mypy-boto3-connectcampaigns-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-03 19:50:36.239065 mypy-boto3-connectcampaigns-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.239065 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-03 19:35:05.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-03 19:35:05.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.239065 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-03 19:50:36.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:50:36.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:36.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:50:36.000000 mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:36.247066 mypy-boto3-connectcampaigns-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:35:04.000000 mypy-boto3-connectcampaigns-1.27.0/setup.py
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/LICENSE` & `mypy-boto3-connectcampaigns-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/PKG-INFO` & `mypy-boto3-connectcampaigns-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ConnectCampaignService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectCampaignService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
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
 
 <a id="mypy-boto3-connectcampaigns"></a>
 
 # mypy-boto3-connectcampaigns
 
 [![PyPI - mypy-boto3-connectcampaigns](https://img.shields.io/pypi/v/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcampaigns?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,49 +330,49 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCampaignResponseTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
+    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
-    CreateCampaignResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
@@ -393,42 +394,42 @@
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

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/README.md` & `mypy-boto3-connectcampaigns-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectcampaigns"></a>
 
 # mypy-boto3-connectcampaigns
 
 [![PyPI - mypy-boto3-connectcampaigns](https://img.shields.io/pypi/v/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcampaigns?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,49 +298,49 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCampaignResponseTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
+    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
-    CreateCampaignResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
@@ -362,42 +362,42 @@
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

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/__init__.py` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/__init__.pyi` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/__main__.py` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCampaignService 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ConnectCampaignService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/client.py` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/client.pyi` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/literals.py` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,23 +63,25 @@
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
@@ -89,30 +91,35 @@
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
@@ -138,14 +145,15 @@
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
@@ -190,51 +198,57 @@
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
@@ -247,14 +261,15 @@
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
@@ -266,28 +281,35 @@
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
@@ -296,14 +318,15 @@
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
@@ -314,55 +337,64 @@
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
@@ -381,8 +413,8 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_campaigns"]
-RegionName = Literal["ap-southeast-2", "eu-west-2", "us-east-1", "us-west-2"]
+RegionName = Literal["ap-southeast-2", "ca-central-1", "eu-west-2", "us-east-1", "us-west-2"]
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/literals.pyi` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -61,23 +61,25 @@
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
@@ -87,30 +89,35 @@
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
@@ -136,14 +143,15 @@
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
@@ -188,51 +196,57 @@
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
@@ -245,14 +259,15 @@
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
@@ -264,28 +279,35 @@
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
@@ -294,14 +316,15 @@
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
@@ -312,55 +335,64 @@
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
@@ -379,8 +411,8 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_campaigns"]
-RegionName = Literal["ap-southeast-2", "eu-west-2", "us-east-1", "us-west-2"]
+RegionName = Literal["ap-southeast-2", "ca-central-1", "eu-west-2", "us-east-1", "us-west-2"]
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/paginator.py` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,34 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import CampaignFiltersTypeDef, ListCampaignsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListCampaignsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: CampaignFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
         """
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/paginator.pyi` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,31 +23,34 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import CampaignFiltersTypeDef, ListCampaignsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListCampaignsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: CampaignFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
         """
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/type_defs.py` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,49 +33,49 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateCampaignResponseTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DialRequestTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
+    "GetCampaignStateResponseTypeDef",
     "GetConnectInstanceConfigRequestRequestTypeDef",
     "GetInstanceOnboardingJobStatusRequestRequestTypeDef",
     "InstanceOnboardingJobStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PauseCampaignRequestRequestTypeDef",
     "SuccessfulRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutDialRequestBatchRequestRequestTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
@@ -110,22 +110,21 @@
         "arn": str,
         "connectInstanceId": str,
         "id": str,
         "name": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
@@ -173,14 +172,21 @@
 ProgressiveDialerConfigTypeDef = TypedDict(
     "ProgressiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -235,14 +241,22 @@
 GetCampaignStateRequestRequestTypeDef = TypedDict(
     "GetCampaignStateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetCampaignStateResponseTypeDef = TypedDict(
+    "GetCampaignStateResponseTypeDef",
+    {
+        "state": CampaignStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConnectInstanceConfigRequestRequestTypeDef = TypedDict(
     "GetConnectInstanceConfigRequestRequestTypeDef",
     {
         "connectInstanceId": str,
     },
 )
 
@@ -271,31 +285,39 @@
 
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 PauseCampaignRequestRequestTypeDef = TypedDict(
     "PauseCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -304,14 +326,25 @@
     {
         "clientToken": str,
         "id": str,
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
 ResumeCampaignRequestRequestTypeDef = TypedDict(
     "ResumeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -404,53 +437,20 @@
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
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
-GetCampaignStateResponseTypeDef = TypedDict(
-    "GetCampaignStateResponseTypeDef",
-    {
-        "state": CampaignStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaryList": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDialRequestBatchRequestRequestTypeDef = TypedDict(
     "PutDialRequestBatchRequestRequestTypeDef",
     {
         "dialRequests": Sequence[DialRequestTypeDef],
@@ -485,48 +485,48 @@
 )
 
 GetCampaignStateBatchResponseTypeDef = TypedDict(
     "GetCampaignStateBatchResponseTypeDef",
     {
         "failedRequests": List[FailedCampaignStateResponseTypeDef],
         "successfulRequests": List[SuccessfulCampaignStateResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceOnboardingJobStatusResponseTypeDef = TypedDict(
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartInstanceOnboardingJobResponseTypeDef = TypedDict(
     "StartInstanceOnboardingJobResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDialRequestBatchResponseTypeDef = TypedDict(
     "PutDialRequestBatchResponseTypeDef",
     {
         "failedRequests": List[FailedRequestTypeDef],
         "successfulRequests": List[SuccessfulRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
@@ -593,18 +593,18 @@
     },
 )
 
 GetConnectInstanceConfigResponseTypeDef = TypedDict(
     "GetConnectInstanceConfigResponseTypeDef",
     {
         "connectInstanceConfig": InstanceConfigTypeDef,
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
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns/type_defs.pyi` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -32,49 +32,49 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateCampaignResponseTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DialRequestTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
+    "GetCampaignStateResponseTypeDef",
     "GetConnectInstanceConfigRequestRequestTypeDef",
     "GetInstanceOnboardingJobStatusRequestRequestTypeDef",
     "InstanceOnboardingJobStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PauseCampaignRequestRequestTypeDef",
     "SuccessfulRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutDialRequestBatchRequestRequestTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
@@ -109,22 +109,21 @@
         "arn": str,
         "connectInstanceId": str,
         "id": str,
         "name": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
@@ -172,14 +171,21 @@
 ProgressiveDialerConfigTypeDef = TypedDict(
     "ProgressiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -232,14 +238,22 @@
 GetCampaignStateRequestRequestTypeDef = TypedDict(
     "GetCampaignStateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetCampaignStateResponseTypeDef = TypedDict(
+    "GetCampaignStateResponseTypeDef",
+    {
+        "state": CampaignStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConnectInstanceConfigRequestRequestTypeDef = TypedDict(
     "GetConnectInstanceConfigRequestRequestTypeDef",
     {
         "connectInstanceId": str,
     },
 )
 
@@ -266,31 +280,39 @@
 )
 
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 PauseCampaignRequestRequestTypeDef = TypedDict(
     "PauseCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -299,14 +321,25 @@
     {
         "clientToken": str,
         "id": str,
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
 ResumeCampaignRequestRequestTypeDef = TypedDict(
     "ResumeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -395,53 +428,20 @@
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
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
-GetCampaignStateResponseTypeDef = TypedDict(
-    "GetCampaignStateResponseTypeDef",
-    {
-        "state": CampaignStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaryList": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDialRequestBatchRequestRequestTypeDef = TypedDict(
     "PutDialRequestBatchRequestRequestTypeDef",
     {
         "dialRequests": Sequence[DialRequestTypeDef],
@@ -476,48 +476,48 @@
 )
 
 GetCampaignStateBatchResponseTypeDef = TypedDict(
     "GetCampaignStateBatchResponseTypeDef",
     {
         "failedRequests": List[FailedCampaignStateResponseTypeDef],
         "successfulRequests": List[SuccessfulCampaignStateResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceOnboardingJobStatusResponseTypeDef = TypedDict(
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartInstanceOnboardingJobResponseTypeDef = TypedDict(
     "StartInstanceOnboardingJobResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDialRequestBatchResponseTypeDef = TypedDict(
     "PutDialRequestBatchResponseTypeDef",
     {
         "failedRequests": List[FailedRequestTypeDef],
         "successfulRequests": List[SuccessfulRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
@@ -580,18 +580,18 @@
     },
 )
 
 GetConnectInstanceConfigResponseTypeDef = TypedDict(
     "GetConnectInstanceConfigResponseTypeDef",
     {
         "connectInstanceConfig": InstanceConfigTypeDef,
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
```

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/PKG-INFO` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ConnectCampaignService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectCampaignService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
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
 
 <a id="mypy-boto3-connectcampaigns"></a>
 
 # mypy-boto3-connectcampaigns
 
 [![PyPI - mypy-boto3-connectcampaigns](https://img.shields.io/pypi/v/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcampaigns?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,49 +330,49 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCampaignResponseTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
+    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
-    CreateCampaignResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
@@ -393,42 +394,42 @@
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

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt` & `mypy-boto3-connectcampaigns-1.27.0/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.26.0.post1/setup.py` & `mypy-boto3-connectcampaigns-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-connectcampaigns.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcampaigns",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCampaignService 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ConnectCampaignService 1.27.0 service generated with"
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
     keywords="boto3 connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_connectcampaigns": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_connectcampaigns": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/",
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


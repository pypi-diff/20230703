# Comparing `tmp/mypy-boto3-gamesparks-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-gamesparks-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamesparks-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:28 2022, max compression
+gzip compressed data, was "mypy-boto3-gamesparks-1.27.0.tar", last modified: Mon Jul  3 19:50:48 2023, max compression
```

## Comparing `mypy-boto3-gamesparks-1.26.0.post1.tar` & `mypy-boto3-gamesparks-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:28.544830 mypy-boto3-gamesparks-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17169 2022-11-01 21:43:28.544830 mypy-boto3-gamesparks-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15716 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:28.536831 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24666 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    24619 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8403 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8401 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8278 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8269 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    29790 2022-11-01 21:35:04.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    29747 2022-11-01 21:35:04.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:28.544830 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17169 2022-11-01 21:43:28.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-01 21:43:28.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:28.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:28.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:28.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:28.000000 mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:28.544830 mypy-boto3-gamesparks-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-01 21:35:03.000000 mypy-boto3-gamesparks-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:48.083280 mypy-boto3-gamesparks-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-03 19:50:48.079280 mypy-boto3-gamesparks-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:48.075280 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29862 2023-07-03 19:38:14.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29819 2023-07-03 19:38:14.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:48.079280 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-03 19:50:47.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:47.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:47.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:47.000000 mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:48.083280 mypy-boto3-gamesparks-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:38:13.000000 mypy-boto3-gamesparks-1.27.0/setup.py
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/LICENSE` & `mypy-boto3-gamesparks-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/PKG-INFO` & `mypy-boto3-gamesparks-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamesparks
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.GameSparks 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.GameSparks 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/
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
 
 <a id="mypy-boto3-gamesparks"></a>
 
 # mypy-boto3-gamesparks
 
 [![PyPI - mypy-boto3-gamesparks](https://img.shields.io/pypi/v/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamesparks?color=blue)](https://pypistats.org/packages/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,23 +354,24 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
-    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
+    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
+    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -378,39 +380,45 @@
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     ImportGameConfigurationSourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
     CreateGameResultTypeDef,
-    DisconnectPlayerResultTypeDef,
-    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -420,21 +428,14 @@
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
     ImportGameConfigurationRequestRequestTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
@@ -453,42 +454,42 @@
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

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/README.md` & `mypy-boto3-gamesparks-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-gamesparks"></a>
 
 # mypy-boto3-gamesparks
 
 [![PyPI - mypy-boto3-gamesparks](https://img.shields.io/pypi/v/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamesparks?color=blue)](https://pypistats.org/packages/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,23 +322,24 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
-    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
+    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
+    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -347,39 +348,45 @@
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     ImportGameConfigurationSourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
     CreateGameResultTypeDef,
-    DisconnectPlayerResultTypeDef,
-    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -389,21 +396,14 @@
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
     ImportGameConfigurationRequestRequestTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
@@ -422,42 +422,42 @@
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

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/__init__.py` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/__init__.pyi` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/__main__.py` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameSparks 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.GameSparks 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks\nOther"
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

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/client.py` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/client.pyi` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/literals.py` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DeploymentActionType",
     "DeploymentStateType",
     "GameStateType",
     "GeneratedCodeJobStateType",
     "ListExtensionVersionsPaginatorName",
     "ListExtensionsPaginatorName",
@@ -37,15 +36,14 @@
     "GameSparksServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DeploymentActionType = Literal["DEPLOY", "UNDEPLOY"]
 DeploymentStateType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING"]
 GameStateType = Literal["ACTIVE", "DELETING"]
 GeneratedCodeJobStateType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING"]
 ListExtensionVersionsPaginatorName = Literal["list_extension_versions"]
 ListExtensionsPaginatorName = Literal["list_extensions"]
 ListGamesPaginatorName = Literal["list_games"]
@@ -68,23 +66,25 @@
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
@@ -94,30 +94,35 @@
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
@@ -143,14 +148,15 @@
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
@@ -195,51 +201,57 @@
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
@@ -252,14 +264,15 @@
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
@@ -271,28 +284,35 @@
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
@@ -301,14 +321,15 @@
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
@@ -319,55 +340,64 @@
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
@@ -394,8 +424,8 @@
     "list_extensions",
     "list_games",
     "list_generated_code_jobs",
     "list_snapshots",
     "list_stage_deployments",
     "list_stages",
 ]
-RegionName = Literal["us-east-1"]
+RegionName = Literal["ap-northeast-1", "us-east-1"]
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/literals.pyi` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DeploymentActionType",
     "DeploymentStateType",
     "GameStateType",
     "GeneratedCodeJobStateType",
     "ListExtensionVersionsPaginatorName",
     "ListExtensionsPaginatorName",
@@ -36,14 +37,15 @@
     "GameSparksServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DeploymentActionType = Literal["DEPLOY", "UNDEPLOY"]
 DeploymentStateType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING"]
 GameStateType = Literal["ACTIVE", "DELETING"]
 GeneratedCodeJobStateType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING"]
 ListExtensionVersionsPaginatorName = Literal["list_extension_versions"]
 ListExtensionsPaginatorName = Literal["list_extensions"]
 ListGamesPaginatorName = Literal["list_games"]
@@ -66,23 +68,25 @@
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
@@ -92,30 +96,35 @@
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
@@ -141,14 +150,15 @@
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
@@ -193,51 +203,57 @@
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
@@ -250,14 +266,15 @@
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
@@ -269,28 +286,35 @@
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
@@ -299,14 +323,15 @@
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
@@ -317,55 +342,64 @@
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
@@ -392,8 +426,8 @@
     "list_extensions",
     "list_games",
     "list_generated_code_jobs",
     "list_snapshots",
     "list_stage_deployments",
     "list_stages",
 ]
-RegionName = Literal["us-east-1"]
+RegionName = Literal["ap-northeast-1", "us-east-1"]
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/paginator.py` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,103 +70,103 @@
 class ListExtensionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, Namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, Namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExtensionVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
         """
 
 
 class ListExtensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
         """
 
 
 class ListGamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
         """
 
 
 class ListGeneratedCodeJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, SnapshotId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, SnapshotId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGeneratedCodeJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
         """
 
 
 class ListSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
         """
 
 
 class ListStageDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, StageName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, StageName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStageDeploymentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
         """
 
 
 class ListStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
         """
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/paginator.pyi` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,97 +67,97 @@
 class ListExtensionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, Namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, Namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExtensionVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
         """
 
 class ListExtensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
         """
 
 class ListGamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
         """
 
 class ListGeneratedCodeJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, SnapshotId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, SnapshotId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGeneratedCodeJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
         """
 
 class ListSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
         """
 
 class ListStageDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, StageName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, StageName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStageDeploymentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
         """
 
 class ListStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
         """
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/type_defs.py` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
     "DeleteGameRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeploymentResultTypeDef",
     "DisconnectPlayerRequestRequestTypeDef",
+    "DisconnectPlayerResultTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
+    "ExportSnapshotResultTypeDef",
     "ExtensionDetailsTypeDef",
     "ExtensionVersionDetailsTypeDef",
     "SectionTypeDef",
     "GameSummaryTypeDef",
     "GeneratedCodeJobDetailsTypeDef",
     "GeneratorTypeDef",
     "GetExtensionRequestRequestTypeDef",
@@ -58,39 +58,45 @@
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
     "ImportGameConfigurationSourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListExtensionsRequestRequestTypeDef",
+    "ListGamesRequestListGamesPaginateTypeDef",
     "ListGamesRequestRequestTypeDef",
+    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
+    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStageDeploymentsRequestRequestTypeDef",
+    "ListStagesRequestListStagesPaginateTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SectionModificationTypeDef",
+    "StartGeneratedCodeJobResultTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
+    "GetPlayerConnectionStatusResultTypeDef",
     "CreateGameResultTypeDef",
-    "DisconnectPlayerResultTypeDef",
-    "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
-    "GetPlayerConnectionStatusResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "StartGeneratedCodeJobResultTypeDef",
     "UpdateGameResultTypeDef",
     "CreateStageResultTypeDef",
     "GetStageResultTypeDef",
     "UpdateStageResultTypeDef",
     "StageDeploymentDetailsTypeDef",
     "StageDeploymentSummaryTypeDef",
     "GetExtensionResultTypeDef",
@@ -100,21 +106,14 @@
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
     "ImportGameConfigurationRequestRequestTypeDef",
-    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    "ListGamesRequestListGamesPaginateTypeDef",
-    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
@@ -146,21 +145,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateGameRequestRequestTypeDef(
     _RequiredCreateGameRequestRequestTypeDef, _OptionalCreateGameRequestRequestTypeDef
 ):
     pass
 
-
 GameDetailsTypeDef = TypedDict(
     "GameDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "EnableTerminationProtection": bool,
@@ -168,46 +165,33 @@
         "Name": str,
         "State": GameStateType,
         "Tags": Dict[str, str],
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
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "Role": str,
         "StageName": str,
     },
@@ -218,21 +202,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
-
 StageDetailsTypeDef = TypedDict(
     "StageDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "GameKey": str,
@@ -275,22 +257,39 @@
     {
         "GameName": str,
         "PlayerId": str,
         "StageName": str,
     },
 )
 
+DisconnectPlayerResultTypeDef = TypedDict(
+    "DisconnectPlayerResultTypeDef",
+    {
+        "DisconnectFailures": List[str],
+        "DisconnectSuccesses": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
 
+ExportSnapshotResultTypeDef = TypedDict(
+    "ExportSnapshotResultTypeDef",
+    {
+        "S3Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExtensionDetailsTypeDef = TypedDict(
     "ExtensionDetailsTypeDef",
     {
         "Description": str,
         "Name": str,
         "Namespace": str,
     },
@@ -378,22 +377,20 @@
     "_OptionalGetGameConfigurationRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
-
 class GetGameConfigurationRequestRequestTypeDef(
     _RequiredGetGameConfigurationRequestRequestTypeDef,
     _OptionalGetGameConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetGameRequestRequestTypeDef = TypedDict(
     "GetGameRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 
@@ -426,21 +423,19 @@
     "_OptionalGetSnapshotRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
-
 class GetSnapshotRequestRequestTypeDef(
     _RequiredGetSnapshotRequestRequestTypeDef, _OptionalGetSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -448,22 +443,20 @@
     "_OptionalGetStageDeploymentRequestRequestTypeDef",
     {
         "DeploymentId": str,
     },
     total=False,
 )
 
-
 class GetStageDeploymentRequestRequestTypeDef(
     _RequiredGetStageDeploymentRequestRequestTypeDef,
     _OptionalGetStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -471,24 +464,35 @@
 ImportGameConfigurationSourceTypeDef = TypedDict(
     "ImportGameConfigurationSourceTypeDef",
     {
         "File": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Namespace": str,
+    },
+)
+_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
+    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListExtensionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -497,40 +501,75 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListExtensionVersionsRequestRequestTypeDef(
     _RequiredListExtensionVersionsRequestRequestTypeDef,
     _OptionalListExtensionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListExtensionsRequestRequestTypeDef = TypedDict(
     "ListExtensionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListGamesRequestListGamesPaginateTypeDef = TypedDict(
+    "ListGamesRequestListGamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGamesRequestRequestTypeDef = TypedDict(
     "ListGamesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "GameName": str,
+        "SnapshotId": str,
+    },
+)
+_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
+    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListGeneratedCodeJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListGeneratedCodeJobsRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -539,21 +578,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGeneratedCodeJobsRequestRequestTypeDef(
     _RequiredListGeneratedCodeJobsRequestRequestTypeDef,
     _OptionalListGeneratedCodeJobsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
+    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
+):
+    pass
 
 _RequiredListSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSnapshotsRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
@@ -562,32 +619,51 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSnapshotsRequestRequestTypeDef(
     _RequiredListSnapshotsRequestRequestTypeDef, _OptionalListSnapshotsRequestRequestTypeDef
 ):
     pass
 
-
 SnapshotSummaryTypeDef = TypedDict(
     "SnapshotSummaryTypeDef",
     {
         "Created": datetime,
         "Description": str,
         "Id": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
+_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "GameName": str,
+        "StageName": str,
+    },
+)
+_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
+    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListStageDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStageDeploymentsRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -596,21 +672,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStageDeploymentsRequestRequestTypeDef(
     _RequiredListStageDeploymentsRequestRequestTypeDef,
     _OptionalListStageDeploymentsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_RequiredListStagesRequestListStagesPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_OptionalListStagesRequestListStagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStagesRequestListStagesPaginateTypeDef(
+    _RequiredListStagesRequestListStagesPaginateTypeDef,
+    _OptionalListStagesRequestListStagesPaginateTypeDef,
+):
+    pass
 
 _RequiredListStagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStagesRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
@@ -619,21 +713,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStagesRequestRequestTypeDef(
     _RequiredListStagesRequestRequestTypeDef, _OptionalListStagesRequestRequestTypeDef
 ):
     pass
 
-
 StageSummaryTypeDef = TypedDict(
     "StageSummaryTypeDef",
     {
         "Description": str,
         "GameKey": str,
         "Name": str,
         "State": StageStateType,
@@ -645,14 +737,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredSectionModificationTypeDef = TypedDict(
     "_RequiredSectionModificationTypeDef",
     {
         "Operation": OperationType,
         "Path": str,
         "Section": str,
     },
@@ -661,20 +782,26 @@
     "_OptionalSectionModificationTypeDef",
     {
         "Value": Mapping[str, Any],
     },
     total=False,
 )
 
-
 class SectionModificationTypeDef(
     _RequiredSectionModificationTypeDef, _OptionalSectionModificationTypeDef
 ):
     pass
 
+StartGeneratedCodeJobResultTypeDef = TypedDict(
+    "StartGeneratedCodeJobResultTypeDef",
+    {
+        "GeneratedCodeJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredStartStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
         "StageName": str,
@@ -684,22 +811,20 @@
     "_OptionalStartStageDeploymentRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartStageDeploymentRequestRequestTypeDef(
     _RequiredStartStageDeploymentRequestRequestTypeDef,
     _OptionalStartStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -722,21 +847,19 @@
     "_OptionalUpdateGameRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateGameRequestRequestTypeDef(
     _RequiredUpdateGameRequestRequestTypeDef, _OptionalUpdateGameRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -744,21 +867,19 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -767,107 +888,72 @@
     {
         "Description": str,
         "Role": str,
     },
     total=False,
 )
 
-
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
-
-CreateGameResultTypeDef = TypedDict(
-    "CreateGameResultTypeDef",
-    {
-        "Game": GameDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisconnectPlayerResultTypeDef = TypedDict(
-    "DisconnectPlayerResultTypeDef",
-    {
-        "DisconnectFailures": List[str],
-        "DisconnectSuccesses": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportSnapshotResultTypeDef = TypedDict(
-    "ExportSnapshotResultTypeDef",
-    {
-        "S3Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGameResultTypeDef = TypedDict(
-    "GetGameResultTypeDef",
-    {
-        "Game": GameDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetPlayerConnectionStatusResultTypeDef = TypedDict(
     "GetPlayerConnectionStatusResultTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
+CreateGameResultTypeDef = TypedDict(
+    "CreateGameResultTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Game": GameDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartGeneratedCodeJobResultTypeDef = TypedDict(
-    "StartGeneratedCodeJobResultTypeDef",
+GetGameResultTypeDef = TypedDict(
+    "GetGameResultTypeDef",
     {
-        "GeneratedCodeJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Game": GameDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGameResultTypeDef = TypedDict(
     "UpdateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStageResultTypeDef = TypedDict(
     "CreateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStageResultTypeDef = TypedDict(
     "GetStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStageResultTypeDef = TypedDict(
     "UpdateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StageDeploymentDetailsTypeDef = TypedDict(
     "StageDeploymentDetailsTypeDef",
     {
         "Created": datetime,
@@ -894,41 +980,41 @@
     total=False,
 )
 
 GetExtensionResultTypeDef = TypedDict(
     "GetExtensionResultTypeDef",
     {
         "Extension": ExtensionDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExtensionsResultTypeDef = TypedDict(
     "ListExtensionsResultTypeDef",
     {
         "Extensions": List[ExtensionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExtensionVersionResultTypeDef = TypedDict(
     "GetExtensionVersionResultTypeDef",
     {
         "ExtensionVersion": ExtensionVersionDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExtensionVersionsResultTypeDef = TypedDict(
     "ListExtensionVersionsResultTypeDef",
     {
         "ExtensionVersions": List[ExtensionVersionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GameConfigurationDetailsTypeDef = TypedDict(
     "GameConfigurationDetailsTypeDef",
     {
         "Created": datetime,
@@ -951,32 +1037,32 @@
 )
 
 ListGamesResultTypeDef = TypedDict(
     "ListGamesResultTypeDef",
     {
         "Games": List[GameSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGeneratedCodeJobResultTypeDef = TypedDict(
     "GetGeneratedCodeJobResultTypeDef",
     {
         "GeneratedCodeJob": GeneratedCodeJobDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGeneratedCodeJobsResultTypeDef = TypedDict(
     "ListGeneratedCodeJobsResultTypeDef",
     {
         "GeneratedCodeJobs": List[GeneratedCodeJobDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartGeneratedCodeJobRequestRequestTypeDef = TypedDict(
     "StartGeneratedCodeJobRequestRequestTypeDef",
     {
         "GameName": str,
@@ -989,158 +1075,29 @@
     "ImportGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "ImportSource": ImportGameConfigurationSourceTypeDef,
     },
 )
 
-_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "Name": str,
-        "Namespace": str,
-    },
-)
-_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
-    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGamesRequestListGamesPaginateTypeDef = TypedDict(
-    "ListGamesRequestListGamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "GameName": str,
-        "SnapshotId": str,
-    },
-)
-_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
-    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
-    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "GameName": str,
-        "StageName": str,
-    },
-)
-_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
-    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_RequiredListStagesRequestListStagesPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_OptionalListStagesRequestListStagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStagesRequestListStagesPaginateTypeDef(
-    _RequiredListStagesRequestListStagesPaginateTypeDef,
-    _OptionalListStagesRequestListStagesPaginateTypeDef,
-):
-    pass
-
-
 ListSnapshotsResultTypeDef = TypedDict(
     "ListSnapshotsResultTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStagesResultTypeDef = TypedDict(
     "ListStagesResultTypeDef",
     {
         "NextToken": str,
         "Stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGameConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
@@ -1148,75 +1105,75 @@
     },
 )
 
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartStageDeploymentResultTypeDef = TypedDict(
     "StartStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStageDeploymentsResultTypeDef = TypedDict(
     "ListStageDeploymentsResultTypeDef",
     {
         "NextToken": str,
         "StageDeployments": List[StageDeploymentSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGameConfigurationResultTypeDef = TypedDict(
     "GetGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportGameConfigurationResultTypeDef = TypedDict(
     "ImportGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGameConfigurationResultTypeDef = TypedDict(
     "UpdateGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotResultTypeDef = TypedDict(
     "GetSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSnapshotResultTypeDef = TypedDict(
     "UpdateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks/type_defs.pyi` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,27 +28,29 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
     "DeleteGameRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeploymentResultTypeDef",
     "DisconnectPlayerRequestRequestTypeDef",
+    "DisconnectPlayerResultTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
+    "ExportSnapshotResultTypeDef",
     "ExtensionDetailsTypeDef",
     "ExtensionVersionDetailsTypeDef",
     "SectionTypeDef",
     "GameSummaryTypeDef",
     "GeneratedCodeJobDetailsTypeDef",
     "GeneratorTypeDef",
     "GetExtensionRequestRequestTypeDef",
@@ -57,39 +59,45 @@
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
     "ImportGameConfigurationSourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListExtensionsRequestRequestTypeDef",
+    "ListGamesRequestListGamesPaginateTypeDef",
     "ListGamesRequestRequestTypeDef",
+    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
+    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStageDeploymentsRequestRequestTypeDef",
+    "ListStagesRequestListStagesPaginateTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SectionModificationTypeDef",
+    "StartGeneratedCodeJobResultTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
+    "GetPlayerConnectionStatusResultTypeDef",
     "CreateGameResultTypeDef",
-    "DisconnectPlayerResultTypeDef",
-    "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
-    "GetPlayerConnectionStatusResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "StartGeneratedCodeJobResultTypeDef",
     "UpdateGameResultTypeDef",
     "CreateStageResultTypeDef",
     "GetStageResultTypeDef",
     "UpdateStageResultTypeDef",
     "StageDeploymentDetailsTypeDef",
     "StageDeploymentSummaryTypeDef",
     "GetExtensionResultTypeDef",
@@ -99,21 +107,14 @@
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
     "ImportGameConfigurationRequestRequestTypeDef",
-    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    "ListGamesRequestListGamesPaginateTypeDef",
-    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
@@ -145,19 +146,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateGameRequestRequestTypeDef(
     _RequiredCreateGameRequestRequestTypeDef, _OptionalCreateGameRequestRequestTypeDef
 ):
     pass
 
+
 GameDetailsTypeDef = TypedDict(
     "GameDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "EnableTerminationProtection": bool,
@@ -165,44 +168,35 @@
         "Name": str,
         "State": GameStateType,
         "Tags": Dict[str, str],
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
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "Role": str,
         "StageName": str,
     },
@@ -213,19 +207,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
+
 StageDetailsTypeDef = TypedDict(
     "StageDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "GameKey": str,
@@ -268,22 +264,39 @@
     {
         "GameName": str,
         "PlayerId": str,
         "StageName": str,
     },
 )
 
+DisconnectPlayerResultTypeDef = TypedDict(
+    "DisconnectPlayerResultTypeDef",
+    {
+        "DisconnectFailures": List[str],
+        "DisconnectSuccesses": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
 
+ExportSnapshotResultTypeDef = TypedDict(
+    "ExportSnapshotResultTypeDef",
+    {
+        "S3Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExtensionDetailsTypeDef = TypedDict(
     "ExtensionDetailsTypeDef",
     {
         "Description": str,
         "Name": str,
         "Namespace": str,
     },
@@ -371,20 +384,22 @@
     "_OptionalGetGameConfigurationRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
+
 class GetGameConfigurationRequestRequestTypeDef(
     _RequiredGetGameConfigurationRequestRequestTypeDef,
     _OptionalGetGameConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetGameRequestRequestTypeDef = TypedDict(
     "GetGameRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 
@@ -417,19 +432,21 @@
     "_OptionalGetSnapshotRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
+
 class GetSnapshotRequestRequestTypeDef(
     _RequiredGetSnapshotRequestRequestTypeDef, _OptionalGetSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -437,20 +454,22 @@
     "_OptionalGetStageDeploymentRequestRequestTypeDef",
     {
         "DeploymentId": str,
     },
     total=False,
 )
 
+
 class GetStageDeploymentRequestRequestTypeDef(
     _RequiredGetStageDeploymentRequestRequestTypeDef,
     _OptionalGetStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -458,24 +477,37 @@
 ImportGameConfigurationSourceTypeDef = TypedDict(
     "ImportGameConfigurationSourceTypeDef",
     {
         "File": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Namespace": str,
+    },
+)
+_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
+    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListExtensionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -484,38 +516,79 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListExtensionVersionsRequestRequestTypeDef(
     _RequiredListExtensionVersionsRequestRequestTypeDef,
     _OptionalListExtensionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
+ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListExtensionsRequestRequestTypeDef = TypedDict(
     "ListExtensionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListGamesRequestListGamesPaginateTypeDef = TypedDict(
+    "ListGamesRequestListGamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGamesRequestRequestTypeDef = TypedDict(
     "ListGamesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "GameName": str,
+        "SnapshotId": str,
+    },
+)
+_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
+    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGeneratedCodeJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListGeneratedCodeJobsRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -524,20 +597,44 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGeneratedCodeJobsRequestRequestTypeDef(
     _RequiredListGeneratedCodeJobsRequestRequestTypeDef,
     _OptionalListGeneratedCodeJobsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
+    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSnapshotsRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalListSnapshotsRequestRequestTypeDef = TypedDict(
@@ -545,30 +642,55 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSnapshotsRequestRequestTypeDef(
     _RequiredListSnapshotsRequestRequestTypeDef, _OptionalListSnapshotsRequestRequestTypeDef
 ):
     pass
 
+
 SnapshotSummaryTypeDef = TypedDict(
     "SnapshotSummaryTypeDef",
     {
         "Created": datetime,
         "Description": str,
         "Id": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
+_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "GameName": str,
+        "StageName": str,
+    },
+)
+_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
+    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStageDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStageDeploymentsRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -577,20 +699,44 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStageDeploymentsRequestRequestTypeDef(
     _RequiredListStageDeploymentsRequestRequestTypeDef,
     _OptionalListStageDeploymentsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_RequiredListStagesRequestListStagesPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_OptionalListStagesRequestListStagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStagesRequestListStagesPaginateTypeDef(
+    _RequiredListStagesRequestListStagesPaginateTypeDef,
+    _OptionalListStagesRequestListStagesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStagesRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalListStagesRequestRequestTypeDef = TypedDict(
@@ -598,19 +744,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStagesRequestRequestTypeDef(
     _RequiredListStagesRequestRequestTypeDef, _OptionalListStagesRequestRequestTypeDef
 ):
     pass
 
+
 StageSummaryTypeDef = TypedDict(
     "StageSummaryTypeDef",
     {
         "Description": str,
         "GameKey": str,
         "Name": str,
         "State": StageStateType,
@@ -622,14 +770,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredSectionModificationTypeDef = TypedDict(
     "_RequiredSectionModificationTypeDef",
     {
         "Operation": OperationType,
         "Path": str,
         "Section": str,
     },
@@ -638,19 +815,29 @@
     "_OptionalSectionModificationTypeDef",
     {
         "Value": Mapping[str, Any],
     },
     total=False,
 )
 
+
 class SectionModificationTypeDef(
     _RequiredSectionModificationTypeDef, _OptionalSectionModificationTypeDef
 ):
     pass
 
+
+StartGeneratedCodeJobResultTypeDef = TypedDict(
+    "StartGeneratedCodeJobResultTypeDef",
+    {
+        "GeneratedCodeJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
         "StageName": str,
     },
@@ -659,20 +846,22 @@
     "_OptionalStartStageDeploymentRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartStageDeploymentRequestRequestTypeDef(
     _RequiredStartStageDeploymentRequestRequestTypeDef,
     _OptionalStartStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -695,19 +884,21 @@
     "_OptionalUpdateGameRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateGameRequestRequestTypeDef(
     _RequiredUpdateGameRequestRequestTypeDef, _OptionalUpdateGameRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -715,19 +906,21 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -736,105 +929,74 @@
     {
         "Description": str,
         "Role": str,
     },
     total=False,
 )
 
+
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
-CreateGameResultTypeDef = TypedDict(
-    "CreateGameResultTypeDef",
-    {
-        "Game": GameDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisconnectPlayerResultTypeDef = TypedDict(
-    "DisconnectPlayerResultTypeDef",
-    {
-        "DisconnectFailures": List[str],
-        "DisconnectSuccesses": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportSnapshotResultTypeDef = TypedDict(
-    "ExportSnapshotResultTypeDef",
-    {
-        "S3Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGameResultTypeDef = TypedDict(
-    "GetGameResultTypeDef",
-    {
-        "Game": GameDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 GetPlayerConnectionStatusResultTypeDef = TypedDict(
     "GetPlayerConnectionStatusResultTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
+CreateGameResultTypeDef = TypedDict(
+    "CreateGameResultTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Game": GameDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartGeneratedCodeJobResultTypeDef = TypedDict(
-    "StartGeneratedCodeJobResultTypeDef",
+GetGameResultTypeDef = TypedDict(
+    "GetGameResultTypeDef",
     {
-        "GeneratedCodeJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Game": GameDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGameResultTypeDef = TypedDict(
     "UpdateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStageResultTypeDef = TypedDict(
     "CreateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStageResultTypeDef = TypedDict(
     "GetStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStageResultTypeDef = TypedDict(
     "UpdateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StageDeploymentDetailsTypeDef = TypedDict(
     "StageDeploymentDetailsTypeDef",
     {
         "Created": datetime,
@@ -861,41 +1023,41 @@
     total=False,
 )
 
 GetExtensionResultTypeDef = TypedDict(
     "GetExtensionResultTypeDef",
     {
         "Extension": ExtensionDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExtensionsResultTypeDef = TypedDict(
     "ListExtensionsResultTypeDef",
     {
         "Extensions": List[ExtensionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExtensionVersionResultTypeDef = TypedDict(
     "GetExtensionVersionResultTypeDef",
     {
         "ExtensionVersion": ExtensionVersionDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExtensionVersionsResultTypeDef = TypedDict(
     "ListExtensionVersionsResultTypeDef",
     {
         "ExtensionVersions": List[ExtensionVersionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GameConfigurationDetailsTypeDef = TypedDict(
     "GameConfigurationDetailsTypeDef",
     {
         "Created": datetime,
@@ -918,32 +1080,32 @@
 )
 
 ListGamesResultTypeDef = TypedDict(
     "ListGamesResultTypeDef",
     {
         "Games": List[GameSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGeneratedCodeJobResultTypeDef = TypedDict(
     "GetGeneratedCodeJobResultTypeDef",
     {
         "GeneratedCodeJob": GeneratedCodeJobDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGeneratedCodeJobsResultTypeDef = TypedDict(
     "ListGeneratedCodeJobsResultTypeDef",
     {
         "GeneratedCodeJobs": List[GeneratedCodeJobDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartGeneratedCodeJobRequestRequestTypeDef = TypedDict(
     "StartGeneratedCodeJobRequestRequestTypeDef",
     {
         "GameName": str,
@@ -956,148 +1118,29 @@
     "ImportGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "ImportSource": ImportGameConfigurationSourceTypeDef,
     },
 )
 
-_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "Name": str,
-        "Namespace": str,
-    },
-)
-_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
-    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-):
-    pass
-
-ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGamesRequestListGamesPaginateTypeDef = TypedDict(
-    "ListGamesRequestListGamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "GameName": str,
-        "SnapshotId": str,
-    },
-)
-_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
-    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
-    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
-):
-    pass
-
-_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "GameName": str,
-        "StageName": str,
-    },
-)
-_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
-    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_RequiredListStagesRequestListStagesPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_OptionalListStagesRequestListStagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStagesRequestListStagesPaginateTypeDef(
-    _RequiredListStagesRequestListStagesPaginateTypeDef,
-    _OptionalListStagesRequestListStagesPaginateTypeDef,
-):
-    pass
-
 ListSnapshotsResultTypeDef = TypedDict(
     "ListSnapshotsResultTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStagesResultTypeDef = TypedDict(
     "ListStagesResultTypeDef",
     {
         "NextToken": str,
         "Stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGameConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
@@ -1105,75 +1148,75 @@
     },
 )
 
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartStageDeploymentResultTypeDef = TypedDict(
     "StartStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStageDeploymentsResultTypeDef = TypedDict(
     "ListStageDeploymentsResultTypeDef",
     {
         "NextToken": str,
         "StageDeployments": List[StageDeploymentSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGameConfigurationResultTypeDef = TypedDict(
     "GetGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportGameConfigurationResultTypeDef = TypedDict(
     "ImportGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGameConfigurationResultTypeDef = TypedDict(
     "UpdateGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotResultTypeDef = TypedDict(
     "GetSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSnapshotResultTypeDef = TypedDict(
     "UpdateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/PKG-INFO` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamesparks
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.GameSparks 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.GameSparks 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/
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
 
 <a id="mypy-boto3-gamesparks"></a>
 
 # mypy-boto3-gamesparks
 
 [![PyPI - mypy-boto3-gamesparks](https://img.shields.io/pypi/v/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamesparks?color=blue)](https://pypistats.org/packages/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,23 +354,24 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
-    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
+    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
+    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -378,39 +380,45 @@
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     ImportGameConfigurationSourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
     CreateGameResultTypeDef,
-    DisconnectPlayerResultTypeDef,
-    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -420,21 +428,14 @@
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
     ImportGameConfigurationRequestRequestTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
@@ -453,42 +454,42 @@
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

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/mypy_boto3_gamesparks.egg-info/SOURCES.txt` & `mypy-boto3-gamesparks-1.27.0/mypy_boto3_gamesparks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.26.0.post1/setup.py` & `mypy-boto3-gamesparks-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-gamesparks.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamesparks",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_gamesparks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GameSparks 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.GameSparks 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 gamesparks type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_gamesparks": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_gamesparks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/",
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


# Comparing `tmp/mypy-boto3-iottwinmaker-1.26.97.tar.gz` & `tmp/mypy-boto3-iottwinmaker-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iottwinmaker-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
+gzip compressed data, was "mypy-boto3-iottwinmaker-1.27.0.tar", last modified: Mon Jul  3 19:50:56 2023, max compression
```

## Comparing `mypy-boto3-iottwinmaker-1.26.97.tar` & `mypy-boto3-iottwinmaker-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43258 2023-03-22 19:32:05.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43185 2023-03-22 19:32:04.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.683470 mypy-boto3-iottwinmaker-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-03 19:50:56.683470 mypy-boto3-iottwinmaker-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.675470 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-03 19:39:55.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-03 19:39:55.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43539 2023-07-03 19:39:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43466 2023-07-03 19:39:55.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.683470 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-03 19:50:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:50:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:56.000000 mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:56.683470 mypy-boto3-iottwinmaker-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:39:54.000000 mypy-boto3-iottwinmaker-1.27.0/setup.py
```

### Comparing `mypy-boto3-iottwinmaker-1.26.97/LICENSE` & `mypy-boto3-iottwinmaker-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iottwinmaker-1.26.97/PKG-INFO` & `mypy-boto3-iottwinmaker-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.26.97
-Summary: Type annotations for boto3.IoTTwinMaker 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTTwinMaker 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-iottwinmaker"></a>
 
 # mypy-boto3-iottwinmaker
 
 [![PyPI - mypy-boto3-iottwinmaker](https://img.shields.io/pypi/v/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,14 +288,15 @@
     OrderByTimeType,
     OrderType,
     ParentEntityUpdateTypeType,
     PricingModeType,
     PricingTierType,
     PropertyGroupUpdateTypeType,
     PropertyUpdateTypeType,
+    SceneErrorCodeType,
     ScopeType,
     StateType,
     SyncJobStateType,
     SyncResourceStateType,
     SyncResourceTypeType,
     TypeType,
     UpdateReasonType,
@@ -315,89 +316,90 @@
 ### Typed dictionaries
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
-    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
+    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
+    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
+    CreateWorkspaceResponseTypeDef,
     LambdaFunctionTypeDef,
     RelationshipTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
+    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
+    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
+    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
     GetSceneRequestRequestTypeDef,
+    SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
+    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePricingPlanRequestRequestTypeDef,
-    UpdateSceneRequestRequestTypeDef,
-    UpdateWorkspaceRequestRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
-    CreateSceneResponseTypeDef,
-    CreateSyncJobResponseTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    DeleteComponentTypeResponseTypeDef,
-    DeleteEntityResponseTypeDef,
-    DeleteSyncJobResponseTypeDef,
-    GetSceneResponseTypeDef,
-    GetWorkspaceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
+    UpdatePricingPlanRequestRequestTypeDef,
+    UpdateSceneRequestRequestTypeDef,
     UpdateSceneResponseTypeDef,
+    UpdateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
     DataConnectorTypeDef,
     DataTypeTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
     PropertyValueEntryTypeDef,
@@ -430,53 +432,53 @@
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> BundleInformationTypeDef:
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

### Comparing `mypy-boto3-iottwinmaker-1.26.97/README.md` & `mypy-boto3-iottwinmaker-1.27.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iottwinmaker"></a>
 
 # mypy-boto3-iottwinmaker
 
 [![PyPI - mypy-boto3-iottwinmaker](https://img.shields.io/pypi/v/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -256,14 +256,15 @@
     OrderByTimeType,
     OrderType,
     ParentEntityUpdateTypeType,
     PricingModeType,
     PricingTierType,
     PropertyGroupUpdateTypeType,
     PropertyUpdateTypeType,
+    SceneErrorCodeType,
     ScopeType,
     StateType,
     SyncJobStateType,
     SyncResourceStateType,
     SyncResourceTypeType,
     TypeType,
     UpdateReasonType,
@@ -283,89 +284,90 @@
 ### Typed dictionaries
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
-    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
+    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
+    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
+    CreateWorkspaceResponseTypeDef,
     LambdaFunctionTypeDef,
     RelationshipTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
+    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
+    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
+    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
     GetSceneRequestRequestTypeDef,
+    SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
+    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePricingPlanRequestRequestTypeDef,
-    UpdateSceneRequestRequestTypeDef,
-    UpdateWorkspaceRequestRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
-    CreateSceneResponseTypeDef,
-    CreateSyncJobResponseTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    DeleteComponentTypeResponseTypeDef,
-    DeleteEntityResponseTypeDef,
-    DeleteSyncJobResponseTypeDef,
-    GetSceneResponseTypeDef,
-    GetWorkspaceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
+    UpdatePricingPlanRequestRequestTypeDef,
+    UpdateSceneRequestRequestTypeDef,
     UpdateSceneResponseTypeDef,
+    UpdateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
     DataConnectorTypeDef,
     DataTypeTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
     PropertyValueEntryTypeDef,
@@ -398,53 +400,53 @@
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> BundleInformationTypeDef:
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

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.py` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.pyi` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.py` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "OrderByTimeType",
     "OrderType",
     "ParentEntityUpdateTypeType",
     "PricingModeType",
     "PricingTierType",
     "PropertyGroupUpdateTypeType",
     "PropertyUpdateTypeType",
+    "SceneErrorCodeType",
     "ScopeType",
     "StateType",
     "SyncJobStateType",
     "SyncResourceStateType",
     "SyncResourceTypeType",
     "TypeType",
     "UpdateReasonType",
@@ -60,14 +61,15 @@
 OrderByTimeType = Literal["ASCENDING", "DESCENDING"]
 OrderType = Literal["ASCENDING", "DESCENDING"]
 ParentEntityUpdateTypeType = Literal["DELETE", "UPDATE"]
 PricingModeType = Literal["BASIC", "STANDARD", "TIERED_BUNDLE"]
 PricingTierType = Literal["TIER_1", "TIER_2", "TIER_3", "TIER_4"]
 PropertyGroupUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
 PropertyUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
+SceneErrorCodeType = Literal["MATTERPORT_ERROR"]
 ScopeType = Literal["ENTITY", "WORKSPACE"]
 StateType = Literal["ACTIVE", "CREATING", "DELETING", "ERROR", "UPDATING"]
 SyncJobStateType = Literal["ACTIVE", "CREATING", "DELETING", "ERROR", "INITIALIZING"]
 SyncResourceStateType = Literal["DELETED", "ERROR", "INITIALIZING", "IN_SYNC", "PROCESSING"]
 SyncResourceTypeType = Literal["COMPONENT_TYPE", "ENTITY"]
 TypeType = Literal["BOOLEAN", "DOUBLE", "INTEGER", "LIST", "LONG", "MAP", "RELATIONSHIP", "STRING"]
 UpdateReasonType = Literal[
@@ -85,14 +87,15 @@
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
@@ -132,14 +135,15 @@
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
@@ -237,14 +241,15 @@
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
@@ -280,14 +285,15 @@
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
@@ -306,16 +312,19 @@
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
@@ -399,15 +408,17 @@
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

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.pyi` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "OrderByTimeType",
     "OrderType",
     "ParentEntityUpdateTypeType",
     "PricingModeType",
     "PricingTierType",
     "PropertyGroupUpdateTypeType",
     "PropertyUpdateTypeType",
+    "SceneErrorCodeType",
     "ScopeType",
     "StateType",
     "SyncJobStateType",
     "SyncResourceStateType",
     "SyncResourceTypeType",
     "TypeType",
     "UpdateReasonType",
@@ -58,14 +59,15 @@
 OrderByTimeType = Literal["ASCENDING", "DESCENDING"]
 OrderType = Literal["ASCENDING", "DESCENDING"]
 ParentEntityUpdateTypeType = Literal["DELETE", "UPDATE"]
 PricingModeType = Literal["BASIC", "STANDARD", "TIERED_BUNDLE"]
 PricingTierType = Literal["TIER_1", "TIER_2", "TIER_3", "TIER_4"]
 PropertyGroupUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
 PropertyUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
+SceneErrorCodeType = Literal["MATTERPORT_ERROR"]
 ScopeType = Literal["ENTITY", "WORKSPACE"]
 StateType = Literal["ACTIVE", "CREATING", "DELETING", "ERROR", "UPDATING"]
 SyncJobStateType = Literal["ACTIVE", "CREATING", "DELETING", "ERROR", "INITIALIZING"]
 SyncResourceStateType = Literal["DELETED", "ERROR", "INITIALIZING", "IN_SYNC", "PROCESSING"]
 SyncResourceTypeType = Literal["COMPONENT_TYPE", "ENTITY"]
 TypeType = Literal["BOOLEAN", "DOUBLE", "INTEGER", "LIST", "LONG", "MAP", "RELATIONSHIP", "STRING"]
 UpdateReasonType = Literal[
@@ -83,14 +85,15 @@
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
@@ -130,14 +133,15 @@
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
@@ -235,14 +239,15 @@
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
@@ -278,14 +283,15 @@
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
@@ -304,16 +310,19 @@
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
@@ -397,15 +406,17 @@
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

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.py` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iottwinmaker service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iottwinmaker.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_iottwinmaker.type_defs import BundleInformationTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: BundleInformationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -42,89 +42,90 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
     "ComponentPropertyGroupResponseTypeDef",
     "PropertyDefinitionRequestTypeDef",
     "PropertyGroupRequestTypeDef",
+    "CreateComponentTypeResponseTypeDef",
+    "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
+    "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
+    "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
+    "CreateWorkspaceResponseTypeDef",
     "LambdaFunctionTypeDef",
     "RelationshipTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
+    "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
+    "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
+    "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
     "GetSceneRequestRequestTypeDef",
+    "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
+    "GetWorkspaceResponseTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
     "SceneSummaryTypeDef",
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
     "PropertyValueTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdatePricingPlanRequestRequestTypeDef",
-    "UpdateSceneRequestRequestTypeDef",
-    "UpdateWorkspaceRequestRequestTypeDef",
-    "CreateComponentTypeResponseTypeDef",
-    "CreateEntityResponseTypeDef",
-    "CreateSceneResponseTypeDef",
-    "CreateSyncJobResponseTypeDef",
-    "CreateWorkspaceResponseTypeDef",
-    "DeleteComponentTypeResponseTypeDef",
-    "DeleteEntityResponseTypeDef",
-    "DeleteSyncJobResponseTypeDef",
-    "GetSceneResponseTypeDef",
-    "GetWorkspaceResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateComponentTypeResponseTypeDef",
     "UpdateEntityResponseTypeDef",
+    "UpdatePricingPlanRequestRequestTypeDef",
+    "UpdateSceneRequestRequestTypeDef",
     "UpdateSceneResponseTypeDef",
+    "UpdateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
     "DataConnectorTypeDef",
     "DataTypeTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
     "GetPropertyValueHistoryRequestRequestTypeDef",
+    "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
     "PropertyValueEntryTypeDef",
@@ -156,25 +157,14 @@
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
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
 _RequiredBundleInformationTypeDef = TypedDict(
     "_RequiredBundleInformationTypeDef",
     {
         "bundleNames": List[str],
     },
 )
 _OptionalBundleInformationTypeDef = TypedDict(
@@ -240,14 +230,35 @@
     {
         "groupType": Literal["TABULAR"],
         "propertyNames": Sequence[str],
     },
     total=False,
 )
 
+CreateComponentTypeResponseTypeDef = TypedDict(
+    "CreateComponentTypeResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEntityResponseTypeDef = TypedDict(
+    "CreateEntityResponseTypeDef",
+    {
+        "entityId": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSceneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
     },
@@ -266,14 +277,23 @@
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
     pass
 
 
+CreateSceneResponseTypeDef = TypedDict(
+    "CreateSceneResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
     },
@@ -289,14 +309,24 @@
 
 class CreateSyncJobRequestRequestTypeDef(
     _RequiredCreateSyncJobRequestRequestTypeDef, _OptionalCreateSyncJobRequestRequestTypeDef
 ):
     pass
 
 
+CreateSyncJobResponseTypeDef = TypedDict(
+    "CreateSyncJobResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": SyncJobStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
         "s3Location": str,
         "role": str,
     },
@@ -313,14 +343,23 @@
 
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -346,14 +385,22 @@
     "DeleteComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
 
+DeleteComponentTypeResponseTypeDef = TypedDict(
+    "DeleteComponentTypeResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityId": str,
     },
 )
@@ -368,14 +415,22 @@
 
 class DeleteEntityRequestRequestTypeDef(
     _RequiredDeleteEntityRequestRequestTypeDef, _OptionalDeleteEntityRequestRequestTypeDef
 ):
     pass
 
 
+DeleteEntityResponseTypeDef = TypedDict(
+    "DeleteEntityResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSceneRequestRequestTypeDef = TypedDict(
     "DeleteSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -384,14 +439,22 @@
     "DeleteSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
     },
 )
 
+DeleteSyncJobResponseTypeDef = TypedDict(
+    "DeleteSyncJobResponseTypeDef",
+    {
+        "state": SyncJobStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -536,14 +599,23 @@
     "GetSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
 
+SceneErrorTypeDef = TypedDict(
+    "SceneErrorTypeDef",
+    {
+        "code": Literal["MATTERPORT_ERROR"],
+        "message": str,
+    },
+    total=False,
+)
+
 _RequiredGetSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredGetSyncJobRequestRequestTypeDef",
     {
         "syncSource": str,
     },
 )
 _OptionalGetSyncJobRequestRequestTypeDef = TypedDict(
@@ -564,14 +636,28 @@
 GetWorkspaceRequestRequestTypeDef = TypedDict(
     "GetWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
+GetWorkspaceResponseTypeDef = TypedDict(
+    "GetWorkspaceResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "description": str,
+        "s3Location": str,
+        "role": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListComponentTypesFilterTypeDef = TypedDict(
     "ListComponentTypesFilterTypeDef",
     {
         "extendsFrom": str,
         "namespace": str,
         "isAbstract": bool,
     },
@@ -685,14 +771,23 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -776,14 +871,25 @@
 )
 
 
 class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -792,14 +898,34 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateComponentTypeResponseTypeDef = TypedDict(
+    "UpdateComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "componentTypeId": str,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateEntityResponseTypeDef = TypedDict(
+    "UpdateEntityResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePricingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingPlanRequestRequestTypeDef",
     {
         "pricingMode": PricingModeType,
     },
 )
 _OptionalUpdatePricingPlanRequestRequestTypeDef = TypedDict(
@@ -838,14 +964,22 @@
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
     pass
 
 
+UpdateSceneResponseTypeDef = TypedDict(
+    "UpdateSceneResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -860,160 +994,19 @@
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
-CreateComponentTypeResponseTypeDef = TypedDict(
-    "CreateComponentTypeResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEntityResponseTypeDef = TypedDict(
-    "CreateEntityResponseTypeDef",
-    {
-        "entityId": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSceneResponseTypeDef = TypedDict(
-    "CreateSceneResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSyncJobResponseTypeDef = TypedDict(
-    "CreateSyncJobResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": SyncJobStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteComponentTypeResponseTypeDef = TypedDict(
-    "DeleteComponentTypeResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEntityResponseTypeDef = TypedDict(
-    "DeleteEntityResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSyncJobResponseTypeDef = TypedDict(
-    "DeleteSyncJobResponseTypeDef",
-    {
-        "state": SyncJobStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSceneResponseTypeDef = TypedDict(
-    "GetSceneResponseTypeDef",
-    {
-        "workspaceId": str,
-        "sceneId": str,
-        "contentLocation": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "description": str,
-        "capabilities": List[str],
-        "sceneMetadata": Dict[str, str],
-        "generatedSceneMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkspaceResponseTypeDef = TypedDict(
-    "GetWorkspaceResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "description": str,
-        "s3Location": str,
-        "role": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateComponentTypeResponseTypeDef = TypedDict(
-    "UpdateComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "componentTypeId": str,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEntityResponseTypeDef = TypedDict(
-    "UpdateEntityResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSceneResponseTypeDef = TypedDict(
-    "UpdateSceneResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPricingPlanTypeDef = TypedDict(
     "_RequiredPricingPlanTypeDef",
     {
         "effectiveDateTime": datetime,
@@ -1143,15 +1136,15 @@
 
 ExecuteQueryResponseTypeDef = TypedDict(
     "ExecuteQueryResponseTypeDef",
     {
         "columnDescriptions": List[ColumnDescriptionTypeDef],
         "rows": List[RowTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
@@ -1190,14 +1183,32 @@
 class GetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredGetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalGetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+GetSceneResponseTypeDef = TypedDict(
+    "GetSceneResponseTypeDef",
+    {
+        "workspaceId": str,
+        "sceneId": str,
+        "contentLocation": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "description": str,
+        "capabilities": List[str],
+        "sceneMetadata": Dict[str, str],
+        "generatedSceneMetadata": Dict[str, str],
+        "error": SceneErrorTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListComponentTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentTypesRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListComponentTypesRequestRequestTypeDef = TypedDict(
@@ -1242,15 +1253,15 @@
 
 
 ListScenesResponseTypeDef = TypedDict(
     "ListScenesResponseTypeDef",
     {
         "sceneSummaries": List[SceneSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSyncResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListSyncResourcesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1275,15 +1286,15 @@
 
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "workspaceSummaries": List[WorkspaceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TabularConditionsTypeDef = TypedDict(
     "TabularConditionsTypeDef",
     {
         "orderBy": Sequence[OrderByTypeDef],
@@ -1335,24 +1346,24 @@
 
 
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePricingPlanResponseTypeDef = TypedDict(
     "UpdatePricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentRequestTypeDef = TypedDict(
     "ComponentRequestTypeDef",
     {
         "description": str,
@@ -1398,15 +1409,15 @@
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
         "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
         "arn": str,
@@ -1464,15 +1475,15 @@
         "arn": str,
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
         "status": SyncJobStatusTypeDef,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SyncJobSummaryTypeDef = TypedDict(
     "SyncJobSummaryTypeDef",
     {
         "arn": str,
@@ -1558,15 +1569,15 @@
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1691,53 +1702,53 @@
         "arn": str,
         "isAbstract": bool,
         "isSchemaInitialized": bool,
         "status": StatusTypeDef,
         "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
         "syncSource": str,
         "componentTypeName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "entitySummaries": List[EntitySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSyncJobsResponseTypeDef = TypedDict(
     "ListSyncJobsResponseTypeDef",
     {
         "syncJobSummaries": List[SyncJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSyncResourcesResponseTypeDef = TypedDict(
     "ListSyncResourcesResponseTypeDef",
     {
         "syncResources": List[SyncResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEntityResponseTypeDef = TypedDict(
     "GetEntityResponseTypeDef",
     {
         "entityId": str,
@@ -1748,25 +1759,25 @@
         "description": str,
         "components": Dict[str, ComponentResponseTypeDef],
         "parentEntityId": str,
         "hasChildEntities": bool,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.pyi` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iottwinmaker service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iottwinmaker.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_iottwinmaker.type_defs import BundleInformationTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: BundleInformationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -41,89 +41,90 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
     "ComponentPropertyGroupResponseTypeDef",
     "PropertyDefinitionRequestTypeDef",
     "PropertyGroupRequestTypeDef",
+    "CreateComponentTypeResponseTypeDef",
+    "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
+    "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
+    "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
+    "CreateWorkspaceResponseTypeDef",
     "LambdaFunctionTypeDef",
     "RelationshipTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
+    "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
+    "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
+    "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
     "GetSceneRequestRequestTypeDef",
+    "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
+    "GetWorkspaceResponseTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
     "SceneSummaryTypeDef",
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
     "PropertyValueTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdatePricingPlanRequestRequestTypeDef",
-    "UpdateSceneRequestRequestTypeDef",
-    "UpdateWorkspaceRequestRequestTypeDef",
-    "CreateComponentTypeResponseTypeDef",
-    "CreateEntityResponseTypeDef",
-    "CreateSceneResponseTypeDef",
-    "CreateSyncJobResponseTypeDef",
-    "CreateWorkspaceResponseTypeDef",
-    "DeleteComponentTypeResponseTypeDef",
-    "DeleteEntityResponseTypeDef",
-    "DeleteSyncJobResponseTypeDef",
-    "GetSceneResponseTypeDef",
-    "GetWorkspaceResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateComponentTypeResponseTypeDef",
     "UpdateEntityResponseTypeDef",
+    "UpdatePricingPlanRequestRequestTypeDef",
+    "UpdateSceneRequestRequestTypeDef",
     "UpdateSceneResponseTypeDef",
+    "UpdateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
     "DataConnectorTypeDef",
     "DataTypeTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
     "GetPropertyValueHistoryRequestRequestTypeDef",
+    "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
     "PropertyValueEntryTypeDef",
@@ -155,25 +156,14 @@
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
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
 _RequiredBundleInformationTypeDef = TypedDict(
     "_RequiredBundleInformationTypeDef",
     {
         "bundleNames": List[str],
     },
 )
 _OptionalBundleInformationTypeDef = TypedDict(
@@ -237,14 +227,35 @@
     {
         "groupType": Literal["TABULAR"],
         "propertyNames": Sequence[str],
     },
     total=False,
 )
 
+CreateComponentTypeResponseTypeDef = TypedDict(
+    "CreateComponentTypeResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEntityResponseTypeDef = TypedDict(
+    "CreateEntityResponseTypeDef",
+    {
+        "entityId": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSceneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
     },
@@ -261,14 +272,23 @@
 )
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
     pass
 
+CreateSceneResponseTypeDef = TypedDict(
+    "CreateSceneResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
     },
@@ -282,14 +302,24 @@
 )
 
 class CreateSyncJobRequestRequestTypeDef(
     _RequiredCreateSyncJobRequestRequestTypeDef, _OptionalCreateSyncJobRequestRequestTypeDef
 ):
     pass
 
+CreateSyncJobResponseTypeDef = TypedDict(
+    "CreateSyncJobResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": SyncJobStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
         "s3Location": str,
         "role": str,
     },
@@ -304,14 +334,23 @@
 )
 
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -337,14 +376,22 @@
     "DeleteComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
 
+DeleteComponentTypeResponseTypeDef = TypedDict(
+    "DeleteComponentTypeResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityId": str,
     },
 )
@@ -357,14 +404,22 @@
 )
 
 class DeleteEntityRequestRequestTypeDef(
     _RequiredDeleteEntityRequestRequestTypeDef, _OptionalDeleteEntityRequestRequestTypeDef
 ):
     pass
 
+DeleteEntityResponseTypeDef = TypedDict(
+    "DeleteEntityResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSceneRequestRequestTypeDef = TypedDict(
     "DeleteSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -373,14 +428,22 @@
     "DeleteSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
     },
 )
 
+DeleteSyncJobResponseTypeDef = TypedDict(
+    "DeleteSyncJobResponseTypeDef",
+    {
+        "state": SyncJobStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -519,14 +582,23 @@
     "GetSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
 
+SceneErrorTypeDef = TypedDict(
+    "SceneErrorTypeDef",
+    {
+        "code": Literal["MATTERPORT_ERROR"],
+        "message": str,
+    },
+    total=False,
+)
+
 _RequiredGetSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredGetSyncJobRequestRequestTypeDef",
     {
         "syncSource": str,
     },
 )
 _OptionalGetSyncJobRequestRequestTypeDef = TypedDict(
@@ -545,14 +617,28 @@
 GetWorkspaceRequestRequestTypeDef = TypedDict(
     "GetWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
+GetWorkspaceResponseTypeDef = TypedDict(
+    "GetWorkspaceResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "description": str,
+        "s3Location": str,
+        "role": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListComponentTypesFilterTypeDef = TypedDict(
     "ListComponentTypesFilterTypeDef",
     {
         "extendsFrom": str,
         "namespace": str,
         "isAbstract": bool,
     },
@@ -658,14 +744,23 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -741,14 +836,25 @@
     },
     total=False,
 )
 
 class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -757,14 +863,34 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateComponentTypeResponseTypeDef = TypedDict(
+    "UpdateComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "componentTypeId": str,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateEntityResponseTypeDef = TypedDict(
+    "UpdateEntityResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePricingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingPlanRequestRequestTypeDef",
     {
         "pricingMode": PricingModeType,
     },
 )
 _OptionalUpdatePricingPlanRequestRequestTypeDef = TypedDict(
@@ -799,14 +925,22 @@
 )
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
     pass
 
+UpdateSceneResponseTypeDef = TypedDict(
+    "UpdateSceneResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -819,160 +953,19 @@
 )
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
-CreateComponentTypeResponseTypeDef = TypedDict(
-    "CreateComponentTypeResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEntityResponseTypeDef = TypedDict(
-    "CreateEntityResponseTypeDef",
-    {
-        "entityId": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSceneResponseTypeDef = TypedDict(
-    "CreateSceneResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSyncJobResponseTypeDef = TypedDict(
-    "CreateSyncJobResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": SyncJobStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteComponentTypeResponseTypeDef = TypedDict(
-    "DeleteComponentTypeResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEntityResponseTypeDef = TypedDict(
-    "DeleteEntityResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSyncJobResponseTypeDef = TypedDict(
-    "DeleteSyncJobResponseTypeDef",
-    {
-        "state": SyncJobStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSceneResponseTypeDef = TypedDict(
-    "GetSceneResponseTypeDef",
-    {
-        "workspaceId": str,
-        "sceneId": str,
-        "contentLocation": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "description": str,
-        "capabilities": List[str],
-        "sceneMetadata": Dict[str, str],
-        "generatedSceneMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkspaceResponseTypeDef = TypedDict(
-    "GetWorkspaceResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "description": str,
-        "s3Location": str,
-        "role": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateComponentTypeResponseTypeDef = TypedDict(
-    "UpdateComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "componentTypeId": str,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEntityResponseTypeDef = TypedDict(
-    "UpdateEntityResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSceneResponseTypeDef = TypedDict(
-    "UpdateSceneResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPricingPlanTypeDef = TypedDict(
     "_RequiredPricingPlanTypeDef",
     {
         "effectiveDateTime": datetime,
@@ -1096,15 +1089,15 @@
 
 ExecuteQueryResponseTypeDef = TypedDict(
     "ExecuteQueryResponseTypeDef",
     {
         "columnDescriptions": List[ColumnDescriptionTypeDef],
         "rows": List[RowTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
@@ -1141,14 +1134,32 @@
 
 class GetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredGetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalGetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
+GetSceneResponseTypeDef = TypedDict(
+    "GetSceneResponseTypeDef",
+    {
+        "workspaceId": str,
+        "sceneId": str,
+        "contentLocation": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "description": str,
+        "capabilities": List[str],
+        "sceneMetadata": Dict[str, str],
+        "generatedSceneMetadata": Dict[str, str],
+        "error": SceneErrorTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListComponentTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentTypesRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListComponentTypesRequestRequestTypeDef = TypedDict(
@@ -1189,15 +1200,15 @@
     pass
 
 ListScenesResponseTypeDef = TypedDict(
     "ListScenesResponseTypeDef",
     {
         "sceneSummaries": List[SceneSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSyncResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListSyncResourcesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1220,15 +1231,15 @@
     pass
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "workspaceSummaries": List[WorkspaceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TabularConditionsTypeDef = TypedDict(
     "TabularConditionsTypeDef",
     {
         "orderBy": Sequence[OrderByTypeDef],
@@ -1276,24 +1287,24 @@
     pass
 
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePricingPlanResponseTypeDef = TypedDict(
     "UpdatePricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentRequestTypeDef = TypedDict(
     "ComponentRequestTypeDef",
     {
         "description": str,
@@ -1339,15 +1350,15 @@
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
         "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
         "arn": str,
@@ -1401,15 +1412,15 @@
         "arn": str,
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
         "status": SyncJobStatusTypeDef,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SyncJobSummaryTypeDef = TypedDict(
     "SyncJobSummaryTypeDef",
     {
         "arn": str,
@@ -1493,15 +1504,15 @@
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1618,53 +1629,53 @@
         "arn": str,
         "isAbstract": bool,
         "isSchemaInitialized": bool,
         "status": StatusTypeDef,
         "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
         "syncSource": str,
         "componentTypeName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "entitySummaries": List[EntitySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSyncJobsResponseTypeDef = TypedDict(
     "ListSyncJobsResponseTypeDef",
     {
         "syncJobSummaries": List[SyncJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSyncResourcesResponseTypeDef = TypedDict(
     "ListSyncResourcesResponseTypeDef",
     {
         "syncResources": List[SyncResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEntityResponseTypeDef = TypedDict(
     "GetEntityResponseTypeDef",
     {
         "entityId": str,
@@ -1675,25 +1686,25 @@
         "description": str,
         "components": Dict[str, ComponentResponseTypeDef],
         "parentEntityId": str,
         "hasChildEntities": bool,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/PKG-INFO` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.26.97
-Summary: Type annotations for boto3.IoTTwinMaker 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTTwinMaker 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-iottwinmaker"></a>
 
 # mypy-boto3-iottwinmaker
 
 [![PyPI - mypy-boto3-iottwinmaker](https://img.shields.io/pypi/v/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,14 +288,15 @@
     OrderByTimeType,
     OrderType,
     ParentEntityUpdateTypeType,
     PricingModeType,
     PricingTierType,
     PropertyGroupUpdateTypeType,
     PropertyUpdateTypeType,
+    SceneErrorCodeType,
     ScopeType,
     StateType,
     SyncJobStateType,
     SyncResourceStateType,
     SyncResourceTypeType,
     TypeType,
     UpdateReasonType,
@@ -315,89 +316,90 @@
 ### Typed dictionaries
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
-    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
+    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
+    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
+    CreateWorkspaceResponseTypeDef,
     LambdaFunctionTypeDef,
     RelationshipTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
+    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
+    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
+    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
     GetSceneRequestRequestTypeDef,
+    SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
+    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePricingPlanRequestRequestTypeDef,
-    UpdateSceneRequestRequestTypeDef,
-    UpdateWorkspaceRequestRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
-    CreateSceneResponseTypeDef,
-    CreateSyncJobResponseTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    DeleteComponentTypeResponseTypeDef,
-    DeleteEntityResponseTypeDef,
-    DeleteSyncJobResponseTypeDef,
-    GetSceneResponseTypeDef,
-    GetWorkspaceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
+    UpdatePricingPlanRequestRequestTypeDef,
+    UpdateSceneRequestRequestTypeDef,
     UpdateSceneResponseTypeDef,
+    UpdateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
     DataConnectorTypeDef,
     DataTypeTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
     PropertyValueEntryTypeDef,
@@ -430,53 +432,53 @@
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> BundleInformationTypeDef:
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

### Comparing `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt` & `mypy-boto3-iottwinmaker-1.27.0/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.26.97/setup.py` & `mypy-boto3-iottwinmaker-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-iottwinmaker.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iottwinmaker",
-    version="1.26.97",
+    version="1.27.0",
     packages=["mypy_boto3_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTTwinMaker 1.26.97 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.IoTTwinMaker 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/",
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


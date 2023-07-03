# Comparing `tmp/mypy-boto3-m2-1.26.57.tar.gz` & `tmp/mypy-boto3-m2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-m2-1.26.57.tar", last modified: Wed Jan 25 20:48:07 2023, max compression
+gzip compressed data, was "mypy-boto3-m2-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-m2-1.26.57.tar` & `mypy-boto3-m2-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.692256 mypy-boto3-m2-1.26.57/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-01-25 20:48:07.676256 mypy-boto3-m2-1.26.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.676256 mypy-boto3-m2-1.26.57/mypy_boto3_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27335 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40890 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40826 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.676256 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:48:07.692256 mypy-boto3-m2-1.26.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.911601 mypy-boto3-m2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-07-03 19:51:03.907601 mypy-boto3-m2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16992 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.907601 mypy-boto3-m2-1.27.0/mypy_boto3_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27363 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27315 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42321 2023-07-03 19:41:25.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42253 2023-07-03 19:41:25.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.907601 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-07-03 19:51:03.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 19:51:03.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:51:03.000000 mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.911601 mypy-boto3-m2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-03 19:41:24.000000 mypy-boto3-m2-1.27.0/setup.py
```

### Comparing `mypy-boto3-m2-1.26.57/LICENSE` & `mypy-boto3-m2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-m2-1.26.57/PKG-INFO` & `mypy-boto3-m2-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.26.57
-Summary: Type annotations for boto3.MainframeModernization 1.26.57 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.MainframeModernization 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,91 +371,95 @@
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
+    PoDetailAttributesTypeDef,
+    PsDetailAttributesTypeDef,
     GdgAttributesTypeDef,
+    PoAttributesTypeDef,
+    PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
+    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
     ListBatchJobExecutionsRequestRequestTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
+    PaginatorConfigTypeDef,
     PrimaryKeyTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
+    UpdateEnvironmentResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    GetApplicationVersionResponseTypeDef,
-    GetDeploymentResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartBatchJobResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
@@ -480,42 +484,42 @@
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

### Comparing `mypy-boto3-m2-1.26.57/README.md` & `mypy-boto3-m2-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,91 +339,95 @@
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
+    PoDetailAttributesTypeDef,
+    PsDetailAttributesTypeDef,
     GdgAttributesTypeDef,
+    PoAttributesTypeDef,
+    PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
+    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
     ListBatchJobExecutionsRequestRequestTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
+    PaginatorConfigTypeDef,
     PrimaryKeyTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
+    UpdateEnvironmentResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    GetApplicationVersionResponseTypeDef,
-    GetDeploymentResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartBatchJobResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
@@ -448,42 +452,42 @@
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

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.py` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.pyi` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/__main__.py` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MainframeModernization 1.26.57\nVersion:        "
-        " 1.26.57\nBuilder version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.MainframeModernization 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.57")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.py` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         *,
         definition: DefinitionTypeDef,
         engineType: EngineTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyId: str = ...,
+        roleArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a new application with given parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_application)
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.pyi` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         *,
         definition: DefinitionTypeDef,
         engineType: EngineTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyId: str = ...,
+        roleArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a new application with given parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_application)
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.py` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationDeploymentLifecycleType",
     "ApplicationLifecycleType",
     "ApplicationVersionLifecycleType",
     "BatchJobExecutionStatusType",
     "BatchJobTypeType",
     "DataSetTaskLifecycleType",
@@ -41,15 +40,14 @@
     "MainframeModernizationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationDeploymentLifecycleType = Literal["Deployed", "Deploying"]
 ApplicationLifecycleType = Literal[
     "Available",
     "Created",
     "Creating",
     "Deleting",
     "Deleting From Environment",
@@ -98,14 +96,15 @@
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
@@ -137,21 +136,23 @@
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
@@ -230,14 +231,15 @@
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
@@ -248,14 +250,15 @@
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
@@ -291,14 +294,15 @@
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
@@ -317,16 +321,19 @@
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
@@ -406,18 +413,21 @@
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

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.pyi` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApplicationDeploymentLifecycleType",
     "ApplicationLifecycleType",
     "ApplicationVersionLifecycleType",
     "BatchJobExecutionStatusType",
     "BatchJobTypeType",
     "DataSetTaskLifecycleType",
@@ -40,14 +41,15 @@
     "MainframeModernizationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApplicationDeploymentLifecycleType = Literal["Deployed", "Deploying"]
 ApplicationLifecycleType = Literal[
     "Available",
     "Created",
     "Creating",
     "Deleting",
     "Deleting From Environment",
@@ -96,14 +98,15 @@
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
@@ -135,21 +138,23 @@
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
@@ -228,14 +233,15 @@
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
@@ -246,14 +252,15 @@
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
@@ -289,14 +296,15 @@
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
@@ -315,16 +323,19 @@
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
@@ -404,18 +415,21 @@
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

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.py` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
         """
 
 
@@ -99,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationspaginator)
         """
 
 
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 
@@ -141,30 +141,30 @@
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         startedAfter: Union[datetime, str] = ...,
         startedBefore: Union[datetime, str] = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 
 class ListDataSetImportHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetImportHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
         """
 
 
@@ -175,45 +175,45 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetspaginator)
         """
 
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
         """
 
 
 class ListEngineVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
     """
 
     def paginate(
-        self, *, engineType: EngineTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, engineType: EngineTypeType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
         """
 
 
@@ -224,13 +224,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.pyi` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
@@ -95,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationspaginator)
         """
 
 class ListBatchJobDefinitionsPaginator(Paginator):
@@ -113,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 class ListBatchJobExecutionsPaginator(Paginator):
@@ -135,29 +135,29 @@
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         startedAfter: Union[datetime, str] = ...,
         startedBefore: Union[datetime, str] = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 class ListDataSetImportHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetImportHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
         """
 
 class ListDataSetsPaginator(Paginator):
@@ -167,43 +167,43 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
         """
 
 class ListEngineVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
     """
 
     def paginate(
-        self, *, engineType: EngineTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, engineType: EngineTypeType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
         """
 
 class ListEnvironmentsPaginator(Paginator):
@@ -213,13 +213,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.py` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,91 +39,95 @@
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "CreateDeploymentResponseTypeDef",
     "HighAvailabilityConfigTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "ExternalLocationTypeDef",
     "DataSetImportSummaryTypeDef",
     "DataSetSummaryTypeDef",
     "RecordLengthTypeDef",
     "GdgDetailAttributesTypeDef",
+    "PoDetailAttributesTypeDef",
+    "PsDetailAttributesTypeDef",
     "GdgAttributesTypeDef",
+    "PoAttributesTypeDef",
+    "PsAttributesTypeDef",
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeployedVersionSummaryTypeDef",
     "DeploymentSummaryTypeDef",
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
+    "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
+    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
     "ListBatchJobExecutionsRequestRequestTypeDef",
+    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
+    "PaginatorConfigTypeDef",
     "PrimaryKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
+    "UpdateEnvironmentResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateDataSetImportTaskResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "GetApplicationVersionResponseTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "ListApplicationVersionsResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartBatchJobResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
-    "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "PendingMaintenanceTypeDef",
     "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
@@ -176,14 +180,15 @@
 _OptionalApplicationSummaryTypeDef = TypedDict(
     "_OptionalApplicationSummaryTypeDef",
     {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
         "environmentId": str,
         "lastStartTime": datetime,
+        "roleArn": str,
         "versionStatus": ApplicationVersionLifecycleType,
     },
     total=False,
 )
 
 
 class ApplicationSummaryTypeDef(
@@ -284,22 +289,29 @@
     {
         "content": str,
         "s3Location": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationArn": str,
+        "applicationId": str,
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSetImportTaskResponseTypeDef = TypedDict(
+    "CreateDataSetImportTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -318,21 +330,37 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HighAvailabilityConfigTypeDef = TypedDict(
     "HighAvailabilityConfigTypeDef",
     {
         "desiredCapacity": int,
     },
 )
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExternalLocationTypeDef = TypedDict(
     "ExternalLocationTypeDef",
     {
         "s3Location": str,
     },
     total=False,
 )
@@ -384,23 +412,78 @@
     {
         "limit": int,
         "rollDisposition": str,
     },
     total=False,
 )
 
+PoDetailAttributesTypeDef = TypedDict(
+    "PoDetailAttributesTypeDef",
+    {
+        "encoding": str,
+        "format": str,
+    },
+)
+
+PsDetailAttributesTypeDef = TypedDict(
+    "PsDetailAttributesTypeDef",
+    {
+        "encoding": str,
+        "format": str,
+    },
+)
+
 GdgAttributesTypeDef = TypedDict(
     "GdgAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
     total=False,
 )
 
+_RequiredPoAttributesTypeDef = TypedDict(
+    "_RequiredPoAttributesTypeDef",
+    {
+        "format": str,
+        "memberFileExtensions": Sequence[str],
+    },
+)
+_OptionalPoAttributesTypeDef = TypedDict(
+    "_OptionalPoAttributesTypeDef",
+    {
+        "encoding": str,
+    },
+    total=False,
+)
+
+
+class PoAttributesTypeDef(_RequiredPoAttributesTypeDef, _OptionalPoAttributesTypeDef):
+    pass
+
+
+_RequiredPsAttributesTypeDef = TypedDict(
+    "_RequiredPsAttributesTypeDef",
+    {
+        "format": str,
+    },
+)
+_OptionalPsAttributesTypeDef = TypedDict(
+    "_OptionalPsAttributesTypeDef",
+    {
+        "encoding": str,
+    },
+    total=False,
+)
+
+
+class PsAttributesTypeDef(_RequiredPsAttributesTypeDef, _OptionalPsAttributesTypeDef):
+    pass
+
+
 DeleteApplicationFromEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     {
         "applicationId": str,
         "environmentId": str,
     },
 )
@@ -524,14 +607,28 @@
     "GetApplicationVersionRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
     },
 )
 
+GetApplicationVersionResponseTypeDef = TypedDict(
+    "GetApplicationVersionResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "definitionContent": str,
+        "description": str,
+        "name": str,
+        "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
@@ -556,31 +653,57 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "deploymentId": str,
     },
 )
 
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "deploymentId": str,
+        "environmentId": str,
+        "status": DeploymentLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "applicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -596,25 +719,58 @@
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "environmentId": str,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "environmentId": str,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
+    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -631,14 +787,41 @@
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "startedAfter": Union[datetime, str],
+        "startedBefore": Union[datetime, str],
+        "status": BatchJobExecutionStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
+    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
@@ -659,14 +842,36 @@
 class ListBatchJobExecutionsRequestRequestTypeDef(
     _RequiredListBatchJobExecutionsRequestRequestTypeDef,
     _OptionalListBatchJobExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
+    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -682,14 +887,37 @@
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDataSetsRequestListDataSetsPaginateTypeDef(
+    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
+    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -705,14 +933,36 @@
 
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -727,24 +977,43 @@
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
 
+ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEngineVersionsRequestRequestTypeDef = TypedDict(
     "ListEngineVersionsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
@@ -755,23 +1024,41 @@
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
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
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
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -784,21 +1071,40 @@
 )
 
 
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartBatchJobResponseTypeDef = TypedDict(
+    "StartBatchJobResponseTypeDef",
+    {
+        "executionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredStopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalStopApplicationRequestRequestTypeDef = TypedDict(
@@ -828,14 +1134,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -853,14 +1167,40 @@
 
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
+UpdateEnvironmentResponseTypeDef = TypedDict(
+    "UpdateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
+    {
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationVersionsResponseTypeDef = TypedDict(
+    "ListApplicationVersionsResponseTypeDef",
+    {
+        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
     total=False,
@@ -885,14 +1225,15 @@
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
         "clientToken": str,
         "description": str,
         "kmsKeyId": str,
+        "roleArn": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateApplicationRequestRequestTypeDef(
@@ -920,126 +1261,14 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationArn": str,
-        "applicationId": str,
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSetImportTaskResponseTypeDef = TypedDict(
-    "CreateDataSetImportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetApplicationVersionResponseTypeDef = TypedDict(
-    "GetApplicationVersionResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "definitionContent": str,
-        "description": str,
-        "name": str,
-        "status": ApplicationVersionLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "deploymentId": str,
-        "environmentId": str,
-        "status": DeploymentLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationVersionsResponseTypeDef = TypedDict(
-    "ListApplicationVersionsResponseTypeDef",
-    {
-        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
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
-StartBatchJobResponseTypeDef = TypedDict(
-    "StartBatchJobResponseTypeDef",
-    {
-        "executionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEnvironmentResponseTypeDef = TypedDict(
-    "UpdateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1047,51 +1276,51 @@
 
 GetDataSetImportTaskResponseTypeDef = TypedDict(
     "GetDataSetImportTaskResponseTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "dataSets": List[DataSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEngineVersionsResponseTypeDef = TypedDict(
     "ListEngineVersionsResponseTypeDef",
     {
         "engineVersions": List[EngineVersionsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
@@ -1114,189 +1343,22 @@
         "lastStartTime": datetime,
         "latestVersion": ApplicationVersionSummaryTypeDef,
         "listenerArns": List[str],
         "listenerPorts": List[int],
         "loadBalancerDnsName": str,
         "logGroups": List[LogGroupSummaryTypeDef],
         "name": str,
+        "roleArn": str,
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "environmentId": str,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "applicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
-    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "startedAfter": Union[datetime, str],
-        "startedBefore": Union[datetime, str],
-        "status": BatchJobExecutionStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
-    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
-    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDataSetsRequestListDataSetsPaginateTypeDef(
-    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
-    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-
-ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
@@ -1339,15 +1401,15 @@
 )
 
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
     "_RequiredBatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
@@ -1387,15 +1449,15 @@
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -1418,15 +1480,15 @@
 
 
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
@@ -1480,42 +1542,46 @@
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
         "storageConfigurations": List[StorageConfigurationTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetOrgAttributesTypeDef = TypedDict(
     "DatasetOrgAttributesTypeDef",
     {
         "gdg": GdgAttributesTypeDef,
+        "po": PoAttributesTypeDef,
+        "ps": PsAttributesTypeDef,
         "vsam": VsamAttributesTypeDef,
     },
     total=False,
 )
 
 DatasetDetailOrgAttributesTypeDef = TypedDict(
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
+        "po": PoDetailAttributesTypeDef,
+        "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
     total=False,
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
@@ -1544,15 +1610,15 @@
         "creationTime": datetime,
         "dataSetName": str,
         "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
         "location": str,
         "recordLength": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.pyi` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,91 +38,95 @@
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "CreateDeploymentResponseTypeDef",
     "HighAvailabilityConfigTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "ExternalLocationTypeDef",
     "DataSetImportSummaryTypeDef",
     "DataSetSummaryTypeDef",
     "RecordLengthTypeDef",
     "GdgDetailAttributesTypeDef",
+    "PoDetailAttributesTypeDef",
+    "PsDetailAttributesTypeDef",
     "GdgAttributesTypeDef",
+    "PoAttributesTypeDef",
+    "PsAttributesTypeDef",
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeployedVersionSummaryTypeDef",
     "DeploymentSummaryTypeDef",
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
+    "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
+    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
     "ListBatchJobExecutionsRequestRequestTypeDef",
+    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
+    "PaginatorConfigTypeDef",
     "PrimaryKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
+    "UpdateEnvironmentResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateDataSetImportTaskResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "GetApplicationVersionResponseTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "ListApplicationVersionsResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartBatchJobResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
-    "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "PendingMaintenanceTypeDef",
     "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
@@ -173,14 +177,15 @@
 _OptionalApplicationSummaryTypeDef = TypedDict(
     "_OptionalApplicationSummaryTypeDef",
     {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
         "environmentId": str,
         "lastStartTime": datetime,
+        "roleArn": str,
         "versionStatus": ApplicationVersionLifecycleType,
     },
     total=False,
 )
 
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
@@ -273,22 +278,29 @@
     {
         "content": str,
         "s3Location": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationArn": str,
+        "applicationId": str,
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSetImportTaskResponseTypeDef = TypedDict(
+    "CreateDataSetImportTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -305,21 +317,37 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HighAvailabilityConfigTypeDef = TypedDict(
     "HighAvailabilityConfigTypeDef",
     {
         "desiredCapacity": int,
     },
 )
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExternalLocationTypeDef = TypedDict(
     "ExternalLocationTypeDef",
     {
         "s3Location": str,
     },
     total=False,
 )
@@ -369,23 +397,74 @@
     {
         "limit": int,
         "rollDisposition": str,
     },
     total=False,
 )
 
+PoDetailAttributesTypeDef = TypedDict(
+    "PoDetailAttributesTypeDef",
+    {
+        "encoding": str,
+        "format": str,
+    },
+)
+
+PsDetailAttributesTypeDef = TypedDict(
+    "PsDetailAttributesTypeDef",
+    {
+        "encoding": str,
+        "format": str,
+    },
+)
+
 GdgAttributesTypeDef = TypedDict(
     "GdgAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
     total=False,
 )
 
+_RequiredPoAttributesTypeDef = TypedDict(
+    "_RequiredPoAttributesTypeDef",
+    {
+        "format": str,
+        "memberFileExtensions": Sequence[str],
+    },
+)
+_OptionalPoAttributesTypeDef = TypedDict(
+    "_OptionalPoAttributesTypeDef",
+    {
+        "encoding": str,
+    },
+    total=False,
+)
+
+class PoAttributesTypeDef(_RequiredPoAttributesTypeDef, _OptionalPoAttributesTypeDef):
+    pass
+
+_RequiredPsAttributesTypeDef = TypedDict(
+    "_RequiredPsAttributesTypeDef",
+    {
+        "format": str,
+    },
+)
+_OptionalPsAttributesTypeDef = TypedDict(
+    "_OptionalPsAttributesTypeDef",
+    {
+        "encoding": str,
+    },
+    total=False,
+)
+
+class PsAttributesTypeDef(_RequiredPsAttributesTypeDef, _OptionalPsAttributesTypeDef):
+    pass
+
 DeleteApplicationFromEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     {
         "applicationId": str,
         "environmentId": str,
     },
 )
@@ -505,14 +584,28 @@
     "GetApplicationVersionRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
     },
 )
 
+GetApplicationVersionResponseTypeDef = TypedDict(
+    "GetApplicationVersionResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "definitionContent": str,
+        "description": str,
+        "name": str,
+        "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
@@ -537,31 +630,55 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "deploymentId": str,
     },
 )
 
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "deploymentId": str,
+        "environmentId": str,
+        "status": DeploymentLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "applicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -575,25 +692,56 @@
 
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "environmentId": str,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "environmentId": str,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
+    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -608,14 +756,39 @@
 
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "startedAfter": Union[datetime, str],
+        "startedBefore": Union[datetime, str],
+        "status": BatchJobExecutionStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
+    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
@@ -634,14 +807,34 @@
 
 class ListBatchJobExecutionsRequestRequestTypeDef(
     _RequiredListBatchJobExecutionsRequestRequestTypeDef,
     _OptionalListBatchJobExecutionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
+    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -655,14 +848,35 @@
 
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDataSetsRequestListDataSetsPaginateTypeDef(
+    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
+    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -676,14 +890,34 @@
 )
 
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -696,24 +930,43 @@
 )
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
+ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEngineVersionsRequestRequestTypeDef = TypedDict(
     "ListEngineVersionsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
@@ -724,23 +977,41 @@
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
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
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
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -751,21 +1022,40 @@
     },
     total=False,
 )
 
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartBatchJobResponseTypeDef = TypedDict(
+    "StartBatchJobResponseTypeDef",
+    {
+        "executionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredStopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalStopApplicationRequestRequestTypeDef = TypedDict(
@@ -793,14 +1083,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -816,14 +1114,40 @@
 )
 
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+UpdateEnvironmentResponseTypeDef = TypedDict(
+    "UpdateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
+    {
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationVersionsResponseTypeDef = TypedDict(
+    "ListApplicationVersionsResponseTypeDef",
+    {
+        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
     total=False,
@@ -848,14 +1172,15 @@
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
         "clientToken": str,
         "description": str,
         "kmsKeyId": str,
+        "roleArn": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
@@ -879,126 +1204,14 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationArn": str,
-        "applicationId": str,
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSetImportTaskResponseTypeDef = TypedDict(
-    "CreateDataSetImportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetApplicationVersionResponseTypeDef = TypedDict(
-    "GetApplicationVersionResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "definitionContent": str,
-        "description": str,
-        "name": str,
-        "status": ApplicationVersionLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "deploymentId": str,
-        "environmentId": str,
-        "status": DeploymentLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationVersionsResponseTypeDef = TypedDict(
-    "ListApplicationVersionsResponseTypeDef",
-    {
-        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
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
-StartBatchJobResponseTypeDef = TypedDict(
-    "StartBatchJobResponseTypeDef",
-    {
-        "executionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEnvironmentResponseTypeDef = TypedDict(
-    "UpdateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1006,51 +1219,51 @@
 
 GetDataSetImportTaskResponseTypeDef = TypedDict(
     "GetDataSetImportTaskResponseTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "dataSets": List[DataSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEngineVersionsResponseTypeDef = TypedDict(
     "ListEngineVersionsResponseTypeDef",
     {
         "engineVersions": List[EngineVersionsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
@@ -1073,177 +1286,22 @@
         "lastStartTime": datetime,
         "latestVersion": ApplicationVersionSummaryTypeDef,
         "listenerArns": List[str],
         "listenerPorts": List[int],
         "loadBalancerDnsName": str,
         "logGroups": List[LogGroupSummaryTypeDef],
         "name": str,
+        "roleArn": str,
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "environmentId": str,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
-    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "startedAfter": Union[datetime, str],
-        "startedBefore": Union[datetime, str],
-        "status": BatchJobExecutionStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
-    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
-    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "applicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDataSetsRequestListDataSetsPaginateTypeDef(
-    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
-    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
@@ -1284,15 +1342,15 @@
 )
 
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
     "_RequiredBatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
@@ -1330,15 +1388,15 @@
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -1359,15 +1417,15 @@
     pass
 
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
@@ -1419,42 +1477,46 @@
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
         "storageConfigurations": List[StorageConfigurationTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetOrgAttributesTypeDef = TypedDict(
     "DatasetOrgAttributesTypeDef",
     {
         "gdg": GdgAttributesTypeDef,
+        "po": PoAttributesTypeDef,
+        "ps": PsAttributesTypeDef,
         "vsam": VsamAttributesTypeDef,
     },
     total=False,
 )
 
 DatasetDetailOrgAttributesTypeDef = TypedDict(
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
+        "po": PoDetailAttributesTypeDef,
+        "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
     total=False,
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
@@ -1481,15 +1543,15 @@
         "creationTime": datetime,
         "dataSetName": str,
         "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
         "location": str,
         "recordLength": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
```

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/PKG-INFO` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.26.57
-Summary: Type annotations for boto3.MainframeModernization 1.26.57 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.MainframeModernization 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,91 +371,95 @@
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
+    PoDetailAttributesTypeDef,
+    PsDetailAttributesTypeDef,
     GdgAttributesTypeDef,
+    PoAttributesTypeDef,
+    PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
+    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
     ListBatchJobExecutionsRequestRequestTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
+    PaginatorConfigTypeDef,
     PrimaryKeyTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
+    UpdateEnvironmentResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    GetApplicationVersionResponseTypeDef,
-    GetDeploymentResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartBatchJobResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
@@ -480,42 +484,42 @@
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

### Comparing `mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/SOURCES.txt` & `mypy-boto3-m2-1.27.0/mypy_boto3_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.57/setup.py` & `mypy-boto3-m2-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-m2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-m2",
-    version="1.26.57",
+    version="1.27.0",
     packages=["mypy_boto3_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MainframeModernization 1.26.57 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.MainframeModernization 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/",
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


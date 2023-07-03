# Comparing `tmp/mypy-boto3-proton-1.26.9.tar.gz` & `tmp/mypy-boto3-proton-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-proton-1.26.9.tar", last modified: Mon Nov 14 20:49:29 2022, max compression
+gzip compressed data, was "mypy-boto3-proton-1.27.0.tar", last modified: Mon Jul  3 19:51:17 2023, max compression
```

## Comparing `mypy-boto3-proton-1.26.9.tar` & `mypy-boto3-proton-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.648561 mypy-boto3-proton-1.26.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    29483 2022-11-14 20:49:29.644561 mypy-boto3-proton-1.26.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    28052 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.644561 mypy-boto3-proton-1.26.9/mypy_boto3_proton/
--rw-r--r--   0 runner    (1001) docker     (121)     7753 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    66522 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    66410 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14001 2022-11-14 20:49:00.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13999 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    24938 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    24915 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    96668 2022-11-14 20:49:02.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    96506 2022-11-14 20:49:01.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10159 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10149 2022-11-14 20:48:59.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.644561 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    29483 2022-11-14 20:49:29.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-14 20:49:29.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-14 20:49:29.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-14 20:49:29.000000 mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 20:49:29.648561 mypy-boto3-proton-1.26.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-11-14 20:48:58.000000 mypy-boto3-proton-1.26.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.151835 mypy-boto3-proton-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-07-03 19:51:17.151835 mypy-boto3-proton-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29149 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.151835 mypy-boto3-proton-1.27.0/mypy_boto3_proton/
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72051 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71930 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105724 2023-07-03 19:43:53.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105551 2023-07-03 19:43:52.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-03 19:43:51.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.151835 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-07-03 19:51:16.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:17.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:16.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:51:16.000000 mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:17.151835 mypy-boto3-proton-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:43:50.000000 mypy-boto3-proton-1.27.0/setup.py
```

### Comparing `mypy-boto3-proton-1.26.9/LICENSE` & `mypy-boto3-proton-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-proton-1.26.9/PKG-INFO` & `mypy-boto3-proton-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-proton
-Version: 1.26.9
-Summary: Type annotations for boto3.Proton 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Proton 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/
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
 
 <a id="mypy-boto3-proton"></a>
 
 # mypy-boto3-proton
 
 [![PyPI - mypy-boto3-proton](https://img.shields.io/pypi/v/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Proton 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[boto3.Proton 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,14 +416,16 @@
 ### Literals
 
 `mypy_boto3_proton.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_proton.literals import (
+    BlockerStatusType,
+    BlockerTypeType,
     ComponentDeletedWaiterName,
     ComponentDeployedWaiterName,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
@@ -437,15 +440,17 @@
     ListEnvironmentTemplateVersionsPaginatorName,
     ListEnvironmentTemplatesPaginatorName,
     ListEnvironmentsPaginatorName,
     ListRepositoriesPaginatorName,
     ListRepositorySyncDefinitionsPaginatorName,
     ListServiceInstanceOutputsPaginatorName,
     ListServiceInstanceProvisionedResourcesPaginatorName,
+    ListServiceInstancesFilterByType,
     ListServiceInstancesPaginatorName,
+    ListServiceInstancesSortByType,
     ListServicePipelineOutputsPaginatorName,
     ListServicePipelineProvisionedResourcesPaginatorName,
     ListServiceTemplateVersionsPaginatorName,
     ListServiceTemplatesPaginatorName,
     ListServicesPaginatorName,
     ListTagsForResourcePaginatorName,
     ProvisionedResourceEngineType,
@@ -458,68 +463,72 @@
     ServiceDeletedWaiterName,
     ServiceInstanceDeployedWaiterName,
     ServicePipelineDeployedWaiterName,
     ServiceStatusType,
     ServiceTemplateSupportedComponentSourceTypeType,
     ServiceTemplateVersionRegisteredWaiterName,
     ServiceUpdatedWaiterName,
+    SortOrderType,
     SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
     ProtonServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
 )
 
 
-def check_value(value: ComponentDeletedWaiterName) -> bool:
+def check_value(value: BlockerStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_proton.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_proton.type_defs import (
     AcceptEnvironmentAccountConnectionInputRequestTypeDef,
     EnvironmentAccountConnectionTypeDef,
-    ResponseMetadataTypeDef,
     RepositoryBranchTypeDef,
     CancelComponentDeploymentInputRequestTypeDef,
     ComponentTypeDef,
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
     ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
     ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
     CompatibleEnvironmentTemplateTypeDef,
     ComponentSummaryTypeDef,
+    ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
     EnvironmentTemplateTypeDef,
     EnvironmentTemplateVersionTypeDef,
     RepositoryTypeDef,
+    CreateServiceSyncConfigInputRequestTypeDef,
+    ServiceSyncConfigTypeDef,
     ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
     TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
+    DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
     EnvironmentAccountConnectionSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
     EnvironmentTemplateSummaryTypeDef,
@@ -530,59 +539,84 @@
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
     GetServiceInstanceInputRequestTypeDef,
+    GetServiceInstanceSyncStatusInputRequestTypeDef,
+    RevisionTypeDef,
+    GetServiceSyncBlockerSummaryInputRequestTypeDef,
+    GetServiceSyncConfigInputRequestTypeDef,
     GetServiceTemplateInputRequestTypeDef,
     GetServiceTemplateVersionInputRequestTypeDef,
     GetTemplateSyncConfigInputRequestTypeDef,
     GetTemplateSyncStatusInputRequestTypeDef,
-    RevisionTypeDef,
-    PaginatorConfigTypeDef,
+    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
     ListComponentOutputsInputRequestTypeDef,
     OutputTypeDef,
+    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
     ProvisionedResourceTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
+    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
     ListEnvironmentOutputsInputRequestTypeDef,
+    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
+    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
     ListEnvironmentTemplateVersionsInputRequestTypeDef,
+    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
     ListEnvironmentTemplatesInputRequestTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositorySummaryTypeDef,
+    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
     ListRepositorySyncDefinitionsInputRequestTypeDef,
     RepositorySyncDefinitionTypeDef,
+    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
     ListServiceInstanceOutputsInputRequestTypeDef,
+    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
     ListServiceInstanceProvisionedResourcesInputRequestTypeDef,
-    ListServiceInstancesInputRequestTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ServiceInstanceSummaryTypeDef,
+    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
     ListServicePipelineOutputsInputRequestTypeDef,
+    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
     ListServicePipelineProvisionedResourcesInputRequestTypeDef,
+    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
     ListServiceTemplateVersionsInputRequestTypeDef,
     ServiceTemplateVersionSummaryTypeDef,
+    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
     ListServiceTemplatesInputRequestTypeDef,
     ServiceTemplateSummaryTypeDef,
+    ListServicesInputListServicesPaginateTypeDef,
     ListServicesInputRequestTypeDef,
     ServiceSummaryTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     RejectEnvironmentAccountConnectionInputRequestTypeDef,
     RepositorySyncEventTypeDef,
     ResourceSyncEventTypeDef,
+    ResponseMetadataTypeDef,
     S3ObjectSourceTypeDef,
+    SyncBlockerContextTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateComponentInputRequestTypeDef,
     UpdateEnvironmentAccountConnectionInputRequestTypeDef,
     UpdateEnvironmentTemplateInputRequestTypeDef,
     UpdateEnvironmentTemplateVersionInputRequestTypeDef,
     UpdateServiceInputRequestTypeDef,
     UpdateServiceInstanceInputRequestTypeDef,
     UpdateServicePipelineInputRequestTypeDef,
+    UpdateServiceSyncBlockerInputRequestTypeDef,
+    UpdateServiceSyncConfigInputRequestTypeDef,
     UpdateServiceTemplateInputRequestTypeDef,
     UpdateTemplateSyncConfigInputRequestTypeDef,
     AcceptEnvironmentAccountConnectionOutputTypeDef,
     CreateEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     RejectEnvironmentAccountConnectionOutputTypeDef,
@@ -591,27 +625,30 @@
     EnvironmentTypeDef,
     CancelComponentDeploymentOutputTypeDef,
     CreateComponentOutputTypeDef,
     DeleteComponentOutputTypeDef,
     GetComponentOutputTypeDef,
     UpdateComponentOutputTypeDef,
     CancelServiceInstanceDeploymentOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
     GetServiceInstanceOutputTypeDef,
     UpdateServiceInstanceOutputTypeDef,
     CancelServicePipelineDeploymentOutputTypeDef,
     ServiceTypeDef,
     UpdateServicePipelineOutputTypeDef,
     UpdateServiceTemplateVersionInputRequestTypeDef,
     ServiceTemplateVersionTypeDef,
     ListComponentsOutputTypeDef,
+    CountsSummaryTypeDef,
     CreateComponentInputRequestTypeDef,
     CreateEnvironmentAccountConnectionInputRequestTypeDef,
     CreateEnvironmentTemplateInputRequestTypeDef,
     CreateRepositoryInputRequestTypeDef,
     CreateServiceInputRequestTypeDef,
+    CreateServiceInstanceInputRequestTypeDef,
     CreateServiceTemplateInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     CreateEnvironmentTemplateOutputTypeDef,
@@ -621,75 +658,63 @@
     CreateEnvironmentTemplateVersionOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     UpdateEnvironmentTemplateVersionOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
     GetComponentInputComponentDeployedWaitTypeDef,
     GetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     GetServiceInputServiceCreatedWaitTypeDef,
     GetServiceInputServiceDeletedWaitTypeDef,
     GetServiceInputServicePipelineDeployedWaitTypeDef,
     GetServiceInputServiceUpdatedWaitTypeDef,
     GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
-    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
-    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
-    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
-    ListServicesInputListServicesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
+    ListServiceInstancesInputRequestTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServicesOutputTypeDef,
     RepositorySyncAttemptTypeDef,
     ResourceSyncAttemptTypeDef,
     TemplateVersionSourceInputTypeDef,
+    SyncBlockerTypeDef,
     GetAccountSettingsOutputTypeDef,
     UpdateAccountSettingsOutputTypeDef,
     CancelEnvironmentDeploymentOutputTypeDef,
     CreateEnvironmentOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
@@ -697,60 +722,65 @@
     DeleteServiceOutputTypeDef,
     GetServiceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
+    ServiceSyncBlockerSummaryTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
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

### Comparing `mypy-boto3-proton-1.26.9/README.md` & `mypy-boto3-proton-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-proton"></a>
 
 # mypy-boto3-proton
 
 [![PyPI - mypy-boto3-proton](https://img.shields.io/pypi/v/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Proton 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[boto3.Proton 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,14 +384,16 @@
 ### Literals
 
 `mypy_boto3_proton.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_proton.literals import (
+    BlockerStatusType,
+    BlockerTypeType,
     ComponentDeletedWaiterName,
     ComponentDeployedWaiterName,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
@@ -406,15 +408,17 @@
     ListEnvironmentTemplateVersionsPaginatorName,
     ListEnvironmentTemplatesPaginatorName,
     ListEnvironmentsPaginatorName,
     ListRepositoriesPaginatorName,
     ListRepositorySyncDefinitionsPaginatorName,
     ListServiceInstanceOutputsPaginatorName,
     ListServiceInstanceProvisionedResourcesPaginatorName,
+    ListServiceInstancesFilterByType,
     ListServiceInstancesPaginatorName,
+    ListServiceInstancesSortByType,
     ListServicePipelineOutputsPaginatorName,
     ListServicePipelineProvisionedResourcesPaginatorName,
     ListServiceTemplateVersionsPaginatorName,
     ListServiceTemplatesPaginatorName,
     ListServicesPaginatorName,
     ListTagsForResourcePaginatorName,
     ProvisionedResourceEngineType,
@@ -427,68 +431,72 @@
     ServiceDeletedWaiterName,
     ServiceInstanceDeployedWaiterName,
     ServicePipelineDeployedWaiterName,
     ServiceStatusType,
     ServiceTemplateSupportedComponentSourceTypeType,
     ServiceTemplateVersionRegisteredWaiterName,
     ServiceUpdatedWaiterName,
+    SortOrderType,
     SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
     ProtonServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
 )
 
 
-def check_value(value: ComponentDeletedWaiterName) -> bool:
+def check_value(value: BlockerStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_proton.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_proton.type_defs import (
     AcceptEnvironmentAccountConnectionInputRequestTypeDef,
     EnvironmentAccountConnectionTypeDef,
-    ResponseMetadataTypeDef,
     RepositoryBranchTypeDef,
     CancelComponentDeploymentInputRequestTypeDef,
     ComponentTypeDef,
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
     ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
     ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
     CompatibleEnvironmentTemplateTypeDef,
     ComponentSummaryTypeDef,
+    ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
     EnvironmentTemplateTypeDef,
     EnvironmentTemplateVersionTypeDef,
     RepositoryTypeDef,
+    CreateServiceSyncConfigInputRequestTypeDef,
+    ServiceSyncConfigTypeDef,
     ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
     TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
+    DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
     EnvironmentAccountConnectionSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
     EnvironmentTemplateSummaryTypeDef,
@@ -499,59 +507,84 @@
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
     GetServiceInstanceInputRequestTypeDef,
+    GetServiceInstanceSyncStatusInputRequestTypeDef,
+    RevisionTypeDef,
+    GetServiceSyncBlockerSummaryInputRequestTypeDef,
+    GetServiceSyncConfigInputRequestTypeDef,
     GetServiceTemplateInputRequestTypeDef,
     GetServiceTemplateVersionInputRequestTypeDef,
     GetTemplateSyncConfigInputRequestTypeDef,
     GetTemplateSyncStatusInputRequestTypeDef,
-    RevisionTypeDef,
-    PaginatorConfigTypeDef,
+    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
     ListComponentOutputsInputRequestTypeDef,
     OutputTypeDef,
+    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
     ProvisionedResourceTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
+    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
     ListEnvironmentOutputsInputRequestTypeDef,
+    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
+    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
     ListEnvironmentTemplateVersionsInputRequestTypeDef,
+    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
     ListEnvironmentTemplatesInputRequestTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositorySummaryTypeDef,
+    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
     ListRepositorySyncDefinitionsInputRequestTypeDef,
     RepositorySyncDefinitionTypeDef,
+    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
     ListServiceInstanceOutputsInputRequestTypeDef,
+    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
     ListServiceInstanceProvisionedResourcesInputRequestTypeDef,
-    ListServiceInstancesInputRequestTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ServiceInstanceSummaryTypeDef,
+    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
     ListServicePipelineOutputsInputRequestTypeDef,
+    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
     ListServicePipelineProvisionedResourcesInputRequestTypeDef,
+    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
     ListServiceTemplateVersionsInputRequestTypeDef,
     ServiceTemplateVersionSummaryTypeDef,
+    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
     ListServiceTemplatesInputRequestTypeDef,
     ServiceTemplateSummaryTypeDef,
+    ListServicesInputListServicesPaginateTypeDef,
     ListServicesInputRequestTypeDef,
     ServiceSummaryTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     RejectEnvironmentAccountConnectionInputRequestTypeDef,
     RepositorySyncEventTypeDef,
     ResourceSyncEventTypeDef,
+    ResponseMetadataTypeDef,
     S3ObjectSourceTypeDef,
+    SyncBlockerContextTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateComponentInputRequestTypeDef,
     UpdateEnvironmentAccountConnectionInputRequestTypeDef,
     UpdateEnvironmentTemplateInputRequestTypeDef,
     UpdateEnvironmentTemplateVersionInputRequestTypeDef,
     UpdateServiceInputRequestTypeDef,
     UpdateServiceInstanceInputRequestTypeDef,
     UpdateServicePipelineInputRequestTypeDef,
+    UpdateServiceSyncBlockerInputRequestTypeDef,
+    UpdateServiceSyncConfigInputRequestTypeDef,
     UpdateServiceTemplateInputRequestTypeDef,
     UpdateTemplateSyncConfigInputRequestTypeDef,
     AcceptEnvironmentAccountConnectionOutputTypeDef,
     CreateEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     RejectEnvironmentAccountConnectionOutputTypeDef,
@@ -560,27 +593,30 @@
     EnvironmentTypeDef,
     CancelComponentDeploymentOutputTypeDef,
     CreateComponentOutputTypeDef,
     DeleteComponentOutputTypeDef,
     GetComponentOutputTypeDef,
     UpdateComponentOutputTypeDef,
     CancelServiceInstanceDeploymentOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
     GetServiceInstanceOutputTypeDef,
     UpdateServiceInstanceOutputTypeDef,
     CancelServicePipelineDeploymentOutputTypeDef,
     ServiceTypeDef,
     UpdateServicePipelineOutputTypeDef,
     UpdateServiceTemplateVersionInputRequestTypeDef,
     ServiceTemplateVersionTypeDef,
     ListComponentsOutputTypeDef,
+    CountsSummaryTypeDef,
     CreateComponentInputRequestTypeDef,
     CreateEnvironmentAccountConnectionInputRequestTypeDef,
     CreateEnvironmentTemplateInputRequestTypeDef,
     CreateRepositoryInputRequestTypeDef,
     CreateServiceInputRequestTypeDef,
+    CreateServiceInstanceInputRequestTypeDef,
     CreateServiceTemplateInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     CreateEnvironmentTemplateOutputTypeDef,
@@ -590,75 +626,63 @@
     CreateEnvironmentTemplateVersionOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     UpdateEnvironmentTemplateVersionOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
     GetComponentInputComponentDeployedWaitTypeDef,
     GetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     GetServiceInputServiceCreatedWaitTypeDef,
     GetServiceInputServiceDeletedWaitTypeDef,
     GetServiceInputServicePipelineDeployedWaitTypeDef,
     GetServiceInputServiceUpdatedWaitTypeDef,
     GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
-    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
-    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
-    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
-    ListServicesInputListServicesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
+    ListServiceInstancesInputRequestTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServicesOutputTypeDef,
     RepositorySyncAttemptTypeDef,
     ResourceSyncAttemptTypeDef,
     TemplateVersionSourceInputTypeDef,
+    SyncBlockerTypeDef,
     GetAccountSettingsOutputTypeDef,
     UpdateAccountSettingsOutputTypeDef,
     CancelEnvironmentDeploymentOutputTypeDef,
     CreateEnvironmentOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
@@ -666,60 +690,65 @@
     DeleteServiceOutputTypeDef,
     GetServiceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
+    ServiceSyncBlockerSummaryTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
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

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/__init__.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/__init__.pyi` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/__main__.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Proton 1.26.9\nVersion:         1.26.9\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Proton 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.9")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/client.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,19 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ComponentDeploymentUpdateTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
+    ListServiceInstancesSortByType,
     RepositoryProviderType,
     ResourceDeploymentStatusType,
+    SortOrderType,
+    SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
@@ -59,39 +62,46 @@
     CompatibleEnvironmentTemplateInputTypeDef,
     CreateComponentOutputTypeDef,
     CreateEnvironmentAccountConnectionOutputTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateEnvironmentTemplateOutputTypeDef,
     CreateEnvironmentTemplateVersionOutputTypeDef,
     CreateRepositoryOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
     CreateServiceOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteComponentOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     DeleteEnvironmentTemplateOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     DeleteServiceOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetComponentOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     GetEnvironmentTemplateOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     GetRepositoryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
     GetServiceInstanceOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
     GetServiceOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
@@ -101,14 +111,15 @@
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListServicesOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -122,14 +133,16 @@
     UpdateEnvironmentAccountConnectionOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateEnvironmentTemplateOutputTypeDef,
     UpdateEnvironmentTemplateVersionOutputTypeDef,
     UpdateServiceInstanceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     UpdateServicePipelineOutputTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
 )
 from .waiter import (
     ComponentDeletedWaiter,
     ComponentDeployedWaiter,
@@ -144,37 +157,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ProtonClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ProtonClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/)
     """
 
     meta: ClientMeta
@@ -183,105 +192,97 @@
     def exceptions(self) -> Exceptions:
         """
         ProtonClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#exceptions)
         """
-
     def accept_environment_account_connection(
         self, *, id: str
     ) -> AcceptEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, an environment account connection request is accepted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#accept_environment_account_connection)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#can_paginate)
         """
-
     def cancel_component_deployment(
         self, *, componentName: str
     ) -> CancelComponentDeploymentOutputTypeDef:
         """
         Attempts to cancel a component deployment (for a component that is in the
         `IN_PROGRESS` deployment status).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_component_deployment)
         """
-
     def cancel_environment_deployment(
         self, *, environmentName: str
     ) -> CancelEnvironmentDeploymentOutputTypeDef:
         """
         Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
         the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_environment_deployment)
         """
-
     def cancel_service_instance_deployment(
         self, *, serviceInstanceName: str, serviceName: str
     ) -> CancelServiceInstanceDeploymentOutputTypeDef:
         """
         Attempts to cancel a service instance deployment on an  UpdateServiceInstance
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_instance_deployment)
         """
-
     def cancel_service_pipeline_deployment(
         self, *, serviceName: str
     ) -> CancelServicePipelineDeploymentOutputTypeDef:
         """
         Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_pipeline_deployment)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#close)
         """
-
     def create_component(
         self,
         *,
         manifest: str,
         name: str,
         templateFile: str,
+        clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateComponentOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_component)
         """
-
     def create_environment(
         self,
         *,
         name: str,
         spec: str,
         templateMajorVersion: str,
         templateName: str,
@@ -296,35 +297,33 @@
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment)
         """
-
     def create_environment_account_connection(
         self,
         *,
         environmentName: str,
         managementAccountId: str,
-        roleArn: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
+        roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_account_connection)
         """
-
     def create_environment_template(
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
@@ -333,15 +332,14 @@
     ) -> CreateEnvironmentTemplateOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template)
         """
-
     def create_environment_template_version(
         self,
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
@@ -350,15 +348,14 @@
     ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template_version)
         """
-
     def create_repository(
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
@@ -366,15 +363,14 @@
     ) -> CreateRepositoryOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_repository)
         """
-
     def create_service(
         self,
         *,
         name: str,
         spec: str,
         templateMajorVersion: str,
         templateName: str,
@@ -387,15 +383,46 @@
     ) -> CreateServiceOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service)
         """
+    def create_service_instance(
+        self,
+        *,
+        name: str,
+        serviceName: str,
+        spec: str,
+        clientToken: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+        templateMajorVersion: str = ...,
+        templateMinorVersion: str = ...
+    ) -> CreateServiceInstanceOutputTypeDef:
+        """
+        Create a service instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_instance)
+        """
+    def create_service_sync_config(
+        self,
+        *,
+        branch: str,
+        filePath: str,
+        repositoryName: str,
+        repositoryProvider: RepositoryProviderType,
+        serviceName: str
+    ) -> CreateServiceSyncConfigOutputTypeDef:
+        """
+        Create the Proton Ops configuration file.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_sync_config)
+        """
     def create_service_template(
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
@@ -404,15 +431,14 @@
     ) -> CreateServiceTemplateOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template)
         """
-
     def create_service_template_version(
         self,
         *,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef],
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
@@ -423,15 +449,14 @@
     ) -> CreateServiceTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template_version)
         """
-
     def create_template_sync_config(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
@@ -441,277 +466,290 @@
         """
         Set up a template to create new template versions automatically by tracking a
         linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_template_sync_config)
         """
-
     def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
-
     def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
-
     def delete_environment_account_connection(
         self, *, id: str
     ) -> DeleteEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, delete an environment account connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_account_connection)
         """
-
     def delete_environment_template(self, *, name: str) -> DeleteEnvironmentTemplateOutputTypeDef:
         """
         If no other major or minor versions of an environment template exist, delete the
         environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template)
         """
-
     def delete_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> DeleteEnvironmentTemplateVersionOutputTypeDef:
         """
         If no other minor versions of an environment template exist, delete a major
         version of the environment template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template_version)
         """
-
     def delete_repository(
         self, *, name: str, provider: RepositoryProviderType
     ) -> DeleteRepositoryOutputTypeDef:
         """
         De-register and unlink your repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_repository)
         """
-
     def delete_service(self, *, name: str) -> DeleteServiceOutputTypeDef:
         """
         Delete a service, with its instances and pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service)
         """
+    def delete_service_sync_config(
+        self, *, serviceName: str
+    ) -> DeleteServiceSyncConfigOutputTypeDef:
+        """
+        Delete the Proton Ops file.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_sync_config)
+        """
     def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputTypeDef:
         """
         If no other major or minor versions of the service template exist, delete the
         service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template)
         """
-
     def delete_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> DeleteServiceTemplateVersionOutputTypeDef:
         """
         If no other minor versions of a service template exist, delete a major version
         of the service template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template_version)
         """
-
     def delete_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
     ) -> DeleteTemplateSyncConfigOutputTypeDef:
         """
         Delete a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_template_sync_config)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#generate_presigned_url)
         """
-
     def get_account_settings(self) -> GetAccountSettingsOutputTypeDef:
         """
         Get detail data for Proton account-wide settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_account_settings)
         """
-
     def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
-
     def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
-
     def get_environment_account_connection(
         self, *, id: str
     ) -> GetEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, get the detailed data for an environment account
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_account_connection)
         """
-
     def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputTypeDef:
         """
         Get detailed data for an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template)
         """
-
     def get_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> GetEnvironmentTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template_version)
         """
-
     def get_repository(
         self, *, name: str, provider: RepositoryProviderType
     ) -> GetRepositoryOutputTypeDef:
         """
         Get detail data for a linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository)
         """
-
     def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: Literal["TEMPLATE_SYNC"]
+        syncType: SyncTypeType
     ) -> GetRepositorySyncStatusOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository_sync_status)
         """
+    def get_resources_summary(self) -> GetResourcesSummaryOutputTypeDef:
+        """
+        Get counts of Proton resources.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_resources_summary)
+        """
     def get_service(self, *, name: str) -> GetServiceOutputTypeDef:
         """
         Get detailed data for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service)
         """
-
     def get_service_instance(
         self, *, name: str, serviceName: str
     ) -> GetServiceInstanceOutputTypeDef:
         """
         Get detailed data for a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance)
         """
+    def get_service_instance_sync_status(
+        self, *, serviceInstanceName: str, serviceName: str
+    ) -> GetServiceInstanceSyncStatusOutputTypeDef:
+        """
+        Get the status of the synced service instance.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance_sync_status)
+        """
+    def get_service_sync_blocker_summary(
+        self, *, serviceName: str, serviceInstanceName: str = ...
+    ) -> GetServiceSyncBlockerSummaryOutputTypeDef:
+        """
+        Get detailed data for the service sync blocker summary.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_blocker_summary)
+        """
+    def get_service_sync_config(self, *, serviceName: str) -> GetServiceSyncConfigOutputTypeDef:
+        """
+        Get detailed information for the service sync configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_config)
+        """
     def get_service_template(self, *, name: str) -> GetServiceTemplateOutputTypeDef:
         """
         Get detailed data for a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template)
         """
-
     def get_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> GetServiceTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template_version)
         """
-
     def get_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
     ) -> GetTemplateSyncConfigOutputTypeDef:
         """
         Get detail data for a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_config)
         """
-
     def get_template_sync_status(
         self, *, templateName: str, templateType: TemplateTypeType, templateVersion: str
     ) -> GetTemplateSyncStatusOutputTypeDef:
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
-
     def list_component_outputs(
         self, *, componentName: str, nextToken: str = ...
     ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
-
     def list_component_provisioned_resources(
         self, *, componentName: str, nextToken: str = ...
     ) -> ListComponentProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a component with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_provisioned_resources)
         """
-
     def list_components(
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
@@ -719,15 +757,14 @@
     ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
-
     def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -735,240 +772,224 @@
     ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
-
     def list_environment_outputs(
         self, *, environmentName: str, nextToken: str = ...
     ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
-
     def list_environment_provisioned_resources(
         self, *, environmentName: str, nextToken: str = ...
     ) -> ListEnvironmentProvisionedResourcesOutputTypeDef:
         """
         List the provisioned resources for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_provisioned_resources)
         """
-
     def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_template_versions)
         """
-
     def list_environment_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListEnvironmentTemplatesOutputTypeDef:
         """
         List environment templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_templates)
         """
-
     def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListEnvironmentsOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environments)
         """
-
     def list_repositories(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListRepositoriesOutputTypeDef:
         """
         List linked repositories with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repositories)
         """
-
     def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: Literal["TEMPLATE_SYNC"],
+        syncType: SyncTypeType,
         nextToken: str = ...
     ) -> ListRepositorySyncDefinitionsOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
-
     def list_service_instance_outputs(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
-
     def list_service_instance_provisioned_resources(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
     ) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service instance with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_provisioned_resources)
         """
-
     def list_service_instances(
-        self, *, maxResults: int = ..., nextToken: str = ..., serviceName: str = ...
+        self,
+        *,
+        filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        serviceName: str = ...,
+        sortBy: ListServiceInstancesSortByType = ...,
+        sortOrder: SortOrderType = ...
     ) -> ListServiceInstancesOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
-
     def list_service_pipeline_outputs(
         self, *, serviceName: str, nextToken: str = ...
     ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
-
     def list_service_pipeline_provisioned_resources(
         self, *, serviceName: str, nextToken: str = ...
     ) -> ListServicePipelineProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service and pipeline with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_provisioned_resources)
         """
-
     def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListServiceTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_template_versions)
         """
-
     def list_service_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServiceTemplatesOutputTypeDef:
         """
         List service templates with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_templates)
         """
-
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServicesOutputTypeDef:
         """
         List services with summaries of detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_services)
         """
-
     def list_tags_for_resource(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         List tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_tags_for_resource)
         """
-
     def notify_resource_deployment_status_change(
         self,
         *,
         resourceArn: str,
         deploymentId: str = ...,
         outputs: Sequence[OutputTypeDef] = ...,
         status: ResourceDeploymentStatusType = ...,
         statusMessage: str = ...
     ) -> Dict[str, Any]:
         """
-        Notify Proton of the following information related to a provisioned resource
-        (environment, service instance, or service pipeline) * For [CodeBuild-based
-        provisioning](https://docs.aws.amazon.com/proton/latest/userguide/ag-works-prov-
-        methods.html#ag-works-prov-methods-codebuild)_ , provid...
+        Notify Proton of status changes to a provisioned resource when you use self-
+        managed provisioning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#notify_resource_deployment_status_change)
         """
-
     def reject_environment_account_connection(
         self, *, id: str
     ) -> RejectEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, reject an environment account connection from another
         environment account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#reject_environment_account_connection)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tag a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Remove a customer tag from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#untag_resource)
         """
-
     def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
         pipelineServiceRoleArn: str = ...
@@ -976,33 +997,32 @@
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_account_settings)
         """
-
     def update_component(
         self,
         *,
         deploymentType: ComponentDeploymentUpdateTypeType,
         name: str,
+        clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         templateFile: str = ...
     ) -> UpdateComponentOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_component)
         """
-
     def update_environment(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
@@ -1016,15 +1036,14 @@
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment)
         """
-
     def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...
@@ -1032,25 +1051,23 @@
         """
         In an environment account, update an environment account connection to use a new
         IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_account_connection)
         """
-
     def update_environment_template(
         self, *, name: str, description: str = ..., displayName: str = ...
     ) -> UpdateEnvironmentTemplateOutputTypeDef:
         """
         Update an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template)
         """
-
     def update_environment_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
@@ -1058,42 +1075,40 @@
     ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template_version)
         """
-
     def update_service(
         self, *, name: str, description: str = ..., spec: str = ...
     ) -> UpdateServiceOutputTypeDef:
         """
         Edit a service description or use a spec to add and delete service instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service)
         """
-
     def update_service_instance(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
+        clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
     ) -> UpdateServiceInstanceOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_instance)
         """
-
     def update_service_pipeline(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
@@ -1101,25 +1116,47 @@
     ) -> UpdateServicePipelineOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_pipeline)
         """
+    def update_service_sync_blocker(
+        self, *, id: str, resolvedReason: str
+    ) -> UpdateServiceSyncBlockerOutputTypeDef:
+        """
+        Update the service sync blocker by resolving it.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_blocker)
+        """
+    def update_service_sync_config(
+        self,
+        *,
+        branch: str,
+        filePath: str,
+        repositoryName: str,
+        repositoryProvider: RepositoryProviderType,
+        serviceName: str
+    ) -> UpdateServiceSyncConfigOutputTypeDef:
+        """
+        Update the Proton Ops config file.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_config)
+        """
     def update_service_template(
         self, *, name: str, description: str = ..., displayName: str = ...
     ) -> UpdateServiceTemplateOutputTypeDef:
         """
         Update a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template)
         """
-
     def update_service_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
@@ -1129,15 +1166,14 @@
     ) -> UpdateServiceTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template_version)
         """
-
     def update_template_sync_config(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
@@ -1147,261 +1183,231 @@
         """
         Update template sync configuration parameters, except for the `templateName` and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_template_sync_config)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_component_outputs"]
     ) -> ListComponentOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_component_provisioned_resources"]
     ) -> ListComponentProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_components"]) -> ListComponentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_account_connections"]
     ) -> ListEnvironmentAccountConnectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_outputs"]
     ) -> ListEnvironmentOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_provisioned_resources"]
     ) -> ListEnvironmentProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_template_versions"]
     ) -> ListEnvironmentTemplateVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_templates"]
     ) -> ListEnvironmentTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environments"]
     ) -> ListEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_repositories"]
     ) -> ListRepositoriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_repository_sync_definitions"]
     ) -> ListRepositorySyncDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_instance_outputs"]
     ) -> ListServiceInstanceOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_instance_provisioned_resources"]
     ) -> ListServiceInstanceProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_instances"]
     ) -> ListServiceInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_pipeline_outputs"]
     ) -> ListServicePipelineOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_pipeline_provisioned_resources"]
     ) -> ListServicePipelineProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_template_versions"]
     ) -> ListServiceTemplateVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_templates"]
     ) -> ListServiceTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["component_deleted"]) -> ComponentDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["component_deployed"]) -> ComponentDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["environment_deployed"]) -> EnvironmentDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["environment_template_version_registered"]
     ) -> EnvironmentTemplateVersionRegisteredWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["service_created"]) -> ServiceCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["service_deleted"]) -> ServiceDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["service_instance_deployed"]
     ) -> ServiceInstanceDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["service_pipeline_deployed"]
     ) -> ServicePipelineDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["service_template_version_registered"]
     ) -> ServiceTemplateVersionRegisteredWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["service_updated"]) -> ServiceUpdatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/client.pyi` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,19 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ComponentDeploymentUpdateTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
+    ListServiceInstancesSortByType,
     RepositoryProviderType,
     ResourceDeploymentStatusType,
+    SortOrderType,
+    SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
@@ -59,39 +62,46 @@
     CompatibleEnvironmentTemplateInputTypeDef,
     CreateComponentOutputTypeDef,
     CreateEnvironmentAccountConnectionOutputTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateEnvironmentTemplateOutputTypeDef,
     CreateEnvironmentTemplateVersionOutputTypeDef,
     CreateRepositoryOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
     CreateServiceOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteComponentOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     DeleteEnvironmentTemplateOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     DeleteServiceOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetComponentOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     GetEnvironmentTemplateOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     GetRepositoryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
     GetServiceInstanceOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
     GetServiceOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
@@ -101,14 +111,15 @@
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListServicesOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -122,14 +133,16 @@
     UpdateEnvironmentAccountConnectionOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateEnvironmentTemplateOutputTypeDef,
     UpdateEnvironmentTemplateVersionOutputTypeDef,
     UpdateServiceInstanceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     UpdateServicePipelineOutputTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
 )
 from .waiter import (
     ComponentDeletedWaiter,
     ComponentDeployedWaiter,
@@ -144,33 +157,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ProtonClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ProtonClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/)
     """
 
     meta: ClientMeta
@@ -179,96 +196,106 @@
     def exceptions(self) -> Exceptions:
         """
         ProtonClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#exceptions)
         """
+
     def accept_environment_account_connection(
         self, *, id: str
     ) -> AcceptEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, an environment account connection request is accepted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#accept_environment_account_connection)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#can_paginate)
         """
+
     def cancel_component_deployment(
         self, *, componentName: str
     ) -> CancelComponentDeploymentOutputTypeDef:
         """
         Attempts to cancel a component deployment (for a component that is in the
         `IN_PROGRESS` deployment status).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_component_deployment)
         """
+
     def cancel_environment_deployment(
         self, *, environmentName: str
     ) -> CancelEnvironmentDeploymentOutputTypeDef:
         """
         Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
         the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_environment_deployment)
         """
+
     def cancel_service_instance_deployment(
         self, *, serviceInstanceName: str, serviceName: str
     ) -> CancelServiceInstanceDeploymentOutputTypeDef:
         """
         Attempts to cancel a service instance deployment on an  UpdateServiceInstance
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_instance_deployment)
         """
+
     def cancel_service_pipeline_deployment(
         self, *, serviceName: str
     ) -> CancelServicePipelineDeploymentOutputTypeDef:
         """
         Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_pipeline_deployment)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#close)
         """
+
     def create_component(
         self,
         *,
         manifest: str,
         name: str,
         templateFile: str,
+        clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateComponentOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_component)
         """
+
     def create_environment(
         self,
         *,
         name: str,
         spec: str,
         templateMajorVersion: str,
         templateName: str,
@@ -283,33 +310,35 @@
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment)
         """
+
     def create_environment_account_connection(
         self,
         *,
         environmentName: str,
         managementAccountId: str,
-        roleArn: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
+        roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_account_connection)
         """
+
     def create_environment_template(
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
@@ -318,14 +347,15 @@
     ) -> CreateEnvironmentTemplateOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template)
         """
+
     def create_environment_template_version(
         self,
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
@@ -334,14 +364,15 @@
     ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template_version)
         """
+
     def create_repository(
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
@@ -349,14 +380,15 @@
     ) -> CreateRepositoryOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_repository)
         """
+
     def create_service(
         self,
         *,
         name: str,
         spec: str,
         templateMajorVersion: str,
         templateName: str,
@@ -369,14 +401,49 @@
     ) -> CreateServiceOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service)
         """
+
+    def create_service_instance(
+        self,
+        *,
+        name: str,
+        serviceName: str,
+        spec: str,
+        clientToken: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+        templateMajorVersion: str = ...,
+        templateMinorVersion: str = ...
+    ) -> CreateServiceInstanceOutputTypeDef:
+        """
+        Create a service instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_instance)
+        """
+
+    def create_service_sync_config(
+        self,
+        *,
+        branch: str,
+        filePath: str,
+        repositoryName: str,
+        repositoryProvider: RepositoryProviderType,
+        serviceName: str
+    ) -> CreateServiceSyncConfigOutputTypeDef:
+        """
+        Create the Proton Ops configuration file.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_sync_config)
+        """
+
     def create_service_template(
         self,
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
@@ -385,14 +452,15 @@
     ) -> CreateServiceTemplateOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template)
         """
+
     def create_service_template_version(
         self,
         *,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef],
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
@@ -403,14 +471,15 @@
     ) -> CreateServiceTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template_version)
         """
+
     def create_template_sync_config(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
@@ -420,249 +489,323 @@
         """
         Set up a template to create new template versions automatically by tracking a
         linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_template_sync_config)
         """
+
     def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
+
     def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
+
     def delete_environment_account_connection(
         self, *, id: str
     ) -> DeleteEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, delete an environment account connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_account_connection)
         """
+
     def delete_environment_template(self, *, name: str) -> DeleteEnvironmentTemplateOutputTypeDef:
         """
         If no other major or minor versions of an environment template exist, delete the
         environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template)
         """
+
     def delete_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> DeleteEnvironmentTemplateVersionOutputTypeDef:
         """
         If no other minor versions of an environment template exist, delete a major
         version of the environment template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template_version)
         """
+
     def delete_repository(
         self, *, name: str, provider: RepositoryProviderType
     ) -> DeleteRepositoryOutputTypeDef:
         """
         De-register and unlink your repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_repository)
         """
+
     def delete_service(self, *, name: str) -> DeleteServiceOutputTypeDef:
         """
         Delete a service, with its instances and pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service)
         """
+
+    def delete_service_sync_config(
+        self, *, serviceName: str
+    ) -> DeleteServiceSyncConfigOutputTypeDef:
+        """
+        Delete the Proton Ops file.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_sync_config)
+        """
+
     def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputTypeDef:
         """
         If no other major or minor versions of the service template exist, delete the
         service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template)
         """
+
     def delete_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> DeleteServiceTemplateVersionOutputTypeDef:
         """
         If no other minor versions of a service template exist, delete a major version
         of the service template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template_version)
         """
+
     def delete_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
     ) -> DeleteTemplateSyncConfigOutputTypeDef:
         """
         Delete a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_template_sync_config)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#generate_presigned_url)
         """
+
     def get_account_settings(self) -> GetAccountSettingsOutputTypeDef:
         """
         Get detail data for Proton account-wide settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_account_settings)
         """
+
     def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
+
     def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
+
     def get_environment_account_connection(
         self, *, id: str
     ) -> GetEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, get the detailed data for an environment account
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_account_connection)
         """
+
     def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputTypeDef:
         """
         Get detailed data for an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template)
         """
+
     def get_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> GetEnvironmentTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template_version)
         """
+
     def get_repository(
         self, *, name: str, provider: RepositoryProviderType
     ) -> GetRepositoryOutputTypeDef:
         """
         Get detail data for a linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository)
         """
+
     def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: Literal["TEMPLATE_SYNC"]
+        syncType: SyncTypeType
     ) -> GetRepositorySyncStatusOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository_sync_status)
         """
+
+    def get_resources_summary(self) -> GetResourcesSummaryOutputTypeDef:
+        """
+        Get counts of Proton resources.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_resources_summary)
+        """
+
     def get_service(self, *, name: str) -> GetServiceOutputTypeDef:
         """
         Get detailed data for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service)
         """
+
     def get_service_instance(
         self, *, name: str, serviceName: str
     ) -> GetServiceInstanceOutputTypeDef:
         """
         Get detailed data for a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance)
         """
+
+    def get_service_instance_sync_status(
+        self, *, serviceInstanceName: str, serviceName: str
+    ) -> GetServiceInstanceSyncStatusOutputTypeDef:
+        """
+        Get the status of the synced service instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance_sync_status)
+        """
+
+    def get_service_sync_blocker_summary(
+        self, *, serviceName: str, serviceInstanceName: str = ...
+    ) -> GetServiceSyncBlockerSummaryOutputTypeDef:
+        """
+        Get detailed data for the service sync blocker summary.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_blocker_summary)
+        """
+
+    def get_service_sync_config(self, *, serviceName: str) -> GetServiceSyncConfigOutputTypeDef:
+        """
+        Get detailed information for the service sync configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_config)
+        """
+
     def get_service_template(self, *, name: str) -> GetServiceTemplateOutputTypeDef:
         """
         Get detailed data for a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template)
         """
+
     def get_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
     ) -> GetServiceTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template_version)
         """
+
     def get_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
     ) -> GetTemplateSyncConfigOutputTypeDef:
         """
         Get detail data for a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_config)
         """
+
     def get_template_sync_status(
         self, *, templateName: str, templateType: TemplateTypeType, templateVersion: str
     ) -> GetTemplateSyncStatusOutputTypeDef:
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
+
     def list_component_outputs(
         self, *, componentName: str, nextToken: str = ...
     ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
+
     def list_component_provisioned_resources(
         self, *, componentName: str, nextToken: str = ...
     ) -> ListComponentProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a component with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_provisioned_resources)
         """
+
     def list_components(
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
@@ -670,14 +813,15 @@
     ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
+
     def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -685,219 +829,245 @@
     ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
+
     def list_environment_outputs(
         self, *, environmentName: str, nextToken: str = ...
     ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
+
     def list_environment_provisioned_resources(
         self, *, environmentName: str, nextToken: str = ...
     ) -> ListEnvironmentProvisionedResourcesOutputTypeDef:
         """
         List the provisioned resources for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_provisioned_resources)
         """
+
     def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_template_versions)
         """
+
     def list_environment_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListEnvironmentTemplatesOutputTypeDef:
         """
         List environment templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_templates)
         """
+
     def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListEnvironmentsOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environments)
         """
+
     def list_repositories(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListRepositoriesOutputTypeDef:
         """
         List linked repositories with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repositories)
         """
+
     def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: Literal["TEMPLATE_SYNC"],
+        syncType: SyncTypeType,
         nextToken: str = ...
     ) -> ListRepositorySyncDefinitionsOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
+
     def list_service_instance_outputs(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
+
     def list_service_instance_provisioned_resources(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
     ) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service instance with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_provisioned_resources)
         """
+
     def list_service_instances(
-        self, *, maxResults: int = ..., nextToken: str = ..., serviceName: str = ...
+        self,
+        *,
+        filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        serviceName: str = ...,
+        sortBy: ListServiceInstancesSortByType = ...,
+        sortOrder: SortOrderType = ...
     ) -> ListServiceInstancesOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
+
     def list_service_pipeline_outputs(
         self, *, serviceName: str, nextToken: str = ...
     ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
+
     def list_service_pipeline_provisioned_resources(
         self, *, serviceName: str, nextToken: str = ...
     ) -> ListServicePipelineProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service and pipeline with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_provisioned_resources)
         """
+
     def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListServiceTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_template_versions)
         """
+
     def list_service_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServiceTemplatesOutputTypeDef:
         """
         List service templates with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_templates)
         """
+
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServicesOutputTypeDef:
         """
         List services with summaries of detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_services)
         """
+
     def list_tags_for_resource(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         List tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_tags_for_resource)
         """
+
     def notify_resource_deployment_status_change(
         self,
         *,
         resourceArn: str,
         deploymentId: str = ...,
         outputs: Sequence[OutputTypeDef] = ...,
         status: ResourceDeploymentStatusType = ...,
         statusMessage: str = ...
     ) -> Dict[str, Any]:
         """
-        Notify Proton of the following information related to a provisioned resource
-        (environment, service instance, or service pipeline) * For [CodeBuild-based
-        provisioning](https://docs.aws.amazon.com/proton/latest/userguide/ag-works-prov-
-        methods.html#ag-works-prov-methods-codebuild)_ , provid...
+        Notify Proton of status changes to a provisioned resource when you use self-
+        managed provisioning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#notify_resource_deployment_status_change)
         """
+
     def reject_environment_account_connection(
         self, *, id: str
     ) -> RejectEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, reject an environment account connection from another
         environment account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#reject_environment_account_connection)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tag a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Remove a customer tag from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#untag_resource)
         """
+
     def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
         pipelineServiceRoleArn: str = ...
@@ -905,31 +1075,34 @@
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_account_settings)
         """
+
     def update_component(
         self,
         *,
         deploymentType: ComponentDeploymentUpdateTypeType,
         name: str,
+        clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         templateFile: str = ...
     ) -> UpdateComponentOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_component)
         """
+
     def update_environment(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
@@ -943,14 +1116,15 @@
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment)
         """
+
     def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...
@@ -958,23 +1132,25 @@
         """
         In an environment account, update an environment account connection to use a new
         IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_account_connection)
         """
+
     def update_environment_template(
         self, *, name: str, description: str = ..., displayName: str = ...
     ) -> UpdateEnvironmentTemplateOutputTypeDef:
         """
         Update an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template)
         """
+
     def update_environment_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
@@ -982,39 +1158,43 @@
     ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template_version)
         """
+
     def update_service(
         self, *, name: str, description: str = ..., spec: str = ...
     ) -> UpdateServiceOutputTypeDef:
         """
         Edit a service description or use a spec to add and delete service instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service)
         """
+
     def update_service_instance(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
+        clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
     ) -> UpdateServiceInstanceOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_instance)
         """
+
     def update_service_pipeline(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
@@ -1022,23 +1202,51 @@
     ) -> UpdateServicePipelineOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_pipeline)
         """
+
+    def update_service_sync_blocker(
+        self, *, id: str, resolvedReason: str
+    ) -> UpdateServiceSyncBlockerOutputTypeDef:
+        """
+        Update the service sync blocker by resolving it.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_blocker)
+        """
+
+    def update_service_sync_config(
+        self,
+        *,
+        branch: str,
+        filePath: str,
+        repositoryName: str,
+        repositoryProvider: RepositoryProviderType,
+        serviceName: str
+    ) -> UpdateServiceSyncConfigOutputTypeDef:
+        """
+        Update the Proton Ops config file.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_config)
+        """
+
     def update_service_template(
         self, *, name: str, description: str = ..., displayName: str = ...
     ) -> UpdateServiceTemplateOutputTypeDef:
         """
         Update a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template)
         """
+
     def update_service_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
@@ -1048,14 +1256,15 @@
     ) -> UpdateServiceTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template_version)
         """
+
     def update_template_sync_config(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
@@ -1065,231 +1274,261 @@
         """
         Update template sync configuration parameters, except for the `templateName` and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_template_sync_config)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_component_outputs"]
     ) -> ListComponentOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_component_provisioned_resources"]
     ) -> ListComponentProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_components"]) -> ListComponentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_account_connections"]
     ) -> ListEnvironmentAccountConnectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_outputs"]
     ) -> ListEnvironmentOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_provisioned_resources"]
     ) -> ListEnvironmentProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_template_versions"]
     ) -> ListEnvironmentTemplateVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_templates"]
     ) -> ListEnvironmentTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environments"]
     ) -> ListEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_repositories"]
     ) -> ListRepositoriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_repository_sync_definitions"]
     ) -> ListRepositorySyncDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_instance_outputs"]
     ) -> ListServiceInstanceOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_instance_provisioned_resources"]
     ) -> ListServiceInstanceProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_instances"]
     ) -> ListServiceInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_pipeline_outputs"]
     ) -> ListServicePipelineOutputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_pipeline_provisioned_resources"]
     ) -> ListServicePipelineProvisionedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_template_versions"]
     ) -> ListServiceTemplateVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_templates"]
     ) -> ListServiceTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["component_deleted"]) -> ComponentDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["component_deployed"]) -> ComponentDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["environment_deployed"]) -> EnvironmentDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["environment_template_version_registered"]
     ) -> EnvironmentTemplateVersionRegisteredWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["service_created"]) -> ServiceCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["service_deleted"]) -> ServiceDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["service_instance_deployed"]
     ) -> ServiceInstanceDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["service_pipeline_deployed"]
     ) -> ServicePipelineDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["service_template_version_registered"]
     ) -> ServiceTemplateVersionRegisteredWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["service_updated"]) -> ServiceUpdatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/literals.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Type annotations for proton service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_proton.literals import ComponentDeletedWaiterName
+    from mypy_boto3_proton.literals import BlockerStatusType
 
-    data: ComponentDeletedWaiterName = "component_deleted"
+    data: BlockerStatusType = "ACTIVE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "BlockerStatusType",
+    "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
     "DeploymentUpdateTypeType",
     "EnvironmentAccountConnectionRequesterAccountTypeType",
     "EnvironmentAccountConnectionStatusType",
@@ -38,15 +40,17 @@
     "ListEnvironmentTemplateVersionsPaginatorName",
     "ListEnvironmentTemplatesPaginatorName",
     "ListEnvironmentsPaginatorName",
     "ListRepositoriesPaginatorName",
     "ListRepositorySyncDefinitionsPaginatorName",
     "ListServiceInstanceOutputsPaginatorName",
     "ListServiceInstanceProvisionedResourcesPaginatorName",
+    "ListServiceInstancesFilterByType",
     "ListServiceInstancesPaginatorName",
+    "ListServiceInstancesSortByType",
     "ListServicePipelineOutputsPaginatorName",
     "ListServicePipelineProvisionedResourcesPaginatorName",
     "ListServiceTemplateVersionsPaginatorName",
     "ListServiceTemplatesPaginatorName",
     "ListServicesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "ProvisionedResourceEngineType",
@@ -59,26 +63,29 @@
     "ServiceDeletedWaiterName",
     "ServiceInstanceDeployedWaiterName",
     "ServicePipelineDeployedWaiterName",
     "ServiceStatusType",
     "ServiceTemplateSupportedComponentSourceTypeType",
     "ServiceTemplateVersionRegisteredWaiterName",
     "ServiceUpdatedWaiterName",
+    "SortOrderType",
     "SyncTypeType",
     "TemplateTypeType",
     "TemplateVersionStatusType",
     "ProtonServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 
+BlockerStatusType = Literal["ACTIVE", "RESOLVED"]
+BlockerTypeType = Literal["AUTOMATED"]
 ComponentDeletedWaiterName = Literal["component_deleted"]
 ComponentDeployedWaiterName = Literal["component_deployed"]
 ComponentDeploymentUpdateTypeType = Literal["CURRENT_VERSION", "NONE"]
 DeploymentStatusType = Literal[
     "CANCELLED",
     "CANCELLING",
     "DELETE_COMPLETE",
@@ -106,15 +113,36 @@
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
 ListRepositorySyncDefinitionsPaginatorName = Literal["list_repository_sync_definitions"]
 ListServiceInstanceOutputsPaginatorName = Literal["list_service_instance_outputs"]
 ListServiceInstanceProvisionedResourcesPaginatorName = Literal[
     "list_service_instance_provisioned_resources"
 ]
+ListServiceInstancesFilterByType = Literal[
+    "createdAtAfter",
+    "createdAtBefore",
+    "deployedTemplateVersionStatus",
+    "deploymentStatus",
+    "environmentName",
+    "lastDeploymentAttemptedAtAfter",
+    "lastDeploymentAttemptedAtBefore",
+    "name",
+    "serviceName",
+    "templateName",
+]
 ListServiceInstancesPaginatorName = Literal["list_service_instances"]
+ListServiceInstancesSortByType = Literal[
+    "createdAt",
+    "deploymentStatus",
+    "environmentName",
+    "lastDeploymentAttemptedAt",
+    "name",
+    "serviceName",
+    "templateName",
+]
 ListServicePipelineOutputsPaginatorName = Literal["list_service_pipeline_outputs"]
 ListServicePipelineProvisionedResourcesPaginatorName = Literal[
     "list_service_pipeline_provisioned_resources"
 ]
 ListServiceTemplateVersionsPaginatorName = Literal["list_service_template_versions"]
 ListServiceTemplatesPaginatorName = Literal["list_service_templates"]
 ListServicesPaginatorName = Literal["list_services"]
@@ -144,15 +172,16 @@
     "UPDATE_FAILED_CLEANUP_FAILED",
     "UPDATE_FAILED_CLEANUP_IN_PROGRESS",
     "UPDATE_IN_PROGRESS",
 ]
 ServiceTemplateSupportedComponentSourceTypeType = Literal["DIRECTLY_DEFINED"]
 ServiceTemplateVersionRegisteredWaiterName = Literal["service_template_version_registered"]
 ServiceUpdatedWaiterName = Literal["service_updated"]
-SyncTypeType = Literal["TEMPLATE_SYNC"]
+SortOrderType = Literal["ASCENDING", "DESCENDING"]
+SyncTypeType = Literal["SERVICE_SYNC", "TEMPLATE_SYNC"]
 TemplateTypeType = Literal["ENVIRONMENT", "SERVICE"]
 TemplateVersionStatusType = Literal[
     "DRAFT", "PUBLISHED", "REGISTRATION_FAILED", "REGISTRATION_IN_PROGRESS"
 ]
 ProtonServiceName = Literal["proton"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -165,23 +194,25 @@
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
@@ -191,30 +222,35 @@
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
@@ -240,14 +276,15 @@
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
@@ -292,51 +329,57 @@
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
@@ -349,14 +392,15 @@
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
@@ -368,28 +412,35 @@
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
@@ -417,56 +468,64 @@
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
@@ -518,8 +577,20 @@
     "service_created",
     "service_deleted",
     "service_instance_deployed",
     "service_pipeline_deployed",
     "service_template_version_registered",
     "service_updated",
 ]
-RegionName = Literal["ap-northeast-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-west-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/literals.pyi` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 Type annotations for proton service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_proton.literals import ComponentDeletedWaiterName
+    from mypy_boto3_proton.literals import BlockerStatusType
 
-    data: ComponentDeletedWaiterName = "component_deleted"
+    data: BlockerStatusType = "ACTIVE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "BlockerStatusType",
+    "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
     "DeploymentUpdateTypeType",
     "EnvironmentAccountConnectionRequesterAccountTypeType",
     "EnvironmentAccountConnectionStatusType",
@@ -37,15 +39,17 @@
     "ListEnvironmentTemplateVersionsPaginatorName",
     "ListEnvironmentTemplatesPaginatorName",
     "ListEnvironmentsPaginatorName",
     "ListRepositoriesPaginatorName",
     "ListRepositorySyncDefinitionsPaginatorName",
     "ListServiceInstanceOutputsPaginatorName",
     "ListServiceInstanceProvisionedResourcesPaginatorName",
+    "ListServiceInstancesFilterByType",
     "ListServiceInstancesPaginatorName",
+    "ListServiceInstancesSortByType",
     "ListServicePipelineOutputsPaginatorName",
     "ListServicePipelineProvisionedResourcesPaginatorName",
     "ListServiceTemplateVersionsPaginatorName",
     "ListServiceTemplatesPaginatorName",
     "ListServicesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "ProvisionedResourceEngineType",
@@ -58,25 +62,28 @@
     "ServiceDeletedWaiterName",
     "ServiceInstanceDeployedWaiterName",
     "ServicePipelineDeployedWaiterName",
     "ServiceStatusType",
     "ServiceTemplateSupportedComponentSourceTypeType",
     "ServiceTemplateVersionRegisteredWaiterName",
     "ServiceUpdatedWaiterName",
+    "SortOrderType",
     "SyncTypeType",
     "TemplateTypeType",
     "TemplateVersionStatusType",
     "ProtonServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+BlockerStatusType = Literal["ACTIVE", "RESOLVED"]
+BlockerTypeType = Literal["AUTOMATED"]
 ComponentDeletedWaiterName = Literal["component_deleted"]
 ComponentDeployedWaiterName = Literal["component_deployed"]
 ComponentDeploymentUpdateTypeType = Literal["CURRENT_VERSION", "NONE"]
 DeploymentStatusType = Literal[
     "CANCELLED",
     "CANCELLING",
     "DELETE_COMPLETE",
@@ -104,15 +111,36 @@
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
 ListRepositorySyncDefinitionsPaginatorName = Literal["list_repository_sync_definitions"]
 ListServiceInstanceOutputsPaginatorName = Literal["list_service_instance_outputs"]
 ListServiceInstanceProvisionedResourcesPaginatorName = Literal[
     "list_service_instance_provisioned_resources"
 ]
+ListServiceInstancesFilterByType = Literal[
+    "createdAtAfter",
+    "createdAtBefore",
+    "deployedTemplateVersionStatus",
+    "deploymentStatus",
+    "environmentName",
+    "lastDeploymentAttemptedAtAfter",
+    "lastDeploymentAttemptedAtBefore",
+    "name",
+    "serviceName",
+    "templateName",
+]
 ListServiceInstancesPaginatorName = Literal["list_service_instances"]
+ListServiceInstancesSortByType = Literal[
+    "createdAt",
+    "deploymentStatus",
+    "environmentName",
+    "lastDeploymentAttemptedAt",
+    "name",
+    "serviceName",
+    "templateName",
+]
 ListServicePipelineOutputsPaginatorName = Literal["list_service_pipeline_outputs"]
 ListServicePipelineProvisionedResourcesPaginatorName = Literal[
     "list_service_pipeline_provisioned_resources"
 ]
 ListServiceTemplateVersionsPaginatorName = Literal["list_service_template_versions"]
 ListServiceTemplatesPaginatorName = Literal["list_service_templates"]
 ListServicesPaginatorName = Literal["list_services"]
@@ -142,15 +170,16 @@
     "UPDATE_FAILED_CLEANUP_FAILED",
     "UPDATE_FAILED_CLEANUP_IN_PROGRESS",
     "UPDATE_IN_PROGRESS",
 ]
 ServiceTemplateSupportedComponentSourceTypeType = Literal["DIRECTLY_DEFINED"]
 ServiceTemplateVersionRegisteredWaiterName = Literal["service_template_version_registered"]
 ServiceUpdatedWaiterName = Literal["service_updated"]
-SyncTypeType = Literal["TEMPLATE_SYNC"]
+SortOrderType = Literal["ASCENDING", "DESCENDING"]
+SyncTypeType = Literal["SERVICE_SYNC", "TEMPLATE_SYNC"]
 TemplateTypeType = Literal["ENVIRONMENT", "SERVICE"]
 TemplateVersionStatusType = Literal[
     "DRAFT", "PUBLISHED", "REGISTRATION_FAILED", "REGISTRATION_IN_PROGRESS"
 ]
 ProtonServiceName = Literal["proton"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -163,23 +192,25 @@
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
@@ -189,30 +220,35 @@
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
@@ -238,14 +274,15 @@
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
@@ -290,51 +327,57 @@
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
@@ -347,14 +390,15 @@
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
@@ -366,28 +410,35 @@
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
@@ -415,56 +466,64 @@
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
@@ -516,8 +575,20 @@
     "service_created",
     "service_deleted",
     "service_instance_deployed",
     "service_pipeline_deployed",
     "service_template_version_registered",
     "service_updated",
 ]
-RegionName = Literal["ap-northeast-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-west-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/paginator.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,25 @@
     list_service_pipeline_provisioned_resources_paginator: ListServicePipelineProvisionedResourcesPaginator = client.get_paginator("list_service_pipeline_provisioned_resources")
     list_service_template_versions_paginator: ListServiceTemplateVersionsPaginator = client.get_paginator("list_service_template_versions")
     list_service_templates_paginator: ListServiceTemplatesPaginator = client.get_paginator("list_service_templates")
     list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
-import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
+    ListServiceInstancesSortByType,
     RepositoryProviderType,
+    SortOrderType,
+    SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
@@ -78,30 +80,25 @@
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListServicesOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
-
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
@@ -117,350 +114,334 @@
     "ListServicePipelineProvisionedResourcesPaginator",
     "ListServiceTemplateVersionsPaginator",
     "ListServiceTemplatesPaginator",
     "ListServicesPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListComponentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
-
 class ListComponentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
         """
 
-
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
-
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
-
 class ListEnvironmentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
-
 class ListEnvironmentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
         """
 
-
 class ListEnvironmentTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
-
 class ListEnvironmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
         """
 
-
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
         """
 
-
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
         """
 
-
 class ListRepositorySyncDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: Literal["TEMPLATE_SYNC"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        syncType: SyncTypeType,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
-
 class ListServiceInstanceOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
-
 class ListServiceInstanceProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
-
 class ListServiceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
     """
 
     def paginate(
-        self, *, serviceName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
+        serviceName: str = ...,
+        sortBy: ListServiceInstancesSortByType = ...,
+        sortOrder: SortOrderType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
         """
 
-
 class ListServicePipelineOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
-
 class ListServicePipelineProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
         """
 
-
 class ListServiceTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
         """
 
-
 class ListServiceTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
         """
 
-
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/paginator.pyi` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,23 +53,25 @@
     list_service_pipeline_provisioned_resources_paginator: ListServicePipelineProvisionedResourcesPaginator = client.get_paginator("list_service_pipeline_provisioned_resources")
     list_service_template_versions_paginator: ListServiceTemplateVersionsPaginator = client.get_paginator("list_service_template_versions")
     list_service_templates_paginator: ListServiceTemplatesPaginator = client.get_paginator("list_service_templates")
     list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
-import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
+    ListServiceInstancesSortByType,
     RepositoryProviderType,
+    SortOrderType,
+    SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
@@ -78,29 +80,25 @@
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListServicesOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
@@ -116,328 +114,356 @@
     "ListServicePipelineProvisionedResourcesPaginator",
     "ListServiceTemplateVersionsPaginator",
     "ListServiceTemplatesPaginator",
     "ListServicesPaginator",
     "ListTagsForResourcePaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListComponentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
+
 class ListComponentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
         """
 
+
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
+
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
+
 class ListEnvironmentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
+
 class ListEnvironmentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
         """
 
+
 class ListEnvironmentTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
+
 class ListEnvironmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
         """
 
+
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
         """
 
+
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
         """
 
+
 class ListRepositorySyncDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
-        syncType: Literal["TEMPLATE_SYNC"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        syncType: SyncTypeType,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
+
 class ListServiceInstanceOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
+
 class ListServiceInstanceProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
+
 class ListServiceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
     """
 
     def paginate(
-        self, *, serviceName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
+        serviceName: str = ...,
+        sortBy: ListServiceInstancesSortByType = ...,
+        sortOrder: SortOrderType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
         """
 
+
 class ListServicePipelineOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
+
 class ListServicePipelineProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
         """
 
+
 class ListServiceTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
         """
 
+
 class ListServiceTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
         """
 
+
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/type_defs.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -12,69 +12,76 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
+    BlockerStatusType,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
+    ListServiceInstancesFilterByType,
+    ListServiceInstancesSortByType,
     ProvisionedResourceEngineType,
     RepositoryProviderType,
     RepositorySyncStatusType,
     ResourceDeploymentStatusType,
     ResourceSyncStatusType,
     ServiceStatusType,
+    SortOrderType,
+    SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     "EnvironmentAccountConnectionTypeDef",
-    "ResponseMetadataTypeDef",
     "RepositoryBranchTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
     "ComponentTypeDef",
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
     "CompatibleEnvironmentTemplateTypeDef",
     "ComponentSummaryTypeDef",
+    "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
     "EnvironmentTemplateTypeDef",
     "EnvironmentTemplateVersionTypeDef",
     "RepositoryTypeDef",
+    "CreateServiceSyncConfigInputRequestTypeDef",
+    "ServiceSyncConfigTypeDef",
     "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
     "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
+    "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     "EnvironmentAccountConnectionSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
     "EnvironmentTemplateSummaryTypeDef",
@@ -85,59 +92,84 @@
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
     "GetServiceInstanceInputRequestTypeDef",
+    "GetServiceInstanceSyncStatusInputRequestTypeDef",
+    "RevisionTypeDef",
+    "GetServiceSyncBlockerSummaryInputRequestTypeDef",
+    "GetServiceSyncConfigInputRequestTypeDef",
     "GetServiceTemplateInputRequestTypeDef",
     "GetServiceTemplateVersionInputRequestTypeDef",
     "GetTemplateSyncConfigInputRequestTypeDef",
     "GetTemplateSyncStatusInputRequestTypeDef",
-    "RevisionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
     "OutputTypeDef",
+    "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
     "ProvisionedResourceTypeDef",
+    "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
+    "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     "ListEnvironmentOutputsInputRequestTypeDef",
+    "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
+    "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
+    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositorySummaryTypeDef",
+    "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
     "ListRepositorySyncDefinitionsInputRequestTypeDef",
     "RepositorySyncDefinitionTypeDef",
+    "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     "ListServiceInstanceOutputsInputRequestTypeDef",
+    "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
     "ListServiceInstanceProvisionedResourcesInputRequestTypeDef",
-    "ListServiceInstancesInputRequestTypeDef",
+    "ListServiceInstancesFilterTypeDef",
     "ServiceInstanceSummaryTypeDef",
+    "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     "ListServicePipelineOutputsInputRequestTypeDef",
+    "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
     "ListServicePipelineProvisionedResourcesInputRequestTypeDef",
+    "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
     "ListServiceTemplateVersionsInputRequestTypeDef",
     "ServiceTemplateVersionSummaryTypeDef",
+    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     "ListServiceTemplatesInputRequestTypeDef",
     "ServiceTemplateSummaryTypeDef",
+    "ListServicesInputListServicesPaginateTypeDef",
     "ListServicesInputRequestTypeDef",
     "ServiceSummaryTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     "RepositorySyncEventTypeDef",
     "ResourceSyncEventTypeDef",
+    "ResponseMetadataTypeDef",
     "S3ObjectSourceTypeDef",
+    "SyncBlockerContextTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateComponentInputRequestTypeDef",
     "UpdateEnvironmentAccountConnectionInputRequestTypeDef",
     "UpdateEnvironmentTemplateInputRequestTypeDef",
     "UpdateEnvironmentTemplateVersionInputRequestTypeDef",
     "UpdateServiceInputRequestTypeDef",
     "UpdateServiceInstanceInputRequestTypeDef",
     "UpdateServicePipelineInputRequestTypeDef",
+    "UpdateServiceSyncBlockerInputRequestTypeDef",
+    "UpdateServiceSyncConfigInputRequestTypeDef",
     "UpdateServiceTemplateInputRequestTypeDef",
     "UpdateTemplateSyncConfigInputRequestTypeDef",
     "AcceptEnvironmentAccountConnectionOutputTypeDef",
     "CreateEnvironmentAccountConnectionOutputTypeDef",
     "DeleteEnvironmentAccountConnectionOutputTypeDef",
     "GetEnvironmentAccountConnectionOutputTypeDef",
     "RejectEnvironmentAccountConnectionOutputTypeDef",
@@ -146,27 +178,30 @@
     "EnvironmentTypeDef",
     "CancelComponentDeploymentOutputTypeDef",
     "CreateComponentOutputTypeDef",
     "DeleteComponentOutputTypeDef",
     "GetComponentOutputTypeDef",
     "UpdateComponentOutputTypeDef",
     "CancelServiceInstanceDeploymentOutputTypeDef",
+    "CreateServiceInstanceOutputTypeDef",
     "GetServiceInstanceOutputTypeDef",
     "UpdateServiceInstanceOutputTypeDef",
     "CancelServicePipelineDeploymentOutputTypeDef",
     "ServiceTypeDef",
     "UpdateServicePipelineOutputTypeDef",
     "UpdateServiceTemplateVersionInputRequestTypeDef",
     "ServiceTemplateVersionTypeDef",
     "ListComponentsOutputTypeDef",
+    "CountsSummaryTypeDef",
     "CreateComponentInputRequestTypeDef",
     "CreateEnvironmentAccountConnectionInputRequestTypeDef",
     "CreateEnvironmentTemplateInputRequestTypeDef",
     "CreateRepositoryInputRequestTypeDef",
     "CreateServiceInputRequestTypeDef",
+    "CreateServiceInstanceInputRequestTypeDef",
     "CreateServiceTemplateInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "CreateEnvironmentTemplateOutputTypeDef",
@@ -176,75 +211,63 @@
     "CreateEnvironmentTemplateVersionOutputTypeDef",
     "DeleteEnvironmentTemplateVersionOutputTypeDef",
     "GetEnvironmentTemplateVersionOutputTypeDef",
     "UpdateEnvironmentTemplateVersionOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "DeleteRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
+    "CreateServiceSyncConfigOutputTypeDef",
+    "DeleteServiceSyncConfigOutputTypeDef",
+    "GetServiceSyncConfigOutputTypeDef",
+    "UpdateServiceSyncConfigOutputTypeDef",
     "CreateServiceTemplateOutputTypeDef",
     "DeleteServiceTemplateOutputTypeDef",
     "GetServiceTemplateOutputTypeDef",
     "UpdateServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigOutputTypeDef",
     "DeleteTemplateSyncConfigOutputTypeDef",
     "GetTemplateSyncConfigOutputTypeDef",
     "UpdateTemplateSyncConfigOutputTypeDef",
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     "ListEnvironmentsOutputTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListEnvironmentTemplatesOutputTypeDef",
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
     "GetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     "GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     "GetServiceInputServiceCreatedWaitTypeDef",
     "GetServiceInputServiceDeletedWaitTypeDef",
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
-    "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
-    "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
-    "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
-    "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
-    "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
-    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
-    "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
-    "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
-    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
-    "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
-    "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
-    "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
-    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
-    "ListServicesInputListServicesPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListComponentOutputsOutputTypeDef",
     "ListEnvironmentOutputsOutputTypeDef",
     "ListServiceInstanceOutputsOutputTypeDef",
     "ListServicePipelineOutputsOutputTypeDef",
     "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
     "ListComponentProvisionedResourcesOutputTypeDef",
     "ListEnvironmentProvisionedResourcesOutputTypeDef",
     "ListServiceInstanceProvisionedResourcesOutputTypeDef",
     "ListServicePipelineProvisionedResourcesOutputTypeDef",
     "ListRepositoriesOutputTypeDef",
     "ListRepositorySyncDefinitionsOutputTypeDef",
+    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
+    "ListServiceInstancesInputRequestTypeDef",
     "ListServiceInstancesOutputTypeDef",
     "ListServiceTemplateVersionsOutputTypeDef",
     "ListServiceTemplatesOutputTypeDef",
     "ListServicesOutputTypeDef",
     "RepositorySyncAttemptTypeDef",
     "ResourceSyncAttemptTypeDef",
     "TemplateVersionSourceInputTypeDef",
+    "SyncBlockerTypeDef",
     "GetAccountSettingsOutputTypeDef",
     "UpdateAccountSettingsOutputTypeDef",
     "CancelEnvironmentDeploymentOutputTypeDef",
     "CreateEnvironmentOutputTypeDef",
     "DeleteEnvironmentOutputTypeDef",
     "GetEnvironmentOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
@@ -252,18 +275,23 @@
     "DeleteServiceOutputTypeDef",
     "GetServiceOutputTypeDef",
     "UpdateServiceOutputTypeDef",
     "CreateServiceTemplateVersionOutputTypeDef",
     "DeleteServiceTemplateVersionOutputTypeDef",
     "GetServiceTemplateVersionOutputTypeDef",
     "UpdateServiceTemplateVersionOutputTypeDef",
+    "GetResourcesSummaryOutputTypeDef",
     "GetRepositorySyncStatusOutputTypeDef",
+    "GetServiceInstanceSyncStatusOutputTypeDef",
     "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
+    "ServiceSyncBlockerSummaryTypeDef",
+    "UpdateServiceSyncBlockerOutputTypeDef",
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
@@ -288,32 +316,19 @@
     {
         "codebuildRoleArn": str,
         "componentRoleArn": str,
     },
     total=False,
 )
 
-
 class EnvironmentAccountConnectionTypeDef(
     _RequiredEnvironmentAccountConnectionTypeDef, _OptionalEnvironmentAccountConnectionTypeDef
 ):
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
 RepositoryBranchTypeDef = TypedDict(
     "RepositoryBranchTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
@@ -339,28 +354,27 @@
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "deploymentStatusMessage": str,
         "description": str,
+        "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
     },
     total=False,
 )
 
-
 class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
-
 CancelEnvironmentDeploymentInputRequestTypeDef = TypedDict(
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
 
@@ -388,24 +402,23 @@
         "templateName": str,
     },
 )
 _OptionalServiceInstanceTypeDef = TypedDict(
     "_OptionalServiceInstanceTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastClientRequestToken": str,
         "spec": str,
     },
     total=False,
 )
 
-
 class ServiceInstanceTypeDef(_RequiredServiceInstanceTypeDef, _OptionalServiceInstanceTypeDef):
     pass
 
-
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -427,19 +440,17 @@
     {
         "deploymentStatusMessage": str,
         "spec": str,
     },
     total=False,
 )
 
-
 class ServicePipelineTypeDef(_RequiredServicePipelineTypeDef, _OptionalServicePipelineTypeDef):
     pass
 
-
 CompatibleEnvironmentTemplateInputTypeDef = TypedDict(
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
@@ -471,18 +482,38 @@
         "lastDeploymentSucceededAt": datetime,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
-
 class ComponentSummaryTypeDef(_RequiredComponentSummaryTypeDef, _OptionalComponentSummaryTypeDef):
     pass
 
+_RequiredResourceCountsSummaryTypeDef = TypedDict(
+    "_RequiredResourceCountsSummaryTypeDef",
+    {
+        "total": int,
+    },
+)
+_OptionalResourceCountsSummaryTypeDef = TypedDict(
+    "_OptionalResourceCountsSummaryTypeDef",
+    {
+        "behindMajor": int,
+        "behindMinor": int,
+        "failed": int,
+        "upToDate": int,
+    },
+    total=False,
+)
+
+class ResourceCountsSummaryTypeDef(
+    _RequiredResourceCountsSummaryTypeDef, _OptionalResourceCountsSummaryTypeDef
+):
+    pass
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
@@ -514,21 +545,19 @@
         "encryptionKey": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
-
 class EnvironmentTemplateTypeDef(
     _RequiredEnvironmentTemplateTypeDef, _OptionalEnvironmentTemplateTypeDef
 ):
     pass
 
-
 _RequiredEnvironmentTemplateVersionTypeDef = TypedDict(
     "_RequiredEnvironmentTemplateVersionTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "majorVersion": str,
@@ -544,21 +573,19 @@
         "recommendedMinorVersion": str,
         "schema": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class EnvironmentTemplateVersionTypeDef(
     _RequiredEnvironmentTemplateVersionTypeDef, _OptionalEnvironmentTemplateVersionTypeDef
 ):
     pass
 
-
 _RequiredRepositoryTypeDef = TypedDict(
     "_RequiredRepositoryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
@@ -568,18 +595,38 @@
     "_OptionalRepositoryTypeDef",
     {
         "encryptionKey": str,
     },
     total=False,
 )
 
-
 class RepositoryTypeDef(_RequiredRepositoryTypeDef, _OptionalRepositoryTypeDef):
     pass
 
+CreateServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "CreateServiceSyncConfigInputRequestTypeDef",
+    {
+        "branch": str,
+        "filePath": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "serviceName": str,
+    },
+)
+
+ServiceSyncConfigTypeDef = TypedDict(
+    "ServiceSyncConfigTypeDef",
+    {
+        "branch": str,
+        "filePath": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "serviceName": str,
+    },
+)
 
 _RequiredServiceTemplateTypeDef = TypedDict(
     "_RequiredServiceTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
@@ -594,19 +641,17 @@
         "encryptionKey": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
-
 class ServiceTemplateTypeDef(_RequiredServiceTemplateTypeDef, _OptionalServiceTemplateTypeDef):
     pass
 
-
 _RequiredCreateTemplateSyncConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateTemplateSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -617,22 +662,20 @@
     "_OptionalCreateTemplateSyncConfigInputRequestTypeDef",
     {
         "subdirectory": str,
     },
     total=False,
 )
 
-
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredTemplateSyncConfigTypeDef = TypedDict(
     "_RequiredTemplateSyncConfigTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -643,21 +686,19 @@
     "_OptionalTemplateSyncConfigTypeDef",
     {
         "subdirectory": str,
     },
     total=False,
 )
 
-
 class TemplateSyncConfigTypeDef(
     _RequiredTemplateSyncConfigTypeDef, _OptionalTemplateSyncConfigTypeDef
 ):
     pass
 
-
 DeleteComponentInputRequestTypeDef = TypedDict(
     "DeleteComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -702,14 +743,21 @@
 DeleteServiceInputRequestTypeDef = TypedDict(
     "DeleteServiceInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "DeleteServiceSyncConfigInputRequestTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+
 DeleteServiceTemplateInputRequestTypeDef = TypedDict(
     "DeleteServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -748,22 +796,20 @@
     "_OptionalEnvironmentAccountConnectionSummaryTypeDef",
     {
         "componentRoleArn": str,
     },
     total=False,
 )
 
-
 class EnvironmentAccountConnectionSummaryTypeDef(
     _RequiredEnvironmentAccountConnectionSummaryTypeDef,
     _OptionalEnvironmentAccountConnectionSummaryTypeDef,
 ):
     pass
 
-
 _RequiredEnvironmentSummaryTypeDef = TypedDict(
     "_RequiredEnvironmentSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "lastDeploymentAttemptedAt": datetime,
@@ -784,21 +830,19 @@
         "environmentAccountId": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
     },
     total=False,
 )
 
-
 class EnvironmentSummaryTypeDef(
     _RequiredEnvironmentSummaryTypeDef, _OptionalEnvironmentSummaryTypeDef
 ):
     pass
 
-
 EnvironmentTemplateFilterTypeDef = TypedDict(
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
@@ -819,21 +863,19 @@
         "displayName": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
-
 class EnvironmentTemplateSummaryTypeDef(
     _RequiredEnvironmentTemplateSummaryTypeDef, _OptionalEnvironmentTemplateSummaryTypeDef
 ):
     pass
 
-
 _RequiredEnvironmentTemplateVersionSummaryTypeDef = TypedDict(
     "_RequiredEnvironmentTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "majorVersion": str,
@@ -848,22 +890,20 @@
         "description": str,
         "recommendedMinorVersion": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class EnvironmentTemplateVersionSummaryTypeDef(
     _RequiredEnvironmentTemplateVersionSummaryTypeDef,
     _OptionalEnvironmentTemplateVersionSummaryTypeDef,
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -916,15 +956,15 @@
 
 GetRepositorySyncStatusInputRequestTypeDef = TypedDict(
     "GetRepositorySyncStatusInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
-        "syncType": Literal["TEMPLATE_SYNC"],
+        "syncType": SyncTypeType,
     },
 )
 
 GetServiceInputRequestTypeDef = TypedDict(
     "GetServiceInputRequestTypeDef",
     {
         "name": str,
@@ -935,14 +975,60 @@
     "GetServiceInstanceInputRequestTypeDef",
     {
         "name": str,
         "serviceName": str,
     },
 )
 
+GetServiceInstanceSyncStatusInputRequestTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusInputRequestTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+)
+
+RevisionTypeDef = TypedDict(
+    "RevisionTypeDef",
+    {
+        "branch": str,
+        "directory": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "sha": str,
+    },
+)
+
+_RequiredGetServiceSyncBlockerSummaryInputRequestTypeDef = TypedDict(
+    "_RequiredGetServiceSyncBlockerSummaryInputRequestTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalGetServiceSyncBlockerSummaryInputRequestTypeDef = TypedDict(
+    "_OptionalGetServiceSyncBlockerSummaryInputRequestTypeDef",
+    {
+        "serviceInstanceName": str,
+    },
+    total=False,
+)
+
+class GetServiceSyncBlockerSummaryInputRequestTypeDef(
+    _RequiredGetServiceSyncBlockerSummaryInputRequestTypeDef,
+    _OptionalGetServiceSyncBlockerSummaryInputRequestTypeDef,
+):
+    pass
+
+GetServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "GetServiceSyncConfigInputRequestTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+
 GetServiceTemplateInputRequestTypeDef = TypedDict(
     "GetServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -968,110 +1054,158 @@
     {
         "templateName": str,
         "templateType": TemplateTypeType,
         "templateVersion": str,
     },
 )
 
-RevisionTypeDef = TypedDict(
-    "RevisionTypeDef",
+_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
-        "branch": str,
-        "directory": str,
-        "repositoryName": str,
-        "repositoryProvider": RepositoryProviderType,
-        "sha": str,
+        "componentName": str,
     },
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
+    _RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef,
+    _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef,
+):
+    pass
+
 _RequiredListComponentOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListComponentOutputsInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
     _OptionalListComponentOutputsInputRequestTypeDef,
 ):
     pass
 
-
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
     total=False,
 )
 
+_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
+    {
+        "componentName": str,
+    },
+)
+_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef(
+    _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
+    _OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListComponentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListComponentProvisionedResourcesInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 _OptionalListComponentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_OptionalListComponentProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListComponentProvisionedResourcesInputRequestTypeDef(
     _RequiredListComponentProvisionedResourcesInputRequestTypeDef,
     _OptionalListComponentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
-
 ProvisionedResourceTypeDef = TypedDict(
     "ProvisionedResourceTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
     total=False,
 )
 
+ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    {
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComponentsInputRequestTypeDef = TypedDict(
     "ListComponentsInputRequestTypeDef",
     {
         "environmentName": str,
         "maxResults": int,
         "nextToken": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
+    {
+        "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
+    },
+)
+_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
+    {
+        "environmentName": str,
+        "statuses": Sequence[EnvironmentAccountConnectionStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef(
+    _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
+    _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputRequestTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
@@ -1081,21 +1215,39 @@
         "maxResults": int,
         "nextToken": str,
         "statuses": Sequence[EnvironmentAccountConnectionStatusType],
     },
     total=False,
 )
 
-
 class ListEnvironmentAccountConnectionsInputRequestTypeDef(
     _RequiredListEnvironmentAccountConnectionsInputRequestTypeDef,
     _OptionalListEnvironmentAccountConnectionsInputRequestTypeDef,
 ):
     pass
 
+_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
+    {
+        "environmentName": str,
+    },
+)
+_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
+    _RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
+    _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
+):
+    pass
 
 _RequiredListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentOutputsInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
@@ -1103,21 +1255,39 @@
     "_OptionalListEnvironmentOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEnvironmentOutputsInputRequestTypeDef(
     _RequiredListEnvironmentOutputsInputRequestTypeDef,
     _OptionalListEnvironmentOutputsInputRequestTypeDef,
 ):
     pass
 
+_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
+    {
+        "environmentName": str,
+    },
+)
+_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef(
+    _RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
+    _OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
+):
+    pass
 
 _RequiredListEnvironmentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentProvisionedResourcesInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
@@ -1125,21 +1295,40 @@
     "_OptionalListEnvironmentProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEnvironmentProvisionedResourcesInputRequestTypeDef(
     _RequiredListEnvironmentProvisionedResourcesInputRequestTypeDef,
     _OptionalListEnvironmentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
+_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
+    {
+        "majorVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef(
+    _RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
+    _OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
+):
+    pass
 
 _RequiredListEnvironmentTemplateVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentTemplateVersionsInputRequestTypeDef",
     {
         "templateName": str,
     },
 )
@@ -1149,83 +1338,139 @@
         "majorVersion": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEnvironmentTemplateVersionsInputRequestTypeDef(
     _RequiredListEnvironmentTemplateVersionsInputRequestTypeDef,
     _OptionalListEnvironmentTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
+ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef = TypedDict(
+    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListEnvironmentTemplatesInputRequestTypeDef = TypedDict(
     "ListEnvironmentTemplatesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 RepositorySummaryTypeDef = TypedDict(
     "RepositorySummaryTypeDef",
     {
         "arn": str,
+        "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
+_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "syncType": SyncTypeType,
+    },
+)
+_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef(
+    _RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
+    _OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRepositorySyncDefinitionsInputRequestTypeDef = TypedDict(
     "_RequiredListRepositorySyncDefinitionsInputRequestTypeDef",
     {
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
-        "syncType": Literal["TEMPLATE_SYNC"],
+        "syncType": SyncTypeType,
     },
 )
 _OptionalListRepositorySyncDefinitionsInputRequestTypeDef = TypedDict(
     "_OptionalListRepositorySyncDefinitionsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRepositorySyncDefinitionsInputRequestTypeDef(
     _RequiredListRepositorySyncDefinitionsInputRequestTypeDef,
     _OptionalListRepositorySyncDefinitionsInputRequestTypeDef,
 ):
     pass
 
-
 RepositorySyncDefinitionTypeDef = TypedDict(
     "RepositorySyncDefinitionTypeDef",
     {
         "branch": str,
         "directory": str,
         "parent": str,
         "target": str,
     },
 )
 
+_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
+    _RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
+    _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
+):
+    pass
+
 _RequiredListServiceInstanceOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListServiceInstanceOutputsInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
@@ -1233,21 +1478,40 @@
     "_OptionalListServiceInstanceOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListServiceInstanceOutputsInputRequestTypeDef(
     _RequiredListServiceInstanceOutputsInputRequestTypeDef,
     _OptionalListServiceInstanceOutputsInputRequestTypeDef,
 ):
     pass
 
+_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef(
+    _RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
+    _OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
+):
+    pass
 
 _RequiredListServiceInstanceProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
@@ -1256,28 +1520,25 @@
     "_OptionalListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListServiceInstanceProvisionedResourcesInputRequestTypeDef(
     _RequiredListServiceInstanceProvisionedResourcesInputRequestTypeDef,
     _OptionalListServiceInstanceProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
-
-ListServiceInstancesInputRequestTypeDef = TypedDict(
-    "ListServiceInstancesInputRequestTypeDef",
+ListServiceInstancesFilterTypeDef = TypedDict(
+    "ListServiceInstancesFilterTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "serviceName": str,
+        "key": ListServiceInstancesFilterByType,
+        "value": str,
     },
     total=False,
 )
 
 _RequiredServiceInstanceSummaryTypeDef = TypedDict(
     "_RequiredServiceInstanceSummaryTypeDef",
     {
@@ -1298,20 +1559,38 @@
     "_OptionalServiceInstanceSummaryTypeDef",
     {
         "deploymentStatusMessage": str,
     },
     total=False,
 )
 
-
 class ServiceInstanceSummaryTypeDef(
     _RequiredServiceInstanceSummaryTypeDef, _OptionalServiceInstanceSummaryTypeDef
 ):
     pass
 
+_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
+    _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
+    _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
+):
+    pass
 
 _RequiredListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListServicePipelineOutputsInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
@@ -1319,21 +1598,39 @@
     "_OptionalListServicePipelineOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListServicePipelineOutputsInputRequestTypeDef(
     _RequiredListServicePipelineOutputsInputRequestTypeDef,
     _OptionalListServicePipelineOutputsInputRequestTypeDef,
 ):
     pass
 
+_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef(
+    _RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
+    _OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
+):
+    pass
 
 _RequiredListServicePipelineProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListServicePipelineProvisionedResourcesInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
@@ -1341,21 +1638,40 @@
     "_OptionalListServicePipelineProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListServicePipelineProvisionedResourcesInputRequestTypeDef(
     _RequiredListServicePipelineProvisionedResourcesInputRequestTypeDef,
     _OptionalListServicePipelineProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
+_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
+    {
+        "majorVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef(
+    _RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
+    _OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
+):
+    pass
 
 _RequiredListServiceTemplateVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListServiceTemplateVersionsInputRequestTypeDef",
     {
         "templateName": str,
     },
 )
@@ -1365,22 +1681,20 @@
         "majorVersion": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredServiceTemplateVersionSummaryTypeDef = TypedDict(
     "_RequiredServiceTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "majorVersion": str,
@@ -1395,20 +1709,26 @@
         "description": str,
         "recommendedMinorVersion": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class ServiceTemplateVersionSummaryTypeDef(
     _RequiredServiceTemplateVersionSummaryTypeDef, _OptionalServiceTemplateVersionSummaryTypeDef
 ):
     pass
 
+ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef = TypedDict(
+    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListServiceTemplatesInputRequestTypeDef = TypedDict(
     "ListServiceTemplatesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
@@ -1431,20 +1751,26 @@
         "displayName": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
-
 class ServiceTemplateSummaryTypeDef(
     _RequiredServiceTemplateSummaryTypeDef, _OptionalServiceTemplateSummaryTypeDef
 ):
     pass
 
+ListServicesInputListServicesPaginateTypeDef = TypedDict(
+    "ListServicesInputListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListServicesInputRequestTypeDef = TypedDict(
     "ListServicesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
@@ -1467,18 +1793,36 @@
     {
         "description": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class ServiceSummaryTypeDef(_RequiredServiceSummaryTypeDef, _OptionalServiceSummaryTypeDef):
     pass
 
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
 
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
@@ -1487,20 +1831,28 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -1517,21 +1869,19 @@
     "_OptionalRepositorySyncEventTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
-
 class RepositorySyncEventTypeDef(
     _RequiredRepositorySyncEventTypeDef, _OptionalRepositorySyncEventTypeDef
 ):
     pass
 
-
 _RequiredResourceSyncEventTypeDef = TypedDict(
     "_RequiredResourceSyncEventTypeDef",
     {
         "event": str,
         "time": datetime,
         "type": str,
     },
@@ -1540,29 +1890,46 @@
     "_OptionalResourceSyncEventTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
-
 class ResourceSyncEventTypeDef(
     _RequiredResourceSyncEventTypeDef, _OptionalResourceSyncEventTypeDef
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
 
 S3ObjectSourceTypeDef = TypedDict(
     "S3ObjectSourceTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
 
+SyncBlockerContextTypeDef = TypedDict(
+    "SyncBlockerContextTypeDef",
+    {
+        "key": str,
+        "value": str,
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
@@ -1573,30 +1940,29 @@
         "deploymentType": ComponentDeploymentUpdateTypeType,
         "name": str,
     },
 )
 _OptionalUpdateComponentInputRequestTypeDef = TypedDict(
     "_OptionalUpdateComponentInputRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "templateFile": str,
     },
     total=False,
 )
 
-
 class UpdateComponentInputRequestTypeDef(
     _RequiredUpdateComponentInputRequestTypeDef, _OptionalUpdateComponentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
@@ -1605,22 +1971,20 @@
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "roleArn": str,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentAccountConnectionInputRequestTypeDef(
     _RequiredUpdateEnvironmentAccountConnectionInputRequestTypeDef,
     _OptionalUpdateEnvironmentAccountConnectionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateEnvironmentTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateEnvironmentTemplateInputRequestTypeDef = TypedDict(
@@ -1628,22 +1992,20 @@
     {
         "description": str,
         "displayName": str,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentTemplateInputRequestTypeDef(
     _RequiredUpdateEnvironmentTemplateInputRequestTypeDef,
     _OptionalUpdateEnvironmentTemplateInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentTemplateVersionInputRequestTypeDef",
     {
         "majorVersion": str,
         "minorVersion": str,
         "templateName": str,
     },
@@ -1653,22 +2015,20 @@
     {
         "description": str,
         "status": TemplateVersionStatusType,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentTemplateVersionInputRequestTypeDef(
     _RequiredUpdateEnvironmentTemplateVersionInputRequestTypeDef,
     _OptionalUpdateEnvironmentTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateServiceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateServiceInputRequestTypeDef = TypedDict(
@@ -1676,47 +2036,44 @@
     {
         "description": str,
         "spec": str,
     },
     total=False,
 )
 
-
 class UpdateServiceInputRequestTypeDef(
     _RequiredUpdateServiceInputRequestTypeDef, _OptionalUpdateServiceInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateServiceInstanceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceInstanceInputRequestTypeDef",
     {
         "deploymentType": DeploymentUpdateTypeType,
         "name": str,
         "serviceName": str,
     },
 )
 _OptionalUpdateServiceInstanceInputRequestTypeDef = TypedDict(
     "_OptionalUpdateServiceInstanceInputRequestTypeDef",
     {
+        "clientToken": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
     },
     total=False,
 )
 
-
 class UpdateServiceInstanceInputRequestTypeDef(
     _RequiredUpdateServiceInstanceInputRequestTypeDef,
     _OptionalUpdateServiceInstanceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateServicePipelineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServicePipelineInputRequestTypeDef",
     {
         "deploymentType": DeploymentUpdateTypeType,
         "serviceName": str,
         "spec": str,
     },
@@ -1726,21 +2083,38 @@
     {
         "templateMajorVersion": str,
         "templateMinorVersion": str,
     },
     total=False,
 )
 
-
 class UpdateServicePipelineInputRequestTypeDef(
     _RequiredUpdateServicePipelineInputRequestTypeDef,
     _OptionalUpdateServicePipelineInputRequestTypeDef,
 ):
     pass
 
+UpdateServiceSyncBlockerInputRequestTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerInputRequestTypeDef",
+    {
+        "id": str,
+        "resolvedReason": str,
+    },
+)
+
+UpdateServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "UpdateServiceSyncConfigInputRequestTypeDef",
+    {
+        "branch": str,
+        "filePath": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "serviceName": str,
+    },
+)
 
 _RequiredUpdateServiceTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -1749,22 +2123,20 @@
     {
         "description": str,
         "displayName": str,
     },
     total=False,
 )
 
-
 class UpdateServiceTemplateInputRequestTypeDef(
     _RequiredUpdateServiceTemplateInputRequestTypeDef,
     _OptionalUpdateServiceTemplateInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateTemplateSyncConfigInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -1775,67 +2147,65 @@
     "_OptionalUpdateTemplateSyncConfigInputRequestTypeDef",
     {
         "subdirectory": str,
     },
     total=False,
 )
 
-
 class UpdateTemplateSyncConfigInputRequestTypeDef(
     _RequiredUpdateTemplateSyncConfigInputRequestTypeDef,
     _OptionalUpdateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-
 AcceptEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "CreateEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "DeleteEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "GetEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "UpdateEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
@@ -1872,88 +2242,94 @@
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
     },
     total=False,
 )
 
-
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
-
 CancelComponentDeploymentOutputTypeDef = TypedDict(
     "CancelComponentDeploymentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateComponentOutputTypeDef = TypedDict(
     "CreateComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteComponentOutputTypeDef = TypedDict(
     "DeleteComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateComponentOutputTypeDef = TypedDict(
     "UpdateComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelServiceInstanceDeploymentOutputTypeDef = TypedDict(
     "CancelServiceInstanceDeploymentOutputTypeDef",
     {
         "serviceInstance": ServiceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateServiceInstanceOutputTypeDef = TypedDict(
+    "CreateServiceInstanceOutputTypeDef",
+    {
+        "serviceInstance": ServiceInstanceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceInstanceOutputTypeDef = TypedDict(
     "GetServiceInstanceOutputTypeDef",
     {
         "serviceInstance": ServiceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceInstanceOutputTypeDef = TypedDict(
     "UpdateServiceInstanceOutputTypeDef",
     {
         "serviceInstance": ServiceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelServicePipelineDeploymentOutputTypeDef = TypedDict(
     "CancelServicePipelineDeploymentOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "arn": str,
@@ -1974,24 +2350,22 @@
         "repositoryConnectionArn": str,
         "repositoryId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
 
-
 UpdateServicePipelineOutputTypeDef = TypedDict(
     "UpdateServicePipelineOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateVersionInputRequestTypeDef",
     {
         "majorVersion": str,
@@ -2006,22 +2380,20 @@
         "description": str,
         "status": TemplateVersionStatusType,
         "supportedComponentSources": Sequence[Literal["DIRECTLY_DEFINED"]],
     },
     total=False,
 )
 
-
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredServiceTemplateVersionTypeDef = TypedDict(
     "_RequiredServiceTemplateVersionTypeDef",
     {
         "arn": str,
         "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
         "createdAt": datetime,
         "lastModifiedAt": datetime,
@@ -2039,85 +2411,94 @@
         "schema": str,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
     },
     total=False,
 )
 
-
 class ServiceTemplateVersionTypeDef(
     _RequiredServiceTemplateVersionTypeDef, _OptionalServiceTemplateVersionTypeDef
 ):
     pass
 
-
 ListComponentsOutputTypeDef = TypedDict(
     "ListComponentsOutputTypeDef",
     {
         "components": List[ComponentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CountsSummaryTypeDef = TypedDict(
+    "CountsSummaryTypeDef",
+    {
+        "components": ResourceCountsSummaryTypeDef,
+        "environmentTemplates": ResourceCountsSummaryTypeDef,
+        "environments": ResourceCountsSummaryTypeDef,
+        "pipelines": ResourceCountsSummaryTypeDef,
+        "serviceInstances": ResourceCountsSummaryTypeDef,
+        "serviceTemplates": ResourceCountsSummaryTypeDef,
+        "services": ResourceCountsSummaryTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
         "name": str,
         "templateFile": str,
     },
 )
 _OptionalCreateComponentInputRequestTypeDef = TypedDict(
     "_OptionalCreateComponentInputRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
         "environmentName": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateComponentInputRequestTypeDef(
     _RequiredCreateComponentInputRequestTypeDef, _OptionalCreateComponentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "environmentName": str,
         "managementAccountId": str,
-        "roleArn": str,
     },
 )
 _OptionalCreateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "_OptionalCreateEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "clientToken": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
+        "roleArn": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEnvironmentAccountConnectionInputRequestTypeDef(
     _RequiredCreateEnvironmentAccountConnectionInputRequestTypeDef,
     _OptionalCreateEnvironmentAccountConnectionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEnvironmentTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateEnvironmentTemplateInputRequestTypeDef = TypedDict(
@@ -2128,22 +2509,20 @@
         "encryptionKey": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEnvironmentTemplateInputRequestTypeDef(
     _RequiredCreateEnvironmentTemplateInputRequestTypeDef,
     _OptionalCreateEnvironmentTemplateInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryInputRequestTypeDef",
     {
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
@@ -2153,21 +2532,19 @@
     {
         "encryptionKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceInputRequestTypeDef",
     {
         "name": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateName": str,
@@ -2182,20 +2559,43 @@
         "repositoryId": str,
         "tags": Sequence[TagTypeDef],
         "templateMinorVersion": str,
     },
     total=False,
 )
 
-
 class CreateServiceInputRequestTypeDef(
     _RequiredCreateServiceInputRequestTypeDef, _OptionalCreateServiceInputRequestTypeDef
 ):
     pass
 
+_RequiredCreateServiceInstanceInputRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceInstanceInputRequestTypeDef",
+    {
+        "name": str,
+        "serviceName": str,
+        "spec": str,
+    },
+)
+_OptionalCreateServiceInstanceInputRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceInstanceInputRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+    },
+    total=False,
+)
+
+class CreateServiceInstanceInputRequestTypeDef(
+    _RequiredCreateServiceInstanceInputRequestTypeDef,
+    _OptionalCreateServiceInstanceInputRequestTypeDef,
+):
+    pass
 
 _RequiredCreateServiceTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -2207,28 +2607,26 @@
         "encryptionKey": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateServiceTemplateInputRequestTypeDef(
     _RequiredCreateServiceTemplateInputRequestTypeDef,
     _OptionalCreateServiceTemplateInputRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
@@ -2256,21 +2654,19 @@
         "provisioningRepository": RepositoryBranchInputTypeDef,
         "tags": Sequence[TagTypeDef],
         "templateMinorVersion": str,
     },
     total=False,
 )
 
-
 class CreateEnvironmentInputRequestTypeDef(
     _RequiredCreateEnvironmentInputRequestTypeDef, _OptionalCreateEnvironmentInputRequestTypeDef
 ):
     pass
 
-
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "deletePipelineProvisioningRepository": bool,
         "pipelineCodebuildRoleArn": str,
         "pipelineProvisioningRepository": RepositoryBranchInputTypeDef,
         "pipelineServiceRoleArn": str,
@@ -2297,189 +2693,228 @@
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
-
 CreateEnvironmentTemplateOutputTypeDef = TypedDict(
     "CreateEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentTemplateOutputTypeDef = TypedDict(
     "DeleteEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentTemplateOutputTypeDef = TypedDict(
     "GetEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentTemplateOutputTypeDef = TypedDict(
     "UpdateEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "CreateEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "DeleteEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "GetEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "UpdateEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryOutputTypeDef = TypedDict(
     "DeleteRepositoryOutputTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateServiceSyncConfigOutputTypeDef = TypedDict(
+    "CreateServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteServiceSyncConfigOutputTypeDef = TypedDict(
+    "DeleteServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetServiceSyncConfigOutputTypeDef = TypedDict(
+    "GetServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateServiceSyncConfigOutputTypeDef = TypedDict(
+    "UpdateServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceTemplateOutputTypeDef = TypedDict(
     "CreateServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceTemplateOutputTypeDef = TypedDict(
     "DeleteServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceTemplateOutputTypeDef = TypedDict(
     "GetServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceTemplateOutputTypeDef = TypedDict(
     "UpdateServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTemplateSyncConfigOutputTypeDef = TypedDict(
     "CreateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTemplateSyncConfigOutputTypeDef = TypedDict(
     "DeleteTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSyncConfigOutputTypeDef = TypedDict(
     "GetTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTemplateSyncConfigOutputTypeDef = TypedDict(
     "UpdateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
         "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsOutputTypeDef = TypedDict(
     "ListEnvironmentsOutputTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    {
+        "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
         "maxResults": int,
@@ -2489,24 +2924,24 @@
 )
 
 ListEnvironmentTemplatesOutputTypeDef = TypedDict(
     "ListEnvironmentTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "templates": List[EnvironmentTemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentTemplateVersionsOutputTypeDef = TypedDict(
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
         "templateVersions": List[EnvironmentTemplateVersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetComponentInputComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeletedWaitTypeDef",
     {
         "name": str,
@@ -2516,66 +2951,60 @@
     "_OptionalGetComponentInputComponentDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetComponentInputComponentDeletedWaitTypeDef(
     _RequiredGetComponentInputComponentDeletedWaitTypeDef,
     _OptionalGetComponentInputComponentDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetComponentInputComponentDeployedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeployedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetComponentInputComponentDeployedWaitTypeDef = TypedDict(
     "_OptionalGetComponentInputComponentDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetComponentInputComponentDeployedWaitTypeDef(
     _RequiredGetComponentInputComponentDeployedWaitTypeDef,
     _OptionalGetComponentInputComponentDeployedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetEnvironmentInputEnvironmentDeployedWaitTypeDef = TypedDict(
     "_RequiredGetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetEnvironmentInputEnvironmentDeployedWaitTypeDef = TypedDict(
     "_OptionalGetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetEnvironmentInputEnvironmentDeployedWaitTypeDef(
     _RequiredGetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     _OptionalGetEnvironmentInputEnvironmentDeployedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef = TypedDict(
     "_RequiredGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     {
         "majorVersion": str,
         "minorVersion": str,
         "templateName": str,
     },
@@ -2584,110 +3013,100 @@
     "_OptionalGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceInputServiceCreatedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServiceCreatedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServiceCreatedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServiceCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceInputServiceCreatedWaitTypeDef(
     _RequiredGetServiceInputServiceCreatedWaitTypeDef,
     _OptionalGetServiceInputServiceCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceInputServiceDeletedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServiceDeletedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServiceDeletedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServiceDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceInputServiceDeletedWaitTypeDef(
     _RequiredGetServiceInputServiceDeletedWaitTypeDef,
     _OptionalGetServiceInputServiceDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceInputServicePipelineDeployedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServicePipelineDeployedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServicePipelineDeployedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServicePipelineDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceInputServicePipelineDeployedWaitTypeDef(
     _RequiredGetServiceInputServicePipelineDeployedWaitTypeDef,
     _OptionalGetServiceInputServicePipelineDeployedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceInputServiceUpdatedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServiceUpdatedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServiceUpdatedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServiceUpdatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceInputServiceUpdatedWaitTypeDef(
     _RequiredGetServiceInputServiceUpdatedWaitTypeDef,
     _OptionalGetServiceInputServiceUpdatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     {
         "name": str,
         "serviceName": str,
     },
 )
@@ -2695,22 +3114,20 @@
     "_OptionalGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef(
     _RequiredGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     _OptionalGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef = TypedDict(
     "_RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
     {
         "majorVersion": str,
         "minorVersion": str,
         "templateName": str,
     },
@@ -2719,410 +3136,53 @@
     "_OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
-
-_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef",
-    {
-        "componentName": str,
-    },
-)
-_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
-    _RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-    _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
-    {
-        "componentName": str,
-    },
-)
-_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef(
-    _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-    _OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-
-ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    {
-        "environmentName": str,
-        "serviceInstanceName": str,
-        "serviceName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
-    {
-        "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
-    },
-)
-_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
-    {
-        "environmentName": str,
-        "statuses": Sequence[EnvironmentAccountConnectionStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef(
-    _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-    _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
-    {
-        "environmentName": str,
-    },
-)
-_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
-    _RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-    _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
-    {
-        "environmentName": str,
-    },
-)
-_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef(
-    _RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-    _OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
-    {
-        "majorVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef(
-    _RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-    _OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef = TypedDict(
-    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
-    {
-        "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "repositoryProvider": RepositoryProviderType,
-        "syncType": Literal["TEMPLATE_SYNC"],
-    },
-)
-_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef(
-    _RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-    _OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
-    {
-        "serviceInstanceName": str,
-        "serviceName": str,
-    },
-)
-_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
-    _RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-    _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
-    {
-        "serviceInstanceName": str,
-        "serviceName": str,
-    },
-)
-_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef(
-    _RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-    _OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-
-ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
-    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
-    {
-        "serviceName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
-    _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-    _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef(
-    _RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-    _OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
-    {
-        "majorVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef(
-    _RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-    _OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef = TypedDict(
-    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServicesInputListServicesPaginateTypeDef = TypedDict(
-    "ListServicesInputListServicesPaginateTypeDef",
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
 ListComponentOutputsOutputTypeDef = TypedDict(
     "ListComponentOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentOutputsOutputTypeDef = TypedDict(
     "ListEnvironmentOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstanceOutputsOutputTypeDef = TypedDict(
     "ListServiceInstanceOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicePipelineOutputsOutputTypeDef = TypedDict(
     "ListServicePipelineOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
     "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
     {
         "resourceArn": str,
@@ -3135,109 +3195,132 @@
         "outputs": Sequence[OutputTypeDef],
         "status": ResourceDeploymentStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
     _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
     _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
 ):
     pass
 
-
 ListComponentProvisionedResourcesOutputTypeDef = TypedDict(
     "ListComponentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentProvisionedResourcesOutputTypeDef = TypedDict(
     "ListEnvironmentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstanceProvisionedResourcesOutputTypeDef = TypedDict(
     "ListServiceInstanceProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicePipelineProvisionedResourcesOutputTypeDef = TypedDict(
     "ListServicePipelineProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "nextToken": str,
         "repositories": List[RepositorySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositorySyncDefinitionsOutputTypeDef = TypedDict(
     "ListRepositorySyncDefinitionsOutputTypeDef",
     {
         "nextToken": str,
         "syncDefinitions": List[RepositorySyncDefinitionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
+    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
+    {
+        "filters": Sequence[ListServiceInstancesFilterTypeDef],
+        "serviceName": str,
+        "sortBy": ListServiceInstancesSortByType,
+        "sortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListServiceInstancesInputRequestTypeDef = TypedDict(
+    "ListServiceInstancesInputRequestTypeDef",
+    {
+        "filters": Sequence[ListServiceInstancesFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+        "serviceName": str,
+        "sortBy": ListServiceInstancesSortByType,
+        "sortOrder": SortOrderType,
     },
+    total=False,
 )
 
 ListServiceInstancesOutputTypeDef = TypedDict(
     "ListServiceInstancesOutputTypeDef",
     {
         "nextToken": str,
         "serviceInstances": List[ServiceInstanceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceTemplateVersionsOutputTypeDef = TypedDict(
     "ListServiceTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
         "templateVersions": List[ServiceTemplateVersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceTemplatesOutputTypeDef = TypedDict(
     "ListServiceTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "templates": List[ServiceTemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesOutputTypeDef = TypedDict(
     "ListServicesOutputTypeDef",
     {
         "nextToken": str,
         "services": List[ServiceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RepositorySyncAttemptTypeDef = TypedDict(
     "RepositorySyncAttemptTypeDef",
     {
         "events": List[RepositorySyncEventTypeDef],
@@ -3262,149 +3345,190 @@
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
+_RequiredSyncBlockerTypeDef = TypedDict(
+    "_RequiredSyncBlockerTypeDef",
+    {
+        "createdAt": datetime,
+        "createdReason": str,
+        "id": str,
+        "status": BlockerStatusType,
+        "type": Literal["AUTOMATED"],
+    },
+)
+_OptionalSyncBlockerTypeDef = TypedDict(
+    "_OptionalSyncBlockerTypeDef",
+    {
+        "contexts": List[SyncBlockerContextTypeDef],
+        "resolvedAt": datetime,
+        "resolvedReason": str,
+    },
+    total=False,
+)
+
+class SyncBlockerTypeDef(_RequiredSyncBlockerTypeDef, _OptionalSyncBlockerTypeDef):
+    pass
+
 GetAccountSettingsOutputTypeDef = TypedDict(
     "GetAccountSettingsOutputTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountSettingsOutputTypeDef = TypedDict(
     "UpdateAccountSettingsOutputTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelEnvironmentDeploymentOutputTypeDef = TypedDict(
     "CancelEnvironmentDeploymentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentOutputTypeDef = TypedDict(
     "CreateEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentOutputTypeDef = TypedDict(
     "DeleteEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceOutputTypeDef = TypedDict(
     "CreateServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceOutputTypeDef = TypedDict(
     "DeleteServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceOutputTypeDef = TypedDict(
     "GetServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceOutputTypeDef = TypedDict(
     "UpdateServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceTemplateVersionOutputTypeDef = TypedDict(
     "CreateServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceTemplateVersionOutputTypeDef = TypedDict(
     "DeleteServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceTemplateVersionOutputTypeDef = TypedDict(
     "GetServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceTemplateVersionOutputTypeDef = TypedDict(
     "UpdateServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetResourcesSummaryOutputTypeDef = TypedDict(
+    "GetResourcesSummaryOutputTypeDef",
+    {
+        "counts": CountsSummaryTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositorySyncStatusOutputTypeDef = TypedDict(
     "GetRepositorySyncStatusOutputTypeDef",
     {
         "latestSync": RepositorySyncAttemptTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetServiceInstanceSyncStatusOutputTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusOutputTypeDef",
+    {
+        "desiredState": RevisionTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
+        "latestSync": ResourceSyncAttemptTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSyncStatusOutputTypeDef = TypedDict(
     "GetTemplateSyncStatusOutputTypeDef",
     {
         "desiredState": RevisionTypeDef,
         "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
         "latestSync": ResourceSyncAttemptTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef",
     {
         "source": TemplateVersionSourceInputTypeDef,
@@ -3418,22 +3542,20 @@
         "description": str,
         "majorVersion": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEnvironmentTemplateVersionInputRequestTypeDef(
     _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef,
     _OptionalCreateEnvironmentTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceTemplateVersionInputRequestTypeDef",
     {
         "compatibleEnvironmentTemplates": Sequence[CompatibleEnvironmentTemplateInputTypeDef],
         "source": TemplateVersionSourceInputTypeDef,
         "templateName": str,
     },
@@ -3446,13 +3568,50 @@
         "majorVersion": str,
         "supportedComponentSources": Sequence[Literal["DIRECTLY_DEFINED"]],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
+
+_RequiredServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "_RequiredServiceSyncBlockerSummaryTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "_OptionalServiceSyncBlockerSummaryTypeDef",
+    {
+        "latestBlockers": List[SyncBlockerTypeDef],
+        "serviceInstanceName": str,
+    },
+    total=False,
+)
+
+class ServiceSyncBlockerSummaryTypeDef(
+    _RequiredServiceSyncBlockerSummaryTypeDef, _OptionalServiceSyncBlockerSummaryTypeDef
+):
+    pass
+
+UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerOutputTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "serviceSyncBlocker": SyncBlockerTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
+    {
+        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/type_defs.pyi` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,68 +12,77 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
+    BlockerStatusType,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
+    ListServiceInstancesFilterByType,
+    ListServiceInstancesSortByType,
     ProvisionedResourceEngineType,
     RepositoryProviderType,
     RepositorySyncStatusType,
     ResourceDeploymentStatusType,
     ResourceSyncStatusType,
     ServiceStatusType,
+    SortOrderType,
+    SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     "EnvironmentAccountConnectionTypeDef",
-    "ResponseMetadataTypeDef",
     "RepositoryBranchTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
     "ComponentTypeDef",
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
     "CompatibleEnvironmentTemplateTypeDef",
     "ComponentSummaryTypeDef",
+    "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
     "EnvironmentTemplateTypeDef",
     "EnvironmentTemplateVersionTypeDef",
     "RepositoryTypeDef",
+    "CreateServiceSyncConfigInputRequestTypeDef",
+    "ServiceSyncConfigTypeDef",
     "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
     "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
+    "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     "EnvironmentAccountConnectionSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
     "EnvironmentTemplateSummaryTypeDef",
@@ -84,59 +93,84 @@
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
     "GetServiceInstanceInputRequestTypeDef",
+    "GetServiceInstanceSyncStatusInputRequestTypeDef",
+    "RevisionTypeDef",
+    "GetServiceSyncBlockerSummaryInputRequestTypeDef",
+    "GetServiceSyncConfigInputRequestTypeDef",
     "GetServiceTemplateInputRequestTypeDef",
     "GetServiceTemplateVersionInputRequestTypeDef",
     "GetTemplateSyncConfigInputRequestTypeDef",
     "GetTemplateSyncStatusInputRequestTypeDef",
-    "RevisionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
     "OutputTypeDef",
+    "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
     "ProvisionedResourceTypeDef",
+    "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
+    "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     "ListEnvironmentOutputsInputRequestTypeDef",
+    "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
+    "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
+    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositorySummaryTypeDef",
+    "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
     "ListRepositorySyncDefinitionsInputRequestTypeDef",
     "RepositorySyncDefinitionTypeDef",
+    "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     "ListServiceInstanceOutputsInputRequestTypeDef",
+    "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
     "ListServiceInstanceProvisionedResourcesInputRequestTypeDef",
-    "ListServiceInstancesInputRequestTypeDef",
+    "ListServiceInstancesFilterTypeDef",
     "ServiceInstanceSummaryTypeDef",
+    "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     "ListServicePipelineOutputsInputRequestTypeDef",
+    "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
     "ListServicePipelineProvisionedResourcesInputRequestTypeDef",
+    "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
     "ListServiceTemplateVersionsInputRequestTypeDef",
     "ServiceTemplateVersionSummaryTypeDef",
+    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     "ListServiceTemplatesInputRequestTypeDef",
     "ServiceTemplateSummaryTypeDef",
+    "ListServicesInputListServicesPaginateTypeDef",
     "ListServicesInputRequestTypeDef",
     "ServiceSummaryTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     "RepositorySyncEventTypeDef",
     "ResourceSyncEventTypeDef",
+    "ResponseMetadataTypeDef",
     "S3ObjectSourceTypeDef",
+    "SyncBlockerContextTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateComponentInputRequestTypeDef",
     "UpdateEnvironmentAccountConnectionInputRequestTypeDef",
     "UpdateEnvironmentTemplateInputRequestTypeDef",
     "UpdateEnvironmentTemplateVersionInputRequestTypeDef",
     "UpdateServiceInputRequestTypeDef",
     "UpdateServiceInstanceInputRequestTypeDef",
     "UpdateServicePipelineInputRequestTypeDef",
+    "UpdateServiceSyncBlockerInputRequestTypeDef",
+    "UpdateServiceSyncConfigInputRequestTypeDef",
     "UpdateServiceTemplateInputRequestTypeDef",
     "UpdateTemplateSyncConfigInputRequestTypeDef",
     "AcceptEnvironmentAccountConnectionOutputTypeDef",
     "CreateEnvironmentAccountConnectionOutputTypeDef",
     "DeleteEnvironmentAccountConnectionOutputTypeDef",
     "GetEnvironmentAccountConnectionOutputTypeDef",
     "RejectEnvironmentAccountConnectionOutputTypeDef",
@@ -145,27 +179,30 @@
     "EnvironmentTypeDef",
     "CancelComponentDeploymentOutputTypeDef",
     "CreateComponentOutputTypeDef",
     "DeleteComponentOutputTypeDef",
     "GetComponentOutputTypeDef",
     "UpdateComponentOutputTypeDef",
     "CancelServiceInstanceDeploymentOutputTypeDef",
+    "CreateServiceInstanceOutputTypeDef",
     "GetServiceInstanceOutputTypeDef",
     "UpdateServiceInstanceOutputTypeDef",
     "CancelServicePipelineDeploymentOutputTypeDef",
     "ServiceTypeDef",
     "UpdateServicePipelineOutputTypeDef",
     "UpdateServiceTemplateVersionInputRequestTypeDef",
     "ServiceTemplateVersionTypeDef",
     "ListComponentsOutputTypeDef",
+    "CountsSummaryTypeDef",
     "CreateComponentInputRequestTypeDef",
     "CreateEnvironmentAccountConnectionInputRequestTypeDef",
     "CreateEnvironmentTemplateInputRequestTypeDef",
     "CreateRepositoryInputRequestTypeDef",
     "CreateServiceInputRequestTypeDef",
+    "CreateServiceInstanceInputRequestTypeDef",
     "CreateServiceTemplateInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "CreateEnvironmentTemplateOutputTypeDef",
@@ -175,75 +212,63 @@
     "CreateEnvironmentTemplateVersionOutputTypeDef",
     "DeleteEnvironmentTemplateVersionOutputTypeDef",
     "GetEnvironmentTemplateVersionOutputTypeDef",
     "UpdateEnvironmentTemplateVersionOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "DeleteRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
+    "CreateServiceSyncConfigOutputTypeDef",
+    "DeleteServiceSyncConfigOutputTypeDef",
+    "GetServiceSyncConfigOutputTypeDef",
+    "UpdateServiceSyncConfigOutputTypeDef",
     "CreateServiceTemplateOutputTypeDef",
     "DeleteServiceTemplateOutputTypeDef",
     "GetServiceTemplateOutputTypeDef",
     "UpdateServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigOutputTypeDef",
     "DeleteTemplateSyncConfigOutputTypeDef",
     "GetTemplateSyncConfigOutputTypeDef",
     "UpdateTemplateSyncConfigOutputTypeDef",
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     "ListEnvironmentsOutputTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListEnvironmentTemplatesOutputTypeDef",
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
     "GetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     "GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     "GetServiceInputServiceCreatedWaitTypeDef",
     "GetServiceInputServiceDeletedWaitTypeDef",
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
-    "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
-    "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
-    "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
-    "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
-    "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
-    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
-    "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
-    "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
-    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
-    "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
-    "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
-    "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
-    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
-    "ListServicesInputListServicesPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListComponentOutputsOutputTypeDef",
     "ListEnvironmentOutputsOutputTypeDef",
     "ListServiceInstanceOutputsOutputTypeDef",
     "ListServicePipelineOutputsOutputTypeDef",
     "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
     "ListComponentProvisionedResourcesOutputTypeDef",
     "ListEnvironmentProvisionedResourcesOutputTypeDef",
     "ListServiceInstanceProvisionedResourcesOutputTypeDef",
     "ListServicePipelineProvisionedResourcesOutputTypeDef",
     "ListRepositoriesOutputTypeDef",
     "ListRepositorySyncDefinitionsOutputTypeDef",
+    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
+    "ListServiceInstancesInputRequestTypeDef",
     "ListServiceInstancesOutputTypeDef",
     "ListServiceTemplateVersionsOutputTypeDef",
     "ListServiceTemplatesOutputTypeDef",
     "ListServicesOutputTypeDef",
     "RepositorySyncAttemptTypeDef",
     "ResourceSyncAttemptTypeDef",
     "TemplateVersionSourceInputTypeDef",
+    "SyncBlockerTypeDef",
     "GetAccountSettingsOutputTypeDef",
     "UpdateAccountSettingsOutputTypeDef",
     "CancelEnvironmentDeploymentOutputTypeDef",
     "CreateEnvironmentOutputTypeDef",
     "DeleteEnvironmentOutputTypeDef",
     "GetEnvironmentOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
@@ -251,18 +276,23 @@
     "DeleteServiceOutputTypeDef",
     "GetServiceOutputTypeDef",
     "UpdateServiceOutputTypeDef",
     "CreateServiceTemplateVersionOutputTypeDef",
     "DeleteServiceTemplateVersionOutputTypeDef",
     "GetServiceTemplateVersionOutputTypeDef",
     "UpdateServiceTemplateVersionOutputTypeDef",
+    "GetResourcesSummaryOutputTypeDef",
     "GetRepositorySyncStatusOutputTypeDef",
+    "GetServiceInstanceSyncStatusOutputTypeDef",
     "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
+    "ServiceSyncBlockerSummaryTypeDef",
+    "UpdateServiceSyncBlockerOutputTypeDef",
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
@@ -287,29 +317,20 @@
     {
         "codebuildRoleArn": str,
         "componentRoleArn": str,
     },
     total=False,
 )
 
+
 class EnvironmentAccountConnectionTypeDef(
     _RequiredEnvironmentAccountConnectionTypeDef, _OptionalEnvironmentAccountConnectionTypeDef
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
 
 RepositoryBranchTypeDef = TypedDict(
     "RepositoryBranchTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
@@ -336,26 +357,29 @@
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "deploymentStatusMessage": str,
         "description": str,
+        "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
     },
     total=False,
 )
 
+
 class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
+
 CancelEnvironmentDeploymentInputRequestTypeDef = TypedDict(
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
 
@@ -383,22 +407,25 @@
         "templateName": str,
     },
 )
 _OptionalServiceInstanceTypeDef = TypedDict(
     "_OptionalServiceInstanceTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastClientRequestToken": str,
         "spec": str,
     },
     total=False,
 )
 
+
 class ServiceInstanceTypeDef(_RequiredServiceInstanceTypeDef, _OptionalServiceInstanceTypeDef):
     pass
 
+
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -420,17 +447,19 @@
     {
         "deploymentStatusMessage": str,
         "spec": str,
     },
     total=False,
 )
 
+
 class ServicePipelineTypeDef(_RequiredServicePipelineTypeDef, _OptionalServicePipelineTypeDef):
     pass
 
+
 CompatibleEnvironmentTemplateInputTypeDef = TypedDict(
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
@@ -462,17 +491,43 @@
         "lastDeploymentSucceededAt": datetime,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+
 class ComponentSummaryTypeDef(_RequiredComponentSummaryTypeDef, _OptionalComponentSummaryTypeDef):
     pass
 
+
+_RequiredResourceCountsSummaryTypeDef = TypedDict(
+    "_RequiredResourceCountsSummaryTypeDef",
+    {
+        "total": int,
+    },
+)
+_OptionalResourceCountsSummaryTypeDef = TypedDict(
+    "_OptionalResourceCountsSummaryTypeDef",
+    {
+        "behindMajor": int,
+        "behindMinor": int,
+        "failed": int,
+        "upToDate": int,
+    },
+    total=False,
+)
+
+
+class ResourceCountsSummaryTypeDef(
+    _RequiredResourceCountsSummaryTypeDef, _OptionalResourceCountsSummaryTypeDef
+):
+    pass
+
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -503,19 +558,21 @@
         "encryptionKey": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
+
 class EnvironmentTemplateTypeDef(
     _RequiredEnvironmentTemplateTypeDef, _OptionalEnvironmentTemplateTypeDef
 ):
     pass
 
+
 _RequiredEnvironmentTemplateVersionTypeDef = TypedDict(
     "_RequiredEnvironmentTemplateVersionTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "majorVersion": str,
@@ -531,19 +588,21 @@
         "recommendedMinorVersion": str,
         "schema": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class EnvironmentTemplateVersionTypeDef(
     _RequiredEnvironmentTemplateVersionTypeDef, _OptionalEnvironmentTemplateVersionTypeDef
 ):
     pass
 
+
 _RequiredRepositoryTypeDef = TypedDict(
     "_RequiredRepositoryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
@@ -553,17 +612,41 @@
     "_OptionalRepositoryTypeDef",
     {
         "encryptionKey": str,
     },
     total=False,
 )
 
+
 class RepositoryTypeDef(_RequiredRepositoryTypeDef, _OptionalRepositoryTypeDef):
     pass
 
+
+CreateServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "CreateServiceSyncConfigInputRequestTypeDef",
+    {
+        "branch": str,
+        "filePath": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "serviceName": str,
+    },
+)
+
+ServiceSyncConfigTypeDef = TypedDict(
+    "ServiceSyncConfigTypeDef",
+    {
+        "branch": str,
+        "filePath": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "serviceName": str,
+    },
+)
+
 _RequiredServiceTemplateTypeDef = TypedDict(
     "_RequiredServiceTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "name": str,
@@ -577,17 +660,19 @@
         "encryptionKey": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
+
 class ServiceTemplateTypeDef(_RequiredServiceTemplateTypeDef, _OptionalServiceTemplateTypeDef):
     pass
 
+
 _RequiredCreateTemplateSyncConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateTemplateSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -598,20 +683,22 @@
     "_OptionalCreateTemplateSyncConfigInputRequestTypeDef",
     {
         "subdirectory": str,
     },
     total=False,
 )
 
+
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredTemplateSyncConfigTypeDef = TypedDict(
     "_RequiredTemplateSyncConfigTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -622,19 +709,21 @@
     "_OptionalTemplateSyncConfigTypeDef",
     {
         "subdirectory": str,
     },
     total=False,
 )
 
+
 class TemplateSyncConfigTypeDef(
     _RequiredTemplateSyncConfigTypeDef, _OptionalTemplateSyncConfigTypeDef
 ):
     pass
 
+
 DeleteComponentInputRequestTypeDef = TypedDict(
     "DeleteComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -679,14 +768,21 @@
 DeleteServiceInputRequestTypeDef = TypedDict(
     "DeleteServiceInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "DeleteServiceSyncConfigInputRequestTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+
 DeleteServiceTemplateInputRequestTypeDef = TypedDict(
     "DeleteServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -725,20 +821,22 @@
     "_OptionalEnvironmentAccountConnectionSummaryTypeDef",
     {
         "componentRoleArn": str,
     },
     total=False,
 )
 
+
 class EnvironmentAccountConnectionSummaryTypeDef(
     _RequiredEnvironmentAccountConnectionSummaryTypeDef,
     _OptionalEnvironmentAccountConnectionSummaryTypeDef,
 ):
     pass
 
+
 _RequiredEnvironmentSummaryTypeDef = TypedDict(
     "_RequiredEnvironmentSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "lastDeploymentAttemptedAt": datetime,
@@ -759,19 +857,21 @@
         "environmentAccountId": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
     },
     total=False,
 )
 
+
 class EnvironmentSummaryTypeDef(
     _RequiredEnvironmentSummaryTypeDef, _OptionalEnvironmentSummaryTypeDef
 ):
     pass
 
+
 EnvironmentTemplateFilterTypeDef = TypedDict(
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
@@ -792,19 +892,21 @@
         "displayName": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
+
 class EnvironmentTemplateSummaryTypeDef(
     _RequiredEnvironmentTemplateSummaryTypeDef, _OptionalEnvironmentTemplateSummaryTypeDef
 ):
     pass
 
+
 _RequiredEnvironmentTemplateVersionSummaryTypeDef = TypedDict(
     "_RequiredEnvironmentTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "majorVersion": str,
@@ -819,20 +921,22 @@
         "description": str,
         "recommendedMinorVersion": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class EnvironmentTemplateVersionSummaryTypeDef(
     _RequiredEnvironmentTemplateVersionSummaryTypeDef,
     _OptionalEnvironmentTemplateVersionSummaryTypeDef,
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -885,15 +989,15 @@
 
 GetRepositorySyncStatusInputRequestTypeDef = TypedDict(
     "GetRepositorySyncStatusInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
-        "syncType": Literal["TEMPLATE_SYNC"],
+        "syncType": SyncTypeType,
     },
 )
 
 GetServiceInputRequestTypeDef = TypedDict(
     "GetServiceInputRequestTypeDef",
     {
         "name": str,
@@ -904,14 +1008,62 @@
     "GetServiceInstanceInputRequestTypeDef",
     {
         "name": str,
         "serviceName": str,
     },
 )
 
+GetServiceInstanceSyncStatusInputRequestTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusInputRequestTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+)
+
+RevisionTypeDef = TypedDict(
+    "RevisionTypeDef",
+    {
+        "branch": str,
+        "directory": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "sha": str,
+    },
+)
+
+_RequiredGetServiceSyncBlockerSummaryInputRequestTypeDef = TypedDict(
+    "_RequiredGetServiceSyncBlockerSummaryInputRequestTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalGetServiceSyncBlockerSummaryInputRequestTypeDef = TypedDict(
+    "_OptionalGetServiceSyncBlockerSummaryInputRequestTypeDef",
+    {
+        "serviceInstanceName": str,
+    },
+    total=False,
+)
+
+
+class GetServiceSyncBlockerSummaryInputRequestTypeDef(
+    _RequiredGetServiceSyncBlockerSummaryInputRequestTypeDef,
+    _OptionalGetServiceSyncBlockerSummaryInputRequestTypeDef,
+):
+    pass
+
+
+GetServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "GetServiceSyncConfigInputRequestTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+
 GetServiceTemplateInputRequestTypeDef = TypedDict(
     "GetServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -937,106 +1089,168 @@
     {
         "templateName": str,
         "templateType": TemplateTypeType,
         "templateVersion": str,
     },
 )
 
-RevisionTypeDef = TypedDict(
-    "RevisionTypeDef",
+_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
-        "branch": str,
-        "directory": str,
-        "repositoryName": str,
-        "repositoryProvider": RepositoryProviderType,
-        "sha": str,
+        "componentName": str,
     },
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
+    _RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef,
+    _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListComponentOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListComponentOutputsInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
     _OptionalListComponentOutputsInputRequestTypeDef,
 ):
     pass
 
+
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
     total=False,
 )
 
+_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
+    {
+        "componentName": str,
+    },
+)
+_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef(
+    _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
+    _OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListComponentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListComponentProvisionedResourcesInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 _OptionalListComponentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_OptionalListComponentProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListComponentProvisionedResourcesInputRequestTypeDef(
     _RequiredListComponentProvisionedResourcesInputRequestTypeDef,
     _OptionalListComponentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
+
 ProvisionedResourceTypeDef = TypedDict(
     "ProvisionedResourceTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
     total=False,
 )
 
+ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    {
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComponentsInputRequestTypeDef = TypedDict(
     "ListComponentsInputRequestTypeDef",
     {
         "environmentName": str,
         "maxResults": int,
         "nextToken": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
+    {
+        "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
+    },
+)
+_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
+    {
+        "environmentName": str,
+        "statuses": Sequence[EnvironmentAccountConnectionStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef(
+    _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
+    _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputRequestTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
@@ -1046,60 +1260,133 @@
         "maxResults": int,
         "nextToken": str,
         "statuses": Sequence[EnvironmentAccountConnectionStatusType],
     },
     total=False,
 )
 
+
 class ListEnvironmentAccountConnectionsInputRequestTypeDef(
     _RequiredListEnvironmentAccountConnectionsInputRequestTypeDef,
     _OptionalListEnvironmentAccountConnectionsInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
+    {
+        "environmentName": str,
+    },
+)
+_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
+    _RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
+    _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentOutputsInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEnvironmentOutputsInputRequestTypeDef(
     _RequiredListEnvironmentOutputsInputRequestTypeDef,
     _OptionalListEnvironmentOutputsInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
+    {
+        "environmentName": str,
+    },
+)
+_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef(
+    _RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
+    _OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEnvironmentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentProvisionedResourcesInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_OptionalListEnvironmentProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEnvironmentProvisionedResourcesInputRequestTypeDef(
     _RequiredListEnvironmentProvisionedResourcesInputRequestTypeDef,
     _OptionalListEnvironmentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
+    {
+        "majorVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef(
+    _RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
+    _OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEnvironmentTemplateVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentTemplateVersionsInputRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalListEnvironmentTemplateVersionsInputRequestTypeDef = TypedDict(
@@ -1108,79 +1395,147 @@
         "majorVersion": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEnvironmentTemplateVersionsInputRequestTypeDef(
     _RequiredListEnvironmentTemplateVersionsInputRequestTypeDef,
     _OptionalListEnvironmentTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
+
+ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef = TypedDict(
+    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentTemplatesInputRequestTypeDef = TypedDict(
     "ListEnvironmentTemplatesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 RepositorySummaryTypeDef = TypedDict(
     "RepositorySummaryTypeDef",
     {
         "arn": str,
+        "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
+_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "syncType": SyncTypeType,
+    },
+)
+_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef(
+    _RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
+    _OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRepositorySyncDefinitionsInputRequestTypeDef = TypedDict(
     "_RequiredListRepositorySyncDefinitionsInputRequestTypeDef",
     {
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
-        "syncType": Literal["TEMPLATE_SYNC"],
+        "syncType": SyncTypeType,
     },
 )
 _OptionalListRepositorySyncDefinitionsInputRequestTypeDef = TypedDict(
     "_OptionalListRepositorySyncDefinitionsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListRepositorySyncDefinitionsInputRequestTypeDef(
     _RequiredListRepositorySyncDefinitionsInputRequestTypeDef,
     _OptionalListRepositorySyncDefinitionsInputRequestTypeDef,
 ):
     pass
 
+
 RepositorySyncDefinitionTypeDef = TypedDict(
     "RepositorySyncDefinitionTypeDef",
     {
         "branch": str,
         "directory": str,
         "parent": str,
         "target": str,
     },
 )
 
+_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
+    _RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
+    _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServiceInstanceOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListServiceInstanceOutputsInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
@@ -1188,20 +1543,45 @@
     "_OptionalListServiceInstanceOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListServiceInstanceOutputsInputRequestTypeDef(
     _RequiredListServiceInstanceOutputsInputRequestTypeDef,
     _OptionalListServiceInstanceOutputsInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef(
+    _RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
+    _OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServiceInstanceProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
@@ -1209,26 +1589,27 @@
     "_OptionalListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListServiceInstanceProvisionedResourcesInputRequestTypeDef(
     _RequiredListServiceInstanceProvisionedResourcesInputRequestTypeDef,
     _OptionalListServiceInstanceProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
-ListServiceInstancesInputRequestTypeDef = TypedDict(
-    "ListServiceInstancesInputRequestTypeDef",
+
+ListServiceInstancesFilterTypeDef = TypedDict(
+    "ListServiceInstancesFilterTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "serviceName": str,
+        "key": ListServiceInstancesFilterByType,
+        "value": str,
     },
     total=False,
 )
 
 _RequiredServiceInstanceSummaryTypeDef = TypedDict(
     "_RequiredServiceInstanceSummaryTypeDef",
     {
@@ -1249,59 +1630,132 @@
     "_OptionalServiceInstanceSummaryTypeDef",
     {
         "deploymentStatusMessage": str,
     },
     total=False,
 )
 
+
 class ServiceInstanceSummaryTypeDef(
     _RequiredServiceInstanceSummaryTypeDef, _OptionalServiceInstanceSummaryTypeDef
 ):
     pass
 
+
+_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
+    "_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
+    "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
+    _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
+    _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_RequiredListServicePipelineOutputsInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListServicePipelineOutputsInputRequestTypeDef(
     _RequiredListServicePipelineOutputsInputRequestTypeDef,
     _OptionalListServicePipelineOutputsInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef(
+    _RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
+    _OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServicePipelineProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListServicePipelineProvisionedResourcesInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineProvisionedResourcesInputRequestTypeDef = TypedDict(
     "_OptionalListServicePipelineProvisionedResourcesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListServicePipelineProvisionedResourcesInputRequestTypeDef(
     _RequiredListServicePipelineProvisionedResourcesInputRequestTypeDef,
     _OptionalListServicePipelineProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
+    {
+        "majorVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef(
+    _RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
+    _OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServiceTemplateVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListServiceTemplateVersionsInputRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalListServiceTemplateVersionsInputRequestTypeDef = TypedDict(
@@ -1310,20 +1764,22 @@
         "majorVersion": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredServiceTemplateVersionSummaryTypeDef = TypedDict(
     "_RequiredServiceTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "majorVersion": str,
@@ -1338,19 +1794,29 @@
         "description": str,
         "recommendedMinorVersion": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class ServiceTemplateVersionSummaryTypeDef(
     _RequiredServiceTemplateVersionSummaryTypeDef, _OptionalServiceTemplateVersionSummaryTypeDef
 ):
     pass
 
+
+ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef = TypedDict(
+    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceTemplatesInputRequestTypeDef = TypedDict(
     "ListServiceTemplatesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1372,19 +1838,29 @@
         "displayName": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
     total=False,
 )
 
+
 class ServiceTemplateSummaryTypeDef(
     _RequiredServiceTemplateSummaryTypeDef, _OptionalServiceTemplateSummaryTypeDef
 ):
     pass
 
+
+ListServicesInputListServicesPaginateTypeDef = TypedDict(
+    "ListServicesInputListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesInputRequestTypeDef = TypedDict(
     "ListServicesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1406,17 +1882,41 @@
     {
         "description": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class ServiceSummaryTypeDef(_RequiredServiceSummaryTypeDef, _OptionalServiceSummaryTypeDef):
     pass
 
+
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
@@ -1424,19 +1924,31 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
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
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1452,19 +1964,21 @@
     "_OptionalRepositorySyncEventTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
+
 class RepositorySyncEventTypeDef(
     _RequiredRepositorySyncEventTypeDef, _OptionalRepositorySyncEventTypeDef
 ):
     pass
 
+
 _RequiredResourceSyncEventTypeDef = TypedDict(
     "_RequiredResourceSyncEventTypeDef",
     {
         "event": str,
         "time": datetime,
         "type": str,
     },
@@ -1473,27 +1987,48 @@
     "_OptionalResourceSyncEventTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
+
 class ResourceSyncEventTypeDef(
     _RequiredResourceSyncEventTypeDef, _OptionalResourceSyncEventTypeDef
 ):
     pass
 
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
 S3ObjectSourceTypeDef = TypedDict(
     "S3ObjectSourceTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
 
+SyncBlockerContextTypeDef = TypedDict(
+    "SyncBlockerContextTypeDef",
+    {
+        "key": str,
+        "value": str,
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
@@ -1504,28 +2039,31 @@
         "deploymentType": ComponentDeploymentUpdateTypeType,
         "name": str,
     },
 )
 _OptionalUpdateComponentInputRequestTypeDef = TypedDict(
     "_OptionalUpdateComponentInputRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "templateFile": str,
     },
     total=False,
 )
 
+
 class UpdateComponentInputRequestTypeDef(
     _RequiredUpdateComponentInputRequestTypeDef, _OptionalUpdateComponentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
@@ -1534,20 +2072,22 @@
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "roleArn": str,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentAccountConnectionInputRequestTypeDef(
     _RequiredUpdateEnvironmentAccountConnectionInputRequestTypeDef,
     _OptionalUpdateEnvironmentAccountConnectionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateEnvironmentTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateEnvironmentTemplateInputRequestTypeDef = TypedDict(
@@ -1555,20 +2095,22 @@
     {
         "description": str,
         "displayName": str,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentTemplateInputRequestTypeDef(
     _RequiredUpdateEnvironmentTemplateInputRequestTypeDef,
     _OptionalUpdateEnvironmentTemplateInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentTemplateVersionInputRequestTypeDef",
     {
         "majorVersion": str,
         "minorVersion": str,
         "templateName": str,
     },
@@ -1578,20 +2120,22 @@
     {
         "description": str,
         "status": TemplateVersionStatusType,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentTemplateVersionInputRequestTypeDef(
     _RequiredUpdateEnvironmentTemplateVersionInputRequestTypeDef,
     _OptionalUpdateEnvironmentTemplateVersionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateServiceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateServiceInputRequestTypeDef = TypedDict(
@@ -1599,43 +2143,48 @@
     {
         "description": str,
         "spec": str,
     },
     total=False,
 )
 
+
 class UpdateServiceInputRequestTypeDef(
     _RequiredUpdateServiceInputRequestTypeDef, _OptionalUpdateServiceInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateServiceInstanceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceInstanceInputRequestTypeDef",
     {
         "deploymentType": DeploymentUpdateTypeType,
         "name": str,
         "serviceName": str,
     },
 )
 _OptionalUpdateServiceInstanceInputRequestTypeDef = TypedDict(
     "_OptionalUpdateServiceInstanceInputRequestTypeDef",
     {
+        "clientToken": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
     },
     total=False,
 )
 
+
 class UpdateServiceInstanceInputRequestTypeDef(
     _RequiredUpdateServiceInstanceInputRequestTypeDef,
     _OptionalUpdateServiceInstanceInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateServicePipelineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServicePipelineInputRequestTypeDef",
     {
         "deploymentType": DeploymentUpdateTypeType,
         "serviceName": str,
         "spec": str,
     },
@@ -1645,20 +2194,41 @@
     {
         "templateMajorVersion": str,
         "templateMinorVersion": str,
     },
     total=False,
 )
 
+
 class UpdateServicePipelineInputRequestTypeDef(
     _RequiredUpdateServicePipelineInputRequestTypeDef,
     _OptionalUpdateServicePipelineInputRequestTypeDef,
 ):
     pass
 
+
+UpdateServiceSyncBlockerInputRequestTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerInputRequestTypeDef",
+    {
+        "id": str,
+        "resolvedReason": str,
+    },
+)
+
+UpdateServiceSyncConfigInputRequestTypeDef = TypedDict(
+    "UpdateServiceSyncConfigInputRequestTypeDef",
+    {
+        "branch": str,
+        "filePath": str,
+        "repositoryName": str,
+        "repositoryProvider": RepositoryProviderType,
+        "serviceName": str,
+    },
+)
+
 _RequiredUpdateServiceTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateServiceTemplateInputRequestTypeDef = TypedDict(
@@ -1666,20 +2236,22 @@
     {
         "description": str,
         "displayName": str,
     },
     total=False,
 )
 
+
 class UpdateServiceTemplateInputRequestTypeDef(
     _RequiredUpdateServiceTemplateInputRequestTypeDef,
     _OptionalUpdateServiceTemplateInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateTemplateSyncConfigInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -1690,65 +2262,67 @@
     "_OptionalUpdateTemplateSyncConfigInputRequestTypeDef",
     {
         "subdirectory": str,
     },
     total=False,
 )
 
+
 class UpdateTemplateSyncConfigInputRequestTypeDef(
     _RequiredUpdateTemplateSyncConfigInputRequestTypeDef,
     _OptionalUpdateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
+
 AcceptEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "CreateEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "DeleteEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "GetEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
     "UpdateEnvironmentAccountConnectionOutputTypeDef",
     {
         "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
@@ -1785,86 +2359,96 @@
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
     },
     total=False,
 )
 
+
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
+
 CancelComponentDeploymentOutputTypeDef = TypedDict(
     "CancelComponentDeploymentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateComponentOutputTypeDef = TypedDict(
     "CreateComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteComponentOutputTypeDef = TypedDict(
     "DeleteComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateComponentOutputTypeDef = TypedDict(
     "UpdateComponentOutputTypeDef",
     {
         "component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelServiceInstanceDeploymentOutputTypeDef = TypedDict(
     "CancelServiceInstanceDeploymentOutputTypeDef",
     {
         "serviceInstance": ServiceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateServiceInstanceOutputTypeDef = TypedDict(
+    "CreateServiceInstanceOutputTypeDef",
+    {
+        "serviceInstance": ServiceInstanceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceInstanceOutputTypeDef = TypedDict(
     "GetServiceInstanceOutputTypeDef",
     {
         "serviceInstance": ServiceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceInstanceOutputTypeDef = TypedDict(
     "UpdateServiceInstanceOutputTypeDef",
     {
         "serviceInstance": ServiceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelServicePipelineDeploymentOutputTypeDef = TypedDict(
     "CancelServicePipelineDeploymentOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "arn": str,
@@ -1885,22 +2469,24 @@
         "repositoryConnectionArn": str,
         "repositoryId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
 
+
 UpdateServicePipelineOutputTypeDef = TypedDict(
     "UpdateServicePipelineOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateVersionInputRequestTypeDef",
     {
         "majorVersion": str,
@@ -1915,20 +2501,22 @@
         "description": str,
         "status": TemplateVersionStatusType,
         "supportedComponentSources": Sequence[Literal["DIRECTLY_DEFINED"]],
     },
     total=False,
 )
 
+
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredServiceTemplateVersionTypeDef = TypedDict(
     "_RequiredServiceTemplateVersionTypeDef",
     {
         "arn": str,
         "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
         "createdAt": datetime,
         "lastModifiedAt": datetime,
@@ -1946,79 +2534,100 @@
         "schema": str,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
     },
     total=False,
 )
 
+
 class ServiceTemplateVersionTypeDef(
     _RequiredServiceTemplateVersionTypeDef, _OptionalServiceTemplateVersionTypeDef
 ):
     pass
 
+
 ListComponentsOutputTypeDef = TypedDict(
     "ListComponentsOutputTypeDef",
     {
         "components": List[ComponentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CountsSummaryTypeDef = TypedDict(
+    "CountsSummaryTypeDef",
+    {
+        "components": ResourceCountsSummaryTypeDef,
+        "environmentTemplates": ResourceCountsSummaryTypeDef,
+        "environments": ResourceCountsSummaryTypeDef,
+        "pipelines": ResourceCountsSummaryTypeDef,
+        "serviceInstances": ResourceCountsSummaryTypeDef,
+        "serviceTemplates": ResourceCountsSummaryTypeDef,
+        "services": ResourceCountsSummaryTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
         "name": str,
         "templateFile": str,
     },
 )
 _OptionalCreateComponentInputRequestTypeDef = TypedDict(
     "_OptionalCreateComponentInputRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
         "environmentName": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateComponentInputRequestTypeDef(
     _RequiredCreateComponentInputRequestTypeDef, _OptionalCreateComponentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "environmentName": str,
         "managementAccountId": str,
-        "roleArn": str,
     },
 )
 _OptionalCreateEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "_OptionalCreateEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "clientToken": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
+        "roleArn": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEnvironmentAccountConnectionInputRequestTypeDef(
     _RequiredCreateEnvironmentAccountConnectionInputRequestTypeDef,
     _OptionalCreateEnvironmentAccountConnectionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEnvironmentTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateEnvironmentTemplateInputRequestTypeDef = TypedDict(
@@ -2029,20 +2638,22 @@
         "encryptionKey": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEnvironmentTemplateInputRequestTypeDef(
     _RequiredCreateEnvironmentTemplateInputRequestTypeDef,
     _OptionalCreateEnvironmentTemplateInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryInputRequestTypeDef",
     {
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
@@ -2052,19 +2663,21 @@
     {
         "encryptionKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceInputRequestTypeDef",
     {
         "name": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateName": str,
@@ -2079,19 +2692,48 @@
         "repositoryId": str,
         "tags": Sequence[TagTypeDef],
         "templateMinorVersion": str,
     },
     total=False,
 )
 
+
 class CreateServiceInputRequestTypeDef(
     _RequiredCreateServiceInputRequestTypeDef, _OptionalCreateServiceInputRequestTypeDef
 ):
     pass
 
+
+_RequiredCreateServiceInstanceInputRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceInstanceInputRequestTypeDef",
+    {
+        "name": str,
+        "serviceName": str,
+        "spec": str,
+    },
+)
+_OptionalCreateServiceInstanceInputRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceInstanceInputRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+    },
+    total=False,
+)
+
+
+class CreateServiceInstanceInputRequestTypeDef(
+    _RequiredCreateServiceInstanceInputRequestTypeDef,
+    _OptionalCreateServiceInstanceInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateServiceTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceTemplateInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceTemplateInputRequestTypeDef = TypedDict(
@@ -2102,26 +2744,28 @@
         "encryptionKey": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateServiceTemplateInputRequestTypeDef(
     _RequiredCreateServiceTemplateInputRequestTypeDef,
     _OptionalCreateServiceTemplateInputRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
@@ -2149,19 +2793,21 @@
         "provisioningRepository": RepositoryBranchInputTypeDef,
         "tags": Sequence[TagTypeDef],
         "templateMinorVersion": str,
     },
     total=False,
 )
 
+
 class CreateEnvironmentInputRequestTypeDef(
     _RequiredCreateEnvironmentInputRequestTypeDef, _OptionalCreateEnvironmentInputRequestTypeDef
 ):
     pass
 
+
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "deletePipelineProvisioningRepository": bool,
         "pipelineCodebuildRoleArn": str,
         "pipelineProvisioningRepository": RepositoryBranchInputTypeDef,
         "pipelineServiceRoleArn": str,
@@ -2188,189 +2834,232 @@
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
+
 CreateEnvironmentTemplateOutputTypeDef = TypedDict(
     "CreateEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentTemplateOutputTypeDef = TypedDict(
     "DeleteEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentTemplateOutputTypeDef = TypedDict(
     "GetEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentTemplateOutputTypeDef = TypedDict(
     "UpdateEnvironmentTemplateOutputTypeDef",
     {
         "environmentTemplate": EnvironmentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "CreateEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "DeleteEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "GetEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
     "UpdateEnvironmentTemplateVersionOutputTypeDef",
     {
         "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryOutputTypeDef = TypedDict(
     "DeleteRepositoryOutputTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateServiceSyncConfigOutputTypeDef = TypedDict(
+    "CreateServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteServiceSyncConfigOutputTypeDef = TypedDict(
+    "DeleteServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetServiceSyncConfigOutputTypeDef = TypedDict(
+    "GetServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateServiceSyncConfigOutputTypeDef = TypedDict(
+    "UpdateServiceSyncConfigOutputTypeDef",
+    {
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceTemplateOutputTypeDef = TypedDict(
     "CreateServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceTemplateOutputTypeDef = TypedDict(
     "DeleteServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceTemplateOutputTypeDef = TypedDict(
     "GetServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceTemplateOutputTypeDef = TypedDict(
     "UpdateServiceTemplateOutputTypeDef",
     {
         "serviceTemplate": ServiceTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTemplateSyncConfigOutputTypeDef = TypedDict(
     "CreateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTemplateSyncConfigOutputTypeDef = TypedDict(
     "DeleteTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSyncConfigOutputTypeDef = TypedDict(
     "GetTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTemplateSyncConfigOutputTypeDef = TypedDict(
     "UpdateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
         "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsOutputTypeDef = TypedDict(
     "ListEnvironmentsOutputTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    {
+        "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
@@ -2378,24 +3067,24 @@
 )
 
 ListEnvironmentTemplatesOutputTypeDef = TypedDict(
     "ListEnvironmentTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "templates": List[EnvironmentTemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentTemplateVersionsOutputTypeDef = TypedDict(
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
         "templateVersions": List[EnvironmentTemplateVersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetComponentInputComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeletedWaitTypeDef",
     {
         "name": str,
@@ -2405,60 +3094,66 @@
     "_OptionalGetComponentInputComponentDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetComponentInputComponentDeletedWaitTypeDef(
     _RequiredGetComponentInputComponentDeletedWaitTypeDef,
     _OptionalGetComponentInputComponentDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetComponentInputComponentDeployedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeployedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetComponentInputComponentDeployedWaitTypeDef = TypedDict(
     "_OptionalGetComponentInputComponentDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetComponentInputComponentDeployedWaitTypeDef(
     _RequiredGetComponentInputComponentDeployedWaitTypeDef,
     _OptionalGetComponentInputComponentDeployedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetEnvironmentInputEnvironmentDeployedWaitTypeDef = TypedDict(
     "_RequiredGetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetEnvironmentInputEnvironmentDeployedWaitTypeDef = TypedDict(
     "_OptionalGetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetEnvironmentInputEnvironmentDeployedWaitTypeDef(
     _RequiredGetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     _OptionalGetEnvironmentInputEnvironmentDeployedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef = TypedDict(
     "_RequiredGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     {
         "majorVersion": str,
         "minorVersion": str,
         "templateName": str,
     },
@@ -2467,100 +3162,110 @@
     "_OptionalGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceInputServiceCreatedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServiceCreatedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServiceCreatedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServiceCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceInputServiceCreatedWaitTypeDef(
     _RequiredGetServiceInputServiceCreatedWaitTypeDef,
     _OptionalGetServiceInputServiceCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceInputServiceDeletedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServiceDeletedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServiceDeletedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServiceDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceInputServiceDeletedWaitTypeDef(
     _RequiredGetServiceInputServiceDeletedWaitTypeDef,
     _OptionalGetServiceInputServiceDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceInputServicePipelineDeployedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServicePipelineDeployedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServicePipelineDeployedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServicePipelineDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceInputServicePipelineDeployedWaitTypeDef(
     _RequiredGetServiceInputServicePipelineDeployedWaitTypeDef,
     _OptionalGetServiceInputServicePipelineDeployedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceInputServiceUpdatedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInputServiceUpdatedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetServiceInputServiceUpdatedWaitTypeDef = TypedDict(
     "_OptionalGetServiceInputServiceUpdatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceInputServiceUpdatedWaitTypeDef(
     _RequiredGetServiceInputServiceUpdatedWaitTypeDef,
     _OptionalGetServiceInputServiceUpdatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef = TypedDict(
     "_RequiredGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     {
         "name": str,
         "serviceName": str,
     },
 )
@@ -2568,20 +3273,22 @@
     "_OptionalGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef(
     _RequiredGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     _OptionalGetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef = TypedDict(
     "_RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
     {
         "majorVersion": str,
         "minorVersion": str,
         "templateName": str,
     },
@@ -2590,382 +3297,55 @@
     "_OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
-_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef",
-    {
-        "componentName": str,
-    },
-)
-_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
-    _RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-    _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-):
-    pass
-
-_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
-    {
-        "componentName": str,
-    },
-)
-_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef(
-    _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-    _OptionalListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    {
-        "environmentName": str,
-        "serviceInstanceName": str,
-        "serviceName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
-    {
-        "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
-    },
-)
-_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
-    {
-        "environmentName": str,
-        "statuses": Sequence[EnvironmentAccountConnectionStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef(
-    _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-    _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
-    {
-        "environmentName": str,
-    },
-)
-_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
-    _RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-    _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
-    {
-        "environmentName": str,
-    },
-)
-_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef(
-    _RequiredListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-    _OptionalListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
-    {
-        "majorVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef(
-    _RequiredListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-    _OptionalListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-):
-    pass
-
-ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef = TypedDict(
-    "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
-    {
-        "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "repositoryProvider": RepositoryProviderType,
-        "syncType": Literal["TEMPLATE_SYNC"],
-    },
-)
-_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef(
-    _RequiredListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-    _OptionalListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
-    {
-        "serviceInstanceName": str,
-        "serviceName": str,
-    },
-)
-_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
-    _RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-    _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-):
-    pass
-
-_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
-    {
-        "serviceInstanceName": str,
-        "serviceName": str,
-    },
-)
-_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef(
-    _RequiredListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-    _OptionalListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
-    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
-    {
-        "serviceName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
-    "_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
-    "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
-    _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-    _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-):
-    pass
-
-_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef(
-    _RequiredListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-    _OptionalListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
-    {
-        "majorVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef(
-    _RequiredListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-    _OptionalListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-):
-    pass
-
-ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef = TypedDict(
-    "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServicesInputListServicesPaginateTypeDef = TypedDict(
-    "ListServicesInputListServicesPaginateTypeDef",
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
 
 ListComponentOutputsOutputTypeDef = TypedDict(
     "ListComponentOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentOutputsOutputTypeDef = TypedDict(
     "ListEnvironmentOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstanceOutputsOutputTypeDef = TypedDict(
     "ListServiceInstanceOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicePipelineOutputsOutputTypeDef = TypedDict(
     "ListServicePipelineOutputsOutputTypeDef",
     {
         "nextToken": str,
         "outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
     "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
     {
         "resourceArn": str,
@@ -2978,107 +3358,134 @@
         "outputs": Sequence[OutputTypeDef],
         "status": ResourceDeploymentStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
     _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
     _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
 ):
     pass
 
+
 ListComponentProvisionedResourcesOutputTypeDef = TypedDict(
     "ListComponentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentProvisionedResourcesOutputTypeDef = TypedDict(
     "ListEnvironmentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstanceProvisionedResourcesOutputTypeDef = TypedDict(
     "ListServiceInstanceProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicePipelineProvisionedResourcesOutputTypeDef = TypedDict(
     "ListServicePipelineProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
         "provisionedResources": List[ProvisionedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "nextToken": str,
         "repositories": List[RepositorySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositorySyncDefinitionsOutputTypeDef = TypedDict(
     "ListRepositorySyncDefinitionsOutputTypeDef",
     {
         "nextToken": str,
         "syncDefinitions": List[RepositorySyncDefinitionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
+    "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
+    {
+        "filters": Sequence[ListServiceInstancesFilterTypeDef],
+        "serviceName": str,
+        "sortBy": ListServiceInstancesSortByType,
+        "sortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListServiceInstancesInputRequestTypeDef = TypedDict(
+    "ListServiceInstancesInputRequestTypeDef",
+    {
+        "filters": Sequence[ListServiceInstancesFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+        "serviceName": str,
+        "sortBy": ListServiceInstancesSortByType,
+        "sortOrder": SortOrderType,
+    },
+    total=False,
+)
+
 ListServiceInstancesOutputTypeDef = TypedDict(
     "ListServiceInstancesOutputTypeDef",
     {
         "nextToken": str,
         "serviceInstances": List[ServiceInstanceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceTemplateVersionsOutputTypeDef = TypedDict(
     "ListServiceTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
         "templateVersions": List[ServiceTemplateVersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceTemplatesOutputTypeDef = TypedDict(
     "ListServiceTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "templates": List[ServiceTemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesOutputTypeDef = TypedDict(
     "ListServicesOutputTypeDef",
     {
         "nextToken": str,
         "services": List[ServiceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RepositorySyncAttemptTypeDef = TypedDict(
     "RepositorySyncAttemptTypeDef",
     {
         "events": List[RepositorySyncEventTypeDef],
@@ -3103,149 +3510,192 @@
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
+_RequiredSyncBlockerTypeDef = TypedDict(
+    "_RequiredSyncBlockerTypeDef",
+    {
+        "createdAt": datetime,
+        "createdReason": str,
+        "id": str,
+        "status": BlockerStatusType,
+        "type": Literal["AUTOMATED"],
+    },
+)
+_OptionalSyncBlockerTypeDef = TypedDict(
+    "_OptionalSyncBlockerTypeDef",
+    {
+        "contexts": List[SyncBlockerContextTypeDef],
+        "resolvedAt": datetime,
+        "resolvedReason": str,
+    },
+    total=False,
+)
+
+
+class SyncBlockerTypeDef(_RequiredSyncBlockerTypeDef, _OptionalSyncBlockerTypeDef):
+    pass
+
+
 GetAccountSettingsOutputTypeDef = TypedDict(
     "GetAccountSettingsOutputTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountSettingsOutputTypeDef = TypedDict(
     "UpdateAccountSettingsOutputTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelEnvironmentDeploymentOutputTypeDef = TypedDict(
     "CancelEnvironmentDeploymentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentOutputTypeDef = TypedDict(
     "CreateEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEnvironmentOutputTypeDef = TypedDict(
     "DeleteEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceOutputTypeDef = TypedDict(
     "CreateServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceOutputTypeDef = TypedDict(
     "DeleteServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceOutputTypeDef = TypedDict(
     "GetServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceOutputTypeDef = TypedDict(
     "UpdateServiceOutputTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceTemplateVersionOutputTypeDef = TypedDict(
     "CreateServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceTemplateVersionOutputTypeDef = TypedDict(
     "DeleteServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceTemplateVersionOutputTypeDef = TypedDict(
     "GetServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceTemplateVersionOutputTypeDef = TypedDict(
     "UpdateServiceTemplateVersionOutputTypeDef",
     {
         "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetResourcesSummaryOutputTypeDef = TypedDict(
+    "GetResourcesSummaryOutputTypeDef",
+    {
+        "counts": CountsSummaryTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositorySyncStatusOutputTypeDef = TypedDict(
     "GetRepositorySyncStatusOutputTypeDef",
     {
         "latestSync": RepositorySyncAttemptTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetServiceInstanceSyncStatusOutputTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusOutputTypeDef",
+    {
+        "desiredState": RevisionTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
+        "latestSync": ResourceSyncAttemptTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSyncStatusOutputTypeDef = TypedDict(
     "GetTemplateSyncStatusOutputTypeDef",
     {
         "desiredState": RevisionTypeDef,
         "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
         "latestSync": ResourceSyncAttemptTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef",
     {
         "source": TemplateVersionSourceInputTypeDef,
@@ -3259,20 +3709,22 @@
         "description": str,
         "majorVersion": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEnvironmentTemplateVersionInputRequestTypeDef(
     _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef,
     _OptionalCreateEnvironmentTemplateVersionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceTemplateVersionInputRequestTypeDef",
     {
         "compatibleEnvironmentTemplates": Sequence[CompatibleEnvironmentTemplateInputTypeDef],
         "source": TemplateVersionSourceInputTypeDef,
         "templateName": str,
     },
@@ -3285,12 +3737,54 @@
         "majorVersion": str,
         "supportedComponentSources": Sequence[Literal["DIRECTLY_DEFINED"]],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
+
+
+_RequiredServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "_RequiredServiceSyncBlockerSummaryTypeDef",
+    {
+        "serviceName": str,
+    },
+)
+_OptionalServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "_OptionalServiceSyncBlockerSummaryTypeDef",
+    {
+        "latestBlockers": List[SyncBlockerTypeDef],
+        "serviceInstanceName": str,
+    },
+    total=False,
+)
+
+
+class ServiceSyncBlockerSummaryTypeDef(
+    _RequiredServiceSyncBlockerSummaryTypeDef, _OptionalServiceSyncBlockerSummaryTypeDef
+):
+    pass
+
+
+UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerOutputTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "serviceSyncBlocker": SyncBlockerTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
+    {
+        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
```

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/waiter.py` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton/waiter.pyi` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/PKG-INFO` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-proton
-Version: 1.26.9
-Summary: Type annotations for boto3.Proton 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Proton 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/
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
 
 <a id="mypy-boto3-proton"></a>
 
 # mypy-boto3-proton
 
 [![PyPI - mypy-boto3-proton](https://img.shields.io/pypi/v/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Proton 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[boto3.Proton 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,14 +416,16 @@
 ### Literals
 
 `mypy_boto3_proton.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_proton.literals import (
+    BlockerStatusType,
+    BlockerTypeType,
     ComponentDeletedWaiterName,
     ComponentDeployedWaiterName,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
@@ -437,15 +440,17 @@
     ListEnvironmentTemplateVersionsPaginatorName,
     ListEnvironmentTemplatesPaginatorName,
     ListEnvironmentsPaginatorName,
     ListRepositoriesPaginatorName,
     ListRepositorySyncDefinitionsPaginatorName,
     ListServiceInstanceOutputsPaginatorName,
     ListServiceInstanceProvisionedResourcesPaginatorName,
+    ListServiceInstancesFilterByType,
     ListServiceInstancesPaginatorName,
+    ListServiceInstancesSortByType,
     ListServicePipelineOutputsPaginatorName,
     ListServicePipelineProvisionedResourcesPaginatorName,
     ListServiceTemplateVersionsPaginatorName,
     ListServiceTemplatesPaginatorName,
     ListServicesPaginatorName,
     ListTagsForResourcePaginatorName,
     ProvisionedResourceEngineType,
@@ -458,68 +463,72 @@
     ServiceDeletedWaiterName,
     ServiceInstanceDeployedWaiterName,
     ServicePipelineDeployedWaiterName,
     ServiceStatusType,
     ServiceTemplateSupportedComponentSourceTypeType,
     ServiceTemplateVersionRegisteredWaiterName,
     ServiceUpdatedWaiterName,
+    SortOrderType,
     SyncTypeType,
     TemplateTypeType,
     TemplateVersionStatusType,
     ProtonServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
 )
 
 
-def check_value(value: ComponentDeletedWaiterName) -> bool:
+def check_value(value: BlockerStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_proton.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_proton.type_defs import (
     AcceptEnvironmentAccountConnectionInputRequestTypeDef,
     EnvironmentAccountConnectionTypeDef,
-    ResponseMetadataTypeDef,
     RepositoryBranchTypeDef,
     CancelComponentDeploymentInputRequestTypeDef,
     ComponentTypeDef,
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
     ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
     ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
     CompatibleEnvironmentTemplateTypeDef,
     ComponentSummaryTypeDef,
+    ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
     EnvironmentTemplateTypeDef,
     EnvironmentTemplateVersionTypeDef,
     RepositoryTypeDef,
+    CreateServiceSyncConfigInputRequestTypeDef,
+    ServiceSyncConfigTypeDef,
     ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
     TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
+    DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
     EnvironmentAccountConnectionSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
     EnvironmentTemplateSummaryTypeDef,
@@ -530,59 +539,84 @@
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
     GetServiceInstanceInputRequestTypeDef,
+    GetServiceInstanceSyncStatusInputRequestTypeDef,
+    RevisionTypeDef,
+    GetServiceSyncBlockerSummaryInputRequestTypeDef,
+    GetServiceSyncConfigInputRequestTypeDef,
     GetServiceTemplateInputRequestTypeDef,
     GetServiceTemplateVersionInputRequestTypeDef,
     GetTemplateSyncConfigInputRequestTypeDef,
     GetTemplateSyncStatusInputRequestTypeDef,
-    RevisionTypeDef,
-    PaginatorConfigTypeDef,
+    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
     ListComponentOutputsInputRequestTypeDef,
     OutputTypeDef,
+    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
     ProvisionedResourceTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
+    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
     ListEnvironmentOutputsInputRequestTypeDef,
+    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
+    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
     ListEnvironmentTemplateVersionsInputRequestTypeDef,
+    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
     ListEnvironmentTemplatesInputRequestTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositorySummaryTypeDef,
+    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
     ListRepositorySyncDefinitionsInputRequestTypeDef,
     RepositorySyncDefinitionTypeDef,
+    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
     ListServiceInstanceOutputsInputRequestTypeDef,
+    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
     ListServiceInstanceProvisionedResourcesInputRequestTypeDef,
-    ListServiceInstancesInputRequestTypeDef,
+    ListServiceInstancesFilterTypeDef,
     ServiceInstanceSummaryTypeDef,
+    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
     ListServicePipelineOutputsInputRequestTypeDef,
+    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
     ListServicePipelineProvisionedResourcesInputRequestTypeDef,
+    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
     ListServiceTemplateVersionsInputRequestTypeDef,
     ServiceTemplateVersionSummaryTypeDef,
+    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
     ListServiceTemplatesInputRequestTypeDef,
     ServiceTemplateSummaryTypeDef,
+    ListServicesInputListServicesPaginateTypeDef,
     ListServicesInputRequestTypeDef,
     ServiceSummaryTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     RejectEnvironmentAccountConnectionInputRequestTypeDef,
     RepositorySyncEventTypeDef,
     ResourceSyncEventTypeDef,
+    ResponseMetadataTypeDef,
     S3ObjectSourceTypeDef,
+    SyncBlockerContextTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateComponentInputRequestTypeDef,
     UpdateEnvironmentAccountConnectionInputRequestTypeDef,
     UpdateEnvironmentTemplateInputRequestTypeDef,
     UpdateEnvironmentTemplateVersionInputRequestTypeDef,
     UpdateServiceInputRequestTypeDef,
     UpdateServiceInstanceInputRequestTypeDef,
     UpdateServicePipelineInputRequestTypeDef,
+    UpdateServiceSyncBlockerInputRequestTypeDef,
+    UpdateServiceSyncConfigInputRequestTypeDef,
     UpdateServiceTemplateInputRequestTypeDef,
     UpdateTemplateSyncConfigInputRequestTypeDef,
     AcceptEnvironmentAccountConnectionOutputTypeDef,
     CreateEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     RejectEnvironmentAccountConnectionOutputTypeDef,
@@ -591,27 +625,30 @@
     EnvironmentTypeDef,
     CancelComponentDeploymentOutputTypeDef,
     CreateComponentOutputTypeDef,
     DeleteComponentOutputTypeDef,
     GetComponentOutputTypeDef,
     UpdateComponentOutputTypeDef,
     CancelServiceInstanceDeploymentOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
     GetServiceInstanceOutputTypeDef,
     UpdateServiceInstanceOutputTypeDef,
     CancelServicePipelineDeploymentOutputTypeDef,
     ServiceTypeDef,
     UpdateServicePipelineOutputTypeDef,
     UpdateServiceTemplateVersionInputRequestTypeDef,
     ServiceTemplateVersionTypeDef,
     ListComponentsOutputTypeDef,
+    CountsSummaryTypeDef,
     CreateComponentInputRequestTypeDef,
     CreateEnvironmentAccountConnectionInputRequestTypeDef,
     CreateEnvironmentTemplateInputRequestTypeDef,
     CreateRepositoryInputRequestTypeDef,
     CreateServiceInputRequestTypeDef,
+    CreateServiceInstanceInputRequestTypeDef,
     CreateServiceTemplateInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     CreateEnvironmentTemplateOutputTypeDef,
@@ -621,75 +658,63 @@
     CreateEnvironmentTemplateVersionOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     UpdateEnvironmentTemplateVersionOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
     GetComponentInputComponentDeployedWaitTypeDef,
     GetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     GetServiceInputServiceCreatedWaitTypeDef,
     GetServiceInputServiceDeletedWaitTypeDef,
     GetServiceInputServicePipelineDeployedWaitTypeDef,
     GetServiceInputServiceUpdatedWaitTypeDef,
     GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
-    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
-    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
-    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
-    ListServicesInputListServicesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListServiceInstanceOutputsOutputTypeDef,
     ListServicePipelineOutputsOutputTypeDef,
     NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServicePipelineProvisionedResourcesOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
+    ListServiceInstancesInputRequestTypeDef,
     ListServiceInstancesOutputTypeDef,
     ListServiceTemplateVersionsOutputTypeDef,
     ListServiceTemplatesOutputTypeDef,
     ListServicesOutputTypeDef,
     RepositorySyncAttemptTypeDef,
     ResourceSyncAttemptTypeDef,
     TemplateVersionSourceInputTypeDef,
+    SyncBlockerTypeDef,
     GetAccountSettingsOutputTypeDef,
     UpdateAccountSettingsOutputTypeDef,
     CancelEnvironmentDeploymentOutputTypeDef,
     CreateEnvironmentOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
@@ -697,60 +722,65 @@
     DeleteServiceOutputTypeDef,
     GetServiceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
+    ServiceSyncBlockerSummaryTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
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

### Comparing `mypy-boto3-proton-1.26.9/mypy_boto3_proton.egg-info/SOURCES.txt` & `mypy-boto3-proton-1.27.0/mypy_boto3_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.26.9/setup.py` & `mypy-boto3-proton-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-proton.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-proton",
-    version="1.26.9",
+    version="1.27.0",
     packages=["mypy_boto3_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Proton 1.26.9 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Proton 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 proton type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_proton": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_proton": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/",
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


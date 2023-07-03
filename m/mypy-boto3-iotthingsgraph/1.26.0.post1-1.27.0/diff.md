# Comparing `tmp/mypy-boto3-iotthingsgraph-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iotthingsgraph-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotthingsgraph-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:34 2022, max compression
+gzip compressed data, was "mypy-boto3-iotthingsgraph-1.27.0.tar", last modified: Mon Jul  3 19:50:56 2023, max compression
```

## Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1.tar` & `mypy-boto3-iotthingsgraph-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.736830 mypy-boto3-iotthingsgraph-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18893 2022-11-01 21:43:34.736830 mypy-boto3-iotthingsgraph-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17424 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.732830 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29251 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    29199 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10485 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10483 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13076 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13064 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    33685 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    33638 2022-11-01 21:36:22.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.736830 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18893 2022-11-01 21:43:34.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-01 21:43:34.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:34.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-01 21:43:34.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:34.736830 mypy-boto3-iotthingsgraph-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-11-01 21:36:21.000000 mypy-boto3-iotthingsgraph-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.547468 mypy-boto3-iotthingsgraph-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-07-03 19:50:56.547468 mypy-boto3-iotthingsgraph-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.523468 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29198 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-03 19:39:53.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-03 19:39:52.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-07-03 19:39:52.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-07-03 19:39:52.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33757 2023-07-03 19:39:54.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33710 2023-07-03 19:39:53.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.547468 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-07-03 19:50:56.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:56.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:56.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:56.000000 mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:56.547468 mypy-boto3-iotthingsgraph-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:39:51.000000 mypy-boto3-iotthingsgraph-1.27.0/setup.py
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/LICENSE` & `mypy-boto3-iotthingsgraph-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTThingsGraph 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTThingsGraph 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
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
 
 <a id="mypy-boto3-iotthingsgraph"></a>
 
 # mypy-boto3-iotthingsgraph
 
 [![PyPI - mypy-boto3-iotthingsgraph](https://img.shields.io/pypi/v/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotthingsgraph?color=blue)](https://pypistats.org/packages/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,90 +381,90 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
-    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
+    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
+    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
+    GetUploadStatusResponseTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
     EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
-    FlowTemplateDescriptionTypeDef,
     CreateFlowTemplateResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DescribeNamespaceResponseTypeDef,
+    FlowTemplateDescriptionTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
-    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
@@ -480,42 +481,42 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/README.md` & `mypy-boto3-iotthingsgraph-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotthingsgraph"></a>
 
 # mypy-boto3-iotthingsgraph
 
 [![PyPI - mypy-boto3-iotthingsgraph](https://img.shields.io/pypi/v/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotthingsgraph?color=blue)](https://pypistats.org/packages/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,90 +349,90 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
-    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
+    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
+    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
+    GetUploadStatusResponseTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
     EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
-    FlowTemplateDescriptionTypeDef,
     CreateFlowTemplateResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DescribeNamespaceResponseTypeDef,
+    FlowTemplateDescriptionTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
-    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
@@ -449,42 +449,42 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/__init__.py` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/__init__.pyi` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/__main__.py` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTThingsGraph 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.IoTThingsGraph 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/client.py` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.delete_system_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/client/#delete_system_template)
         """
 
     def deploy_system_instance(self, *, id: str = ...) -> DeploySystemInstanceResponseTypeDef:
         """
         **Greengrass and Cloud Deployments** Deploys the system instance to the target
-        specified in `CreateSystemInstance` .
+        specified in `CreateSystemInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.deploy_system_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/client/#deploy_system_instance)
         """
 
     def deprecate_flow_template(self, *, id: str) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/client.pyi` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.delete_system_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/client/#delete_system_template)
         """
     def deploy_system_instance(self, *, id: str = ...) -> DeploySystemInstanceResponseTypeDef:
         """
         **Greengrass and Cloud Deployments** Deploys the system instance to the target
-        specified in `CreateSystemInstance` .
+        specified in `CreateSystemInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.deploy_system_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/client/#deploy_system_instance)
         """
     def deprecate_flow_template(self, *, id: str) -> Dict[str, Any]:
         """
         Deprecates the specified workflow.
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/literals.py` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,23 +124,25 @@
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
@@ -150,30 +152,35 @@
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
@@ -199,14 +206,15 @@
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
@@ -251,51 +259,57 @@
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
@@ -308,14 +322,15 @@
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
@@ -327,28 +342,35 @@
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
@@ -357,14 +379,15 @@
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
@@ -375,55 +398,64 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/literals.pyi` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -122,23 +122,25 @@
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
@@ -148,30 +150,35 @@
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
@@ -197,14 +204,15 @@
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
@@ -249,51 +257,57 @@
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
@@ -306,14 +320,15 @@
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
@@ -325,28 +340,35 @@
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
@@ -355,14 +377,15 @@
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
@@ -373,55 +396,64 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/paginator.py` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,60 +88,60 @@
 class GetFlowTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetFlowTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
         """
 
 
 class GetSystemTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSystemTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
         """
 
 
 class ListFlowExecutionMessagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
     """
 
     def paginate(
-        self, *, flowExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, flowExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFlowExecutionMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -153,15 +153,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 
@@ -174,15 +174,15 @@
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 
@@ -192,15 +192,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 
@@ -210,15 +210,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 
@@ -228,15 +228,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 
@@ -247,13 +247,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/paginator.pyi` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -85,57 +85,57 @@
 class GetFlowTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetFlowTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
         """
 
 class GetSystemTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSystemTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
         """
 
 class ListFlowExecutionMessagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
     """
 
     def paginate(
-        self, *, flowExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, flowExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFlowExecutionMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
         """
 
 class SearchEntitiesPaginator(Paginator):
@@ -146,15 +146,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 class SearchFlowExecutionsPaginator(Paginator):
@@ -166,15 +166,15 @@
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 class SearchFlowTemplatesPaginator(Paginator):
@@ -183,15 +183,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 class SearchSystemInstancesPaginator(Paginator):
@@ -200,15 +200,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 class SearchSystemTemplatesPaginator(Paginator):
@@ -217,15 +217,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 class SearchThingsPaginator(Paginator):
@@ -235,13 +235,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/type_defs.py` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,90 +37,90 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
+    "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
     "DeprecateSystemTemplateRequestRequestTypeDef",
     "DescribeNamespaceRequestRequestTypeDef",
+    "DescribeNamespaceResponseTypeDef",
     "DissociateEntityFromThingRequestRequestTypeDef",
     "EntityFilterTypeDef",
     "FlowExecutionMessageTypeDef",
     "FlowExecutionSummaryTypeDef",
     "FlowTemplateFilterTypeDef",
     "GetEntitiesRequestRequestTypeDef",
     "GetFlowTemplateRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
+    "GetNamespaceDeletionStatusResponseTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
+    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
+    "GetUploadStatusResponseTypeDef",
+    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchFlowExecutionsRequestRequestTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
+    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
     "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
-    "FlowTemplateDescriptionTypeDef",
     "CreateFlowTemplateResponseTypeDef",
-    "DeleteNamespaceResponseTypeDef",
-    "DescribeNamespaceResponseTypeDef",
+    "FlowTemplateDescriptionTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    "GetUploadStatusResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
-    "UploadEntityDefinitionsResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
     "SystemTemplateDescriptionTypeDef",
     "UpdateSystemTemplateResponseTypeDef",
     "SystemInstanceDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
+    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
-    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
-    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -167,25 +167,14 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
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
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "cloudMetricEnabled": bool,
         "metricRuleRoleArn": str,
     },
     total=False,
@@ -229,14 +218,23 @@
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSystemInstanceRequestRequestTypeDef = TypedDict(
     "DeleteSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
     total=False,
 )
@@ -283,14 +281,26 @@
     "DescribeNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
     total=False,
 )
 
+DescribeNamespaceResponseTypeDef = TypedDict(
+    "DescribeNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "trackingNamespaceName": str,
+        "trackingNamespaceVersion": int,
+        "namespaceVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DissociateEntityFromThingRequestRequestTypeDef = TypedDict(
     "DissociateEntityFromThingRequestRequestTypeDef",
     {
         "thingName": str,
         "entityType": EntityTypeType,
     },
 )
@@ -374,24 +384,36 @@
 
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "id": str,
+    },
+)
+_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
+    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -407,14 +429,26 @@
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
 
+GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "status": NamespaceDeletionStatusType,
+        "errorCode": Literal["VALIDATION_FAILED"],
+        "errorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSystemInstanceRequestRequestTypeDef = TypedDict(
     "GetSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -435,14 +469,36 @@
 
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
+    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -465,14 +521,50 @@
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
+GetUploadStatusResponseTypeDef = TypedDict(
+    "GetUploadStatusResponseTypeDef",
+    {
+        "uploadId": str,
+        "uploadStatus": UploadStatusType,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "namespaceVersion": int,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+    },
+)
+_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
+    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -488,14 +580,36 @@
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -511,14 +625,35 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
         "systemInstanceId": str,
     },
 )
 _OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
@@ -537,14 +672,39 @@
 class SearchFlowExecutionsRequestRequestTypeDef(
     _RequiredSearchFlowExecutionsRequestRequestTypeDef,
     _OptionalSearchFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
+
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -577,14 +737,37 @@
 
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "entityId": str,
+    },
+)
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "namespaceVersion": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+):
+    pass
+
+
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
     total=False,
@@ -602,14 +785,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UploadEntityDefinitionsResponseTypeDef = TypedDict(
+    "UploadEntityDefinitionsResponseTypeDef",
+    {
+        "uploadId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateFlowTemplateRequestRequestTypeDef = TypedDict(
@@ -714,110 +905,55 @@
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
     total=False,
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
-    {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
-    },
-    total=False,
-)
-
 CreateFlowTemplateResponseTypeDef = TypedDict(
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeNamespaceResponseTypeDef = TypedDict(
-    "DescribeNamespaceResponseTypeDef",
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
     {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "trackingNamespaceName": str,
-        "trackingNamespaceVersion": int,
-        "namespaceVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
     },
+    total=False,
 )
 
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "status": NamespaceDeletionStatusType,
-        "errorCode": Literal["VALIDATION_FAILED"],
-        "errorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUploadStatusResponseTypeDef = TypedDict(
-    "GetUploadStatusResponseTypeDef",
-    {
-        "uploadId": str,
-        "uploadStatus": UploadStatusType,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "namespaceVersion": int,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchFlowTemplatesResponseTypeDef = TypedDict(
     "SearchFlowTemplatesResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowTemplateResponseTypeDef = TypedDict(
     "UpdateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UploadEntityDefinitionsResponseTypeDef = TypedDict(
-    "UploadEntityDefinitionsResponseTypeDef",
-    {
-        "uploadId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSystemInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemInstanceRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
@@ -845,15 +981,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -861,67 +997,67 @@
     },
 )
 
 CreateSystemInstanceResponseTypeDef = TypedDict(
     "CreateSystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploySystemInstanceResponseTypeDef = TypedDict(
     "DeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
         "greengrassDeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchSystemInstancesResponseTypeDef = TypedDict(
     "SearchSystemInstancesResponseTypeDef",
     {
         "summaries": List[SystemInstanceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UndeploySystemInstanceResponseTypeDef = TypedDict(
     "UndeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSystemTemplateResponseTypeDef = TypedDict(
     "CreateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSystemTemplateRevisionsResponseTypeDef = TypedDict(
     "GetSystemTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchSystemTemplatesResponseTypeDef = TypedDict(
     "SearchSystemTemplatesResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SystemTemplateDescriptionTypeDef = TypedDict(
     "SystemTemplateDescriptionTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
@@ -931,15 +1067,15 @@
     total=False,
 )
 
 UpdateSystemTemplateResponseTypeDef = TypedDict(
     "UpdateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SystemInstanceDescriptionTypeDef = TypedDict(
     "SystemInstanceDescriptionTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
@@ -973,226 +1109,90 @@
 
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
 
-ListFlowExecutionMessagesResponseTypeDef = TypedDict(
-    "ListFlowExecutionMessagesResponseTypeDef",
-    {
-        "messages": List[FlowExecutionMessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchFlowExecutionsResponseTypeDef = TypedDict(
-    "SearchFlowExecutionsResponseTypeDef",
-    {
-        "summaries": List[FlowExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestRequestTypeDef",
-    {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
-    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
-    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-    },
-)
-_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
-    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+ListFlowExecutionMessagesResponseTypeDef = TypedDict(
+    "ListFlowExecutionMessagesResponseTypeDef",
     {
-        "systemInstanceId": str,
+        "messages": List[FlowExecutionMessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+
+SearchFlowExecutionsResponseTypeDef = TypedDict(
+    "SearchFlowExecutionsResponseTypeDef",
     {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "summaries": List[FlowExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
-
-
-SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestRequestTypeDef",
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "entityId": str,
-    },
-)
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
-        "namespaceVersion": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
-):
-    pass
-
-
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = TypedDict(
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 SearchSystemTemplatesRequestRequestTypeDef = TypedDict(
     "SearchSystemTemplatesRequestRequestTypeDef",
     {
@@ -1203,61 +1203,61 @@
     total=False,
 )
 
 SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = TypedDict(
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     {
         "filters": Sequence[SystemTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 SearchThingsResponseTypeDef = TypedDict(
     "SearchThingsResponseTypeDef",
     {
         "things": List[ThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEntitiesResponseTypeDef = TypedDict(
     "GetEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchEntitiesResponseTypeDef = TypedDict(
     "SearchEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFlowTemplateResponseTypeDef = TypedDict(
     "GetFlowTemplateResponseTypeDef",
     {
         "description": FlowTemplateDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSystemTemplateResponseTypeDef = TypedDict(
     "GetSystemTemplateResponseTypeDef",
     {
         "description": SystemTemplateDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSystemInstanceResponseTypeDef = TypedDict(
     "GetSystemInstanceResponseTypeDef",
     {
         "description": SystemInstanceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph/type_defs.pyi` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,90 +36,90 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
+    "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
     "DeprecateSystemTemplateRequestRequestTypeDef",
     "DescribeNamespaceRequestRequestTypeDef",
+    "DescribeNamespaceResponseTypeDef",
     "DissociateEntityFromThingRequestRequestTypeDef",
     "EntityFilterTypeDef",
     "FlowExecutionMessageTypeDef",
     "FlowExecutionSummaryTypeDef",
     "FlowTemplateFilterTypeDef",
     "GetEntitiesRequestRequestTypeDef",
     "GetFlowTemplateRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
+    "GetNamespaceDeletionStatusResponseTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
+    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
+    "GetUploadStatusResponseTypeDef",
+    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchFlowExecutionsRequestRequestTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
+    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
     "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
-    "FlowTemplateDescriptionTypeDef",
     "CreateFlowTemplateResponseTypeDef",
-    "DeleteNamespaceResponseTypeDef",
-    "DescribeNamespaceResponseTypeDef",
+    "FlowTemplateDescriptionTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    "GetUploadStatusResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
-    "UploadEntityDefinitionsResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
     "SystemTemplateDescriptionTypeDef",
     "UpdateSystemTemplateResponseTypeDef",
     "SystemInstanceDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
+    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
-    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
-    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -164,25 +164,14 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
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
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "cloudMetricEnabled": bool,
         "metricRuleRoleArn": str,
     },
     total=False,
@@ -226,14 +215,23 @@
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSystemInstanceRequestRequestTypeDef = TypedDict(
     "DeleteSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
     total=False,
 )
@@ -280,14 +278,26 @@
     "DescribeNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
     total=False,
 )
 
+DescribeNamespaceResponseTypeDef = TypedDict(
+    "DescribeNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "trackingNamespaceName": str,
+        "trackingNamespaceVersion": int,
+        "namespaceVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DissociateEntityFromThingRequestRequestTypeDef = TypedDict(
     "DissociateEntityFromThingRequestRequestTypeDef",
     {
         "thingName": str,
         "entityType": EntityTypeType,
     },
 )
@@ -367,24 +377,34 @@
 )
 
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "id": str,
+    },
+)
+_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
+    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -398,14 +418,26 @@
 
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
+GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "status": NamespaceDeletionStatusType,
+        "errorCode": Literal["VALIDATION_FAILED"],
+        "errorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSystemInstanceRequestRequestTypeDef = TypedDict(
     "GetSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -424,14 +456,34 @@
 )
 
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
+    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -452,14 +504,48 @@
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
+GetUploadStatusResponseTypeDef = TypedDict(
+    "GetUploadStatusResponseTypeDef",
+    {
+        "uploadId": str,
+        "uploadStatus": UploadStatusType,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "namespaceVersion": int,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+    },
+)
+_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
+    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+):
+    pass
+
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -473,14 +559,34 @@
 
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -494,14 +600,35 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
         "systemInstanceId": str,
     },
 )
 _OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
@@ -518,14 +645,37 @@
 
 class SearchFlowExecutionsRequestRequestTypeDef(
     _RequiredSearchFlowExecutionsRequestRequestTypeDef,
     _OptionalSearchFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -556,14 +706,35 @@
 )
 
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "entityId": str,
+    },
+)
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "namespaceVersion": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+):
+    pass
+
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
     total=False,
@@ -581,14 +752,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UploadEntityDefinitionsResponseTypeDef = TypedDict(
+    "UploadEntityDefinitionsResponseTypeDef",
+    {
+        "uploadId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateFlowTemplateRequestRequestTypeDef = TypedDict(
@@ -685,110 +864,55 @@
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
     total=False,
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
-    {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
-    },
-    total=False,
-)
-
 CreateFlowTemplateResponseTypeDef = TypedDict(
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeNamespaceResponseTypeDef = TypedDict(
-    "DescribeNamespaceResponseTypeDef",
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
     {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "trackingNamespaceName": str,
-        "trackingNamespaceVersion": int,
-        "namespaceVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
     },
+    total=False,
 )
 
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "status": NamespaceDeletionStatusType,
-        "errorCode": Literal["VALIDATION_FAILED"],
-        "errorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUploadStatusResponseTypeDef = TypedDict(
-    "GetUploadStatusResponseTypeDef",
-    {
-        "uploadId": str,
-        "uploadStatus": UploadStatusType,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "namespaceVersion": int,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchFlowTemplatesResponseTypeDef = TypedDict(
     "SearchFlowTemplatesResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowTemplateResponseTypeDef = TypedDict(
     "UpdateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UploadEntityDefinitionsResponseTypeDef = TypedDict(
-    "UploadEntityDefinitionsResponseTypeDef",
-    {
-        "uploadId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSystemInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemInstanceRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
@@ -814,15 +938,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -830,67 +954,67 @@
     },
 )
 
 CreateSystemInstanceResponseTypeDef = TypedDict(
     "CreateSystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploySystemInstanceResponseTypeDef = TypedDict(
     "DeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
         "greengrassDeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchSystemInstancesResponseTypeDef = TypedDict(
     "SearchSystemInstancesResponseTypeDef",
     {
         "summaries": List[SystemInstanceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UndeploySystemInstanceResponseTypeDef = TypedDict(
     "UndeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSystemTemplateResponseTypeDef = TypedDict(
     "CreateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSystemTemplateRevisionsResponseTypeDef = TypedDict(
     "GetSystemTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchSystemTemplatesResponseTypeDef = TypedDict(
     "SearchSystemTemplatesResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SystemTemplateDescriptionTypeDef = TypedDict(
     "SystemTemplateDescriptionTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
@@ -900,15 +1024,15 @@
     total=False,
 )
 
 UpdateSystemTemplateResponseTypeDef = TypedDict(
     "UpdateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SystemInstanceDescriptionTypeDef = TypedDict(
     "SystemInstanceDescriptionTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
@@ -940,212 +1064,88 @@
 )
 
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
-ListFlowExecutionMessagesResponseTypeDef = TypedDict(
-    "ListFlowExecutionMessagesResponseTypeDef",
-    {
-        "messages": List[FlowExecutionMessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchFlowExecutionsResponseTypeDef = TypedDict(
-    "SearchFlowExecutionsResponseTypeDef",
-    {
-        "summaries": List[FlowExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestRequestTypeDef",
-    {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
-    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
-    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-    },
-)
-_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
-    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-):
-    pass
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+ListFlowExecutionMessagesResponseTypeDef = TypedDict(
+    "ListFlowExecutionMessagesResponseTypeDef",
     {
-        "systemInstanceId": str,
+        "messages": List[FlowExecutionMessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+
+SearchFlowExecutionsResponseTypeDef = TypedDict(
+    "SearchFlowExecutionsResponseTypeDef",
     {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "summaries": List[FlowExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
-
-SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestRequestTypeDef",
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "entityId": str,
-    },
-)
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
-        "namespaceVersion": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
-):
-    pass
-
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = TypedDict(
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 SearchSystemTemplatesRequestRequestTypeDef = TypedDict(
     "SearchSystemTemplatesRequestRequestTypeDef",
     {
@@ -1156,61 +1156,61 @@
     total=False,
 )
 
 SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = TypedDict(
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     {
         "filters": Sequence[SystemTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 SearchThingsResponseTypeDef = TypedDict(
     "SearchThingsResponseTypeDef",
     {
         "things": List[ThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEntitiesResponseTypeDef = TypedDict(
     "GetEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchEntitiesResponseTypeDef = TypedDict(
     "SearchEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFlowTemplateResponseTypeDef = TypedDict(
     "GetFlowTemplateResponseTypeDef",
     {
         "description": FlowTemplateDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSystemTemplateResponseTypeDef = TypedDict(
     "GetSystemTemplateResponseTypeDef",
     {
         "description": SystemTemplateDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSystemInstanceResponseTypeDef = TypedDict(
     "GetSystemInstanceResponseTypeDef",
     {
         "description": SystemInstanceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTThingsGraph 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTThingsGraph 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
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
 
 <a id="mypy-boto3-iotthingsgraph"></a>
 
 # mypy-boto3-iotthingsgraph
 
 [![PyPI - mypy-boto3-iotthingsgraph](https://img.shields.io/pypi/v/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotthingsgraph?color=blue)](https://pypistats.org/packages/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,90 +381,90 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
-    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
+    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
+    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
+    GetUploadStatusResponseTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
     EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
-    FlowTemplateDescriptionTypeDef,
     CreateFlowTemplateResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DescribeNamespaceResponseTypeDef,
+    FlowTemplateDescriptionTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
-    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
@@ -480,42 +481,42 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt` & `mypy-boto3-iotthingsgraph-1.27.0/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.26.0.post1/setup.py` & `mypy-boto3-iotthingsgraph-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iotthingsgraph.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotthingsgraph",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTThingsGraph 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.IoTThingsGraph 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iotthingsgraph": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iotthingsgraph": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/",
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


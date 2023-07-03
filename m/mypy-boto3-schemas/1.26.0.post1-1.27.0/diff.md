# Comparing `tmp/mypy-boto3-schemas-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-schemas-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-schemas-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:58 2022, max compression
+gzip compressed data, was "mypy-boto3-schemas-1.27.0.tar", last modified: Mon Jul  3 19:51:25 2023, max compression
```

## Comparing `mypy-boto3-schemas-1.26.0.post1.tar` & `mypy-boto3-schemas-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.436848 mypy-boto3-schemas-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16647 2022-11-01 21:43:58.424848 mypy-boto3-schemas-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15206 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.424848 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23385 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    23341 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8240 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8238 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    26113 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    26074 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-11-01 21:40:57.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.424848 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16647 2022-11-01 21:43:58.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-11-01 21:43:58.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:58.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:58.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:58.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-01 21:43:58.000000 mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:58.436848 mypy-boto3-schemas-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-11-01 21:40:56.000000 mypy-boto3-schemas-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-07-03 19:47:34.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-03 19:47:34.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/setup.py
```

### Comparing `mypy-boto3-schemas-1.26.0.post1/LICENSE` & `mypy-boto3-schemas-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-schemas-1.26.0.post1/PKG-INFO` & `mypy-boto3-schemas-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Schemas 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Schemas 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
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
 
 <a id="mypy-boto3-schemas"></a>
 
 # mypy-boto3-schemas
 
 [![PyPI - mypy-boto3-schemas](https://img.shields.io/pypi/v/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,79 +360,79 @@
 
 `mypy_boto3_schemas.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDiscovererResponseTypeDef,
     CreateRegistryRequestRequestTypeDef,
+    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
+    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
+    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
+    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
+    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
+    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
     ListDiscoverersRequestRequestTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
+    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
+    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
+    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateRegistryRequestRequestTypeDef,
-    UpdateSchemaRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DescribeCodeBindingResponseTypeDef,
-    DescribeDiscovererResponseTypeDef,
-    DescribeRegistryResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportSchemaResponseTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutCodeBindingResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartDiscovererResponseTypeDef,
-    StopDiscovererResponseTypeDef,
     UpdateDiscovererResponseTypeDef,
+    UpdateRegistryRequestRequestTypeDef,
     UpdateRegistryResponseTypeDef,
+    UpdateSchemaRequestRequestTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
 
@@ -443,42 +444,42 @@
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

### Comparing `mypy-boto3-schemas-1.26.0.post1/README.md` & `mypy-boto3-schemas-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-schemas"></a>
 
 # mypy-boto3-schemas
 
 [![PyPI - mypy-boto3-schemas](https://img.shields.io/pypi/v/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,79 +328,79 @@
 
 `mypy_boto3_schemas.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDiscovererResponseTypeDef,
     CreateRegistryRequestRequestTypeDef,
+    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
+    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
+    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
+    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
+    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
+    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
     ListDiscoverersRequestRequestTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
+    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
+    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
+    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateRegistryRequestRequestTypeDef,
-    UpdateSchemaRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DescribeCodeBindingResponseTypeDef,
-    DescribeDiscovererResponseTypeDef,
-    DescribeRegistryResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportSchemaResponseTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutCodeBindingResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartDiscovererResponseTypeDef,
-    StopDiscovererResponseTypeDef,
     UpdateDiscovererResponseTypeDef,
+    UpdateRegistryRequestRequestTypeDef,
     UpdateRegistryResponseTypeDef,
+    UpdateSchemaRequestRequestTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
 
@@ -412,42 +412,42 @@
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

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/__init__.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/__init__.pyi` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/__main__.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Schemas 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Schemas 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/client.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/client.pyi` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/literals.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,23 +59,25 @@
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
@@ -85,30 +87,35 @@
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
@@ -134,14 +141,15 @@
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
@@ -186,51 +194,57 @@
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
@@ -243,14 +257,15 @@
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
@@ -262,28 +277,35 @@
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
@@ -292,14 +314,15 @@
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
@@ -310,55 +333,64 @@
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

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/literals.pyi` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,23 +57,25 @@
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
@@ -83,30 +85,35 @@
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
@@ -132,14 +139,15 @@
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
@@ -184,51 +192,57 @@
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
@@ -241,14 +255,15 @@
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
@@ -260,28 +275,35 @@
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
@@ -290,14 +312,15 @@
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
@@ -308,55 +331,64 @@
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

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/paginator.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,103 +44,100 @@
     "ListDiscoverersPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
     "SearchSchemasPaginator",
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
 class ListDiscoverersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listdiscovererspaginator)
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listdiscovererspaginator)
         """
 
-
 class ListRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listregistriespaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listregistriespaginator)
         """
 
-
 class ListSchemaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self, *, RegistryName: str, SchemaName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        RegistryName: str,
+        SchemaName: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
         """
 
-
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaspaginator)
         """
 
-
 class SearchSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
     """
 
     def paginate(
-        self, *, Keywords: str, RegistryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Keywords: str, RegistryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
         """
```

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/paginator.pyi` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,96 +44,107 @@
     "ListDiscoverersPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
     "SearchSchemasPaginator",
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
 class ListDiscoverersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listdiscovererspaginator)
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listdiscovererspaginator)
         """
 
+
 class ListRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listregistriespaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listregistriespaginator)
         """
 
+
 class ListSchemaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self, *, RegistryName: str, SchemaName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        RegistryName: str,
+        SchemaName: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
         """
 
+
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaspaginator)
         """
 
+
 class SearchSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
     """
 
     def paginate(
-        self, *, Keywords: str, RegistryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Keywords: str, RegistryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
         """
```

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/type_defs.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,79 +23,79 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateDiscovererRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDiscovererResponseTypeDef",
     "CreateRegistryRequestRequestTypeDef",
+    "CreateRegistryResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "CreateSchemaResponseTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSchemaVersionRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeBindingRequestRequestTypeDef",
+    "DescribeCodeBindingResponseTypeDef",
     "DescribeDiscovererRequestRequestTypeDef",
+    "DescribeDiscovererResponseTypeDef",
     "DescribeRegistryRequestRequestTypeDef",
+    "DescribeRegistryResponseTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
+    "DescribeSchemaResponseTypeDef",
     "DiscovererSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportSchemaRequestRequestTypeDef",
+    "ExportSchemaResponseTypeDef",
     "GetCodeBindingSourceRequestRequestTypeDef",
+    "GetCodeBindingSourceResponseTypeDef",
     "GetDiscoveredSchemaRequestRequestTypeDef",
+    "GetDiscoveredSchemaResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
     "ListDiscoverersRequestRequestTypeDef",
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
     "ListRegistriesRequestRequestTypeDef",
     "RegistrySummaryTypeDef",
+    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsRequestRequestTypeDef",
     "SchemaVersionSummaryTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutCodeBindingRequestRequestTypeDef",
+    "PutCodeBindingResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchSchemaVersionSummaryTypeDef",
     "SearchSchemasRequestRequestTypeDef",
+    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "StartDiscovererRequestRequestTypeDef",
+    "StartDiscovererResponseTypeDef",
     "StopDiscovererRequestRequestTypeDef",
+    "StopDiscovererResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDiscovererRequestRequestTypeDef",
-    "UpdateRegistryRequestRequestTypeDef",
-    "UpdateSchemaRequestRequestTypeDef",
-    "CreateDiscovererResponseTypeDef",
-    "CreateRegistryResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "DescribeCodeBindingResponseTypeDef",
-    "DescribeDiscovererResponseTypeDef",
-    "DescribeRegistryResponseTypeDef",
-    "DescribeSchemaResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportSchemaResponseTypeDef",
-    "GetCodeBindingSourceResponseTypeDef",
-    "GetDiscoveredSchemaResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutCodeBindingResponseTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "StartDiscovererResponseTypeDef",
-    "StopDiscovererResponseTypeDef",
     "UpdateDiscovererResponseTypeDef",
+    "UpdateRegistryRequestRequestTypeDef",
     "UpdateRegistryResponseTypeDef",
+    "UpdateSchemaRequestRequestTypeDef",
     "UpdateSchemaResponseTypeDef",
     "DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     "ListDiscoverersResponseTypeDef",
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "SearchSchemaSummaryTypeDef",
     "SearchSchemasResponseTypeDef",
 )
 
@@ -118,22 +118,25 @@
 
 class CreateDiscovererRequestRequestTypeDef(
     _RequiredCreateDiscovererRequestRequestTypeDef, _OptionalCreateDiscovererRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDiscovererResponseTypeDef = TypedDict(
+    "CreateDiscovererResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
@@ -151,14 +154,25 @@
 
 class CreateRegistryRequestRequestTypeDef(
     _RequiredCreateRegistryRequestRequestTypeDef, _OptionalCreateRegistryRequestRequestTypeDef
 ):
     pass
 
 
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "Content": str,
         "RegistryName": str,
         "SchemaName": str,
         "Type": TypeType,
@@ -176,14 +190,29 @@
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDiscovererRequestRequestTypeDef = TypedDict(
     "DeleteDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
@@ -248,28 +277,64 @@
 class DescribeCodeBindingRequestRequestTypeDef(
     _RequiredDescribeCodeBindingRequestRequestTypeDef,
     _OptionalDescribeCodeBindingRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeCodeBindingResponseTypeDef = TypedDict(
+    "DescribeCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDiscovererRequestRequestTypeDef = TypedDict(
     "DescribeDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
+DescribeDiscovererResponseTypeDef = TypedDict(
+    "DescribeDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRegistryRequestRequestTypeDef = TypedDict(
     "DescribeRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 
+DescribeRegistryResponseTypeDef = TypedDict(
+    "DescribeRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -284,27 +349,50 @@
 
 class DescribeSchemaRequestRequestTypeDef(
     _RequiredDescribeSchemaRequestRequestTypeDef, _OptionalDescribeSchemaRequestRequestTypeDef
 ):
     pass
 
 
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DiscovererSummaryTypeDef = TypedDict(
     "DiscovererSummaryTypeDef",
     {
         "DiscovererArn": str,
         "DiscovererId": str,
         "SourceArn": str,
         "State": DiscovererStateType,
         "CrossAccount": bool,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredExportSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredExportSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "Type": str,
     },
@@ -320,14 +408,26 @@
 
 class ExportSchemaRequestRequestTypeDef(
     _RequiredExportSchemaRequestRequestTypeDef, _OptionalExportSchemaRequestRequestTypeDef
 ):
     pass
 
 
+ExportSchemaResponseTypeDef = TypedDict(
+    "ExportSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Type": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetCodeBindingSourceRequestRequestTypeDef = TypedDict(
     "_RequiredGetCodeBindingSourceRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -344,36 +444,61 @@
 class GetCodeBindingSourceRequestRequestTypeDef(
     _RequiredGetCodeBindingSourceRequestRequestTypeDef,
     _OptionalGetCodeBindingSourceRequestRequestTypeDef,
 ):
     pass
 
 
+GetCodeBindingSourceResponseTypeDef = TypedDict(
+    "GetCodeBindingSourceResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDiscoveredSchemaRequestRequestTypeDef = TypedDict(
     "GetDiscoveredSchemaRequestRequestTypeDef",
     {
         "Events": Sequence[str],
         "Type": TypeType,
     },
 )
 
+GetDiscoveredSchemaResponseTypeDef = TypedDict(
+    "GetDiscoveredSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    {
+        "DiscovererIdPrefix": str,
+        "SourceArnPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDiscoverersRequestRequestTypeDef = TypedDict(
     "ListDiscoverersRequestRequestTypeDef",
     {
@@ -381,14 +506,24 @@
         "Limit": int,
         "NextToken": str,
         "SourceArnPrefix": str,
     },
     total=False,
 )
 
+ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    {
+        "RegistryNamePrefix": str,
+        "Scope": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRegistriesRequestRequestTypeDef = TypedDict(
     "ListRegistriesRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
         "RegistryNamePrefix": str,
         "Scope": str,
@@ -402,14 +537,37 @@
         "RegistryArn": str,
         "RegistryName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "RegistryName": str,
+        "SchemaName": str,
+    },
+)
+_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSchemaVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -437,14 +595,37 @@
         "SchemaName": str,
         "SchemaVersion": str,
         "Type": TypeType,
     },
     total=False,
 )
 
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "RegistryName": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "SchemaNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -479,14 +660,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 _RequiredPutCodeBindingRequestRequestTypeDef = TypedDict(
     "_RequiredPutCodeBindingRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -502,14 +701,25 @@
 
 class PutCodeBindingRequestRequestTypeDef(
     _RequiredPutCodeBindingRequestRequestTypeDef, _OptionalPutCodeBindingRequestRequestTypeDef
 ):
     pass
 
 
+PutCodeBindingResponseTypeDef = TypedDict(
+    "PutCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -524,14 +734,34 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
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
 SearchSchemaVersionSummaryTypeDef = TypedDict(
     "SearchSchemaVersionSummaryTypeDef",
     {
         "CreatedDate": datetime,
         "SchemaVersion": str,
         "Type": TypeType,
     },
@@ -557,28 +787,69 @@
 
 class SearchSchemasRequestRequestTypeDef(
     _RequiredSearchSchemasRequestRequestTypeDef, _OptionalSearchSchemasRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "Keywords": str,
+        "RegistryName": str,
+    },
+)
+_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SearchSchemasRequestSearchSchemasPaginateTypeDef(
+    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
+    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
+):
+    pass
+
+
 StartDiscovererRequestRequestTypeDef = TypedDict(
     "StartDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
+StartDiscovererResponseTypeDef = TypedDict(
+    "StartDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopDiscovererRequestRequestTypeDef = TypedDict(
     "StopDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
+StopDiscovererResponseTypeDef = TypedDict(
+    "StopDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -609,14 +880,28 @@
 
 class UpdateDiscovererRequestRequestTypeDef(
     _RequiredUpdateDiscovererRequestRequestTypeDef, _OptionalUpdateDiscovererRequestRequestTypeDef
 ):
     pass
 
 
+UpdateDiscovererResponseTypeDef = TypedDict(
+    "UpdateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalUpdateRegistryRequestRequestTypeDef = TypedDict(
@@ -630,14 +915,25 @@
 
 class UpdateRegistryRequestRequestTypeDef(
     _RequiredUpdateRegistryRequestRequestTypeDef, _OptionalUpdateRegistryRequestRequestTypeDef
 ):
     pass
 
 
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -655,233 +951,26 @@
 
 class UpdateSchemaRequestRequestTypeDef(
     _RequiredUpdateSchemaRequestRequestTypeDef, _OptionalUpdateSchemaRequestRequestTypeDef
 ):
     pass
 
 
-CreateDiscovererResponseTypeDef = TypedDict(
-    "CreateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCodeBindingResponseTypeDef = TypedDict(
-    "DescribeCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDiscovererResponseTypeDef = TypedDict(
-    "DescribeDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRegistryResponseTypeDef = TypedDict(
-    "DescribeRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
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
-ExportSchemaResponseTypeDef = TypedDict(
-    "ExportSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Type": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCodeBindingSourceResponseTypeDef = TypedDict(
-    "GetCodeBindingSourceResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDiscoveredSchemaResponseTypeDef = TypedDict(
-    "GetDiscoveredSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutCodeBindingResponseTypeDef = TypedDict(
-    "PutCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDiscovererResponseTypeDef = TypedDict(
-    "StartDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopDiscovererResponseTypeDef = TypedDict(
-    "StopDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDiscovererResponseTypeDef = TypedDict(
-    "UpdateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateSchemaResponseTypeDef = TypedDict(
     "UpdateSchemaResponseTypeDef",
     {
         "Description": str,
         "LastModified": datetime,
         "SchemaArn": str,
         "SchemaName": str,
         "SchemaVersion": str,
         "Tags": Dict[str, str],
         "Type": str,
         "VersionCreatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     {
         "Language": str,
@@ -907,131 +996,42 @@
 
 
 ListDiscoverersResponseTypeDef = TypedDict(
     "ListDiscoverersResponseTypeDef",
     {
         "Discoverers": List[DiscovererSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
-    {
-        "DiscovererIdPrefix": str,
-        "SourceArnPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    {
-        "RegistryNamePrefix": str,
-        "Scope": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "RegistryName": str,
-        "SchemaName": str,
-    },
-)
-_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "RegistryName": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "SchemaNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-
-_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "Keywords": str,
-        "RegistryName": str,
-    },
-)
-_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class SearchSchemasRequestSearchSchemasPaginateTypeDef(
-    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
-    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
-):
-    pass
-
-
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "NextToken": str,
         "Registries": List[RegistrySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "NextToken": str,
         "SchemaVersions": List[SchemaVersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SchemaSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchSchemaSummaryTypeDef = TypedDict(
     "SearchSchemaSummaryTypeDef",
     {
         "RegistryName": str,
@@ -1043,10 +1043,10 @@
 )
 
 SearchSchemasResponseTypeDef = TypedDict(
     "SearchSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SearchSchemaSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/type_defs.pyi` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,79 +22,79 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateDiscovererRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDiscovererResponseTypeDef",
     "CreateRegistryRequestRequestTypeDef",
+    "CreateRegistryResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "CreateSchemaResponseTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSchemaVersionRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeBindingRequestRequestTypeDef",
+    "DescribeCodeBindingResponseTypeDef",
     "DescribeDiscovererRequestRequestTypeDef",
+    "DescribeDiscovererResponseTypeDef",
     "DescribeRegistryRequestRequestTypeDef",
+    "DescribeRegistryResponseTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
+    "DescribeSchemaResponseTypeDef",
     "DiscovererSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportSchemaRequestRequestTypeDef",
+    "ExportSchemaResponseTypeDef",
     "GetCodeBindingSourceRequestRequestTypeDef",
+    "GetCodeBindingSourceResponseTypeDef",
     "GetDiscoveredSchemaRequestRequestTypeDef",
+    "GetDiscoveredSchemaResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
     "ListDiscoverersRequestRequestTypeDef",
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
     "ListRegistriesRequestRequestTypeDef",
     "RegistrySummaryTypeDef",
+    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsRequestRequestTypeDef",
     "SchemaVersionSummaryTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutCodeBindingRequestRequestTypeDef",
+    "PutCodeBindingResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchSchemaVersionSummaryTypeDef",
     "SearchSchemasRequestRequestTypeDef",
+    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "StartDiscovererRequestRequestTypeDef",
+    "StartDiscovererResponseTypeDef",
     "StopDiscovererRequestRequestTypeDef",
+    "StopDiscovererResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDiscovererRequestRequestTypeDef",
-    "UpdateRegistryRequestRequestTypeDef",
-    "UpdateSchemaRequestRequestTypeDef",
-    "CreateDiscovererResponseTypeDef",
-    "CreateRegistryResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "DescribeCodeBindingResponseTypeDef",
-    "DescribeDiscovererResponseTypeDef",
-    "DescribeRegistryResponseTypeDef",
-    "DescribeSchemaResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportSchemaResponseTypeDef",
-    "GetCodeBindingSourceResponseTypeDef",
-    "GetDiscoveredSchemaResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutCodeBindingResponseTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "StartDiscovererResponseTypeDef",
-    "StopDiscovererResponseTypeDef",
     "UpdateDiscovererResponseTypeDef",
+    "UpdateRegistryRequestRequestTypeDef",
     "UpdateRegistryResponseTypeDef",
+    "UpdateSchemaRequestRequestTypeDef",
     "UpdateSchemaResponseTypeDef",
     "DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     "ListDiscoverersResponseTypeDef",
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
-    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "SearchSchemaSummaryTypeDef",
     "SearchSchemasResponseTypeDef",
 )
 
@@ -115,22 +115,25 @@
 )
 
 class CreateDiscovererRequestRequestTypeDef(
     _RequiredCreateDiscovererRequestRequestTypeDef, _OptionalCreateDiscovererRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDiscovererResponseTypeDef = TypedDict(
+    "CreateDiscovererResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
@@ -146,14 +149,25 @@
 )
 
 class CreateRegistryRequestRequestTypeDef(
     _RequiredCreateRegistryRequestRequestTypeDef, _OptionalCreateRegistryRequestRequestTypeDef
 ):
     pass
 
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "Content": str,
         "RegistryName": str,
         "SchemaName": str,
         "Type": TypeType,
@@ -169,14 +183,29 @@
 )
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDiscovererRequestRequestTypeDef = TypedDict(
     "DeleteDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
@@ -239,28 +268,64 @@
 
 class DescribeCodeBindingRequestRequestTypeDef(
     _RequiredDescribeCodeBindingRequestRequestTypeDef,
     _OptionalDescribeCodeBindingRequestRequestTypeDef,
 ):
     pass
 
+DescribeCodeBindingResponseTypeDef = TypedDict(
+    "DescribeCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDiscovererRequestRequestTypeDef = TypedDict(
     "DescribeDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
+DescribeDiscovererResponseTypeDef = TypedDict(
+    "DescribeDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRegistryRequestRequestTypeDef = TypedDict(
     "DescribeRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 
+DescribeRegistryResponseTypeDef = TypedDict(
+    "DescribeRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -273,27 +338,50 @@
 )
 
 class DescribeSchemaRequestRequestTypeDef(
     _RequiredDescribeSchemaRequestRequestTypeDef, _OptionalDescribeSchemaRequestRequestTypeDef
 ):
     pass
 
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DiscovererSummaryTypeDef = TypedDict(
     "DiscovererSummaryTypeDef",
     {
         "DiscovererArn": str,
         "DiscovererId": str,
         "SourceArn": str,
         "State": DiscovererStateType,
         "CrossAccount": bool,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredExportSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredExportSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "Type": str,
     },
@@ -307,14 +395,26 @@
 )
 
 class ExportSchemaRequestRequestTypeDef(
     _RequiredExportSchemaRequestRequestTypeDef, _OptionalExportSchemaRequestRequestTypeDef
 ):
     pass
 
+ExportSchemaResponseTypeDef = TypedDict(
+    "ExportSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Type": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetCodeBindingSourceRequestRequestTypeDef = TypedDict(
     "_RequiredGetCodeBindingSourceRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -329,36 +429,61 @@
 
 class GetCodeBindingSourceRequestRequestTypeDef(
     _RequiredGetCodeBindingSourceRequestRequestTypeDef,
     _OptionalGetCodeBindingSourceRequestRequestTypeDef,
 ):
     pass
 
+GetCodeBindingSourceResponseTypeDef = TypedDict(
+    "GetCodeBindingSourceResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDiscoveredSchemaRequestRequestTypeDef = TypedDict(
     "GetDiscoveredSchemaRequestRequestTypeDef",
     {
         "Events": Sequence[str],
         "Type": TypeType,
     },
 )
 
+GetDiscoveredSchemaResponseTypeDef = TypedDict(
+    "GetDiscoveredSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    {
+        "DiscovererIdPrefix": str,
+        "SourceArnPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDiscoverersRequestRequestTypeDef = TypedDict(
     "ListDiscoverersRequestRequestTypeDef",
     {
@@ -366,14 +491,24 @@
         "Limit": int,
         "NextToken": str,
         "SourceArnPrefix": str,
     },
     total=False,
 )
 
+ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    {
+        "RegistryNamePrefix": str,
+        "Scope": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRegistriesRequestRequestTypeDef = TypedDict(
     "ListRegistriesRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
         "RegistryNamePrefix": str,
         "Scope": str,
@@ -387,14 +522,35 @@
         "RegistryArn": str,
         "RegistryName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "RegistryName": str,
+        "SchemaName": str,
+    },
+)
+_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListSchemaVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -420,14 +576,35 @@
         "SchemaName": str,
         "SchemaVersion": str,
         "Type": TypeType,
     },
     total=False,
 )
 
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "RegistryName": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "SchemaNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -460,14 +637,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 _RequiredPutCodeBindingRequestRequestTypeDef = TypedDict(
     "_RequiredPutCodeBindingRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -481,14 +676,25 @@
 )
 
 class PutCodeBindingRequestRequestTypeDef(
     _RequiredPutCodeBindingRequestRequestTypeDef, _OptionalPutCodeBindingRequestRequestTypeDef
 ):
     pass
 
+PutCodeBindingResponseTypeDef = TypedDict(
+    "PutCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -501,14 +707,34 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
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
 SearchSchemaVersionSummaryTypeDef = TypedDict(
     "SearchSchemaVersionSummaryTypeDef",
     {
         "CreatedDate": datetime,
         "SchemaVersion": str,
         "Type": TypeType,
     },
@@ -532,28 +758,67 @@
 )
 
 class SearchSchemasRequestRequestTypeDef(
     _RequiredSearchSchemasRequestRequestTypeDef, _OptionalSearchSchemasRequestRequestTypeDef
 ):
     pass
 
+_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "Keywords": str,
+        "RegistryName": str,
+    },
+)
+_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SearchSchemasRequestSearchSchemasPaginateTypeDef(
+    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
+    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
+):
+    pass
+
 StartDiscovererRequestRequestTypeDef = TypedDict(
     "StartDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
+StartDiscovererResponseTypeDef = TypedDict(
+    "StartDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopDiscovererRequestRequestTypeDef = TypedDict(
     "StopDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
+StopDiscovererResponseTypeDef = TypedDict(
+    "StopDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -582,14 +847,28 @@
 )
 
 class UpdateDiscovererRequestRequestTypeDef(
     _RequiredUpdateDiscovererRequestRequestTypeDef, _OptionalUpdateDiscovererRequestRequestTypeDef
 ):
     pass
 
+UpdateDiscovererResponseTypeDef = TypedDict(
+    "UpdateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalUpdateRegistryRequestRequestTypeDef = TypedDict(
@@ -601,14 +880,25 @@
 )
 
 class UpdateRegistryRequestRequestTypeDef(
     _RequiredUpdateRegistryRequestRequestTypeDef, _OptionalUpdateRegistryRequestRequestTypeDef
 ):
     pass
 
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -624,233 +914,26 @@
 )
 
 class UpdateSchemaRequestRequestTypeDef(
     _RequiredUpdateSchemaRequestRequestTypeDef, _OptionalUpdateSchemaRequestRequestTypeDef
 ):
     pass
 
-CreateDiscovererResponseTypeDef = TypedDict(
-    "CreateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCodeBindingResponseTypeDef = TypedDict(
-    "DescribeCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDiscovererResponseTypeDef = TypedDict(
-    "DescribeDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRegistryResponseTypeDef = TypedDict(
-    "DescribeRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
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
-ExportSchemaResponseTypeDef = TypedDict(
-    "ExportSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Type": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCodeBindingSourceResponseTypeDef = TypedDict(
-    "GetCodeBindingSourceResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDiscoveredSchemaResponseTypeDef = TypedDict(
-    "GetDiscoveredSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutCodeBindingResponseTypeDef = TypedDict(
-    "PutCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDiscovererResponseTypeDef = TypedDict(
-    "StartDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopDiscovererResponseTypeDef = TypedDict(
-    "StopDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDiscovererResponseTypeDef = TypedDict(
-    "UpdateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateSchemaResponseTypeDef = TypedDict(
     "UpdateSchemaResponseTypeDef",
     {
         "Description": str,
         "LastModified": datetime,
         "SchemaArn": str,
         "SchemaName": str,
         "SchemaVersion": str,
         "Tags": Dict[str, str],
         "Type": str,
         "VersionCreatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     {
         "Language": str,
@@ -874,125 +957,42 @@
     pass
 
 ListDiscoverersResponseTypeDef = TypedDict(
     "ListDiscoverersResponseTypeDef",
     {
         "Discoverers": List[DiscovererSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
-    {
-        "DiscovererIdPrefix": str,
-        "SourceArnPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    {
-        "RegistryNamePrefix": str,
-        "Scope": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "RegistryName": str,
-        "SchemaName": str,
-    },
-)
-_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "RegistryName": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "SchemaNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "Keywords": str,
-        "RegistryName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchSchemasRequestSearchSchemasPaginateTypeDef(
-    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
-    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
-):
-    pass
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "NextToken": str,
         "Registries": List[RegistrySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "NextToken": str,
         "SchemaVersions": List[SchemaVersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SchemaSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchSchemaSummaryTypeDef = TypedDict(
     "SearchSchemaSummaryTypeDef",
     {
         "RegistryName": str,
@@ -1004,10 +1004,10 @@
 )
 
 SearchSchemasResponseTypeDef = TypedDict(
     "SearchSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SearchSchemaSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/waiter.py` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas/waiter.pyi` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/PKG-INFO` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Schemas 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Schemas 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
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
 
 <a id="mypy-boto3-schemas"></a>
 
 # mypy-boto3-schemas
 
 [![PyPI - mypy-boto3-schemas](https://img.shields.io/pypi/v/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,79 +360,79 @@
 
 `mypy_boto3_schemas.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDiscovererResponseTypeDef,
     CreateRegistryRequestRequestTypeDef,
+    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
+    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
+    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
+    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
+    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
+    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
     ListDiscoverersRequestRequestTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
+    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
+    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
+    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateRegistryRequestRequestTypeDef,
-    UpdateSchemaRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DescribeCodeBindingResponseTypeDef,
-    DescribeDiscovererResponseTypeDef,
-    DescribeRegistryResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportSchemaResponseTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutCodeBindingResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartDiscovererResponseTypeDef,
-    StopDiscovererResponseTypeDef,
     UpdateDiscovererResponseTypeDef,
+    UpdateRegistryRequestRequestTypeDef,
     UpdateRegistryResponseTypeDef,
+    UpdateSchemaRequestRequestTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
 
@@ -443,42 +444,42 @@
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

### Comparing `mypy-boto3-schemas-1.26.0.post1/mypy_boto3_schemas.egg-info/SOURCES.txt` & `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.26.0.post1/setup.py` & `mypy-boto3-schemas-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
 Setup script for mypy-boto3-schemas.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-schemas",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Schemas 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Schemas 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 schemas type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_schemas": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_schemas": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/",
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


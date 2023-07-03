# Comparing `tmp/mypy-boto3-resource-explorer-2-1.26.93.tar.gz` & `tmp/mypy-boto3-resource-explorer-2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-explorer-2-1.26.93.tar", last modified: Thu Mar 16 19:19:49 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-explorer-2-1.27.0.tar", last modified: Mon Jul  3 19:51:20 2023, max compression
```

## Comparing `mypy-boto3-resource-explorer-2-1.26.93.tar` & `mypy-boto3-resource-explorer-2-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.211278 mypy-boto3-resource-explorer-2-1.26.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-03-16 19:19:49.211278 mypy-boto3-resource-explorer-2-1.26.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.211278 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-03-16 19:19:39.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-03-16 19:19:39.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.211278 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-03-16 19:19:49.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-16 19:19:49.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:19:49.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:19:49.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-16 19:19:49.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-16 19:19:49.000000 mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 19:19:49.211278 mypy-boto3-resource-explorer-2-1.26.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-16 19:19:38.000000 mypy-boto3-resource-explorer-2-1.26.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.995883 mypy-boto3-resource-explorer-2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-03 19:51:19.995883 mypy-boto3-resource-explorer-2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.995883 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-03 19:46:20.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-07-03 19:46:20.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-03 19:46:20.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.995883 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-03 19:51:19.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:51:19.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:51:19.000000 mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:19.995883 mypy-boto3-resource-explorer-2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-03 19:46:17.000000 mypy-boto3-resource-explorer-2-1.27.0/setup.py
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/LICENSE` & `mypy-boto3-resource-explorer-2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/PKG-INFO` & `mypy-boto3-resource-explorer-2-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-explorer-2
-Version: 1.26.93
-Summary: Type annotations for boto3.ResourceExplorer 1.26.93 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ResourceExplorer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-resource-explorer-2"></a>
 
 # mypy-boto3-resource-explorer-2
 
 [![PyPI - mypy-boto3-resource-explorer-2](https://img.shields.io/pypi/v/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-explorer-2?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,54 +336,54 @@
 
 `mypy_boto3_resource_explorer_2.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateDefaultViewOutputTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
+    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
+    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
     IndexTypeDef,
-    PaginatorConfigTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
     ListIndexesInputRequestTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
+    ListViewsOutputTypeDef,
+    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
+    ResponseMetadataTypeDef,
     SearchInputRequestTypeDef,
+    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
-    CreateIndexOutputTypeDef,
-    DeleteIndexOutputTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
     ViewTypeDef,
     ListIndexesOutputTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
-    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
     SearchOutputTypeDef,
@@ -397,42 +397,42 @@
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

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/README.md` & `mypy-boto3-resource-explorer-2-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resource-explorer-2"></a>
 
 # mypy-boto3-resource-explorer-2
 
 [![PyPI - mypy-boto3-resource-explorer-2](https://img.shields.io/pypi/v/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-explorer-2?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,54 +304,54 @@
 
 `mypy_boto3_resource_explorer_2.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateDefaultViewOutputTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
+    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
+    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
     IndexTypeDef,
-    PaginatorConfigTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
     ListIndexesInputRequestTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
+    ListViewsOutputTypeDef,
+    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
+    ResponseMetadataTypeDef,
     SearchInputRequestTypeDef,
+    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
-    CreateIndexOutputTypeDef,
-    DeleteIndexOutputTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
     ViewTypeDef,
     ListIndexesOutputTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
-    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
     SearchOutputTypeDef,
@@ -365,42 +365,42 @@
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

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/__init__.py` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/__init__.pyi` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/__main__.py` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceExplorer 1.26.93\nVersion:         1.26.93\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.ResourceExplorer 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.93")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/client.py` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/client.pyi` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/literals.py` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -99,14 +100,15 @@
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
@@ -204,14 +206,15 @@
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
@@ -247,14 +250,15 @@
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
@@ -273,16 +277,19 @@
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
@@ -366,15 +373,17 @@
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
@@ -394,16 +403,14 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_indexes", "list_supported_resource_types", "list_views", "search"]
 RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/literals.pyi` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -97,14 +98,15 @@
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
@@ -202,14 +204,15 @@
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
@@ -245,14 +248,15 @@
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
@@ -271,16 +275,19 @@
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
@@ -364,15 +371,17 @@
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
@@ -392,16 +401,14 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_indexes", "list_supported_resource_types", "list_views", "search"]
 RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/paginator.py` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,84 +41,78 @@
 __all__ = (
     "ListIndexesPaginator",
     "ListSupportedResourceTypesPaginator",
     "ListViewsPaginator",
     "SearchPaginator",
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
 class ListIndexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listindexespaginator)
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listindexespaginator)
         """
 
-
 class ListSupportedResourceTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSupportedResourceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
         """
 
-
 class ListViewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListViewsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
         """
 
-
 class SearchPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#searchpaginator)
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/paginator.pyi` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,78 +41,84 @@
 __all__ = (
     "ListIndexesPaginator",
     "ListSupportedResourceTypesPaginator",
     "ListViewsPaginator",
     "SearchPaginator",
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
 class ListIndexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listindexespaginator)
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listindexespaginator)
         """
 
+
 class ListSupportedResourceTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSupportedResourceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
         """
 
+
 class ListViewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListViewsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
         """
 
+
 class SearchPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#searchpaginator)
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/type_defs.py` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,54 +21,54 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateDefaultViewOutputTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
+    "CreateIndexOutputTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
+    "DeleteIndexOutputTypeDef",
     "DeleteViewInputRequestTypeDef",
+    "DeleteViewOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDefaultViewOutputTypeDef",
+    "GetIndexOutputTypeDef",
     "GetViewInputRequestTypeDef",
     "IndexTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListIndexesInputListIndexesPaginateTypeDef",
     "ListIndexesInputRequestTypeDef",
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListViewsInputListViewsPaginateTypeDef",
     "ListViewsInputRequestTypeDef",
+    "ListViewsOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchInputRequestTypeDef",
+    "SearchInputSearchPaginateTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
-    "AssociateDefaultViewOutputTypeDef",
-    "CreateIndexOutputTypeDef",
-    "DeleteIndexOutputTypeDef",
-    "DeleteViewOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDefaultViewOutputTypeDef",
-    "GetIndexOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
     "ViewTypeDef",
     "ListIndexesOutputTypeDef",
-    "ListIndexesInputListIndexesPaginateTypeDef",
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    "ListViewsInputListViewsPaginateTypeDef",
-    "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
     "SearchOutputTypeDef",
@@ -77,22 +77,19 @@
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateDefaultViewOutputTypeDef = TypedDict(
+    "AssociateDefaultViewOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ViewArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetViewErrorTypeDef = TypedDict(
     "BatchGetViewErrorTypeDef",
     {
         "ErrorMessage": str,
@@ -113,14 +110,24 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+CreateIndexOutputTypeDef = TypedDict(
+    "CreateIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IncludedPropertyTypeDef = TypedDict(
     "IncludedPropertyTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -134,21 +141,69 @@
 DeleteIndexInputRequestTypeDef = TypedDict(
     "DeleteIndexInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteIndexOutputTypeDef = TypedDict(
+    "DeleteIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "LastUpdatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteViewInputRequestTypeDef = TypedDict(
     "DeleteViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
+DeleteViewOutputTypeDef = TypedDict(
+    "DeleteViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDefaultViewOutputTypeDef = TypedDict(
+    "GetDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetIndexOutputTypeDef = TypedDict(
+    "GetIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "ReplicatingFrom": List[str],
+        "ReplicatingTo": List[str],
+        "State": IndexStateType,
+        "Tags": Dict[str, str],
+        "Type": IndexTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetViewInputRequestTypeDef = TypedDict(
     "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
@@ -158,20 +213,20 @@
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
+    "ListIndexesInputListIndexesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Regions": Sequence[str],
+        "Type": IndexTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListIndexesInputRequestTypeDef = TypedDict(
     "ListIndexesInputRequestTypeDef",
     {
@@ -179,14 +234,22 @@
         "NextToken": str,
         "Regions": Sequence[str],
         "Type": IndexTypeType,
     },
     total=False,
 )
 
+ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSupportedResourceTypesInputRequestTypeDef = TypedDict(
     "ListSupportedResourceTypesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -204,23 +267,58 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListViewsInputListViewsPaginateTypeDef = TypedDict(
+    "ListViewsInputListViewsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListViewsInputRequestTypeDef = TypedDict(
     "ListViewsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListViewsOutputTypeDef = TypedDict(
+    "ListViewsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Views": List[str],
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
 ResourceCountTypeDef = TypedDict(
     "ResourceCountTypeDef",
     {
         "Complete": bool,
         "TotalResources": int,
     },
     total=False,
@@ -232,14 +330,25 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
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
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalSearchInputRequestTypeDef = TypedDict(
@@ -255,14 +364,36 @@
 
 class SearchInputRequestTypeDef(
     _RequiredSearchInputRequestTypeDef, _OptionalSearchInputRequestTypeDef
 ):
     pass
 
 
+_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
+    "_RequiredSearchInputSearchPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
+    "_OptionalSearchInputSearchPaginateTypeDef",
+    {
+        "ViewArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SearchInputSearchPaginateTypeDef(
+    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
+):
+    pass
+
+
 _RequiredTagResourceInputRequestTypeDef = TypedDict(
     "_RequiredTagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceInputRequestTypeDef = TypedDict(
@@ -292,105 +423,22 @@
     "UpdateIndexTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": IndexTypeType,
     },
 )
 
-AssociateDefaultViewOutputTypeDef = TypedDict(
-    "AssociateDefaultViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIndexOutputTypeDef = TypedDict(
-    "CreateIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteIndexOutputTypeDef = TypedDict(
-    "DeleteIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "LastUpdatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteViewOutputTypeDef = TypedDict(
-    "DeleteViewOutputTypeDef",
-    {
-        "ViewArn": str,
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
-GetDefaultViewOutputTypeDef = TypedDict(
-    "GetDefaultViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIndexOutputTypeDef = TypedDict(
-    "GetIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "ReplicatingFrom": List[str],
-        "ReplicatingTo": List[str],
-        "State": IndexStateType,
-        "Tags": Dict[str, str],
-        "Type": IndexTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListViewsOutputTypeDef = TypedDict(
-    "ListViewsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Views": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateIndexTypeOutputTypeDef = TypedDict(
     "UpdateIndexTypeOutputTypeDef",
     {
         "Arn": str,
         "LastUpdatedAt": datetime,
         "State": IndexStateType,
         "Type": IndexTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateViewInputRequestTypeDef = TypedDict(
     "_RequiredCreateViewInputRequestTypeDef",
     {
         "ViewName": str,
@@ -450,72 +498,24 @@
 )
 
 ListIndexesOutputTypeDef = TypedDict(
     "ListIndexesOutputTypeDef",
     {
         "Indexes": List[IndexTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
-    "ListIndexesInputListIndexesPaginateTypeDef",
-    {
-        "Regions": Sequence[str],
-        "Type": IndexTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListViewsInputListViewsPaginateTypeDef = TypedDict(
-    "ListViewsInputListViewsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
-    "_RequiredSearchInputSearchPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
-    "_OptionalSearchInputSearchPaginateTypeDef",
-    {
-        "ViewArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
-
-class SearchInputSearchPaginateTypeDef(
-    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
-):
-    pass
-
-
 ListSupportedResourceTypesOutputTypeDef = TypedDict(
     "ListSupportedResourceTypesOutputTypeDef",
     {
         "NextToken": str,
         "ResourceTypes": List[SupportedResourceTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Arn": str,
@@ -530,46 +530,46 @@
 )
 
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateViewOutputTypeDef = TypedDict(
     "CreateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetViewOutputTypeDef = TypedDict(
     "GetViewOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "View": ViewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchOutputTypeDef = TypedDict(
     "SearchOutputTypeDef",
     {
         "Count": ResourceCountTypeDef,
         "NextToken": str,
         "Resources": List[ResourceTypeDef],
         "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2/type_defs.pyi` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,54 +20,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateDefaultViewOutputTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
+    "CreateIndexOutputTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
+    "DeleteIndexOutputTypeDef",
     "DeleteViewInputRequestTypeDef",
+    "DeleteViewOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDefaultViewOutputTypeDef",
+    "GetIndexOutputTypeDef",
     "GetViewInputRequestTypeDef",
     "IndexTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListIndexesInputListIndexesPaginateTypeDef",
     "ListIndexesInputRequestTypeDef",
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListViewsInputListViewsPaginateTypeDef",
     "ListViewsInputRequestTypeDef",
+    "ListViewsOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchInputRequestTypeDef",
+    "SearchInputSearchPaginateTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
-    "AssociateDefaultViewOutputTypeDef",
-    "CreateIndexOutputTypeDef",
-    "DeleteIndexOutputTypeDef",
-    "DeleteViewOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDefaultViewOutputTypeDef",
-    "GetIndexOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
     "ViewTypeDef",
     "ListIndexesOutputTypeDef",
-    "ListIndexesInputListIndexesPaginateTypeDef",
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    "ListViewsInputListViewsPaginateTypeDef",
-    "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
     "SearchOutputTypeDef",
@@ -76,22 +76,19 @@
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateDefaultViewOutputTypeDef = TypedDict(
+    "AssociateDefaultViewOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ViewArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetViewErrorTypeDef = TypedDict(
     "BatchGetViewErrorTypeDef",
     {
         "ErrorMessage": str,
@@ -112,14 +109,24 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+CreateIndexOutputTypeDef = TypedDict(
+    "CreateIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IncludedPropertyTypeDef = TypedDict(
     "IncludedPropertyTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -133,21 +140,69 @@
 DeleteIndexInputRequestTypeDef = TypedDict(
     "DeleteIndexInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteIndexOutputTypeDef = TypedDict(
+    "DeleteIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "LastUpdatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteViewInputRequestTypeDef = TypedDict(
     "DeleteViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
+DeleteViewOutputTypeDef = TypedDict(
+    "DeleteViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDefaultViewOutputTypeDef = TypedDict(
+    "GetDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetIndexOutputTypeDef = TypedDict(
+    "GetIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "ReplicatingFrom": List[str],
+        "ReplicatingTo": List[str],
+        "State": IndexStateType,
+        "Tags": Dict[str, str],
+        "Type": IndexTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetViewInputRequestTypeDef = TypedDict(
     "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
@@ -157,20 +212,20 @@
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
+    "ListIndexesInputListIndexesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Regions": Sequence[str],
+        "Type": IndexTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListIndexesInputRequestTypeDef = TypedDict(
     "ListIndexesInputRequestTypeDef",
     {
@@ -178,14 +233,22 @@
         "NextToken": str,
         "Regions": Sequence[str],
         "Type": IndexTypeType,
     },
     total=False,
 )
 
+ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSupportedResourceTypesInputRequestTypeDef = TypedDict(
     "ListSupportedResourceTypesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -203,23 +266,58 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListViewsInputListViewsPaginateTypeDef = TypedDict(
+    "ListViewsInputListViewsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListViewsInputRequestTypeDef = TypedDict(
     "ListViewsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListViewsOutputTypeDef = TypedDict(
+    "ListViewsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Views": List[str],
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
 ResourceCountTypeDef = TypedDict(
     "ResourceCountTypeDef",
     {
         "Complete": bool,
         "TotalResources": int,
     },
     total=False,
@@ -231,14 +329,25 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
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
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalSearchInputRequestTypeDef = TypedDict(
@@ -252,14 +361,34 @@
 )
 
 class SearchInputRequestTypeDef(
     _RequiredSearchInputRequestTypeDef, _OptionalSearchInputRequestTypeDef
 ):
     pass
 
+_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
+    "_RequiredSearchInputSearchPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
+    "_OptionalSearchInputSearchPaginateTypeDef",
+    {
+        "ViewArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SearchInputSearchPaginateTypeDef(
+    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
+):
+    pass
+
 _RequiredTagResourceInputRequestTypeDef = TypedDict(
     "_RequiredTagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceInputRequestTypeDef = TypedDict(
@@ -287,105 +416,22 @@
     "UpdateIndexTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": IndexTypeType,
     },
 )
 
-AssociateDefaultViewOutputTypeDef = TypedDict(
-    "AssociateDefaultViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIndexOutputTypeDef = TypedDict(
-    "CreateIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteIndexOutputTypeDef = TypedDict(
-    "DeleteIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "LastUpdatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteViewOutputTypeDef = TypedDict(
-    "DeleteViewOutputTypeDef",
-    {
-        "ViewArn": str,
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
-GetDefaultViewOutputTypeDef = TypedDict(
-    "GetDefaultViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIndexOutputTypeDef = TypedDict(
-    "GetIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "ReplicatingFrom": List[str],
-        "ReplicatingTo": List[str],
-        "State": IndexStateType,
-        "Tags": Dict[str, str],
-        "Type": IndexTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListViewsOutputTypeDef = TypedDict(
-    "ListViewsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Views": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateIndexTypeOutputTypeDef = TypedDict(
     "UpdateIndexTypeOutputTypeDef",
     {
         "Arn": str,
         "LastUpdatedAt": datetime,
         "State": IndexStateType,
         "Type": IndexTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateViewInputRequestTypeDef = TypedDict(
     "_RequiredCreateViewInputRequestTypeDef",
     {
         "ViewName": str,
@@ -441,70 +487,24 @@
 )
 
 ListIndexesOutputTypeDef = TypedDict(
     "ListIndexesOutputTypeDef",
     {
         "Indexes": List[IndexTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
-    "ListIndexesInputListIndexesPaginateTypeDef",
-    {
-        "Regions": Sequence[str],
-        "Type": IndexTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListViewsInputListViewsPaginateTypeDef = TypedDict(
-    "ListViewsInputListViewsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
-    "_RequiredSearchInputSearchPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
-    "_OptionalSearchInputSearchPaginateTypeDef",
-    {
-        "ViewArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchInputSearchPaginateTypeDef(
-    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
-):
-    pass
-
 ListSupportedResourceTypesOutputTypeDef = TypedDict(
     "ListSupportedResourceTypesOutputTypeDef",
     {
         "NextToken": str,
         "ResourceTypes": List[SupportedResourceTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Arn": str,
@@ -519,46 +519,46 @@
 )
 
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateViewOutputTypeDef = TypedDict(
     "CreateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetViewOutputTypeDef = TypedDict(
     "GetViewOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "View": ViewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchOutputTypeDef = TypedDict(
     "SearchOutputTypeDef",
     {
         "Count": ResourceCountTypeDef,
         "NextToken": str,
         "Resources": List[ResourceTypeDef],
         "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-explorer-2
-Version: 1.26.93
-Summary: Type annotations for boto3.ResourceExplorer 1.26.93 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ResourceExplorer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-resource-explorer-2"></a>
 
 # mypy-boto3-resource-explorer-2
 
 [![PyPI - mypy-boto3-resource-explorer-2](https://img.shields.io/pypi/v/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-explorer-2?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,54 +336,54 @@
 
 `mypy_boto3_resource_explorer_2.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateDefaultViewOutputTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
+    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
+    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
     IndexTypeDef,
-    PaginatorConfigTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
     ListIndexesInputRequestTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
+    ListViewsOutputTypeDef,
+    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
+    ResponseMetadataTypeDef,
     SearchInputRequestTypeDef,
+    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
-    CreateIndexOutputTypeDef,
-    DeleteIndexOutputTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
     ViewTypeDef,
     ListIndexesOutputTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
-    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
     SearchOutputTypeDef,
@@ -397,42 +397,42 @@
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

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt` & `mypy-boto3-resource-explorer-2-1.27.0/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.26.93/setup.py` & `mypy-boto3-resource-explorer-2-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-resource-explorer-2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-explorer-2",
-    version="1.26.93",
+    version="1.27.0",
     packages=["mypy_boto3_resource_explorer_2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceExplorer 1.26.93 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.ResourceExplorer 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -47,11 +47,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/"
         ),
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


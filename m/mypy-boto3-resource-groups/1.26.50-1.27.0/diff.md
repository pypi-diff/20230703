# Comparing `tmp/mypy-boto3-resource-groups-1.26.50.tar.gz` & `tmp/mypy-boto3-resource-groups-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-groups-1.26.50.tar", last modified: Fri Jan 13 20:26:28 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-groups-1.27.0.tar", last modified: Mon Jul  3 19:51:20 2023, max compression
```

## Comparing `mypy-boto3-resource-groups-1.26.50.tar` & `mypy-boto3-resource-groups-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:26:28.130257 mypy-boto3-resource-groups-1.26.50/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-01-13 20:26:28.130257 mypy-boto3-resource-groups-1.26.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:26:28.130257 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:26:28.130257 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-01-13 20:26:28.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-13 20:26:28.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 20:26:28.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 20:26:28.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-13 20:26:28.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-13 20:26:28.000000 mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 20:26:28.130257 mypy-boto3-resource-groups-1.26.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-13 20:26:19.000000 mypy-boto3-resource-groups-1.26.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.011884 mypy-boto3-resource-groups-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-03 19:51:20.011884 mypy-boto3-resource-groups-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.003883 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-03 19:46:21.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.011884 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-03 19:51:19.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:51:19.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:19.000000 mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:20.011884 mypy-boto3-resource-groups-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-03 19:46:20.000000 mypy-boto3-resource-groups-1.27.0/setup.py
```

### Comparing `mypy-boto3-resource-groups-1.26.50/LICENSE` & `mypy-boto3-resource-groups-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-resource-groups-1.26.50/PKG-INFO` & `mypy-boto3-resource-groups-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.26.50
-Summary: Type annotations for boto3.ResourceGroups 1.26.50 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ResourceGroups 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-groups?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.26.50](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,54 +341,54 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
-    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
+    GetTagsOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
-    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
+    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
+    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
+    GetAccountSettingsOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
     DeleteGroupOutputTypeDef,
-    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
-    GetTagsOutputTypeDef,
-    TagOutputTypeDef,
-    UntagOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
     GroupConfigurationItemTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
     CreateGroupInputRequestTypeDef,
@@ -407,42 +407,42 @@
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

### Comparing `mypy-boto3-resource-groups-1.26.50/README.md` & `mypy-boto3-resource-groups-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-groups?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.26.50](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,54 +309,54 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
-    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
+    GetTagsOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
-    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
+    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
+    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
+    GetAccountSettingsOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
     DeleteGroupOutputTypeDef,
-    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
-    GetTagsOutputTypeDef,
-    TagOutputTypeDef,
-    UntagOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
     GroupConfigurationItemTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
     CreateGroupInputRequestTypeDef,
@@ -375,42 +375,42 @@
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

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/__init__.py` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/__init__.pyi` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/__main__.py` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroups 1.26.50\nVersion:         1.26.50\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ResourceGroups 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.50")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/client.py` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/client.pyi` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/literals.py` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GroupConfigurationStatusType",
     "GroupFilterNameType",
     "GroupLifecycleEventsDesiredStatusType",
     "GroupLifecycleEventsStatusType",
     "ListGroupResourcesPaginatorName",
     "ListGroupsPaginatorName",
@@ -34,15 +33,14 @@
     "ResourceGroupsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GroupConfigurationStatusType = Literal["UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"]
 GroupFilterNameType = Literal["configuration-type", "resource-type"]
 GroupLifecycleEventsDesiredStatusType = Literal["ACTIVE", "INACTIVE"]
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
@@ -66,14 +64,15 @@
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
@@ -105,21 +104,23 @@
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
@@ -198,14 +199,15 @@
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
@@ -216,14 +218,15 @@
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
@@ -259,14 +262,15 @@
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
@@ -285,16 +289,19 @@
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
@@ -374,18 +381,21 @@
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
@@ -411,21 +421,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/literals.pyi` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "GroupConfigurationStatusType",
     "GroupFilterNameType",
     "GroupLifecycleEventsDesiredStatusType",
     "GroupLifecycleEventsStatusType",
     "ListGroupResourcesPaginatorName",
     "ListGroupsPaginatorName",
@@ -33,14 +34,15 @@
     "ResourceGroupsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 GroupConfigurationStatusType = Literal["UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"]
 GroupFilterNameType = Literal["configuration-type", "resource-type"]
 GroupLifecycleEventsDesiredStatusType = Literal["ACTIVE", "INACTIVE"]
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
@@ -64,14 +66,15 @@
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
@@ -103,21 +106,23 @@
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
@@ -196,14 +201,15 @@
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
@@ -214,14 +220,15 @@
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
@@ -257,14 +264,15 @@
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
@@ -283,16 +291,19 @@
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
@@ -372,18 +383,21 @@
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
@@ -409,21 +423,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/paginator.py` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 
@@ -76,28 +76,31 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
         """
 
 
 class SearchResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
     """
 
     def paginate(
-        self, *, ResourceQuery: ResourceQueryTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ResourceQuery: ResourceQueryTypeDef,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/paginator.pyi` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 class ListGroupsPaginator(Paginator):
@@ -72,27 +72,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
         """
 
 class SearchResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
     """
 
     def paginate(
-        self, *, ResourceQuery: ResourceQueryTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ResourceQuery: ResourceQueryTypeDef,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/type_defs.py` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,54 +33,54 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
+    "GetTagsOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagInputRequestTypeDef",
+    "TagOutputTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
+    "UntagOutputTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
+    "GetAccountSettingsOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
     "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
+    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
     "DeleteGroupOutputTypeDef",
-    "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
-    "GetTagsOutputTypeDef",
-    "TagOutputTypeDef",
-    "UntagOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
     "GroupConfigurationItemTypeDef",
+    "ListGroupsInputListGroupsPaginateTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
     "CreateGroupInputRequestTypeDef",
@@ -125,25 +125,14 @@
 )
 
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
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
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
@@ -188,14 +177,23 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+GetTagsOutputTypeDef = TypedDict(
+    "GetTagsOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
@@ -242,24 +240,14 @@
     "PendingResourceTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ResourceFilterTypeDef = TypedDict(
     "ResourceFilterTypeDef",
     {
         "Name": Literal["resource-type"],
         "Values": Sequence[str],
     },
 )
@@ -286,22 +274,52 @@
     {
         "ErrorCode": QueryErrorCodeType,
         "Message": str,
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
 TagInputRequestTypeDef = TypedDict(
     "TagInputRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UngroupResourcesInputRequestTypeDef = TypedDict(
     "UngroupResourcesInputRequestTypeDef",
     {
         "Group": str,
         "ResourceArns": Sequence[str],
     },
 )
@@ -310,14 +328,23 @@
     "UntagInputRequestTypeDef",
     {
         "Arn": str,
         "Keys": Sequence[str],
     },
 )
 
+UntagOutputTypeDef = TypedDict(
+    "UntagOutputTypeDef",
+    {
+        "Arn": str,
+        "Keys": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
     },
     total=False,
 )
@@ -328,14 +355,30 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GroupQueryTypeDef = TypedDict(
     "GroupQueryTypeDef",
     {
         "GroupName": str,
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
@@ -358,14 +401,36 @@
 
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
 
+_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SearchResourcesInputSearchResourcesPaginateTypeDef(
+    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
+    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -384,74 +449,31 @@
     pass
 
 
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupOutputTypeDef = TypedDict(
     "GetGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsOutputTypeDef = TypedDict(
-    "GetTagsOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UntagOutputTypeDef = TypedDict(
-    "UntagOutputTypeDef",
-    {
-        "Arn": str,
-        "Keys": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupOutputTypeDef = TypedDict(
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
@@ -468,14 +490,23 @@
 
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
 
+ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[GroupFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -484,76 +515,45 @@
 
 ListGroupsOutputTypeDef = TypedDict(
     "ListGroupsOutputTypeDef",
     {
         "GroupIdentifiers": List[GroupIdentifierTypeDef],
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GroupResourcesOutputTypeDef = TypedDict(
     "GroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UngroupResourcesOutputTypeDef = TypedDict(
     "UngroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[GroupFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class SearchResourcesInputSearchResourcesPaginateTypeDef(
-    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
-    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
-):
-    pass
-
-
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListGroupResourcesInputRequestTypeDef = TypedDict(
     "ListGroupResourcesInputRequestTypeDef",
     {
@@ -577,31 +577,31 @@
 
 SearchResourcesOutputTypeDef = TypedDict(
     "SearchResourcesOutputTypeDef",
     {
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupQueryOutputTypeDef = TypedDict(
     "GetGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupQueryOutputTypeDef = TypedDict(
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateGroupInputRequestTypeDef",
     {
         "Name": str,
@@ -648,29 +648,29 @@
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups/type_defs.pyi` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -32,54 +32,54 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
+    "GetTagsOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagInputRequestTypeDef",
+    "TagOutputTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
+    "UntagOutputTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
+    "GetAccountSettingsOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
     "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
+    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
     "DeleteGroupOutputTypeDef",
-    "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
-    "GetTagsOutputTypeDef",
-    "TagOutputTypeDef",
-    "UntagOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
     "GroupConfigurationItemTypeDef",
+    "ListGroupsInputListGroupsPaginateTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
     "CreateGroupInputRequestTypeDef",
@@ -122,25 +122,14 @@
     },
     total=False,
 )
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
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
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
@@ -185,14 +174,23 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+GetTagsOutputTypeDef = TypedDict(
+    "GetTagsOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
@@ -237,24 +235,14 @@
     "PendingResourceTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ResourceFilterTypeDef = TypedDict(
     "ResourceFilterTypeDef",
     {
         "Name": Literal["resource-type"],
         "Values": Sequence[str],
     },
 )
@@ -281,22 +269,52 @@
     {
         "ErrorCode": QueryErrorCodeType,
         "Message": str,
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
 TagInputRequestTypeDef = TypedDict(
     "TagInputRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UngroupResourcesInputRequestTypeDef = TypedDict(
     "UngroupResourcesInputRequestTypeDef",
     {
         "Group": str,
         "ResourceArns": Sequence[str],
     },
 )
@@ -305,14 +323,23 @@
     "UntagInputRequestTypeDef",
     {
         "Arn": str,
         "Keys": Sequence[str],
     },
 )
 
+UntagOutputTypeDef = TypedDict(
+    "UntagOutputTypeDef",
+    {
+        "Arn": str,
+        "Keys": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
     },
     total=False,
 )
@@ -323,14 +350,30 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GroupQueryTypeDef = TypedDict(
     "GroupQueryTypeDef",
     {
         "GroupName": str,
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
@@ -351,14 +394,34 @@
 )
 
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
+_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SearchResourcesInputSearchResourcesPaginateTypeDef(
+    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
+    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -375,74 +438,31 @@
 ):
     pass
 
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupOutputTypeDef = TypedDict(
     "GetGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsOutputTypeDef = TypedDict(
-    "GetTagsOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UntagOutputTypeDef = TypedDict(
-    "UntagOutputTypeDef",
-    {
-        "Arn": str,
-        "Keys": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupOutputTypeDef = TypedDict(
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
@@ -457,14 +477,23 @@
 )
 
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
+ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[GroupFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -473,74 +502,45 @@
 
 ListGroupsOutputTypeDef = TypedDict(
     "ListGroupsOutputTypeDef",
     {
         "GroupIdentifiers": List[GroupIdentifierTypeDef],
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GroupResourcesOutputTypeDef = TypedDict(
     "GroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UngroupResourcesOutputTypeDef = TypedDict(
     "UngroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[GroupFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchResourcesInputSearchResourcesPaginateTypeDef(
-    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
-    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
-):
-    pass
-
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListGroupResourcesInputRequestTypeDef = TypedDict(
     "ListGroupResourcesInputRequestTypeDef",
     {
@@ -564,31 +564,31 @@
 
 SearchResourcesOutputTypeDef = TypedDict(
     "SearchResourcesOutputTypeDef",
     {
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupQueryOutputTypeDef = TypedDict(
     "GetGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupQueryOutputTypeDef = TypedDict(
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateGroupInputRequestTypeDef",
     {
         "Name": str,
@@ -633,29 +633,29 @@
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/PKG-INFO` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.26.50
-Summary: Type annotations for boto3.ResourceGroups 1.26.50 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ResourceGroups 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-groups?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.26.50](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,54 +341,54 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
-    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
+    GetTagsOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
-    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
+    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
+    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
+    GetAccountSettingsOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
     DeleteGroupOutputTypeDef,
-    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
-    GetTagsOutputTypeDef,
-    TagOutputTypeDef,
-    UntagOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
     GroupConfigurationItemTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
     CreateGroupInputRequestTypeDef,
@@ -407,42 +407,42 @@
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

### Comparing `mypy-boto3-resource-groups-1.26.50/mypy_boto3_resource_groups.egg-info/SOURCES.txt` & `mypy-boto3-resource-groups-1.27.0/mypy_boto3_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.26.50/setup.py` & `mypy-boto3-resource-groups-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-resource-groups.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-groups",
-    version="1.26.50",
+    version="1.27.0",
     packages=["mypy_boto3_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroups 1.26.50 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ResourceGroups 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/",
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


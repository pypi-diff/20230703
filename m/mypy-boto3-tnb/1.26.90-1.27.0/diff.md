# Comparing `tmp/mypy-boto3-tnb-1.26.90.tar.gz` & `tmp/mypy-boto3-tnb-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-tnb-1.26.90.tar", last modified: Mon Mar 13 19:32:22 2023, max compression
+gzip compressed data, was "mypy-boto3-tnb-1.27.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
```

## Comparing `mypy-boto3-tnb-1.26.90.tar` & `mypy-boto3-tnb-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.899340 mypy-boto3-tnb-1.26.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-03-13 19:32:22.899340 mypy-boto3-tnb-1.26.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.895340 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-03-13 19:32:10.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-03-13 19:32:10.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34684 2023-03-13 19:32:10.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34653 2023-03-13 19:32:10.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 19:32:09.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.899340 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-03-13 19:32:22.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-13 19:32:22.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 19:32:22.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-13 19:32:22.000000 mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:32:22.899340 mypy-boto3-tnb-1.26.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-13 19:32:08.000000 mypy-boto3-tnb-1.26.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.972105 mypy-boto3-tnb-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-03 19:51:33.972105 mypy-boto3-tnb-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.972105 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34750 2023-07-03 19:49:08.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34719 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.972105 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-03 19:51:33.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:33.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:33.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:33.000000 mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:33.972105 mypy-boto3-tnb-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-03 19:49:07.000000 mypy-boto3-tnb-1.27.0/setup.py
```

### Comparing `mypy-boto3-tnb-1.26.90/LICENSE` & `mypy-boto3-tnb-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-tnb-1.26.90/PKG-INFO` & `mypy-boto3-tnb-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-tnb
-Version: 1.26.90
-Summary: Type annotations for boto3.TelcoNetworkBuilder 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.TelcoNetworkBuilder 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-tnb"></a>
 
 # mypy-boto3-tnb
 
 [![PyPI - mypy-boto3-tnb](https://img.shields.io/pypi/v/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-tnb?color=blue)](https://pypistats.org/packages/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,86 +357,86 @@
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutSolFunctionPackageContentInputRequestTypeDef,
     PutSolNetworkPackageContentInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
@@ -468,42 +468,42 @@
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

### Comparing `mypy-boto3-tnb-1.26.90/README.md` & `mypy-boto3-tnb-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-tnb"></a>
 
 # mypy-boto3-tnb
 
 [![PyPI - mypy-boto3-tnb](https://img.shields.io/pypi/v/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-tnb?color=blue)](https://pypistats.org/packages/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,86 +325,86 @@
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutSolFunctionPackageContentInputRequestTypeDef,
     PutSolNetworkPackageContentInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
@@ -436,42 +436,42 @@
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

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/__init__.py` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/__init__.pyi` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/__main__.py` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TelcoNetworkBuilder 1.26.90\nVersion:         1.26.90\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.TelcoNetworkBuilder 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.90")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/client.py` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/client.pyi` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/literals.py` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -242,14 +244,15 @@
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
@@ -285,14 +288,15 @@
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
@@ -311,16 +315,19 @@
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
@@ -404,15 +411,17 @@
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

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/literals.pyi` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -240,14 +242,15 @@
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
@@ -283,14 +286,15 @@
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
@@ -309,16 +313,19 @@
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
@@ -402,15 +409,17 @@
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

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/paginator.py` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -44,91 +44,84 @@
     "ListSolFunctionInstancesPaginator",
     "ListSolFunctionPackagesPaginator",
     "ListSolNetworkInstancesPaginator",
     "ListSolNetworkOperationsPaginator",
     "ListSolNetworkPackagesPaginator",
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
 class ListSolFunctionInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolFunctionInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
         """
 
-
 class ListSolFunctionPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolFunctionPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
         """
 
-
 class ListSolNetworkInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolNetworkInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
         """
 
-
 class ListSolNetworkOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolNetworkOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
         """
 
-
 class ListSolNetworkPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolNetworkPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
         """
```

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/paginator.pyi` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,84 +44,91 @@
     "ListSolFunctionInstancesPaginator",
     "ListSolFunctionPackagesPaginator",
     "ListSolNetworkInstancesPaginator",
     "ListSolNetworkOperationsPaginator",
     "ListSolNetworkPackagesPaginator",
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
 class ListSolFunctionInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolFunctionInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
         """
 
+
 class ListSolFunctionPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolFunctionPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
         """
 
+
 class ListSolNetworkInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolNetworkInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
         """
 
+
 class ListSolNetworkOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolNetworkOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
         """
 
+
 class ListSolNetworkPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSolNetworkPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
         """
```

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/type_defs.py` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,86 +41,86 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateSolFunctionPackageOutputTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
+    "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
+    "CreateSolNetworkPackageOutputTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
     "DeleteSolNetworkPackageInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "ToscaOverrideTypeDef",
     "GetSolFunctionInstanceInputRequestTypeDef",
     "GetSolFunctionInstanceMetadataTypeDef",
     "GetSolFunctionPackageContentInputRequestTypeDef",
+    "GetSolFunctionPackageContentOutputTypeDef",
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
     "GetSolFunctionPackageInputRequestTypeDef",
     "GetSolInstantiatedVnfInfoTypeDef",
     "GetSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkInstanceMetadataTypeDef",
     "LcmOperationInfoTypeDef",
     "GetSolNetworkOperationInputRequestTypeDef",
     "GetSolNetworkOperationMetadataTypeDef",
     "ProblemDetailsTypeDef",
     "GetSolNetworkPackageContentInputRequestTypeDef",
+    "GetSolNetworkPackageContentOutputTypeDef",
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
     "GetSolNetworkPackageInputRequestTypeDef",
     "GetSolVnfcResourceInfoMetadataTypeDef",
     "InstantiateSolNetworkInstanceInputRequestTypeDef",
+    "InstantiateSolNetworkInstanceOutputTypeDef",
     "ListSolFunctionInstanceMetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
     "ListSolFunctionInstancesInputRequestTypeDef",
     "ListSolFunctionPackageMetadataTypeDef",
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
     "ListSolFunctionPackagesInputRequestTypeDef",
     "ListSolNetworkInstanceMetadataTypeDef",
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutSolFunctionPackageContentInputRequestTypeDef",
     "PutSolNetworkPackageContentInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
+    "TerminateSolNetworkInstanceOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
+    "UpdateSolFunctionPackageOutputTypeDef",
     "UpdateSolNetworkModifyTypeDef",
+    "UpdateSolNetworkInstanceOutputTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
+    "UpdateSolNetworkPackageOutputTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
-    "CreateSolFunctionPackageOutputTypeDef",
-    "CreateSolNetworkInstanceOutputTypeDef",
-    "CreateSolNetworkPackageOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetSolFunctionPackageContentOutputTypeDef",
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    "GetSolNetworkPackageContentOutputTypeDef",
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "TerminateSolNetworkInstanceOutputTypeDef",
-    "UpdateSolFunctionPackageOutputTypeDef",
-    "UpdateSolNetworkInstanceOutputTypeDef",
-    "UpdateSolNetworkPackageOutputTypeDef",
     "GetSolNetworkOperationTaskDetailsTypeDef",
     "FunctionArtifactMetaTypeDef",
     "NetworkArtifactMetaTypeDef",
     "GetSolNetworkInstanceOutputTypeDef",
     "GetSolVnfcResourceInfoTypeDef",
     "ListSolFunctionInstanceInfoTypeDef",
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolFunctionPackageInfoTypeDef",
     "ListSolNetworkInstanceInfoTypeDef",
     "ListSolNetworkOperationsInfoTypeDef",
     "ListSolNetworkPackageInfoTypeDef",
     "UpdateSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkOperationOutputTypeDef",
     "GetSolFunctionPackageMetadataTypeDef",
@@ -155,22 +155,24 @@
     "CreateSolFunctionPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSolFunctionPackageOutputTypeDef = TypedDict(
+    "CreateSolFunctionPackageOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "id": str,
+        "onboardingState": OnboardingStateType,
+        "operationalState": OperationalStateType,
+        "tags": Dict[str, str],
+        "usageState": UsageStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSolNetworkInstanceInputRequestTypeDef = TypedDict(
     "_RequiredCreateSolNetworkInstanceInputRequestTypeDef",
     {
         "nsName": str,
@@ -190,22 +192,47 @@
 class CreateSolNetworkInstanceInputRequestTypeDef(
     _RequiredCreateSolNetworkInstanceInputRequestTypeDef,
     _OptionalCreateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
+CreateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "CreateSolNetworkInstanceOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsInstanceName": str,
+        "nsdInfoId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "CreateSolNetworkPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+CreateSolNetworkPackageOutputTypeDef = TypedDict(
+    "CreateSolNetworkPackageOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsdOnboardingState": NsdOnboardingStateType,
+        "nsdOperationalState": NsdOperationalStateType,
+        "nsdUsageState": NsdUsageStateType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSolFunctionPackageInputRequestTypeDef = TypedDict(
     "DeleteSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -219,14 +246,21 @@
 DeleteSolNetworkPackageInputRequestTypeDef = TypedDict(
     "DeleteSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "cause": str,
         "details": str,
     },
     total=False,
@@ -260,22 +294,40 @@
     "GetSolFunctionPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "vnfPkgId": str,
     },
 )
 
+GetSolFunctionPackageContentOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "packageContent": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolFunctionPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
     {
         "accept": Literal["text/plain"],
         "vnfPkgId": str,
     },
 )
 
+GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "vnfd": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolFunctionPackageInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -347,21 +399,39 @@
     "GetSolNetworkPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "nsdInfoId": str,
     },
 )
 
+GetSolNetworkPackageContentOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "nsdContent": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolNetworkPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
+GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "nsd": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolNetworkPackageInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
@@ -395,28 +465,35 @@
 class InstantiateSolNetworkInstanceInputRequestTypeDef(
     _RequiredInstantiateSolNetworkInstanceInputRequestTypeDef,
     _OptionalInstantiateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
+InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListSolFunctionInstanceMetadataTypeDef = TypedDict(
     "ListSolFunctionInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSolFunctionInstancesInputRequestTypeDef = TypedDict(
     "ListSolFunctionInstancesInputRequestTypeDef",
     {
@@ -430,14 +507,22 @@
     "ListSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolFunctionPackagesInputRequestTypeDef = TypedDict(
     "ListSolFunctionPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -447,14 +532,22 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolNetworkInstancesInputRequestTypeDef = TypedDict(
     "ListSolNetworkInstancesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -464,14 +557,22 @@
     "ListSolNetworkOperationsMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolNetworkOperationsInputRequestTypeDef = TypedDict(
     "ListSolNetworkOperationsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -481,14 +582,22 @@
     "ListSolNetworkPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolNetworkPackagesInputRequestTypeDef = TypedDict(
     "ListSolNetworkPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -497,14 +606,32 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
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
 _RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -543,14 +670,25 @@
 class PutSolNetworkPackageContentInputRequestTypeDef(
     _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
     _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
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
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -573,14 +711,23 @@
 class TerminateSolNetworkInstanceInputRequestTypeDef(
     _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
     _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
+TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -589,30 +736,55 @@
     "UpdateSolFunctionPackageInputRequestTypeDef",
     {
         "operationalState": OperationalStateType,
         "vnfPkgId": str,
     },
 )
 
+UpdateSolFunctionPackageOutputTypeDef = TypedDict(
+    "UpdateSolFunctionPackageOutputTypeDef",
+    {
+        "operationalState": OperationalStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSolNetworkModifyTypeDef = TypedDict(
     "UpdateSolNetworkModifyTypeDef",
     {
         "vnfConfigurableProperties": Mapping[str, Any],
         "vnfInstanceId": str,
     },
 )
 
+UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "UpdateSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
         "nsdOperationalState": NsdOperationalStateType,
     },
 )
 
+UpdateSolNetworkPackageOutputTypeDef = TypedDict(
+    "UpdateSolNetworkPackageOutputTypeDef",
+    {
+        "nsdOperationalState": NsdOperationalStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -651,146 +823,14 @@
 class ValidateSolNetworkPackageContentInputRequestTypeDef(
     _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
     _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
 
-CreateSolFunctionPackageOutputTypeDef = TypedDict(
-    "CreateSolFunctionPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "onboardingState": OnboardingStateType,
-        "operationalState": OperationalStateType,
-        "tags": Dict[str, str],
-        "usageState": UsageStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "CreateSolNetworkInstanceOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsInstanceName": str,
-        "nsdInfoId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolNetworkPackageOutputTypeDef = TypedDict(
-    "CreateSolNetworkPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsdOnboardingState": NsdOnboardingStateType,
-        "nsdOperationalState": NsdOperationalStateType,
-        "nsdUsageState": NsdUsageStateType,
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
-GetSolFunctionPackageContentOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "packageContent": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "vnfd": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSolNetworkPackageContentOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "nsdContent": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "nsd": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "TerminateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSolFunctionPackageOutputTypeDef = TypedDict(
-    "UpdateSolFunctionPackageOutputTypeDef",
-    {
-        "operationalState": OperationalStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "UpdateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSolNetworkPackageOutputTypeDef = TypedDict(
-    "UpdateSolNetworkPackageOutputTypeDef",
-    {
-        "nsdOperationalState": NsdOperationalStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetSolNetworkOperationTaskDetailsTypeDef = TypedDict(
     "GetSolNetworkOperationTaskDetailsTypeDef",
     {
         "taskContext": Dict[str, str],
         "taskEndTime": datetime,
         "taskErrorDetails": ErrorInfoTypeDef,
         "taskName": str,
@@ -825,15 +865,15 @@
         "metadata": GetSolNetworkInstanceMetadataTypeDef,
         "nsInstanceDescription": str,
         "nsInstanceName": str,
         "nsState": NsStateType,
         "nsdId": str,
         "nsdInfoId": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolVnfcResourceInfoTypeDef = TypedDict(
     "GetSolVnfcResourceInfoTypeDef",
     {
         "metadata": GetSolVnfcResourceInfoMetadataTypeDef,
@@ -864,54 +904,14 @@
 
 class ListSolFunctionInstanceInfoTypeDef(
     _RequiredListSolFunctionInstanceInfoTypeDef, _OptionalListSolFunctionInstanceInfoTypeDef
 ):
     pass
 
 
-ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListSolFunctionPackageInfoTypeDef = TypedDict(
     "_RequiredListSolFunctionPackageInfoTypeDef",
     {
         "arn": str,
         "id": str,
         "onboardingState": OnboardingStateType,
         "operationalState": OperationalStateType,
@@ -1040,15 +1040,15 @@
         "id": str,
         "lcmOperationType": LcmOperationTypeType,
         "metadata": GetSolNetworkOperationMetadataTypeDef,
         "nsInstanceId": str,
         "operationState": NsLcmOperationStateType,
         "tags": Dict[str, str],
         "tasks": List[GetSolNetworkOperationTaskDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetSolFunctionPackageMetadataTypeDef = TypedDict(
     "_RequiredGetSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
@@ -1134,51 +1134,51 @@
 )
 
 ListSolFunctionInstancesOutputTypeDef = TypedDict(
     "ListSolFunctionInstancesOutputTypeDef",
     {
         "functionInstances": List[ListSolFunctionInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolFunctionPackagesOutputTypeDef = TypedDict(
     "ListSolFunctionPackagesOutputTypeDef",
     {
         "functionPackages": List[ListSolFunctionPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolNetworkInstancesOutputTypeDef = TypedDict(
     "ListSolNetworkInstancesOutputTypeDef",
     {
         "networkInstances": List[ListSolNetworkInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolNetworkOperationsOutputTypeDef = TypedDict(
     "ListSolNetworkOperationsOutputTypeDef",
     {
         "networkOperations": List[ListSolNetworkOperationsInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolNetworkPackagesOutputTypeDef = TypedDict(
     "ListSolNetworkPackagesOutputTypeDef",
     {
         "networkPackages": List[ListSolNetworkPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolFunctionPackageOutputTypeDef = TypedDict(
     "GetSolFunctionPackageOutputTypeDef",
     {
         "arn": str,
@@ -1188,41 +1188,41 @@
         "operationalState": OperationalStateType,
         "tags": Dict[str, str],
         "usageState": UsageStateType,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutSolFunctionPackageContentOutputTypeDef = TypedDict(
     "PutSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": PutSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidateSolFunctionPackageContentOutputTypeDef = TypedDict(
     "ValidateSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": ValidateSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolNetworkPackageOutputTypeDef = TypedDict(
     "GetSolNetworkPackageOutputTypeDef",
     {
         "arn": str,
@@ -1232,43 +1232,43 @@
         "nsdName": str,
         "nsdOnboardingState": NsdOnboardingStateType,
         "nsdOperationalState": NsdOperationalStateType,
         "nsdUsageState": NsdUsageStateType,
         "nsdVersion": str,
         "tags": Dict[str, str],
         "vnfPkgIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutSolNetworkPackageContentOutputTypeDef = TypedDict(
     "PutSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": PutSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidateSolNetworkPackageContentOutputTypeDef = TypedDict(
     "ValidateSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": ValidateSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolFunctionInstanceOutputTypeDef = TypedDict(
     "GetSolFunctionInstanceOutputTypeDef",
     {
         "arn": str,
@@ -1279,10 +1279,10 @@
         "nsInstanceId": str,
         "tags": Dict[str, str],
         "vnfPkgId": str,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb/type_defs.pyi` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,86 +40,86 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateSolFunctionPackageOutputTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
+    "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
+    "CreateSolNetworkPackageOutputTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
     "DeleteSolNetworkPackageInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "ToscaOverrideTypeDef",
     "GetSolFunctionInstanceInputRequestTypeDef",
     "GetSolFunctionInstanceMetadataTypeDef",
     "GetSolFunctionPackageContentInputRequestTypeDef",
+    "GetSolFunctionPackageContentOutputTypeDef",
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
     "GetSolFunctionPackageInputRequestTypeDef",
     "GetSolInstantiatedVnfInfoTypeDef",
     "GetSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkInstanceMetadataTypeDef",
     "LcmOperationInfoTypeDef",
     "GetSolNetworkOperationInputRequestTypeDef",
     "GetSolNetworkOperationMetadataTypeDef",
     "ProblemDetailsTypeDef",
     "GetSolNetworkPackageContentInputRequestTypeDef",
+    "GetSolNetworkPackageContentOutputTypeDef",
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
     "GetSolNetworkPackageInputRequestTypeDef",
     "GetSolVnfcResourceInfoMetadataTypeDef",
     "InstantiateSolNetworkInstanceInputRequestTypeDef",
+    "InstantiateSolNetworkInstanceOutputTypeDef",
     "ListSolFunctionInstanceMetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
     "ListSolFunctionInstancesInputRequestTypeDef",
     "ListSolFunctionPackageMetadataTypeDef",
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
     "ListSolFunctionPackagesInputRequestTypeDef",
     "ListSolNetworkInstanceMetadataTypeDef",
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutSolFunctionPackageContentInputRequestTypeDef",
     "PutSolNetworkPackageContentInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
+    "TerminateSolNetworkInstanceOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
+    "UpdateSolFunctionPackageOutputTypeDef",
     "UpdateSolNetworkModifyTypeDef",
+    "UpdateSolNetworkInstanceOutputTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
+    "UpdateSolNetworkPackageOutputTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
-    "CreateSolFunctionPackageOutputTypeDef",
-    "CreateSolNetworkInstanceOutputTypeDef",
-    "CreateSolNetworkPackageOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetSolFunctionPackageContentOutputTypeDef",
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    "GetSolNetworkPackageContentOutputTypeDef",
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "TerminateSolNetworkInstanceOutputTypeDef",
-    "UpdateSolFunctionPackageOutputTypeDef",
-    "UpdateSolNetworkInstanceOutputTypeDef",
-    "UpdateSolNetworkPackageOutputTypeDef",
     "GetSolNetworkOperationTaskDetailsTypeDef",
     "FunctionArtifactMetaTypeDef",
     "NetworkArtifactMetaTypeDef",
     "GetSolNetworkInstanceOutputTypeDef",
     "GetSolVnfcResourceInfoTypeDef",
     "ListSolFunctionInstanceInfoTypeDef",
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolFunctionPackageInfoTypeDef",
     "ListSolNetworkInstanceInfoTypeDef",
     "ListSolNetworkOperationsInfoTypeDef",
     "ListSolNetworkPackageInfoTypeDef",
     "UpdateSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkOperationOutputTypeDef",
     "GetSolFunctionPackageMetadataTypeDef",
@@ -154,22 +154,24 @@
     "CreateSolFunctionPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSolFunctionPackageOutputTypeDef = TypedDict(
+    "CreateSolFunctionPackageOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "id": str,
+        "onboardingState": OnboardingStateType,
+        "operationalState": OperationalStateType,
+        "tags": Dict[str, str],
+        "usageState": UsageStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSolNetworkInstanceInputRequestTypeDef = TypedDict(
     "_RequiredCreateSolNetworkInstanceInputRequestTypeDef",
     {
         "nsName": str,
@@ -187,22 +189,47 @@
 
 class CreateSolNetworkInstanceInputRequestTypeDef(
     _RequiredCreateSolNetworkInstanceInputRequestTypeDef,
     _OptionalCreateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
+CreateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "CreateSolNetworkInstanceOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsInstanceName": str,
+        "nsdInfoId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "CreateSolNetworkPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+CreateSolNetworkPackageOutputTypeDef = TypedDict(
+    "CreateSolNetworkPackageOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsdOnboardingState": NsdOnboardingStateType,
+        "nsdOperationalState": NsdOperationalStateType,
+        "nsdUsageState": NsdUsageStateType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSolFunctionPackageInputRequestTypeDef = TypedDict(
     "DeleteSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -216,14 +243,21 @@
 DeleteSolNetworkPackageInputRequestTypeDef = TypedDict(
     "DeleteSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "cause": str,
         "details": str,
     },
     total=False,
@@ -257,22 +291,40 @@
     "GetSolFunctionPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "vnfPkgId": str,
     },
 )
 
+GetSolFunctionPackageContentOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "packageContent": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolFunctionPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
     {
         "accept": Literal["text/plain"],
         "vnfPkgId": str,
     },
 )
 
+GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "vnfd": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolFunctionPackageInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -342,21 +394,39 @@
     "GetSolNetworkPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "nsdInfoId": str,
     },
 )
 
+GetSolNetworkPackageContentOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "nsdContent": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolNetworkPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
+GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "nsd": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSolNetworkPackageInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
@@ -388,28 +458,35 @@
 
 class InstantiateSolNetworkInstanceInputRequestTypeDef(
     _RequiredInstantiateSolNetworkInstanceInputRequestTypeDef,
     _OptionalInstantiateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
+InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListSolFunctionInstanceMetadataTypeDef = TypedDict(
     "ListSolFunctionInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSolFunctionInstancesInputRequestTypeDef = TypedDict(
     "ListSolFunctionInstancesInputRequestTypeDef",
     {
@@ -423,14 +500,22 @@
     "ListSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolFunctionPackagesInputRequestTypeDef = TypedDict(
     "ListSolFunctionPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -440,14 +525,22 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolNetworkInstancesInputRequestTypeDef = TypedDict(
     "ListSolNetworkInstancesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -457,14 +550,22 @@
     "ListSolNetworkOperationsMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolNetworkOperationsInputRequestTypeDef = TypedDict(
     "ListSolNetworkOperationsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -474,14 +575,22 @@
     "ListSolNetworkPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
+ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSolNetworkPackagesInputRequestTypeDef = TypedDict(
     "ListSolNetworkPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -490,14 +599,32 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
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
 _RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -532,14 +659,25 @@
 
 class PutSolNetworkPackageContentInputRequestTypeDef(
     _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
     _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
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
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -560,14 +698,23 @@
 
 class TerminateSolNetworkInstanceInputRequestTypeDef(
     _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
     _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
+TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -576,30 +723,55 @@
     "UpdateSolFunctionPackageInputRequestTypeDef",
     {
         "operationalState": OperationalStateType,
         "vnfPkgId": str,
     },
 )
 
+UpdateSolFunctionPackageOutputTypeDef = TypedDict(
+    "UpdateSolFunctionPackageOutputTypeDef",
+    {
+        "operationalState": OperationalStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSolNetworkModifyTypeDef = TypedDict(
     "UpdateSolNetworkModifyTypeDef",
     {
         "vnfConfigurableProperties": Mapping[str, Any],
         "vnfInstanceId": str,
     },
 )
 
+UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "UpdateSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
         "nsdOperationalState": NsdOperationalStateType,
     },
 )
 
+UpdateSolNetworkPackageOutputTypeDef = TypedDict(
+    "UpdateSolNetworkPackageOutputTypeDef",
+    {
+        "nsdOperationalState": NsdOperationalStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -634,146 +806,14 @@
 
 class ValidateSolNetworkPackageContentInputRequestTypeDef(
     _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
     _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
-CreateSolFunctionPackageOutputTypeDef = TypedDict(
-    "CreateSolFunctionPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "onboardingState": OnboardingStateType,
-        "operationalState": OperationalStateType,
-        "tags": Dict[str, str],
-        "usageState": UsageStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "CreateSolNetworkInstanceOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsInstanceName": str,
-        "nsdInfoId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSolNetworkPackageOutputTypeDef = TypedDict(
-    "CreateSolNetworkPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsdOnboardingState": NsdOnboardingStateType,
-        "nsdOperationalState": NsdOperationalStateType,
-        "nsdUsageState": NsdUsageStateType,
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
-GetSolFunctionPackageContentOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "packageContent": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "vnfd": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSolNetworkPackageContentOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "nsdContent": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "nsd": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "TerminateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSolFunctionPackageOutputTypeDef = TypedDict(
-    "UpdateSolFunctionPackageOutputTypeDef",
-    {
-        "operationalState": OperationalStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "UpdateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSolNetworkPackageOutputTypeDef = TypedDict(
-    "UpdateSolNetworkPackageOutputTypeDef",
-    {
-        "nsdOperationalState": NsdOperationalStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetSolNetworkOperationTaskDetailsTypeDef = TypedDict(
     "GetSolNetworkOperationTaskDetailsTypeDef",
     {
         "taskContext": Dict[str, str],
         "taskEndTime": datetime,
         "taskErrorDetails": ErrorInfoTypeDef,
         "taskName": str,
@@ -808,15 +848,15 @@
         "metadata": GetSolNetworkInstanceMetadataTypeDef,
         "nsInstanceDescription": str,
         "nsInstanceName": str,
         "nsState": NsStateType,
         "nsdId": str,
         "nsdInfoId": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolVnfcResourceInfoTypeDef = TypedDict(
     "GetSolVnfcResourceInfoTypeDef",
     {
         "metadata": GetSolVnfcResourceInfoMetadataTypeDef,
@@ -845,54 +885,14 @@
 )
 
 class ListSolFunctionInstanceInfoTypeDef(
     _RequiredListSolFunctionInstanceInfoTypeDef, _OptionalListSolFunctionInstanceInfoTypeDef
 ):
     pass
 
-ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListSolFunctionPackageInfoTypeDef = TypedDict(
     "_RequiredListSolFunctionPackageInfoTypeDef",
     {
         "arn": str,
         "id": str,
         "onboardingState": OnboardingStateType,
         "operationalState": OperationalStateType,
@@ -1013,15 +1013,15 @@
         "id": str,
         "lcmOperationType": LcmOperationTypeType,
         "metadata": GetSolNetworkOperationMetadataTypeDef,
         "nsInstanceId": str,
         "operationState": NsLcmOperationStateType,
         "tags": Dict[str, str],
         "tasks": List[GetSolNetworkOperationTaskDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetSolFunctionPackageMetadataTypeDef = TypedDict(
     "_RequiredGetSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
@@ -1103,51 +1103,51 @@
 )
 
 ListSolFunctionInstancesOutputTypeDef = TypedDict(
     "ListSolFunctionInstancesOutputTypeDef",
     {
         "functionInstances": List[ListSolFunctionInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolFunctionPackagesOutputTypeDef = TypedDict(
     "ListSolFunctionPackagesOutputTypeDef",
     {
         "functionPackages": List[ListSolFunctionPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolNetworkInstancesOutputTypeDef = TypedDict(
     "ListSolNetworkInstancesOutputTypeDef",
     {
         "networkInstances": List[ListSolNetworkInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolNetworkOperationsOutputTypeDef = TypedDict(
     "ListSolNetworkOperationsOutputTypeDef",
     {
         "networkOperations": List[ListSolNetworkOperationsInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSolNetworkPackagesOutputTypeDef = TypedDict(
     "ListSolNetworkPackagesOutputTypeDef",
     {
         "networkPackages": List[ListSolNetworkPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolFunctionPackageOutputTypeDef = TypedDict(
     "GetSolFunctionPackageOutputTypeDef",
     {
         "arn": str,
@@ -1157,41 +1157,41 @@
         "operationalState": OperationalStateType,
         "tags": Dict[str, str],
         "usageState": UsageStateType,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutSolFunctionPackageContentOutputTypeDef = TypedDict(
     "PutSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": PutSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidateSolFunctionPackageContentOutputTypeDef = TypedDict(
     "ValidateSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": ValidateSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolNetworkPackageOutputTypeDef = TypedDict(
     "GetSolNetworkPackageOutputTypeDef",
     {
         "arn": str,
@@ -1201,43 +1201,43 @@
         "nsdName": str,
         "nsdOnboardingState": NsdOnboardingStateType,
         "nsdOperationalState": NsdOperationalStateType,
         "nsdUsageState": NsdUsageStateType,
         "nsdVersion": str,
         "tags": Dict[str, str],
         "vnfPkgIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutSolNetworkPackageContentOutputTypeDef = TypedDict(
     "PutSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": PutSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidateSolNetworkPackageContentOutputTypeDef = TypedDict(
     "ValidateSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": ValidateSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSolFunctionInstanceOutputTypeDef = TypedDict(
     "GetSolFunctionInstanceOutputTypeDef",
     {
         "arn": str,
@@ -1248,10 +1248,10 @@
         "nsInstanceId": str,
         "tags": Dict[str, str],
         "vnfPkgId": str,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/PKG-INFO` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-tnb
-Version: 1.26.90
-Summary: Type annotations for boto3.TelcoNetworkBuilder 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.TelcoNetworkBuilder 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-tnb"></a>
 
 # mypy-boto3-tnb
 
 [![PyPI - mypy-boto3-tnb](https://img.shields.io/pypi/v/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-tnb?color=blue)](https://pypistats.org/packages/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,86 +357,86 @@
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutSolFunctionPackageContentInputRequestTypeDef,
     PutSolNetworkPackageContentInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
@@ -468,42 +468,42 @@
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

### Comparing `mypy-boto3-tnb-1.26.90/mypy_boto3_tnb.egg-info/SOURCES.txt` & `mypy-boto3-tnb-1.27.0/mypy_boto3_tnb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.26.90/setup.py` & `mypy-boto3-tnb-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-tnb.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-tnb",
-    version="1.26.90",
+    version="1.27.0",
     packages=["mypy_boto3_tnb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TelcoNetworkBuilder 1.26.90 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.TelcoNetworkBuilder 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/",
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


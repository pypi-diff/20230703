# Comparing `tmp/mypy-boto3-ecr-public-1.26.46.tar.gz` & `tmp/mypy-boto3-ecr-public-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-public-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-public-1.27.0.tar", last modified: Mon Jul  3 19:50:42 2023, max compression
```

## Comparing `mypy-boto3-ecr-public-1.26.46.tar` & `mypy-boto3-ecr-public-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.308431 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.655182 mypy-boto3-ecr-public-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-07-03 19:50:42.651182 mypy-boto3-ecr-public-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.651182 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-03 19:36:57.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-03 19:36:58.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-03 19:36:57.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-03 19:36:57.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 19:36:57.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-07-03 19:36:59.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-07-03 19:36:58.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.651182 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-07-03 19:50:42.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:42.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:42.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:42.000000 mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:42.655182 mypy-boto3-ecr-public-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-03 19:36:56.000000 mypy-boto3-ecr-public-1.27.0/setup.py
```

### Comparing `mypy-boto3-ecr-public-1.26.46/LICENSE` & `mypy-boto3-ecr-public-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ecr-public-1.26.46/PKG-INFO` & `mypy-boto3-ecr-public-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.26.46
-Summary: Type annotations for boto3.ECRPublic 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ECRPublic 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,65 +343,65 @@
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
-    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
+    CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
+    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
+    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UploadLayerPartResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
@@ -417,42 +417,42 @@
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

### Comparing `mypy-boto3-ecr-public-1.26.46/README.md` & `mypy-boto3-ecr-public-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,65 +311,65 @@
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
-    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
+    CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
+    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
+    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UploadLayerPartResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
@@ -385,42 +385,42 @@
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

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.py` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.pyi` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__main__.py` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECRPublic 1.26.46\nVersion:         1.26.46\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.ECRPublic 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.46")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.py` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.pyi` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.py` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,15 @@
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
@@ -92,31 +93,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -195,14 +199,15 @@
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
@@ -213,14 +218,15 @@
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
@@ -256,14 +262,15 @@
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
@@ -282,16 +289,19 @@
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
@@ -371,18 +381,21 @@
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

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.pyi` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,15 @@
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
@@ -90,31 +91,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -193,14 +197,15 @@
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
@@ -211,14 +216,15 @@
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
@@ -254,14 +260,15 @@
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
@@ -280,16 +287,19 @@
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
@@ -369,18 +379,21 @@
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

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.py` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 
@@ -83,30 +83,30 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagespaginator)
         """
 
 
 class DescribeRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
         """
 
 
@@ -117,13 +117,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.pyi` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 class DescribeImagesPaginator(Paginator):
@@ -79,29 +79,29 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeimagespaginator)
         """
 
 class DescribeRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describeregistriespaginator)
         """
 
 class DescribeRepositoriesPaginator(Paginator):
@@ -111,13 +111,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.py` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,71 +25,70 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
-    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
     "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
     "ImageDetailTypeDef",
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
     "DescribeRegistriesRequestRequestTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "RegistryCatalogDataTypeDef",
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
+    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
-    "BatchCheckLayerAvailabilityResponseTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "UploadLayerPartResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "BatchCheckLayerAvailabilityResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "PutRepositoryCatalogDataRequestRequestTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
-    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
@@ -117,22 +116,20 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -146,25 +143,14 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
@@ -182,21 +168,30 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 RepositoryCatalogDataInputTypeDef = TypedDict(
     "RepositoryCatalogDataInputTypeDef",
     {
         "description": str,
         "architectures": Sequence[str],
         "operatingSystems": Sequence[str],
@@ -252,21 +247,29 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -275,31 +278,40 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
+    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -308,21 +320,19 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImageTagsRequestRequestTypeDef(
     _RequiredDescribeImageTagsRequestRequestTypeDef, _OptionalDescribeImageTagsRequestRequestTypeDef
 ):
     pass
 
-
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -330,23 +340,41 @@
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
         "artifactMediaType": str,
     },
     total=False,
 )
 
+DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRegistriesRequestRequestTypeDef = TypedDict(
     "DescribeRegistriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -372,43 +400,49 @@
     "_OptionalGetRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredGetRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalGetRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ReferencedImageDetailTypeDef = TypedDict(
     "ReferencedImageDetailTypeDef",
     {
         "imageDigest": str,
         "imageSizeInBytes": int,
         "imagePushedAt": datetime,
@@ -428,29 +462,46 @@
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -461,21 +512,19 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
-
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
-
 PutRegistryCatalogDataRequestRequestTypeDef = TypedDict(
     "PutRegistryCatalogDataRequestRequestTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
@@ -486,14 +535,25 @@
         "name": str,
         "status": RegistryAliasStatusType,
         "primaryRegistryAlias": bool,
         "defaultRegistryAlias": bool,
     },
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -502,21 +562,29 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -536,121 +604,89 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
-    {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "lastByteReceived": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": AuthorizationDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
     {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
+_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
-        "registryId": str,
         "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeleteImageRequestRequestTypeDef",
+class BatchDeleteImageRequestRequestTypeDef(
+    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
+):
+    pass
+
+_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeleteImageRequestRequestTypeDef",
+_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class BatchDeleteImageRequestRequestTypeDef(
-    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
+class DescribeImagesRequestDescribeImagesPaginateTypeDef(
+    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
+    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -660,21 +696,19 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
-
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
         "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
@@ -704,22 +738,20 @@
     "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
@@ -727,26 +759,24 @@
     {
         "catalogData": RepositoryCatalogDataInputTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -754,139 +784,74 @@
     },
 )
 
 GetRepositoryCatalogDataResponseTypeDef = TypedDict(
     "GetRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRepositoryCatalogDataResponseTypeDef = TypedDict(
     "PutRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
-    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "repositoryName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "registryId": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeImagesRequestDescribeImagesPaginateTypeDef(
-    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
-    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
-):
-    pass
-
-
-DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegistryCatalogDataResponseTypeDef = TypedDict(
     "GetRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRegistryCatalogDataResponseTypeDef = TypedDict(
     "PutRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageTagDetailTypeDef = TypedDict(
     "ImageTagDetailTypeDef",
     {
         "imageTag": str,
@@ -908,36 +873,36 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRegistriesResponseTypeDef = TypedDict(
     "DescribeRegistriesResponseTypeDef",
     {
         "registries": List[RegistryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.pyi` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,70 +25,71 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
-    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
     "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
     "DescribeImageTagsRequestRequestTypeDef",
     "ImageDetailTypeDef",
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
     "DescribeRegistriesRequestRequestTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "RegistryCatalogDataTypeDef",
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
+    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
-    "BatchCheckLayerAvailabilityResponseTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "UploadLayerPartResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "BatchCheckLayerAvailabilityResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "PutRepositoryCatalogDataRequestRequestTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
-    "DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
@@ -116,20 +117,22 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
+
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -143,25 +146,14 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
@@ -179,20 +171,33 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RepositoryCatalogDataInputTypeDef = TypedDict(
     "RepositoryCatalogDataInputTypeDef",
     {
         "description": str,
         "architectures": Sequence[str],
         "operatingSystems": Sequence[str],
         "logoImageBlob": Union[str, bytes, IO[Any], StreamingBody],
@@ -247,20 +252,32 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -268,29 +285,44 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "repositoryName": str,
+    },
+)
+_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
+    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -299,19 +331,21 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImageTagsRequestRequestTypeDef(
     _RequiredDescribeImageTagsRequestRequestTypeDef, _OptionalDescribeImageTagsRequestRequestTypeDef
 ):
     pass
 
+
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -319,23 +353,41 @@
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
         "artifactMediaType": str,
     },
     total=False,
 )
 
+DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
+    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRegistriesRequestRequestTypeDef = TypedDict(
     "DescribeRegistriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -361,40 +413,54 @@
     "_OptionalGetRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredGetRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalGetRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReferencedImageDetailTypeDef = TypedDict(
     "ReferencedImageDetailTypeDef",
     {
         "imageDigest": str,
         "imageSizeInBytes": int,
         "imagePushedAt": datetime,
         "imageManifestMediaType": str,
@@ -413,27 +479,48 @@
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -444,19 +531,21 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
+
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
+
 PutRegistryCatalogDataRequestRequestTypeDef = TypedDict(
     "PutRegistryCatalogDataRequestRequestTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
@@ -467,14 +556,25 @@
         "name": str,
         "status": RegistryAliasStatusType,
         "primaryRegistryAlias": bool,
         "defaultRegistryAlias": bool,
     },
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -483,20 +583,32 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -515,117 +627,95 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
-    {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "lastByteReceived": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": AuthorizationDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
     {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
+_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
-        "registryId": str,
         "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-_RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeleteImageRequestRequestTypeDef",
+
+class BatchDeleteImageRequestRequestTypeDef(
+    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
-_OptionalBatchDeleteImageRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeleteImageRequestRequestTypeDef",
+_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
+        "imageIds": Sequence[ImageIdentifierTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class BatchDeleteImageRequestRequestTypeDef(
-    _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
+
+class DescribeImagesRequestDescribeImagesPaginateTypeDef(
+    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
+    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -635,19 +725,21 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
+
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
         "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
@@ -677,20 +769,22 @@
     "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
@@ -698,24 +792,26 @@
     {
         "catalogData": RepositoryCatalogDataInputTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -723,135 +819,74 @@
     },
 )
 
 GetRepositoryCatalogDataResponseTypeDef = TypedDict(
     "GetRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRepositoryCatalogDataResponseTypeDef = TypedDict(
     "PutRepositoryCatalogDataResponseTypeDef",
     {
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "catalogData": RepositoryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
-    _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "registryId": str,
-        "imageIds": Sequence[ImageIdentifierTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeImagesRequestDescribeImagesPaginateTypeDef(
-    _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
-    _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
-):
-    pass
-
-DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = TypedDict(
-    "DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegistryCatalogDataResponseTypeDef = TypedDict(
     "GetRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRegistryCatalogDataResponseTypeDef = TypedDict(
     "PutRegistryCatalogDataResponseTypeDef",
     {
         "registryCatalogData": RegistryCatalogDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageTagDetailTypeDef = TypedDict(
     "ImageTagDetailTypeDef",
     {
         "imageTag": str,
@@ -873,36 +908,36 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageTagsResponseTypeDef = TypedDict(
     "DescribeImageTagsResponseTypeDef",
     {
         "imageTagDetails": List[ImageTagDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRegistriesResponseTypeDef = TypedDict(
     "DescribeRegistriesResponseTypeDef",
     {
         "registries": List[RegistryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/PKG-INFO` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.26.46
-Summary: Type annotations for boto3.ECRPublic 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ECRPublic 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,65 +343,65 @@
 
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
-    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
+    CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
     DescribeImageTagsRequestRequestTypeDef,
     ImageDetailTypeDef,
+    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
     DescribeRegistriesRequestRequestTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     RegistryCatalogDataTypeDef,
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
+    InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
+    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     UploadLayerPartResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
@@ -417,42 +417,42 @@
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

### Comparing `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/SOURCES.txt` & `mypy-boto3-ecr-public-1.27.0/mypy_boto3_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.46/setup.py` & `mypy-boto3-ecr-public-1.27.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-ecr-public.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr-public",
-    version="1.26.46",
+    version="1.27.0",
     packages=["mypy_boto3_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECRPublic 1.26.46 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.ECRPublic 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/",
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


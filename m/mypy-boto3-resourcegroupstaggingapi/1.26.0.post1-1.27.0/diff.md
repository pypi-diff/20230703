# Comparing `tmp/mypy-boto3-resourcegroupstaggingapi-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-resourcegroupstaggingapi-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resourcegroupstaggingapi-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:54 2022, max compression
+gzip compressed data, was "mypy-boto3-resourcegroupstaggingapi-1.27.0.tar", last modified: Mon Jul  3 19:51:20 2023, max compression
```

## Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1.tar` & `mypy-boto3-resourcegroupstaggingapi-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:54.572845 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14852 2022-11-01 21:43:54.572845 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13343 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:54.572845 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11246 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    11227 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8160 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5996 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5990 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8243 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8238 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:04.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:54.572845 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14852 2022-11-01 21:43:54.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-01 21:43:54.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:54.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:54.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:54.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-01 21:43:54.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:54.572845 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-11-01 21:40:03.000000 mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.015884 mypy-boto3-resourcegroupstaggingapi-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-03 19:51:20.007883 mypy-boto3-resourcegroupstaggingapi-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.999883 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:22.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.007883 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-03 19:51:19.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 19:51:19.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 19:51:19.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:20.015884 mypy-boto3-resourcegroupstaggingapi-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 19:46:21.000000 mypy-boto3-resourcegroupstaggingapi-1.27.0/setup.py
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/LICENSE` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/PKG-INFO` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resourcegroupstaggingapi
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/
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
 
 <a id="mypy-boto3-resourcegroupstaggingapi"></a>
 
 # mypy-boto3-resourcegroupstaggingapi
 
 [![PyPI - mypy-boto3-resourcegroupstaggingapi](https://img.shields.io/pypi/v/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,34 +337,34 @@
 
 `mypy_boto3_resourcegroupstaggingapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeReportCreationOutputTypeDef,
     FailureInfoTypeDef,
-    PaginatorConfigTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
+    GetTagValuesOutputTypeDef,
+    PaginatorConfigTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
-    DescribeReportCreationOutputTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
 
@@ -375,42 +376,42 @@
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/README.md` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resourcegroupstaggingapi"></a>
 
 # mypy-boto3-resourcegroupstaggingapi
 
 [![PyPI - mypy-boto3-resourcegroupstaggingapi](https://img.shields.io/pypi/v/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,34 +305,34 @@
 
 `mypy_boto3_resourcegroupstaggingapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeReportCreationOutputTypeDef,
     FailureInfoTypeDef,
-    PaginatorConfigTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
+    GetTagValuesOutputTypeDef,
+    PaginatorConfigTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
-    DescribeReportCreationOutputTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
 
@@ -344,42 +344,42 @@
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/__init__.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/__init__.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/__main__.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/client.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,25 +185,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/client/#start_report_creation)
         """
 
     def tag_resources(
         self, *, ResourceARNList: Sequence[str], Tags: Mapping[str, str]
     ) -> TagResourcesOutputTypeDef:
         """
-        .
+        Applies one or more tags to the specified resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.tag_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/client/#tag_resources)
         """
 
     def untag_resources(
         self, *, ResourceARNList: Sequence[str], TagKeys: Sequence[str]
     ) -> UntagResourcesOutputTypeDef:
         """
-        .
+        Removes the specified tags from the specified resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.untag_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/client/#untag_resources)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/client.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -171,24 +171,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.start_report_creation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/client/#start_report_creation)
         """
     def tag_resources(
         self, *, ResourceARNList: Sequence[str], Tags: Mapping[str, str]
     ) -> TagResourcesOutputTypeDef:
         """
-        .
+        Applies one or more tags to the specified resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.tag_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/client/#tag_resources)
         """
     def untag_resources(
         self, *, ResourceARNList: Sequence[str], TagKeys: Sequence[str]
     ) -> UntagResourcesOutputTypeDef:
         """
-        .
+        Removes the specified tags from the specified resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.untag_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/client/#untag_resources)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["get_compliance_summary"]
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/literals.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/literals.pyi`

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
     "ErrorCodeType",
     "GetComplianceSummaryPaginatorName",
     "GetResourcesPaginatorName",
     "GetTagKeysPaginatorName",
     "GetTagValuesPaginatorName",
     "GroupByAttributeType",
@@ -30,15 +29,14 @@
     "ResourceGroupsTaggingAPIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ErrorCodeType = Literal["InternalServiceException", "InvalidParameterException"]
 GetComplianceSummaryPaginatorName = Literal["get_compliance_summary"]
 GetResourcesPaginatorName = Literal["get_resources"]
 GetTagKeysPaginatorName = Literal["get_tag_keys"]
 GetTagValuesPaginatorName = Literal["get_tag_values"]
 GroupByAttributeType = Literal["REGION", "RESOURCE_TYPE", "TARGET_ID"]
 TargetIdTypeType = Literal["ACCOUNT", "OU", "ROOT"]
@@ -54,23 +52,25 @@
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
@@ -80,30 +80,35 @@
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
@@ -129,14 +134,15 @@
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
@@ -181,51 +187,57 @@
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
@@ -238,14 +250,15 @@
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
@@ -257,28 +270,35 @@
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
@@ -287,14 +307,15 @@
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
@@ -305,55 +326,64 @@
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
@@ -379,21 +409,25 @@
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/literals.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ErrorCodeType",
     "GetComplianceSummaryPaginatorName",
     "GetResourcesPaginatorName",
     "GetTagKeysPaginatorName",
     "GetTagValuesPaginatorName",
     "GroupByAttributeType",
@@ -29,14 +30,15 @@
     "ResourceGroupsTaggingAPIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ErrorCodeType = Literal["InternalServiceException", "InvalidParameterException"]
 GetComplianceSummaryPaginatorName = Literal["get_compliance_summary"]
 GetResourcesPaginatorName = Literal["get_resources"]
 GetTagKeysPaginatorName = Literal["get_tag_keys"]
 GetTagValuesPaginatorName = Literal["get_tag_values"]
 GroupByAttributeType = Literal["REGION", "RESOURCE_TYPE", "TARGET_ID"]
 TargetIdTypeType = Literal["ACCOUNT", "OU", "ROOT"]
@@ -52,23 +54,25 @@
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
@@ -78,30 +82,35 @@
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
@@ -127,14 +136,15 @@
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
@@ -179,51 +189,57 @@
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
@@ -236,14 +252,15 @@
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
@@ -255,28 +272,35 @@
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
@@ -285,14 +309,15 @@
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
@@ -303,55 +328,64 @@
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
@@ -377,21 +411,25 @@
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/paginator.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 
@@ -90,43 +90,43 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 
 class GetTagKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTagKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
         """
 
 
 class GetTagValuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
     """
 
     def paginate(
-        self, *, Key: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Key: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTagValuesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
         """
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/paginator.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 class GetResourcesPaginator(Paginator):
@@ -86,41 +86,41 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 class GetTagKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTagKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
         """
 
 class GetTagValuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
     """
 
     def paginate(
-        self, *, Key: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Key: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTagValuesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
         """
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/type_defs.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,34 +20,34 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ComplianceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeReportCreationOutputTypeDef",
     "FailureInfoTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
     "TagFilterTypeDef",
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
     "GetTagKeysInputRequestTypeDef",
+    "GetTagKeysOutputTypeDef",
+    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetTagValuesInputRequestTypeDef",
+    "GetTagValuesOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "StartReportCreationInputRequestTypeDef",
     "TagResourcesInputRequestTypeDef",
     "UntagResourcesInputRequestTypeDef",
-    "DescribeReportCreationOutputTypeDef",
-    "GetTagKeysOutputTypeDef",
-    "GetTagValuesOutputTypeDef",
     "TagResourcesOutputTypeDef",
     "UntagResourcesOutputTypeDef",
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetComplianceSummaryOutputTypeDef",
     "GetResourcesInputGetResourcesPaginateTypeDef",
     "GetResourcesInputRequestTypeDef",
     "ResourceTagMappingTypeDef",
     "GetResourcesOutputTypeDef",
 )
 
@@ -57,41 +57,43 @@
         "NoncompliantKeys": List[str],
         "KeysWithNoncompliantValues": List[str],
         "ComplianceStatus": bool,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeReportCreationOutputTypeDef = TypedDict(
+    "DescribeReportCreationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": str,
+        "S3Location": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "StatusCode": int,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TargetIdFilters": Sequence[str],
+        "RegionFilters": Sequence[str],
+        "ResourceTypeFilters": Sequence[str],
+        "TagKeyFilters": Sequence[str],
+        "GroupBy": Sequence[GroupByAttributeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetComplianceSummaryInputRequestTypeDef = TypedDict(
     "GetComplianceSummaryInputRequestTypeDef",
     {
@@ -124,22 +126,61 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetTagKeysInputRequestTypeDef = TypedDict(
     "GetTagKeysInputRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
+GetTagKeysOutputTypeDef = TypedDict(
+    "GetTagKeysOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagKeys": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetTagValuesInputGetTagValuesPaginateTypeDef(
+    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
+    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetTagValuesInputRequestTypeDef = TypedDict(
     "_RequiredGetTagValuesInputRequestTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalGetTagValuesInputRequestTypeDef = TypedDict(
@@ -153,22 +194,52 @@
 
 class GetTagValuesInputRequestTypeDef(
     _RequiredGetTagValuesInputRequestTypeDef, _OptionalGetTagValuesInputRequestTypeDef
 ):
     pass
 
 
+GetTagValuesOutputTypeDef = TypedDict(
+    "GetTagValuesOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagValues": List[str],
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 StartReportCreationInputRequestTypeDef = TypedDict(
     "StartReportCreationInputRequestTypeDef",
     {
         "S3Bucket": str,
     },
 )
 
@@ -184,120 +255,49 @@
     "UntagResourcesInputRequestTypeDef",
     {
         "ResourceARNList": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
-DescribeReportCreationOutputTypeDef = TypedDict(
-    "DescribeReportCreationOutputTypeDef",
-    {
-        "Status": str,
-        "S3Location": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagKeysOutputTypeDef = TypedDict(
-    "GetTagKeysOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagKeys": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagValuesOutputTypeDef = TypedDict(
-    "GetTagValuesOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagValues": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourcesOutputTypeDef = TypedDict(
     "TagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourcesOutputTypeDef = TypedDict(
     "UntagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
-    {
-        "TargetIdFilters": Sequence[str],
-        "RegionFilters": Sequence[str],
-        "ResourceTypeFilters": Sequence[str],
-        "TagKeyFilters": Sequence[str],
-        "GroupBy": Sequence[GroupByAttributeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "Key": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTagValuesInputGetTagValuesPaginateTypeDef(
-    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
-    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
-):
-    pass
-
 
 GetComplianceSummaryOutputTypeDef = TypedDict(
     "GetComplianceSummaryOutputTypeDef",
     {
         "SummaryList": List[SummaryTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcesInputGetResourcesPaginateTypeDef = TypedDict(
     "GetResourcesInputGetResourcesPaginateTypeDef",
     {
         "TagFilters": Sequence[TagFilterTypeDef],
         "TagsPerPage": int,
         "ResourceTypeFilters": Sequence[str],
         "IncludeComplianceDetails": bool,
         "ExcludeCompliantResources": bool,
         "ResourceARNList": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetResourcesInputRequestTypeDef = TypedDict(
     "GetResourcesInputRequestTypeDef",
     {
@@ -324,10 +324,10 @@
 )
 
 GetResourcesOutputTypeDef = TypedDict(
     "GetResourcesOutputTypeDef",
     {
         "PaginationToken": str,
         "ResourceTagMappingList": List[ResourceTagMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ComplianceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeReportCreationOutputTypeDef",
     "FailureInfoTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
     "TagFilterTypeDef",
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
     "GetTagKeysInputRequestTypeDef",
+    "GetTagKeysOutputTypeDef",
+    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetTagValuesInputRequestTypeDef",
+    "GetTagValuesOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "StartReportCreationInputRequestTypeDef",
     "TagResourcesInputRequestTypeDef",
     "UntagResourcesInputRequestTypeDef",
-    "DescribeReportCreationOutputTypeDef",
-    "GetTagKeysOutputTypeDef",
-    "GetTagValuesOutputTypeDef",
     "TagResourcesOutputTypeDef",
     "UntagResourcesOutputTypeDef",
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetComplianceSummaryOutputTypeDef",
     "GetResourcesInputGetResourcesPaginateTypeDef",
     "GetResourcesInputRequestTypeDef",
     "ResourceTagMappingTypeDef",
     "GetResourcesOutputTypeDef",
 )
 
@@ -56,41 +56,43 @@
         "NoncompliantKeys": List[str],
         "KeysWithNoncompliantValues": List[str],
         "ComplianceStatus": bool,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeReportCreationOutputTypeDef = TypedDict(
+    "DescribeReportCreationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": str,
+        "S3Location": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "StatusCode": int,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TargetIdFilters": Sequence[str],
+        "RegionFilters": Sequence[str],
+        "ResourceTypeFilters": Sequence[str],
+        "TagKeyFilters": Sequence[str],
+        "GroupBy": Sequence[GroupByAttributeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetComplianceSummaryInputRequestTypeDef = TypedDict(
     "GetComplianceSummaryInputRequestTypeDef",
     {
@@ -123,22 +125,59 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetTagKeysInputRequestTypeDef = TypedDict(
     "GetTagKeysInputRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
+GetTagKeysOutputTypeDef = TypedDict(
+    "GetTagKeysOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagKeys": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetTagValuesInputGetTagValuesPaginateTypeDef(
+    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
+    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetTagValuesInputRequestTypeDef = TypedDict(
     "_RequiredGetTagValuesInputRequestTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalGetTagValuesInputRequestTypeDef = TypedDict(
@@ -150,22 +189,52 @@
 )
 
 class GetTagValuesInputRequestTypeDef(
     _RequiredGetTagValuesInputRequestTypeDef, _OptionalGetTagValuesInputRequestTypeDef
 ):
     pass
 
+GetTagValuesOutputTypeDef = TypedDict(
+    "GetTagValuesOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagValues": List[str],
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 StartReportCreationInputRequestTypeDef = TypedDict(
     "StartReportCreationInputRequestTypeDef",
     {
         "S3Bucket": str,
     },
 )
 
@@ -181,118 +250,49 @@
     "UntagResourcesInputRequestTypeDef",
     {
         "ResourceARNList": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
-DescribeReportCreationOutputTypeDef = TypedDict(
-    "DescribeReportCreationOutputTypeDef",
-    {
-        "Status": str,
-        "S3Location": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagKeysOutputTypeDef = TypedDict(
-    "GetTagKeysOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagKeys": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagValuesOutputTypeDef = TypedDict(
-    "GetTagValuesOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagValues": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourcesOutputTypeDef = TypedDict(
     "TagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourcesOutputTypeDef = TypedDict(
     "UntagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
-    {
-        "TargetIdFilters": Sequence[str],
-        "RegionFilters": Sequence[str],
-        "ResourceTypeFilters": Sequence[str],
-        "TagKeyFilters": Sequence[str],
-        "GroupBy": Sequence[GroupByAttributeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetTagValuesInputGetTagValuesPaginateTypeDef(
-    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
-    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
-):
-    pass
-
 GetComplianceSummaryOutputTypeDef = TypedDict(
     "GetComplianceSummaryOutputTypeDef",
     {
         "SummaryList": List[SummaryTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcesInputGetResourcesPaginateTypeDef = TypedDict(
     "GetResourcesInputGetResourcesPaginateTypeDef",
     {
         "TagFilters": Sequence[TagFilterTypeDef],
         "TagsPerPage": int,
         "ResourceTypeFilters": Sequence[str],
         "IncludeComplianceDetails": bool,
         "ExcludeCompliantResources": bool,
         "ResourceARNList": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetResourcesInputRequestTypeDef = TypedDict(
     "GetResourcesInputRequestTypeDef",
     {
@@ -319,10 +319,10 @@
 )
 
 GetResourcesOutputTypeDef = TypedDict(
     "GetResourcesOutputTypeDef",
     {
         "PaginationToken": str,
         "ResourceTagMappingList": List[ResourceTagMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resourcegroupstaggingapi
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/
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
 
 <a id="mypy-boto3-resourcegroupstaggingapi"></a>
 
 # mypy-boto3-resourcegroupstaggingapi
 
 [![PyPI - mypy-boto3-resourcegroupstaggingapi](https://img.shields.io/pypi/v/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,34 +337,34 @@
 
 `mypy_boto3_resourcegroupstaggingapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeReportCreationOutputTypeDef,
     FailureInfoTypeDef,
-    PaginatorConfigTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
+    GetTagValuesOutputTypeDef,
+    PaginatorConfigTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
-    DescribeReportCreationOutputTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
 
@@ -375,42 +376,42 @@
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.26.0.post1/setup.py` & `mypy-boto3-resourcegroupstaggingapi-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 """
 Setup script for mypy-boto3-resourcegroupstaggingapi.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resourcegroupstaggingapi",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords=(
         "boto3 resourcegroupstaggingapi type-annotations boto3-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_resourcegroupstaggingapi": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_resourcegroupstaggingapi": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/"
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


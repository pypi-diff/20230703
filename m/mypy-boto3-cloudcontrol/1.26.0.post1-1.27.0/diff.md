# Comparing `tmp/mypy-boto3-cloudcontrol-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cloudcontrol-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudcontrol-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:11 2022, max compression
+gzip compressed data, was "mypy-boto3-cloudcontrol-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-cloudcontrol-1.26.0.post1.tar` & `mypy-boto3-cloudcontrol-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:11.764839 mypy-boto3-cloudcontrol-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14718 2022-11-01 21:43:11.764839 mypy-boto3-cloudcontrol-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13254 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:11.760839 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10786 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10768 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8429 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8427 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9701 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9686 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-11-01 21:31:18.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:11.764839 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14718 2022-11-01 21:43:11.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-01 21:43:11.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:11.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:11.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:11.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:11.000000 mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:11.764839 mypy-boto3-cloudcontrol-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-11-01 21:31:17.000000 mypy-boto3-cloudcontrol-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.306941 mypy-boto3-cloudcontrol-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-07-03 19:50:29.302941 mypy-boto3-cloudcontrol-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.302941 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-03 19:33:37.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-03 19:33:37.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.302941 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-07-03 19:50:29.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 19:50:29.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:29.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:29.000000 mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.306941 mypy-boto3-cloudcontrol-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 19:33:36.000000 mypy-boto3-cloudcontrol-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/LICENSE` & `mypy-boto3-cloudcontrol-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/PKG-INFO` & `mypy-boto3-cloudcontrol-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudcontrol
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CloudControlApi 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudControlApi 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/
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
 
 <a id="mypy-boto3-cloudcontrol"></a>
 
 # mypy-boto3-cloudcontrol
 
 [![PyPI - mypy-boto3-cloudcontrol](https://img.shields.io/pypi/v/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudcontrol?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,35 +354,35 @@
 `mypy_boto3_cloudcontrol.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
-    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
 def get_structure() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
@@ -390,42 +391,42 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/README.md` & `mypy-boto3-cloudcontrol-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudcontrol"></a>
 
 # mypy-boto3-cloudcontrol
 
 [![PyPI - mypy-boto3-cloudcontrol](https://img.shields.io/pypi/v/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudcontrol?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,35 +322,35 @@
 `mypy_boto3_cloudcontrol.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
-    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
 def get_structure() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
@@ -359,42 +359,42 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/__init__.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/__init__.pyi` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/__main__.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudControlApi 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CloudControlApi 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/client.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         Identifier: str,
         PatchDocument: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ClientToken: str = ...
     ) -> UpdateResourceOutputTypeDef:
         """
-        .
+        Updates the specified property values in the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.update_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/client/#update_resource)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/client.pyi` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         Identifier: str,
         PatchDocument: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ClientToken: str = ...
     ) -> UpdateResourceOutputTypeDef:
         """
-        .
+        Updates the specified property values in the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.update_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/client/#update_resource)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_requests"]
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/literals.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,25 @@
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
@@ -97,30 +99,35 @@
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
@@ -146,14 +153,15 @@
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
@@ -198,51 +206,57 @@
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
@@ -255,14 +269,15 @@
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
@@ -274,28 +289,35 @@
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
@@ -304,14 +326,15 @@
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
@@ -322,55 +345,64 @@
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
@@ -397,21 +429,25 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/literals.pyi` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,25 @@
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
@@ -95,30 +97,35 @@
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
@@ -144,14 +151,15 @@
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
@@ -196,51 +204,57 @@
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
@@ -253,14 +267,15 @@
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
@@ -272,28 +287,35 @@
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
@@ -302,14 +324,15 @@
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
@@ -320,55 +343,64 @@
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
@@ -395,21 +427,25 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/paginator.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 
@@ -72,13 +72,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/paginator.pyi` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 class ListResourcesPaginator(Paginator):
@@ -68,13 +68,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/type_defs.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,35 +22,35 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
     "ResourceDescriptionTypeDef",
     "GetResourceRequestStatusInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceRequestStatusFilterTypeDef",
+    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourcesInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateResourceInputRequestTypeDef",
     "CancelResourceRequestOutputTypeDef",
     "CreateResourceOutputTypeDef",
     "DeleteResourceOutputTypeDef",
     "GetResourceRequestStatusOutputTypeDef",
     "ListResourceRequestsOutputTypeDef",
     "UpdateResourceOutputTypeDef",
     "GetResourceOutputTypeDef",
     "ListResourcesOutputTypeDef",
     "GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
-    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     "ListResourceRequestsInputRequestTypeDef",
 )
 
 CancelResourceRequestInputRequestTypeDef = TypedDict(
     "CancelResourceRequestInputRequestTypeDef",
     {
@@ -71,25 +71,14 @@
         "StatusMessage": str,
         "ErrorCode": HandlerErrorCodeType,
         "RetryAfter": datetime,
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
 _RequiredCreateResourceInputRequestTypeDef = TypedDict(
     "_RequiredCreateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "DesiredState": str,
     },
 )
@@ -178,33 +167,48 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ResourceRequestStatusFilterTypeDef = TypedDict(
+    "ResourceRequestStatusFilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Operations": Sequence[OperationType],
+        "OperationStatuses": Sequence[OperationStatusType],
     },
     total=False,
 )
 
-ResourceRequestStatusFilterTypeDef = TypedDict(
-    "ResourceRequestStatusFilterTypeDef",
+_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
     {
-        "Operations": Sequence[OperationType],
-        "OperationStatuses": Sequence[OperationStatusType],
+        "TypeName": str,
+    },
+)
+_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeVersionId": str,
+        "RoleArn": str,
+        "ResourceModel": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListResourcesInputListResourcesPaginateTypeDef(
+    _RequiredListResourcesInputListResourcesPaginateTypeDef,
+    _OptionalListResourcesInputListResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesInputRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalListResourcesInputRequestTypeDef = TypedDict(
@@ -222,14 +226,35 @@
 
 class ListResourcesInputRequestTypeDef(
     _RequiredListResourcesInputRequestTypeDef, _OptionalListResourcesInputRequestTypeDef
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
 _RequiredUpdateResourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "Identifier": str,
         "PatchDocument": str,
     },
@@ -251,75 +276,75 @@
     pass
 
 
 CancelResourceRequestOutputTypeDef = TypedDict(
     "CancelResourceRequestOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateResourceOutputTypeDef = TypedDict(
     "CreateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteResourceOutputTypeDef = TypedDict(
     "DeleteResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceRequestStatusOutputTypeDef = TypedDict(
     "GetResourceRequestStatusOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceRequestsOutputTypeDef = TypedDict(
     "ListResourceRequestsOutputTypeDef",
     {
         "ResourceRequestStatusSummaries": List[ProgressEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceOutputTypeDef = TypedDict(
     "UpdateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceOutputTypeDef = TypedDict(
     "GetResourceOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescription": ResourceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesOutputTypeDef = TypedDict(
     "ListResourcesOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescriptions": List[ResourceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef = TypedDict(
     "_RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
     {
         "RequestToken": str,
@@ -337,44 +362,19 @@
 class GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef(
     _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
     _OptionalGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
 ):
     pass
 
 
-_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeName": str,
-    },
-)
-_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeVersionId": str,
-        "RoleArn": str,
-        "ResourceModel": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResourcesInputListResourcesPaginateTypeDef(
-    _RequiredListResourcesInputListResourcesPaginateTypeDef,
-    _OptionalListResourcesInputListResourcesPaginateTypeDef,
-):
-    pass
-
-
 ListResourceRequestsInputListResourceRequestsPaginateTypeDef = TypedDict(
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     {
         "ResourceRequestStatusFilter": ResourceRequestStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListResourceRequestsInputRequestTypeDef = TypedDict(
     "ListResourceRequestsInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/type_defs.pyi` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,35 +21,35 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
     "ResourceDescriptionTypeDef",
     "GetResourceRequestStatusInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceRequestStatusFilterTypeDef",
+    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourcesInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateResourceInputRequestTypeDef",
     "CancelResourceRequestOutputTypeDef",
     "CreateResourceOutputTypeDef",
     "DeleteResourceOutputTypeDef",
     "GetResourceRequestStatusOutputTypeDef",
     "ListResourceRequestsOutputTypeDef",
     "UpdateResourceOutputTypeDef",
     "GetResourceOutputTypeDef",
     "ListResourcesOutputTypeDef",
     "GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
-    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     "ListResourceRequestsInputRequestTypeDef",
 )
 
 CancelResourceRequestInputRequestTypeDef = TypedDict(
     "CancelResourceRequestInputRequestTypeDef",
     {
@@ -70,25 +70,14 @@
         "StatusMessage": str,
         "ErrorCode": HandlerErrorCodeType,
         "RetryAfter": datetime,
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
 _RequiredCreateResourceInputRequestTypeDef = TypedDict(
     "_RequiredCreateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "DesiredState": str,
     },
 )
@@ -171,33 +160,46 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ResourceRequestStatusFilterTypeDef = TypedDict(
+    "ResourceRequestStatusFilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Operations": Sequence[OperationType],
+        "OperationStatuses": Sequence[OperationStatusType],
     },
     total=False,
 )
 
-ResourceRequestStatusFilterTypeDef = TypedDict(
-    "ResourceRequestStatusFilterTypeDef",
+_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
     {
-        "Operations": Sequence[OperationType],
-        "OperationStatuses": Sequence[OperationStatusType],
+        "TypeName": str,
+    },
+)
+_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeVersionId": str,
+        "RoleArn": str,
+        "ResourceModel": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListResourcesInputListResourcesPaginateTypeDef(
+    _RequiredListResourcesInputListResourcesPaginateTypeDef,
+    _OptionalListResourcesInputListResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesInputRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalListResourcesInputRequestTypeDef = TypedDict(
@@ -213,14 +215,35 @@
 )
 
 class ListResourcesInputRequestTypeDef(
     _RequiredListResourcesInputRequestTypeDef, _OptionalListResourcesInputRequestTypeDef
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
 _RequiredUpdateResourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "Identifier": str,
         "PatchDocument": str,
     },
@@ -240,75 +263,75 @@
 ):
     pass
 
 CancelResourceRequestOutputTypeDef = TypedDict(
     "CancelResourceRequestOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateResourceOutputTypeDef = TypedDict(
     "CreateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteResourceOutputTypeDef = TypedDict(
     "DeleteResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceRequestStatusOutputTypeDef = TypedDict(
     "GetResourceRequestStatusOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceRequestsOutputTypeDef = TypedDict(
     "ListResourceRequestsOutputTypeDef",
     {
         "ResourceRequestStatusSummaries": List[ProgressEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceOutputTypeDef = TypedDict(
     "UpdateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceOutputTypeDef = TypedDict(
     "GetResourceOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescription": ResourceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesOutputTypeDef = TypedDict(
     "ListResourcesOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescriptions": List[ResourceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef = TypedDict(
     "_RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
     {
         "RequestToken": str,
@@ -324,42 +347,19 @@
 
 class GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef(
     _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
     _OptionalGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
 ):
     pass
 
-_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeName": str,
-    },
-)
-_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeVersionId": str,
-        "RoleArn": str,
-        "ResourceModel": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResourcesInputListResourcesPaginateTypeDef(
-    _RequiredListResourcesInputListResourcesPaginateTypeDef,
-    _OptionalListResourcesInputListResourcesPaginateTypeDef,
-):
-    pass
-
 ListResourceRequestsInputListResourceRequestsPaginateTypeDef = TypedDict(
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     {
         "ResourceRequestStatusFilter": ResourceRequestStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListResourceRequestsInputRequestTypeDef = TypedDict(
     "ListResourceRequestsInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/waiter.py` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol/waiter.pyi` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/PKG-INFO` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudcontrol
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CloudControlApi 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudControlApi 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/
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
 
 <a id="mypy-boto3-cloudcontrol"></a>
 
 # mypy-boto3-cloudcontrol
 
 [![PyPI - mypy-boto3-cloudcontrol](https://img.shields.io/pypi/v/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudcontrol?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,35 +354,35 @@
 `mypy_boto3_cloudcontrol.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
-    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
 def get_structure() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
@@ -390,42 +391,42 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt` & `mypy-boto3-cloudcontrol-1.27.0/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.26.0.post1/setup.py` & `mypy-boto3-cloudcontrol-1.27.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cloudcontrol.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudcontrol",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudControlApi 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CloudControlApi 1.27.0 service generated with"
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
     keywords="boto3 cloudcontrol type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cloudcontrol": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cloudcontrol": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/",
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


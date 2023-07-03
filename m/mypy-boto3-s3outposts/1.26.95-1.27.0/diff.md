# Comparing `tmp/mypy-boto3-s3outposts-1.26.95.tar.gz` & `tmp/mypy-boto3-s3outposts-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3outposts-1.26.95.tar", last modified: Mon Mar 20 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-s3outposts-1.27.0.tar", last modified: Mon Jul  3 19:51:23 2023, max compression
```

## Comparing `mypy-boto3-s3outposts-1.26.95.tar` & `mypy-boto3-s3outposts-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.539024 mypy-boto3-s3outposts-1.26.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-03-20 19:32:46.539024 mypy-boto3-s3outposts-1.26.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.539024 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.539024 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-03-20 19:32:46.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-20 19:32:46.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 19:32:46.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-20 19:32:46.000000 mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:32:46.539024 mypy-boto3-s3outposts-1.26.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-20 19:32:31.000000 mypy-boto3-s3outposts-1.26.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:23.227924 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/setup.py
```

### Comparing `mypy-boto3-s3outposts-1.26.95/LICENSE` & `mypy-boto3-s3outposts-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-s3outposts-1.26.95/PKG-INFO` & `mypy-boto3-s3outposts-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3outposts
-Version: 1.26.95
-Summary: Type annotations for boto3.S3Outposts 1.26.95 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.S3Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-s3outposts"></a>
 
 # mypy-boto3-s3outposts
 
 [![PyPI - mypy-boto3-s3outposts](https://img.shields.io/pypi/v/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [mypy-boto3-s3outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3outposts.type_defs import (
     CreateEndpointRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEndpointResultTypeDef,
     DeleteEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     FailedReasonTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
+    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
     ListOutpostsWithS3RequestRequestTypeDef,
     OutpostTypeDef,
+    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListSharedEndpointsRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EndpointTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListOutpostsWithS3ResultTypeDef,
     ListEndpointsResultTypeDef,
     ListSharedEndpointsResultTypeDef,
 )
 
 
 def get_structure() -> CreateEndpointRequestRequestTypeDef:
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

### Comparing `mypy-boto3-s3outposts-1.26.95/README.md` & `mypy-boto3-s3outposts-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-s3outposts"></a>
 
 # mypy-boto3-s3outposts
 
 [![PyPI - mypy-boto3-s3outposts](https://img.shields.io/pypi/v/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [mypy-boto3-s3outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,29 +301,29 @@
 
 `mypy_boto3_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3outposts.type_defs import (
     CreateEndpointRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEndpointResultTypeDef,
     DeleteEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     FailedReasonTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
+    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
     ListOutpostsWithS3RequestRequestTypeDef,
     OutpostTypeDef,
+    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListSharedEndpointsRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EndpointTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListOutpostsWithS3ResultTypeDef,
     ListEndpointsResultTypeDef,
     ListSharedEndpointsResultTypeDef,
 )
 
 
 def get_structure() -> CreateEndpointRequestRequestTypeDef:
@@ -333,42 +333,42 @@
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

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/__init__.py` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/__init__.pyi` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/__main__.py` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Outposts 1.26.95\nVersion:         1.26.95\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.S3Outposts 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.95")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/client.py` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/client.pyi` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/literals.py` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.py`

 * *Files 2% similar despite different names*

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
```

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/literals.pyi` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -95,14 +96,15 @@
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
@@ -200,14 +202,15 @@
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
@@ -243,14 +246,15 @@
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
@@ -269,16 +273,19 @@
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
@@ -362,15 +369,17 @@
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

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/paginator.py` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,61 +32,56 @@
     ListOutpostsWithS3ResultTypeDef,
     ListSharedEndpointsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEndpointsPaginator", "ListOutpostsWithS3Paginator", "ListSharedEndpointsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
         """
 
-
 class ListOutpostsWithS3Paginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOutpostsWithS3ResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
         """
 
-
 class ListSharedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
     """
 
     def paginate(
-        self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, OutpostId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSharedEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
         """
```

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/paginator.pyi` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,56 +32,61 @@
     ListOutpostsWithS3ResultTypeDef,
     ListSharedEndpointsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEndpointsPaginator", "ListOutpostsWithS3Paginator", "ListSharedEndpointsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
         """
 
+
 class ListOutpostsWithS3Paginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOutpostsWithS3ResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
         """
 
+
 class ListSharedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
     """
 
     def paginate(
-        self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, OutpostId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSharedEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
         """
```

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/type_defs.py` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,32 +18,31 @@
 from .literals import EndpointAccessTypeType, EndpointStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateEndpointRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEndpointResultTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FailedReasonTypeDef",
     "NetworkInterfaceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
     "ListOutpostsWithS3RequestRequestTypeDef",
     "OutpostTypeDef",
+    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListSharedEndpointsRequestRequestTypeDef",
-    "CreateEndpointResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "EndpointTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
-    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListOutpostsWithS3ResultTypeDef",
     "ListEndpointsResultTypeDef",
     "ListSharedEndpointsResultTypeDef",
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
@@ -58,40 +57,42 @@
     {
         "AccessType": EndpointAccessTypeType,
         "CustomerOwnedIpv4Pool": str,
     },
     total=False,
 )
 
-
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateEndpointResultTypeDef = TypedDict(
+    "CreateEndpointResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "EndpointArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "EndpointId": str,
         "OutpostId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FailedReasonTypeDef = TypedDict(
     "FailedReasonTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -101,33 +102,39 @@
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOutpostsWithS3RequestRequestTypeDef = TypedDict(
     "ListOutpostsWithS3RequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -140,14 +147,34 @@
         "OutpostId": str,
         "OwnerId": str,
         "CapacityInBytes": int,
     },
     total=False,
 )
 
+_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
+    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+):
+    pass
+
 _RequiredListSharedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListSharedEndpointsRequestRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalListSharedEndpointsRequestRequestTypeDef = TypedDict(
@@ -155,34 +182,38 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSharedEndpointsRequestRequestTypeDef(
     _RequiredListSharedEndpointsRequestRequestTypeDef,
     _OptionalListSharedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
-CreateEndpointResultTypeDef = TypedDict(
-    "CreateEndpointResultTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EndpointArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
@@ -197,71 +228,33 @@
         "AccessType": EndpointAccessTypeType,
         "CustomerOwnedIpv4Pool": str,
         "FailedReason": FailedReasonTypeDef,
     },
     total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "OutpostId": str,
-    },
-)
-_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
-    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-):
-    pass
-
-
 ListOutpostsWithS3ResultTypeDef = TypedDict(
     "ListOutpostsWithS3ResultTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointsResultTypeDef = TypedDict(
     "ListEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSharedEndpointsResultTypeDef = TypedDict(
     "ListSharedEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts/type_defs.pyi` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,32 @@
 from .literals import EndpointAccessTypeType, EndpointStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateEndpointRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEndpointResultTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FailedReasonTypeDef",
     "NetworkInterfaceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
     "ListOutpostsWithS3RequestRequestTypeDef",
     "OutpostTypeDef",
+    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListSharedEndpointsRequestRequestTypeDef",
-    "CreateEndpointResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "EndpointTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
-    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListOutpostsWithS3ResultTypeDef",
     "ListEndpointsResultTypeDef",
     "ListSharedEndpointsResultTypeDef",
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
@@ -57,38 +58,44 @@
     {
         "AccessType": EndpointAccessTypeType,
         "CustomerOwnedIpv4Pool": str,
     },
     total=False,
 )
 
+
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+CreateEndpointResultTypeDef = TypedDict(
+    "CreateEndpointResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "EndpointArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "EndpointId": str,
         "OutpostId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FailedReasonTypeDef = TypedDict(
     "FailedReasonTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -98,33 +105,39 @@
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOutpostsWithS3RequestRequestTypeDef = TypedDict(
     "ListOutpostsWithS3RequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -137,14 +150,36 @@
         "OutpostId": str,
         "OwnerId": str,
         "CapacityInBytes": int,
     },
     total=False,
 )
 
+_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
+    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSharedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListSharedEndpointsRequestRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalListSharedEndpointsRequestRequestTypeDef = TypedDict(
@@ -152,32 +187,40 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSharedEndpointsRequestRequestTypeDef(
     _RequiredListSharedEndpointsRequestRequestTypeDef,
     _OptionalListSharedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-CreateEndpointResultTypeDef = TypedDict(
-    "CreateEndpointResultTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EndpointArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
@@ -192,69 +235,33 @@
         "AccessType": EndpointAccessTypeType,
         "CustomerOwnedIpv4Pool": str,
         "FailedReason": FailedReasonTypeDef,
     },
     total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "OutpostId": str,
-    },
-)
-_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
-    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-):
-    pass
-
 ListOutpostsWithS3ResultTypeDef = TypedDict(
     "ListOutpostsWithS3ResultTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointsResultTypeDef = TypedDict(
     "ListEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSharedEndpointsResultTypeDef = TypedDict(
     "ListSharedEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/PKG-INFO` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3outposts
-Version: 1.26.95
-Summary: Type annotations for boto3.S3Outposts 1.26.95 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.S3Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-s3outposts"></a>
 
 # mypy-boto3-s3outposts
 
 [![PyPI - mypy-boto3-s3outposts](https://img.shields.io/pypi/v/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [mypy-boto3-s3outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3outposts.type_defs import (
     CreateEndpointRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEndpointResultTypeDef,
     DeleteEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     FailedReasonTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
+    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
     ListOutpostsWithS3RequestRequestTypeDef,
     OutpostTypeDef,
+    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListSharedEndpointsRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EndpointTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListOutpostsWithS3ResultTypeDef,
     ListEndpointsResultTypeDef,
     ListSharedEndpointsResultTypeDef,
 )
 
 
 def get_structure() -> CreateEndpointRequestRequestTypeDef:
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

### Comparing `mypy-boto3-s3outposts-1.26.95/mypy_boto3_s3outposts.egg-info/SOURCES.txt` & `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.26.95/setup.py` & `mypy-boto3-s3outposts-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-s3outposts.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3outposts",
-    version="1.26.95",
+    version="1.27.0",
     packages=["mypy_boto3_s3outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Outposts 1.26.95 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.S3Outposts 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/",
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


# Comparing `tmp/mypy-boto3-oam-1.26.17.tar.gz` & `tmp/mypy-boto3-oam-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-oam-1.26.17.tar", last modified: Mon Nov 28 04:09:27 2022, max compression
+gzip compressed data, was "mypy-boto3-oam-1.27.0.tar", last modified: Mon Jul  3 19:51:11 2023, max compression
```

## Comparing `mypy-boto3-oam-1.26.17.tar` & `mypy-boto3-oam-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.604745 mypy-boto3-oam-1.26.17/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14073 2022-11-28 04:09:27.604745 mypy-boto3-oam-1.26.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12619 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.596745 mypy-boto3-oam-1.26.17/mypy_boto3_oam/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      958 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13260 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    13235 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8009 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     8007 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3935 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     9629 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2022-11-28 04:09:03.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.604745 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14073 2022-11-28 04:09:27.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-11-28 04:09:27.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:27.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:27.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-28 04:09:27.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-28 04:09:27.000000 mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:09:27.604745 mypy-boto3-oam-1.26.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2022-11-28 04:09:02.000000 mypy-boto3-oam-1.26.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:11.003732 mypy-boto3-oam-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-07-03 19:51:10.999732 mypy-boto3-oam-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.999732 mypy-boto3-oam-1.27.0/mypy_boto3_oam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-07-03 19:42:54.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.999732 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-07-03 19:51:10.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:10.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:10.000000 mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:11.003732 mypy-boto3-oam-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-03 19:42:53.000000 mypy-boto3-oam-1.27.0/setup.py
```

### Comparing `mypy-boto3-oam-1.26.17/LICENSE` & `mypy-boto3-oam-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-oam-1.26.17/PKG-INFO` & `mypy-boto3-oam-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-oam
-Version: 1.26.17
-Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/
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
 
 <a id="mypy-boto3-oam"></a>
 
 # mypy-boto3-oam
 
 [![PyPI - mypy-boto3-oam](https://img.shields.io/pypi/v/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-oam?color=blue)](https://pypistats.org/packages/mypy-boto3-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchObservabilityAccessManager 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[boto3.CloudWatchObservabilityAccessManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-oam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,44 +331,44 @@
 
 `mypy_boto3_oam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_oam.type_defs import (
     CreateLinkInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLinkOutputTypeDef,
     CreateSinkInputRequestTypeDef,
+    CreateSinkOutputTypeDef,
     DeleteLinkInputRequestTypeDef,
     DeleteSinkInputRequestTypeDef,
     GetLinkInputRequestTypeDef,
+    GetLinkOutputTypeDef,
     GetSinkInputRequestTypeDef,
+    GetSinkOutputTypeDef,
     GetSinkPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetSinkPolicyOutputTypeDef,
+    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
     ListAttachedLinksInputRequestTypeDef,
     ListAttachedLinksItemTypeDef,
+    ListLinksInputListLinksPaginateTypeDef,
     ListLinksInputRequestTypeDef,
     ListLinksItemTypeDef,
+    ListSinksInputListSinksPaginateTypeDef,
     ListSinksInputRequestTypeDef,
     ListSinksItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutSinkPolicyInputRequestTypeDef,
+    PutSinkPolicyOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
-    CreateSinkOutputTypeDef,
-    GetLinkOutputTypeDef,
-    GetSinkOutputTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
 )
 
 
 def get_structure() -> CreateLinkInputRequestTypeDef:
@@ -377,42 +378,42 @@
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

### Comparing `mypy-boto3-oam-1.26.17/README.md` & `mypy-boto3-oam-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-oam"></a>
 
 # mypy-boto3-oam
 
 [![PyPI - mypy-boto3-oam](https://img.shields.io/pypi/v/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-oam?color=blue)](https://pypistats.org/packages/mypy-boto3-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchObservabilityAccessManager 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[boto3.CloudWatchObservabilityAccessManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-oam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,44 +299,44 @@
 
 `mypy_boto3_oam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_oam.type_defs import (
     CreateLinkInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLinkOutputTypeDef,
     CreateSinkInputRequestTypeDef,
+    CreateSinkOutputTypeDef,
     DeleteLinkInputRequestTypeDef,
     DeleteSinkInputRequestTypeDef,
     GetLinkInputRequestTypeDef,
+    GetLinkOutputTypeDef,
     GetSinkInputRequestTypeDef,
+    GetSinkOutputTypeDef,
     GetSinkPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetSinkPolicyOutputTypeDef,
+    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
     ListAttachedLinksInputRequestTypeDef,
     ListAttachedLinksItemTypeDef,
+    ListLinksInputListLinksPaginateTypeDef,
     ListLinksInputRequestTypeDef,
     ListLinksItemTypeDef,
+    ListSinksInputListSinksPaginateTypeDef,
     ListSinksInputRequestTypeDef,
     ListSinksItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutSinkPolicyInputRequestTypeDef,
+    PutSinkPolicyOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
-    CreateSinkOutputTypeDef,
-    GetLinkOutputTypeDef,
-    GetSinkOutputTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
 )
 
 
 def get_structure() -> CreateLinkInputRequestTypeDef:
@@ -346,42 +346,42 @@
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

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/__init__.py` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/__init__.pyi` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/__main__.py` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchObservabilityAccessManager 1.26.17\nVersion:        "
-        " 1.26.17\nBuilder version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.CloudWatchObservabilityAccessManager 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.17")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/client.py` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/client.pyi` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/literals.py` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,23 +48,25 @@
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
@@ -75,30 +77,34 @@
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
@@ -124,14 +130,15 @@
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
@@ -176,14 +183,15 @@
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
@@ -194,34 +202,38 @@
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
@@ -234,14 +246,15 @@
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
@@ -254,28 +267,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -303,30 +322,34 @@
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
@@ -342,18 +365,21 @@
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
@@ -383,14 +409,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/literals.pyi` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -46,23 +46,25 @@
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
@@ -73,30 +75,34 @@
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
@@ -122,14 +128,15 @@
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
@@ -174,14 +181,15 @@
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
@@ -192,34 +200,38 @@
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
@@ -232,14 +244,15 @@
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
@@ -252,28 +265,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -301,30 +320,34 @@
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
@@ -340,18 +363,21 @@
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
@@ -381,14 +407,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/paginator.py` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 class ListAttachedLinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listattachedlinkspaginator)
     """
 
     def paginate(
-        self, *, SinkIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SinkIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttachedLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listattachedlinkspaginator)
         """
 
 
 class ListLinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listlinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listlinkspaginator)
         """
 
 
 class ListSinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listsinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listsinkspaginator)
         """
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/paginator.pyi` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,41 +47,41 @@
 class ListAttachedLinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listattachedlinkspaginator)
     """
 
     def paginate(
-        self, *, SinkIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SinkIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttachedLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listattachedlinkspaginator)
         """
 
 class ListLinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listlinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listlinkspaginator)
         """
 
 class ListSinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listsinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/paginators/#listsinkspaginator)
         """
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/type_defs.py` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,44 +20,44 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateLinkInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateLinkOutputTypeDef",
     "CreateSinkInputRequestTypeDef",
+    "CreateSinkOutputTypeDef",
     "DeleteLinkInputRequestTypeDef",
     "DeleteSinkInputRequestTypeDef",
     "GetLinkInputRequestTypeDef",
+    "GetLinkOutputTypeDef",
     "GetSinkInputRequestTypeDef",
+    "GetSinkOutputTypeDef",
     "GetSinkPolicyInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetSinkPolicyOutputTypeDef",
+    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
     "ListAttachedLinksInputRequestTypeDef",
     "ListAttachedLinksItemTypeDef",
+    "ListLinksInputListLinksPaginateTypeDef",
     "ListLinksInputRequestTypeDef",
     "ListLinksItemTypeDef",
+    "ListSinksInputListSinksPaginateTypeDef",
     "ListSinksInputRequestTypeDef",
     "ListSinksItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutSinkPolicyInputRequestTypeDef",
+    "PutSinkPolicyOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateLinkInputRequestTypeDef",
-    "CreateLinkOutputTypeDef",
-    "CreateSinkOutputTypeDef",
-    "GetLinkOutputTypeDef",
-    "GetSinkOutputTypeDef",
-    "GetSinkPolicyOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PutSinkPolicyOutputTypeDef",
     "UpdateLinkOutputTypeDef",
-    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    "ListLinksInputListLinksPaginateTypeDef",
-    "ListSinksInputListSinksPaginateTypeDef",
     "ListAttachedLinksOutputTypeDef",
     "ListLinksOutputTypeDef",
     "ListSinksOutputTypeDef",
 )
 
 _RequiredCreateLinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateLinkInputRequestTypeDef",
@@ -78,22 +78,25 @@
 
 class CreateLinkInputRequestTypeDef(
     _RequiredCreateLinkInputRequestTypeDef, _OptionalCreateLinkInputRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLinkOutputTypeDef = TypedDict(
+    "CreateLinkOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateSinkInputRequestTypeDef",
     {
         "Name": str,
@@ -110,14 +113,25 @@
 
 class CreateSinkInputRequestTypeDef(
     _RequiredCreateSinkInputRequestTypeDef, _OptionalCreateSinkInputRequestTypeDef
 ):
     pass
 
 
+CreateSinkOutputTypeDef = TypedDict(
+    "CreateSinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLinkInputRequestTypeDef = TypedDict(
     "DeleteLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -131,38 +145,85 @@
 GetLinkInputRequestTypeDef = TypedDict(
     "GetLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+GetLinkOutputTypeDef = TypedDict(
+    "GetLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSinkInputRequestTypeDef = TypedDict(
     "GetSinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+GetSinkOutputTypeDef = TypedDict(
+    "GetSinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSinkPolicyInputRequestTypeDef = TypedDict(
     "GetSinkPolicyInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetSinkPolicyOutputTypeDef = TypedDict(
+    "GetSinkPolicyOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "SinkArn": str,
+        "SinkId": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "SinkIdentifier": str,
+    },
+)
+_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
+    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAttachedLinksInputRequestTypeDef = TypedDict(
     "_RequiredListAttachedLinksInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 _OptionalListAttachedLinksInputRequestTypeDef = TypedDict(
@@ -187,14 +248,22 @@
         "Label": str,
         "LinkArn": str,
         "ResourceTypes": List[str],
     },
     total=False,
 )
 
+ListLinksInputListLinksPaginateTypeDef = TypedDict(
+    "ListLinksInputListLinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLinksInputRequestTypeDef = TypedDict(
     "ListLinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -208,14 +277,22 @@
         "Label": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
     },
     total=False,
 )
 
+ListSinksInputListSinksPaginateTypeDef = TypedDict(
+    "ListSinksInputListSinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSinksInputRequestTypeDef = TypedDict(
     "ListSinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -234,195 +311,118 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PutSinkPolicyInputRequestTypeDef = TypedDict(
-    "PutSinkPolicyInputRequestTypeDef",
-    {
-        "SinkIdentifier": str,
-        "Policy": str,
-    },
-)
-
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
-    },
-)
-
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-UpdateLinkInputRequestTypeDef = TypedDict(
-    "UpdateLinkInputRequestTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
-        "Identifier": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLinkOutputTypeDef = TypedDict(
-    "CreateLinkOutputTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-CreateSinkOutputTypeDef = TypedDict(
-    "CreateSinkOutputTypeDef",
+PutSinkPolicyInputRequestTypeDef = TypedDict(
+    "PutSinkPolicyInputRequestTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SinkIdentifier": str,
+        "Policy": str,
     },
 )
 
-GetLinkOutputTypeDef = TypedDict(
-    "GetLinkOutputTypeDef",
+PutSinkPolicyOutputTypeDef = TypedDict(
+    "PutSinkPolicyOutputTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
         "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SinkId": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSinkOutputTypeDef = TypedDict(
-    "GetSinkOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-GetSinkPolicyOutputTypeDef = TypedDict(
-    "GetSinkPolicyOutputTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-PutSinkPolicyOutputTypeDef = TypedDict(
-    "PutSinkPolicyOutputTypeDef",
+UpdateLinkInputRequestTypeDef = TypedDict(
+    "UpdateLinkInputRequestTypeDef",
     {
-        "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Identifier": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
     },
 )
 
 UpdateLinkOutputTypeDef = TypedDict(
     "UpdateLinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Label": str,
         "LabelTemplate": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    {
-        "SinkIdentifier": str,
-    },
-)
-_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
-    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-):
-    pass
-
-
-ListLinksInputListLinksPaginateTypeDef = TypedDict(
-    "ListLinksInputListLinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListSinksInputListSinksPaginateTypeDef = TypedDict(
-    "ListSinksInputListSinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListAttachedLinksOutputTypeDef = TypedDict(
     "ListAttachedLinksOutputTypeDef",
     {
         "Items": List[ListAttachedLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLinksOutputTypeDef = TypedDict(
     "ListLinksOutputTypeDef",
     {
         "Items": List[ListLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSinksOutputTypeDef = TypedDict(
     "ListSinksOutputTypeDef",
     {
         "Items": List[ListSinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam/type_defs.pyi` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -19,44 +19,44 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateLinkInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateLinkOutputTypeDef",
     "CreateSinkInputRequestTypeDef",
+    "CreateSinkOutputTypeDef",
     "DeleteLinkInputRequestTypeDef",
     "DeleteSinkInputRequestTypeDef",
     "GetLinkInputRequestTypeDef",
+    "GetLinkOutputTypeDef",
     "GetSinkInputRequestTypeDef",
+    "GetSinkOutputTypeDef",
     "GetSinkPolicyInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetSinkPolicyOutputTypeDef",
+    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
     "ListAttachedLinksInputRequestTypeDef",
     "ListAttachedLinksItemTypeDef",
+    "ListLinksInputListLinksPaginateTypeDef",
     "ListLinksInputRequestTypeDef",
     "ListLinksItemTypeDef",
+    "ListSinksInputListSinksPaginateTypeDef",
     "ListSinksInputRequestTypeDef",
     "ListSinksItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutSinkPolicyInputRequestTypeDef",
+    "PutSinkPolicyOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateLinkInputRequestTypeDef",
-    "CreateLinkOutputTypeDef",
-    "CreateSinkOutputTypeDef",
-    "GetLinkOutputTypeDef",
-    "GetSinkOutputTypeDef",
-    "GetSinkPolicyOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PutSinkPolicyOutputTypeDef",
     "UpdateLinkOutputTypeDef",
-    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    "ListLinksInputListLinksPaginateTypeDef",
-    "ListSinksInputListSinksPaginateTypeDef",
     "ListAttachedLinksOutputTypeDef",
     "ListLinksOutputTypeDef",
     "ListSinksOutputTypeDef",
 )
 
 _RequiredCreateLinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateLinkInputRequestTypeDef",
@@ -75,22 +75,25 @@
 )
 
 class CreateLinkInputRequestTypeDef(
     _RequiredCreateLinkInputRequestTypeDef, _OptionalCreateLinkInputRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLinkOutputTypeDef = TypedDict(
+    "CreateLinkOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateSinkInputRequestTypeDef",
     {
         "Name": str,
@@ -105,14 +108,25 @@
 )
 
 class CreateSinkInputRequestTypeDef(
     _RequiredCreateSinkInputRequestTypeDef, _OptionalCreateSinkInputRequestTypeDef
 ):
     pass
 
+CreateSinkOutputTypeDef = TypedDict(
+    "CreateSinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLinkInputRequestTypeDef = TypedDict(
     "DeleteLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -126,38 +140,83 @@
 GetLinkInputRequestTypeDef = TypedDict(
     "GetLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+GetLinkOutputTypeDef = TypedDict(
+    "GetLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSinkInputRequestTypeDef = TypedDict(
     "GetSinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+GetSinkOutputTypeDef = TypedDict(
+    "GetSinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSinkPolicyInputRequestTypeDef = TypedDict(
     "GetSinkPolicyInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetSinkPolicyOutputTypeDef = TypedDict(
+    "GetSinkPolicyOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "SinkArn": str,
+        "SinkId": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "SinkIdentifier": str,
+    },
+)
+_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
+    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+):
+    pass
+
 _RequiredListAttachedLinksInputRequestTypeDef = TypedDict(
     "_RequiredListAttachedLinksInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 _OptionalListAttachedLinksInputRequestTypeDef = TypedDict(
@@ -180,14 +239,22 @@
         "Label": str,
         "LinkArn": str,
         "ResourceTypes": List[str],
     },
     total=False,
 )
 
+ListLinksInputListLinksPaginateTypeDef = TypedDict(
+    "ListLinksInputListLinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLinksInputRequestTypeDef = TypedDict(
     "ListLinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -201,14 +268,22 @@
         "Label": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
     },
     total=False,
 )
 
+ListSinksInputListSinksPaginateTypeDef = TypedDict(
+    "ListSinksInputListSinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSinksInputRequestTypeDef = TypedDict(
     "ListSinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -227,193 +302,118 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PutSinkPolicyInputRequestTypeDef = TypedDict(
-    "PutSinkPolicyInputRequestTypeDef",
-    {
-        "SinkIdentifier": str,
-        "Policy": str,
-    },
-)
-
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
-    },
-)
-
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-UpdateLinkInputRequestTypeDef = TypedDict(
-    "UpdateLinkInputRequestTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
-        "Identifier": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLinkOutputTypeDef = TypedDict(
-    "CreateLinkOutputTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-CreateSinkOutputTypeDef = TypedDict(
-    "CreateSinkOutputTypeDef",
+PutSinkPolicyInputRequestTypeDef = TypedDict(
+    "PutSinkPolicyInputRequestTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SinkIdentifier": str,
+        "Policy": str,
     },
 )
 
-GetLinkOutputTypeDef = TypedDict(
-    "GetLinkOutputTypeDef",
+PutSinkPolicyOutputTypeDef = TypedDict(
+    "PutSinkPolicyOutputTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
         "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SinkId": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSinkOutputTypeDef = TypedDict(
-    "GetSinkOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-GetSinkPolicyOutputTypeDef = TypedDict(
-    "GetSinkPolicyOutputTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-PutSinkPolicyOutputTypeDef = TypedDict(
-    "PutSinkPolicyOutputTypeDef",
+UpdateLinkInputRequestTypeDef = TypedDict(
+    "UpdateLinkInputRequestTypeDef",
     {
-        "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Identifier": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
     },
 )
 
 UpdateLinkOutputTypeDef = TypedDict(
     "UpdateLinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Label": str,
         "LabelTemplate": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    {
-        "SinkIdentifier": str,
-    },
-)
-_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
-    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-):
-    pass
-
-ListLinksInputListLinksPaginateTypeDef = TypedDict(
-    "ListLinksInputListLinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSinksInputListSinksPaginateTypeDef = TypedDict(
-    "ListSinksInputListSinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListAttachedLinksOutputTypeDef = TypedDict(
     "ListAttachedLinksOutputTypeDef",
     {
         "Items": List[ListAttachedLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLinksOutputTypeDef = TypedDict(
     "ListLinksOutputTypeDef",
     {
         "Items": List[ListLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSinksOutputTypeDef = TypedDict(
     "ListSinksOutputTypeDef",
     {
         "Items": List[ListSinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/PKG-INFO` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-oam
-Version: 1.26.17
-Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/
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
 
 <a id="mypy-boto3-oam"></a>
 
 # mypy-boto3-oam
 
 [![PyPI - mypy-boto3-oam](https://img.shields.io/pypi/v/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-oam?color=blue)](https://pypistats.org/packages/mypy-boto3-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchObservabilityAccessManager 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[boto3.CloudWatchObservabilityAccessManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-oam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,44 +331,44 @@
 
 `mypy_boto3_oam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_oam.type_defs import (
     CreateLinkInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLinkOutputTypeDef,
     CreateSinkInputRequestTypeDef,
+    CreateSinkOutputTypeDef,
     DeleteLinkInputRequestTypeDef,
     DeleteSinkInputRequestTypeDef,
     GetLinkInputRequestTypeDef,
+    GetLinkOutputTypeDef,
     GetSinkInputRequestTypeDef,
+    GetSinkOutputTypeDef,
     GetSinkPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetSinkPolicyOutputTypeDef,
+    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
     ListAttachedLinksInputRequestTypeDef,
     ListAttachedLinksItemTypeDef,
+    ListLinksInputListLinksPaginateTypeDef,
     ListLinksInputRequestTypeDef,
     ListLinksItemTypeDef,
+    ListSinksInputListSinksPaginateTypeDef,
     ListSinksInputRequestTypeDef,
     ListSinksItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutSinkPolicyInputRequestTypeDef,
+    PutSinkPolicyOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
-    CreateSinkOutputTypeDef,
-    GetLinkOutputTypeDef,
-    GetSinkOutputTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
 )
 
 
 def get_structure() -> CreateLinkInputRequestTypeDef:
@@ -377,42 +378,42 @@
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

### Comparing `mypy-boto3-oam-1.26.17/mypy_boto3_oam.egg-info/SOURCES.txt` & `mypy-boto3-oam-1.27.0/mypy_boto3_oam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.26.17/setup.py` & `mypy-boto3-oam-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-oam.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-oam",
-    version="1.26.17",
+    version="1.27.0",
     packages=["mypy_boto3_oam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchObservabilityAccessManager 1.26.17 service generated"
-        " with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.CloudWatchObservabilityAccessManager 1.27.0 service generated"
+        " with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 oam type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_oam": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_oam": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/",
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


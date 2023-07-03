# Comparing `tmp/mypy-boto3-macie-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-macie-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:42 2022, max compression
+gzip compressed data, was "mypy-boto3-macie-1.27.0.tar", last modified: Mon Jul  3 19:51:04 2023, max compression
```

## Comparing `mypy-boto3-macie-1.26.0.post1.tar` & `mypy-boto3-macie-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:42.224834 mypy-boto3-macie-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13578 2022-11-01 21:43:42.220834 mypy-boto3-macie-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12145 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:42.220834 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8456 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7385 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7383 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8347 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8334 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:42.220834 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13578 2022-11-01 21:43:42.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-01 21:43:42.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:42.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:42.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:42.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-01 21:43:42.000000 mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:42.224834 mypy-boto3-macie-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-11-01 21:37:37.000000 mypy-boto3-macie-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:04.175606 mypy-boto3-macie-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-03 19:51:04.175606 mypy-boto3-macie-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:04.167606 mypy-boto3-macie-1.27.0/mypy_boto3_macie/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:04.175606 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-03 19:51:04.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:51:04.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:04.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:04.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:04.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:04.000000 mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:04.175606 mypy-boto3-macie-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:41:29.000000 mypy-boto3-macie-1.27.0/setup.py
```

### Comparing `mypy-boto3-macie-1.26.0.post1/LICENSE` & `mypy-boto3-macie-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-macie-1.26.0.post1/PKG-INFO` & `mypy-boto3-macie-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Macie 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Macie 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/
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
 
 <a id="mypy-boto3-macie"></a>
 
 # mypy-boto3-macie
 
 [![PyPI - mypy-boto3-macie](https://img.shields.io/pypi/v/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie?color=blue)](https://pypistats.org/packages/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,30 +325,30 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    PaginatorConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
@@ -361,42 +362,42 @@
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

### Comparing `mypy-boto3-macie-1.26.0.post1/README.md` & `mypy-boto3-macie-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-macie"></a>
 
 # mypy-boto3-macie
 
 [![PyPI - mypy-boto3-macie](https://img.shields.io/pypi/v/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie?color=blue)](https://pypistats.org/packages/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,30 +293,30 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    PaginatorConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
@@ -330,42 +330,42 @@
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

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/__init__.py` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/__init__.pyi` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/__main__.py` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Macie 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie\nOther"
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

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/client.py` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/client.pyi` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/literals.py` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/literals.py`

 * *Files 11% similar despite different names*

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
@@ -74,30 +76,35 @@
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
@@ -123,14 +130,15 @@
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
@@ -175,51 +183,57 @@
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
@@ -232,14 +246,15 @@
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
@@ -251,28 +266,35 @@
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
@@ -281,14 +303,15 @@
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
@@ -299,55 +322,64 @@
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

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/literals.pyi` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/literals.pyi`

 * *Files 11% similar despite different names*

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
@@ -72,30 +74,35 @@
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
@@ -121,14 +128,15 @@
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
@@ -173,51 +181,57 @@
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
@@ -230,14 +244,15 @@
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
@@ -249,28 +264,35 @@
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
@@ -279,14 +301,15 @@
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
@@ -297,55 +320,64 @@
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

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/paginator.py` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMemberAccountsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
         """
 
 
 class ListS3ResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
     """
 
     def paginate(
-        self, *, memberAccountId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, memberAccountId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListS3ResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
         """
```

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/paginator.pyi` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMemberAccountsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
         """
 
 class ListS3ResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
     """
 
     def paginate(
-        self, *, memberAccountId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, memberAccountId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListS3ResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
         """
```

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/type_defs.py` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListMemberAccountsResultTypeDef",
     "AssociateS3ResourcesRequestRequestTypeDef",
     "ListS3ResourcesResultTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
@@ -56,25 +56,14 @@
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
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
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
         "continuous": Literal["FULL"],
     },
 )
@@ -110,20 +99,25 @@
 )
 
 
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
@@ -137,28 +131,51 @@
     "MemberAccountTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
+    {
+        "memberAccountId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListS3ResourcesRequestRequestTypeDef = TypedDict(
     "ListS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
 
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
@@ -230,37 +247,20 @@
         "failedItem": S3ResourceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
-    {
-        "memberAccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMemberAccountsResultTypeDef = TypedDict(
     "ListMemberAccountsResultTypeDef",
     {
         "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
@@ -283,15 +283,15 @@
 
 
 ListS3ResourcesResultTypeDef = TypedDict(
     "ListS3ResourcesResultTypeDef",
     {
         "s3Resources": List[S3ResourceClassificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
@@ -312,26 +312,26 @@
     pass
 
 
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateS3ResourcesResultTypeDef = TypedDict(
     "DisassociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateS3ResourcesResultTypeDef = TypedDict(
     "UpdateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie/type_defs.pyi` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -23,30 +23,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListMemberAccountsResultTypeDef",
     "AssociateS3ResourcesRequestRequestTypeDef",
     "ListS3ResourcesResultTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
@@ -55,25 +55,14 @@
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
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
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
         "continuous": Literal["FULL"],
     },
 )
@@ -107,20 +96,25 @@
     },
     total=False,
 )
 
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
@@ -134,28 +128,51 @@
     "MemberAccountTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
+    {
+        "memberAccountId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListS3ResourcesRequestRequestTypeDef = TypedDict(
     "ListS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
 
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
@@ -221,37 +238,20 @@
         "failedItem": S3ResourceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
-    {
-        "memberAccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMemberAccountsResultTypeDef = TypedDict(
     "ListMemberAccountsResultTypeDef",
     {
         "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
@@ -272,15 +272,15 @@
     pass
 
 ListS3ResourcesResultTypeDef = TypedDict(
     "ListS3ResourcesResultTypeDef",
     {
         "s3Resources": List[S3ResourceClassificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
@@ -299,26 +299,26 @@
 ):
     pass
 
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateS3ResourcesResultTypeDef = TypedDict(
     "DisassociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateS3ResourcesResultTypeDef = TypedDict(
     "UpdateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/PKG-INFO` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Macie 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Macie 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/
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
 
 <a id="mypy-boto3-macie"></a>
 
 # mypy-boto3-macie
 
 [![PyPI - mypy-boto3-macie](https://img.shields.io/pypi/v/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie?color=blue)](https://pypistats.org/packages/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,30 +325,30 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    PaginatorConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
@@ -361,42 +362,42 @@
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

### Comparing `mypy-boto3-macie-1.26.0.post1/mypy_boto3_macie.egg-info/SOURCES.txt` & `mypy-boto3-macie-1.27.0/mypy_boto3_macie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.26.0.post1/setup.py` & `mypy-boto3-macie-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-macie.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-macie",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_macie"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Macie 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 macie type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_macie": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_macie": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/",
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


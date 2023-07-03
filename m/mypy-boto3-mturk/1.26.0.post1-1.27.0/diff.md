# Comparing `tmp/mypy-boto3-mturk-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-mturk-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mturk-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:46 2022, max compression
+gzip compressed data, was "mypy-boto3-mturk-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
```

## Comparing `mypy-boto3-mturk-1.26.0.post1.tar` & `mypy-boto3-mturk-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:46.916838 mypy-boto3-mturk-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18181 2022-11-01 21:43:46.916838 mypy-boto3-mturk-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16748 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:46.908837 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    33241 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9885 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9883 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11217 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11206 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    37514 2022-11-01 21:38:29.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    37459 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:28.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:46.916838 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18181 2022-11-01 21:43:46.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-01 21:43:46.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:46.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:46.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:46.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-01 21:43:46.000000 mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:46.916838 mypy-boto3-mturk-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-11-01 21:38:27.000000 mypy-boto3-mturk-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.459722 mypy-boto3-mturk-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-03 19:51:10.455722 mypy-boto3-mturk-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.455722 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-03 19:42:33.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-03 19:42:33.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-03 19:42:33.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-03 19:42:33.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-07-03 19:42:35.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37521 2023-07-03 19:42:33.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.455722 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-03 19:51:10.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:51:10.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:10.000000 mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.459722 mypy-boto3-mturk-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:42:32.000000 mypy-boto3-mturk-1.27.0/setup.py
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/LICENSE` & `mypy-boto3-mturk-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mturk-1.26.0.post1/PKG-INFO` & `mypy-boto3-mturk-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MTurk 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MTurk 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
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
 
 <a id="mypy-boto3-mturk"></a>
 
 # mypy-boto3-mturk
 
 [![PyPI - mypy-boto3-mturk](https://img.shields.io/pypi/v/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mturk?color=blue)](https://pypistats.org/packages/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,72 +378,72 @@
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    ResponseMetadataTypeDef,
+    CreateHITTypeResponseTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
+    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
+    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
     UpdateExpirationForHITRequestRequestTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
-    CreateHITTypeResponseTypeDef,
-    GetAccountBalanceResponseTypeDef,
-    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     QualificationRequirementTypeDef,
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
@@ -473,42 +474,42 @@
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

### Comparing `mypy-boto3-mturk-1.26.0.post1/README.md` & `mypy-boto3-mturk-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mturk"></a>
 
 # mypy-boto3-mturk
 
 [![PyPI - mypy-boto3-mturk](https://img.shields.io/pypi/v/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mturk?color=blue)](https://pypistats.org/packages/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,72 +346,72 @@
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    ResponseMetadataTypeDef,
+    CreateHITTypeResponseTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
+    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
+    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
     UpdateExpirationForHITRequestRequestTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
-    CreateHITTypeResponseTypeDef,
-    GetAccountBalanceResponseTypeDef,
-    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     QualificationRequirementTypeDef,
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
@@ -442,42 +442,42 @@
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

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/__init__.py` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/__init__.pyi` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/__main__.py` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MTurk 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.MTurk 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/client.py` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#get_qualification_score)
         """
 
     def get_qualification_type(
         self, *, QualificationTypeId: str
     ) -> GetQualificationTypeResponseTypeDef:
         """
-        The `GetQualificationType` operation retrieves information about a Qualification
+        The `GetQualificationType`operation retrieves information about a Qualification
         type using its ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.get_qualification_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#get_qualification_type)
         """
 
     def list_assignments_for_hit(
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/client.pyi` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.get_qualification_score)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#get_qualification_score)
         """
     def get_qualification_type(
         self, *, QualificationTypeId: str
     ) -> GetQualificationTypeResponseTypeDef:
         """
-        The `GetQualificationType` operation retrieves information about a Qualification
+        The `GetQualificationType`operation retrieves information about a Qualification
         type using its ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.get_qualification_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#get_qualification_type)
         """
     def list_assignments_for_hit(
         self,
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/literals.py` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,23 +110,25 @@
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
@@ -136,30 +138,35 @@
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
@@ -185,14 +192,15 @@
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
@@ -237,51 +245,57 @@
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
@@ -294,14 +308,15 @@
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
@@ -313,28 +328,35 @@
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
@@ -343,14 +365,15 @@
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
@@ -361,55 +384,64 @@
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

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/literals.pyi` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -108,23 +108,25 @@
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
@@ -134,30 +136,35 @@
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
@@ -183,14 +190,15 @@
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
@@ -235,51 +243,57 @@
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
@@ -292,14 +306,15 @@
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
@@ -311,28 +326,35 @@
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
@@ -341,14 +363,15 @@
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
@@ -359,55 +382,64 @@
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

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/paginator.py` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -61,172 +61,161 @@
     "ListQualificationRequestsPaginator",
     "ListQualificationTypesPaginator",
     "ListReviewableHITsPaginator",
     "ListWorkerBlocksPaginator",
     "ListWorkersWithQualificationTypePaginator",
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
 class ListAssignmentsForHITPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
-
 class ListBonusPaymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
         """
 
-
 class ListHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
         """
 
-
 class ListHITsForQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QualificationTypeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHITsForQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
         """
 
-
 class ListQualificationRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QualificationTypeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQualificationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
         """
 
-
 class ListQualificationTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
     """
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
         """
 
-
 class ListReviewableHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReviewableHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
         """
 
-
 class ListWorkerBlocksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkerBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
         """
 
-
 class ListWorkersWithQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/paginator.pyi` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/paginator.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,161 +61,172 @@
     "ListQualificationRequestsPaginator",
     "ListQualificationTypesPaginator",
     "ListReviewableHITsPaginator",
     "ListWorkerBlocksPaginator",
     "ListWorkersWithQualificationTypePaginator",
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
 class ListAssignmentsForHITPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
+
 class ListBonusPaymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
         """
 
+
 class ListHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
         """
 
+
 class ListHITsForQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QualificationTypeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHITsForQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
         """
 
+
 class ListQualificationRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QualificationTypeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQualificationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
         """
 
+
 class ListQualificationTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
     """
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
         """
 
+
 class ListReviewableHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReviewableHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
         """
 
+
 class ListWorkerBlocksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkerBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
         """
 
+
 class ListWorkersWithQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/type_defs.py` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,72 +41,72 @@
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
     "HITLayoutParameterTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateHITTypeResponseTypeDef",
     "CreateQualificationTypeRequestRequestTypeDef",
     "QualificationTypeTypeDef",
     "CreateWorkerBlockRequestRequestTypeDef",
     "DeleteHITRequestRequestTypeDef",
     "DeleteQualificationTypeRequestRequestTypeDef",
     "DeleteWorkerBlockRequestRequestTypeDef",
     "DisassociateQualificationFromWorkerRequestRequestTypeDef",
+    "GetAccountBalanceResponseTypeDef",
     "GetAssignmentRequestRequestTypeDef",
     "GetFileUploadURLRequestRequestTypeDef",
+    "GetFileUploadURLResponseTypeDef",
     "GetHITRequestRequestTypeDef",
     "GetQualificationScoreRequestRequestTypeDef",
     "GetQualificationTypeRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
     "ListAssignmentsForHITRequestRequestTypeDef",
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
     "ListBonusPaymentsRequestRequestTypeDef",
+    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
     "ListHITsForQualificationTypeRequestRequestTypeDef",
+    "ListHITsRequestListHITsPaginateTypeDef",
     "ListHITsRequestRequestTypeDef",
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationRequestsRequestRequestTypeDef",
     "QualificationRequestTypeDef",
+    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListQualificationTypesRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITRequestRequestTypeDef",
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
+    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
     "UpdateExpirationForHITRequestRequestTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
-    "CreateHITTypeResponseTypeDef",
-    "GetAccountBalanceResponseTypeDef",
-    "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
-    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    "ListHITsRequestListHITsPaginateTypeDef",
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
     "QualificationRequirementTypeDef",
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
@@ -255,22 +255,19 @@
     "HITLayoutParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateHITTypeResponseTypeDef = TypedDict(
+    "CreateHITTypeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "HITTypeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQualificationTypeRequestRequestTypeDef",
     {
         "Name": str,
@@ -382,14 +379,23 @@
 class DisassociateQualificationFromWorkerRequestRequestTypeDef(
     _RequiredDisassociateQualificationFromWorkerRequestRequestTypeDef,
     _OptionalDisassociateQualificationFromWorkerRequestRequestTypeDef,
 ):
     pass
 
 
+GetAccountBalanceResponseTypeDef = TypedDict(
+    "GetAccountBalanceResponseTypeDef",
+    {
+        "AvailableBalance": str,
+        "OnHoldBalance": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAssignmentRequestRequestTypeDef = TypedDict(
     "GetAssignmentRequestRequestTypeDef",
     {
         "AssignmentId": str,
     },
 )
 
@@ -397,14 +403,22 @@
     "GetFileUploadURLRequestRequestTypeDef",
     {
         "AssignmentId": str,
         "QuestionIdentifier": str,
     },
 )
 
+GetFileUploadURLResponseTypeDef = TypedDict(
+    "GetFileUploadURLResponseTypeDef",
+    {
+        "FileUploadURL": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHITRequestRequestTypeDef = TypedDict(
     "GetHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 
@@ -419,24 +433,37 @@
 GetQualificationTypeRequestRequestTypeDef = TypedDict(
     "GetQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HITId": str,
+    },
+)
+_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "AssignmentStatuses": Sequence[AssignmentStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
+    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssignmentsForHITRequestRequestTypeDef = TypedDict(
     "_RequiredListAssignmentsForHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalListAssignmentsForHITRequestRequestTypeDef = TypedDict(
@@ -453,25 +480,57 @@
 class ListAssignmentsForHITRequestRequestTypeDef(
     _RequiredListAssignmentsForHITRequestRequestTypeDef,
     _OptionalListAssignmentsForHITRequestRequestTypeDef,
 ):
     pass
 
 
+ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    {
+        "HITId": str,
+        "AssignmentId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBonusPaymentsRequestRequestTypeDef = TypedDict(
     "ListBonusPaymentsRequestRequestTypeDef",
     {
         "HITId": str,
         "AssignmentId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
+    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListHITsForQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -487,23 +546,40 @@
 class ListHITsForQualificationTypeRequestRequestTypeDef(
     _RequiredListHITsForQualificationTypeRequestRequestTypeDef,
     _OptionalListHITsForQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
+ListHITsRequestListHITsPaginateTypeDef = TypedDict(
+    "ListHITsRequestListHITsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHITsRequestRequestTypeDef = TypedDict(
     "ListHITsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQualificationRequestsRequestRequestTypeDef = TypedDict(
     "ListQualificationRequestsRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -519,14 +595,38 @@
         "Test": str,
         "Answer": str,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
+_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "MustBeRequestable": bool,
+    },
+)
+_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "Query": str,
+        "MustBeOwnedByCaller": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
+    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListQualificationTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListQualificationTypesRequestRequestTypeDef",
     {
         "MustBeRequestable": bool,
     },
 )
 _OptionalListQualificationTypesRequestRequestTypeDef = TypedDict(
@@ -570,25 +670,43 @@
 class ListReviewPolicyResultsForHITRequestRequestTypeDef(
     _RequiredListReviewPolicyResultsForHITRequestRequestTypeDef,
     _OptionalListReviewPolicyResultsForHITRequestRequestTypeDef,
 ):
     pass
 
 
+ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    {
+        "HITTypeId": str,
+        "Status": ReviewableHITStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReviewableHITsRequestRequestTypeDef = TypedDict(
     "ListReviewableHITsRequestRequestTypeDef",
     {
         "HITTypeId": str,
         "Status": ReviewableHITStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorkerBlocksRequestRequestTypeDef = TypedDict(
     "ListWorkerBlocksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -599,14 +717,37 @@
     {
         "WorkerId": str,
         "Reason": str,
     },
     total=False,
 )
 
+_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "Status": QualificationStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
+    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersWithQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -671,14 +812,24 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
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
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -710,14 +861,25 @@
 class RejectQualificationRequestRequestRequestTypeDef(
     _RequiredRejectQualificationRequestRequestRequestTypeDef,
     _OptionalRejectQualificationRequestRequestRequestTypeDef,
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
 ReviewActionDetailTypeDef = TypedDict(
     "ReviewActionDetailTypeDef",
     {
         "ActionId": str,
         "ActionName": str,
         "TargetId": str,
         "TargetType": str,
@@ -829,247 +991,85 @@
 class UpdateQualificationTypeRequestRequestTypeDef(
     _RequiredUpdateQualificationTypeRequestRequestTypeDef,
     _OptionalUpdateQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
-CreateHITTypeResponseTypeDef = TypedDict(
-    "CreateHITTypeResponseTypeDef",
-    {
-        "HITTypeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountBalanceResponseTypeDef = TypedDict(
-    "GetAccountBalanceResponseTypeDef",
-    {
-        "AvailableBalance": str,
-        "OnHoldBalance": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFileUploadURLResponseTypeDef = TypedDict(
-    "GetFileUploadURLResponseTypeDef",
-    {
-        "FileUploadURL": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAssignmentsForHITResponseTypeDef = TypedDict(
     "ListAssignmentsForHITResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Assignments": List[AssignmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBonusPaymentsResponseTypeDef = TypedDict(
     "ListBonusPaymentsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "BonusPayments": List[BonusPaymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateQualificationTypeResponseTypeDef = TypedDict(
     "CreateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQualificationTypeResponseTypeDef = TypedDict(
     "GetQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQualificationTypesResponseTypeDef = TypedDict(
     "ListQualificationTypesResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationTypes": List[QualificationTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateQualificationTypeResponseTypeDef = TypedDict(
     "UpdateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "HITId": str,
-    },
-)
-_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "AssignmentStatuses": Sequence[AssignmentStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
-    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-):
-    pass
-
-
-ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    {
-        "HITId": str,
-        "AssignmentId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
-    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-):
-    pass
-
-
-ListHITsRequestListHITsPaginateTypeDef = TypedDict(
-    "ListHITsRequestListHITsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "MustBeRequestable": bool,
-    },
-)
-_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "Query": str,
-        "MustBeOwnedByCaller": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
-    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-):
-    pass
-
-
-ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    {
-        "HITTypeId": str,
-        "Status": ReviewableHITStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "Status": QualificationStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
-    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-):
-    pass
-
-
 ListQualificationRequestsResponseTypeDef = TypedDict(
     "ListQualificationRequestsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationRequests": List[QualificationRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkerBlocksResponseTypeDef = TypedDict(
     "ListWorkerBlocksResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
@@ -1138,15 +1138,15 @@
     pass
 
 
 NotifyWorkersResponseTypeDef = TypedDict(
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
@@ -1219,25 +1219,25 @@
     total=False,
 )
 
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
     "ListWorkersWithQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
@@ -1256,70 +1256,70 @@
     pass
 
 
 CreateHITResponseTypeDef = TypedDict(
     "CreateHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHITWithHITTypeResponseTypeDef = TypedDict(
     "CreateHITWithHITTypeResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssignmentResponseTypeDef = TypedDict(
     "GetAssignmentResponseTypeDef",
     {
         "Assignment": AssignmentTypeDef,
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHITResponseTypeDef = TypedDict(
     "GetHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHITsForQualificationTypeResponseTypeDef = TypedDict(
     "ListHITsForQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHITsResponseTypeDef = TypedDict(
     "ListHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReviewableHITsResponseTypeDef = TypedDict(
     "ListReviewableHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
@@ -1389,10 +1389,10 @@
     {
         "HITId": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "AssignmentReviewReport": ReviewReportTypeDef,
         "HITReviewReport": ReviewReportTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk/type_defs.pyi` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -40,72 +40,72 @@
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
     "HITLayoutParameterTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateHITTypeResponseTypeDef",
     "CreateQualificationTypeRequestRequestTypeDef",
     "QualificationTypeTypeDef",
     "CreateWorkerBlockRequestRequestTypeDef",
     "DeleteHITRequestRequestTypeDef",
     "DeleteQualificationTypeRequestRequestTypeDef",
     "DeleteWorkerBlockRequestRequestTypeDef",
     "DisassociateQualificationFromWorkerRequestRequestTypeDef",
+    "GetAccountBalanceResponseTypeDef",
     "GetAssignmentRequestRequestTypeDef",
     "GetFileUploadURLRequestRequestTypeDef",
+    "GetFileUploadURLResponseTypeDef",
     "GetHITRequestRequestTypeDef",
     "GetQualificationScoreRequestRequestTypeDef",
     "GetQualificationTypeRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
     "ListAssignmentsForHITRequestRequestTypeDef",
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
     "ListBonusPaymentsRequestRequestTypeDef",
+    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
     "ListHITsForQualificationTypeRequestRequestTypeDef",
+    "ListHITsRequestListHITsPaginateTypeDef",
     "ListHITsRequestRequestTypeDef",
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationRequestsRequestRequestTypeDef",
     "QualificationRequestTypeDef",
+    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListQualificationTypesRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITRequestRequestTypeDef",
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
+    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
     "UpdateExpirationForHITRequestRequestTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
-    "CreateHITTypeResponseTypeDef",
-    "GetAccountBalanceResponseTypeDef",
-    "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
-    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    "ListHITsRequestListHITsPaginateTypeDef",
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
     "QualificationRequirementTypeDef",
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
@@ -246,22 +246,19 @@
     "HITLayoutParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateHITTypeResponseTypeDef = TypedDict(
+    "CreateHITTypeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "HITTypeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQualificationTypeRequestRequestTypeDef",
     {
         "Name": str,
@@ -367,14 +364,23 @@
 
 class DisassociateQualificationFromWorkerRequestRequestTypeDef(
     _RequiredDisassociateQualificationFromWorkerRequestRequestTypeDef,
     _OptionalDisassociateQualificationFromWorkerRequestRequestTypeDef,
 ):
     pass
 
+GetAccountBalanceResponseTypeDef = TypedDict(
+    "GetAccountBalanceResponseTypeDef",
+    {
+        "AvailableBalance": str,
+        "OnHoldBalance": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAssignmentRequestRequestTypeDef = TypedDict(
     "GetAssignmentRequestRequestTypeDef",
     {
         "AssignmentId": str,
     },
 )
 
@@ -382,14 +388,22 @@
     "GetFileUploadURLRequestRequestTypeDef",
     {
         "AssignmentId": str,
         "QuestionIdentifier": str,
     },
 )
 
+GetFileUploadURLResponseTypeDef = TypedDict(
+    "GetFileUploadURLResponseTypeDef",
+    {
+        "FileUploadURL": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHITRequestRequestTypeDef = TypedDict(
     "GetHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 
@@ -404,24 +418,35 @@
 GetQualificationTypeRequestRequestTypeDef = TypedDict(
     "GetQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HITId": str,
+    },
+)
+_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "AssignmentStatuses": Sequence[AssignmentStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
+    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssignmentsForHITRequestRequestTypeDef = TypedDict(
     "_RequiredListAssignmentsForHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalListAssignmentsForHITRequestRequestTypeDef = TypedDict(
@@ -436,25 +461,55 @@
 
 class ListAssignmentsForHITRequestRequestTypeDef(
     _RequiredListAssignmentsForHITRequestRequestTypeDef,
     _OptionalListAssignmentsForHITRequestRequestTypeDef,
 ):
     pass
 
+ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    {
+        "HITId": str,
+        "AssignmentId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBonusPaymentsRequestRequestTypeDef = TypedDict(
     "ListBonusPaymentsRequestRequestTypeDef",
     {
         "HITId": str,
         "AssignmentId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
+    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+):
+    pass
+
 _RequiredListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListHITsForQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -468,23 +523,40 @@
 
 class ListHITsForQualificationTypeRequestRequestTypeDef(
     _RequiredListHITsForQualificationTypeRequestRequestTypeDef,
     _OptionalListHITsForQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
+ListHITsRequestListHITsPaginateTypeDef = TypedDict(
+    "ListHITsRequestListHITsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHITsRequestRequestTypeDef = TypedDict(
     "ListHITsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQualificationRequestsRequestRequestTypeDef = TypedDict(
     "ListQualificationRequestsRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -500,14 +572,36 @@
         "Test": str,
         "Answer": str,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
+_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "MustBeRequestable": bool,
+    },
+)
+_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "Query": str,
+        "MustBeOwnedByCaller": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
+    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+):
+    pass
+
 _RequiredListQualificationTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListQualificationTypesRequestRequestTypeDef",
     {
         "MustBeRequestable": bool,
     },
 )
 _OptionalListQualificationTypesRequestRequestTypeDef = TypedDict(
@@ -547,25 +641,43 @@
 
 class ListReviewPolicyResultsForHITRequestRequestTypeDef(
     _RequiredListReviewPolicyResultsForHITRequestRequestTypeDef,
     _OptionalListReviewPolicyResultsForHITRequestRequestTypeDef,
 ):
     pass
 
+ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    {
+        "HITTypeId": str,
+        "Status": ReviewableHITStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReviewableHITsRequestRequestTypeDef = TypedDict(
     "ListReviewableHITsRequestRequestTypeDef",
     {
         "HITTypeId": str,
         "Status": ReviewableHITStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorkerBlocksRequestRequestTypeDef = TypedDict(
     "ListWorkerBlocksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -576,14 +688,35 @@
     {
         "WorkerId": str,
         "Reason": str,
     },
     total=False,
 )
 
+_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "Status": QualificationStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
+    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+):
+    pass
+
 _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersWithQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -644,14 +777,24 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
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
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -681,14 +824,25 @@
 
 class RejectQualificationRequestRequestRequestTypeDef(
     _RequiredRejectQualificationRequestRequestRequestTypeDef,
     _OptionalRejectQualificationRequestRequestRequestTypeDef,
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
 ReviewActionDetailTypeDef = TypedDict(
     "ReviewActionDetailTypeDef",
     {
         "ActionId": str,
         "ActionName": str,
         "TargetId": str,
         "TargetType": str,
@@ -794,239 +948,85 @@
 
 class UpdateQualificationTypeRequestRequestTypeDef(
     _RequiredUpdateQualificationTypeRequestRequestTypeDef,
     _OptionalUpdateQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
-CreateHITTypeResponseTypeDef = TypedDict(
-    "CreateHITTypeResponseTypeDef",
-    {
-        "HITTypeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountBalanceResponseTypeDef = TypedDict(
-    "GetAccountBalanceResponseTypeDef",
-    {
-        "AvailableBalance": str,
-        "OnHoldBalance": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFileUploadURLResponseTypeDef = TypedDict(
-    "GetFileUploadURLResponseTypeDef",
-    {
-        "FileUploadURL": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAssignmentsForHITResponseTypeDef = TypedDict(
     "ListAssignmentsForHITResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Assignments": List[AssignmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBonusPaymentsResponseTypeDef = TypedDict(
     "ListBonusPaymentsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "BonusPayments": List[BonusPaymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateQualificationTypeResponseTypeDef = TypedDict(
     "CreateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQualificationTypeResponseTypeDef = TypedDict(
     "GetQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQualificationTypesResponseTypeDef = TypedDict(
     "ListQualificationTypesResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationTypes": List[QualificationTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateQualificationTypeResponseTypeDef = TypedDict(
     "UpdateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "HITId": str,
-    },
-)
-_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "AssignmentStatuses": Sequence[AssignmentStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
-    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-):
-    pass
-
-ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    {
-        "HITId": str,
-        "AssignmentId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
-    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-):
-    pass
-
-ListHITsRequestListHITsPaginateTypeDef = TypedDict(
-    "ListHITsRequestListHITsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "MustBeRequestable": bool,
-    },
-)
-_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "Query": str,
-        "MustBeOwnedByCaller": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
-    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-):
-    pass
-
-ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    {
-        "HITTypeId": str,
-        "Status": ReviewableHITStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "Status": QualificationStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
-    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-):
-    pass
 
 ListQualificationRequestsResponseTypeDef = TypedDict(
     "ListQualificationRequestsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationRequests": List[QualificationRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkerBlocksResponseTypeDef = TypedDict(
     "ListWorkerBlocksResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
@@ -1091,15 +1091,15 @@
 ):
     pass
 
 NotifyWorkersResponseTypeDef = TypedDict(
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
@@ -1170,25 +1170,25 @@
     total=False,
 )
 
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
     "ListWorkersWithQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
@@ -1205,70 +1205,70 @@
 class ReviewPolicyTypeDef(_RequiredReviewPolicyTypeDef, _OptionalReviewPolicyTypeDef):
     pass
 
 CreateHITResponseTypeDef = TypedDict(
     "CreateHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHITWithHITTypeResponseTypeDef = TypedDict(
     "CreateHITWithHITTypeResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssignmentResponseTypeDef = TypedDict(
     "GetAssignmentResponseTypeDef",
     {
         "Assignment": AssignmentTypeDef,
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHITResponseTypeDef = TypedDict(
     "GetHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHITsForQualificationTypeResponseTypeDef = TypedDict(
     "ListHITsForQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHITsResponseTypeDef = TypedDict(
     "ListHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReviewableHITsResponseTypeDef = TypedDict(
     "ListReviewableHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
@@ -1334,10 +1334,10 @@
     {
         "HITId": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "AssignmentReviewReport": ReviewReportTypeDef,
         "HITReviewReport": ReviewReportTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/PKG-INFO` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MTurk 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MTurk 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
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
 
 <a id="mypy-boto3-mturk"></a>
 
 # mypy-boto3-mturk
 
 [![PyPI - mypy-boto3-mturk](https://img.shields.io/pypi/v/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mturk?color=blue)](https://pypistats.org/packages/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,72 +378,72 @@
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    ResponseMetadataTypeDef,
+    CreateHITTypeResponseTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
+    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
+    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
     UpdateExpirationForHITRequestRequestTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
-    CreateHITTypeResponseTypeDef,
-    GetAccountBalanceResponseTypeDef,
-    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     QualificationRequirementTypeDef,
     QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
@@ -473,42 +474,42 @@
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

### Comparing `mypy-boto3-mturk-1.26.0.post1/mypy_boto3_mturk.egg-info/SOURCES.txt` & `mypy-boto3-mturk-1.27.0/mypy_boto3_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.26.0.post1/setup.py` & `mypy-boto3-mturk-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-mturk.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mturk",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MTurk 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.MTurk 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 mturk type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_mturk": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_mturk": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/",
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


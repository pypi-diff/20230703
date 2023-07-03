# Comparing `tmp/mypy-boto3-support-1.26.61.tar.gz` & `tmp/mypy-boto3-support-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-support-1.26.61.tar", last modified: Tue Jan 31 20:49:59 2023, max compression
+gzip compressed data, was "mypy-boto3-support-1.27.0.tar", last modified: Mon Jul  3 19:51:32 2023, max compression
```

## Comparing `mypy-boto3-support-1.26.61.tar` & `mypy-boto3-support-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:59.038196 mypy-boto3-support-1.26.61/mypy_boto3_support/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-01-31 20:49:39.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/mypy_boto3_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-31 20:49:58.000000 mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:59.050196 mypy-boto3-support-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-31 20:49:38.000000 mypy-boto3-support-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:32.764085 mypy-boto3-support-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 19:51:32.764085 mypy-boto3-support-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:32.760085 mypy-boto3-support-1.27.0/mypy_boto3_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14850 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/mypy_boto3_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:32.764085 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 19:51:32.000000 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:51:32.000000 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:32.000000 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:32.000000 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:32.000000 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:32.000000 mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:32.764085 mypy-boto3-support-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:48:55.000000 mypy-boto3-support-1.27.0/setup.py
```

### Comparing `mypy-boto3-support-1.26.61/LICENSE` & `mypy-boto3-support-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-support-1.26.61/PKG-INFO` & `mypy-boto3-support-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.26.61
-Summary: Type annotations for boto3.Support 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Support 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,55 +322,63 @@
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
     AttachmentTypeDef,
-    ResponseMetadataTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
     CategoryTypeDef,
+    DateIntervalTypeDef,
+    SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
+    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCasesRequestRequestTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
+    DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
+    DescribeSupportedLanguagesRequestRequestTypeDef,
+    SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
+    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
+    ResolveCaseResponseTypeDef,
+    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
-    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
     ServiceTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    CommunicationTypeOptionsTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
+    DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
     DescribeServicesResponseTypeDef,
+    DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
@@ -383,42 +391,42 @@
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

### Comparing `mypy-boto3-support-1.26.61/README.md` & `mypy-boto3-support-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,55 +290,63 @@
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
     AttachmentTypeDef,
-    ResponseMetadataTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
     CategoryTypeDef,
+    DateIntervalTypeDef,
+    SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
+    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCasesRequestRequestTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
+    DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
+    DescribeSupportedLanguagesRequestRequestTypeDef,
+    SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
+    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
+    ResolveCaseResponseTypeDef,
+    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
-    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
     ServiceTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    CommunicationTypeOptionsTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
+    DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
     DescribeServicesResponseTypeDef,
+    DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
@@ -351,42 +359,42 @@
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

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.py` & `mypy-boto3-support-1.27.0/mypy_boto3_support/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/__init__.pyi` & `mypy-boto3-support-1.27.0/mypy_boto3_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/__main__.py` & `mypy-boto3-support-1.27.0/mypy_boto3_support/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Support 1.26.61\nVersion:         1.26.61\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Support 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/client.py` & `mypy-boto3-support-1.27.0/mypy_boto3_support/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,16 +23,18 @@
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     AttachmentTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
+    DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
+    DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     ResolveCaseResponseTypeDef,
 )
@@ -61,14 +63,15 @@
     AttachmentSetIdNotFound: Type[BotocoreClientError]
     AttachmentSetSizeLimitExceeded: Type[BotocoreClientError]
     CaseCreationLimitExceeded: Type[BotocoreClientError]
     CaseIdNotFound: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     DescribeAttachmentLimitExceeded: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
+    ThrottlingException: Type[BotocoreClientError]
 
 
 class SupportClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/)
     """
@@ -185,14 +188,25 @@
         """
         Returns communications and attachments for one or more support cases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_communications)
         """
 
+    def describe_create_case_options(
+        self, *, issueType: str, serviceCode: str, language: str, categoryCode: str
+    ) -> DescribeCreateCaseOptionsResponseTypeDef:
+        """
+        Returns a list of CreateCaseOption types along with the corresponding supported
+        hours and language availability.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_create_case_options)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_create_case_options)
+        """
+
     def describe_services(
         self, *, serviceCodeList: Sequence[str] = ..., language: str = ...
     ) -> DescribeServicesResponseTypeDef:
         """
         Returns the current list of Amazon Web Services services and a list of service
         categories for each service.
 
@@ -206,14 +220,25 @@
         """
         Returns the list of severity levels that you can assign to a support case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_severity_levels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_severity_levels)
         """
 
+    def describe_supported_languages(
+        self, *, issueType: str, serviceCode: str, categoryCode: str
+    ) -> DescribeSupportedLanguagesResponseTypeDef:
+        """
+        Returns a list of supported languages for a specified `categoryCode`,
+        `issueType` and `serviceCode`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_supported_languages)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_supported_languages)
+        """
+
     def describe_trusted_advisor_check_refresh_statuses(
         self, *, checkIds: Sequence[str]
     ) -> DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef:
         """
         Returns the refresh status of the Trusted Advisor checks that have the specified
         check IDs.
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/client.pyi` & `mypy-boto3-support-1.27.0/mypy_boto3_support/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,18 @@
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     AttachmentTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
+    DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
+    DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     ResolveCaseResponseTypeDef,
 )
@@ -58,14 +60,15 @@
     AttachmentSetIdNotFound: Type[BotocoreClientError]
     AttachmentSetSizeLimitExceeded: Type[BotocoreClientError]
     CaseCreationLimitExceeded: Type[BotocoreClientError]
     CaseIdNotFound: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     DescribeAttachmentLimitExceeded: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
+    ThrottlingException: Type[BotocoreClientError]
 
 class SupportClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/)
     """
 
@@ -172,14 +175,24 @@
     ) -> DescribeCommunicationsResponseTypeDef:
         """
         Returns communications and attachments for one or more support cases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_communications)
         """
+    def describe_create_case_options(
+        self, *, issueType: str, serviceCode: str, language: str, categoryCode: str
+    ) -> DescribeCreateCaseOptionsResponseTypeDef:
+        """
+        Returns a list of CreateCaseOption types along with the corresponding supported
+        hours and language availability.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_create_case_options)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_create_case_options)
+        """
     def describe_services(
         self, *, serviceCodeList: Sequence[str] = ..., language: str = ...
     ) -> DescribeServicesResponseTypeDef:
         """
         Returns the current list of Amazon Web Services services and a list of service
         categories for each service.
 
@@ -191,14 +204,24 @@
     ) -> DescribeSeverityLevelsResponseTypeDef:
         """
         Returns the list of severity levels that you can assign to a support case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_severity_levels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_severity_levels)
         """
+    def describe_supported_languages(
+        self, *, issueType: str, serviceCode: str, categoryCode: str
+    ) -> DescribeSupportedLanguagesResponseTypeDef:
+        """
+        Returns a list of supported languages for a specified `categoryCode`,
+        `issueType` and `serviceCode`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_supported_languages)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_supported_languages)
+        """
     def describe_trusted_advisor_check_refresh_statuses(
         self, *, checkIds: Sequence[str]
     ) -> DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef:
         """
         Returns the refresh status of the Trusted Advisor checks that have the specified
         check IDs.
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/literals.py` & `mypy-boto3-support-1.27.0/mypy_boto3_support/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
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
@@ -90,14 +91,15 @@
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
@@ -176,14 +178,15 @@
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
@@ -194,14 +197,15 @@
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
@@ -237,14 +241,15 @@
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
@@ -263,16 +268,19 @@
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
@@ -352,18 +360,21 @@
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

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/literals.pyi` & `mypy-boto3-support-1.27.0/mypy_boto3_support/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
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
@@ -88,14 +89,15 @@
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
@@ -174,14 +176,15 @@
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
@@ -192,14 +195,15 @@
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
@@ -235,14 +239,15 @@
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
@@ -261,16 +266,19 @@
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
@@ -350,18 +358,21 @@
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

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.py` & `mypy-boto3-support-1.27.0/mypy_boto3_support/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecasespaginator)
         """
 
 
@@ -76,13 +76,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/paginator.pyi` & `mypy-boto3-support-1.27.0/mypy_boto3_support/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecasespaginator)
         """
 
 class DescribeCommunicationsPaginator(Paginator):
@@ -72,13 +72,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.py` & `mypy-boto3-support-1.27.0/mypy_boto3_support/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,55 +20,63 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttachmentTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
+    "AddCommunicationToCaseResponseTypeDef",
     "AttachmentDetailsTypeDef",
     "CategoryTypeDef",
+    "DateIntervalTypeDef",
+    "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
+    "CreateCaseResponseTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCasesRequestRequestTypeDef",
+    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeCommunicationsRequestRequestTypeDef",
+    "DescribeCreateCaseOptionsRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "DescribeSeverityLevelsRequestRequestTypeDef",
     "SeverityLevelTypeDef",
+    "DescribeSupportedLanguagesRequestRequestTypeDef",
+    "SupportedLanguageTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     "TrustedAdvisorCheckRefreshStatusTypeDef",
     "DescribeTrustedAdvisorCheckResultRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef",
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
+    "PaginatorConfigTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
+    "ResolveCaseResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetRequestRequestTypeDef",
-    "AddAttachmentsToSetResponseTypeDef",
-    "AddCommunicationToCaseResponseTypeDef",
-    "CreateCaseResponseTypeDef",
     "DescribeAttachmentResponseTypeDef",
-    "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
     "ServiceTypeDef",
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
-    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    "CommunicationTypeOptionsTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
+    "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
     "DescribeServicesResponseTypeDef",
+    "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
@@ -78,22 +86,20 @@
     {
         "fileName": str,
         "data": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddAttachmentsToSetResponseTypeDef = TypedDict(
+    "AddAttachmentsToSetResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "attachmentSetId": str,
+        "expiryTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "_RequiredAddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
@@ -113,14 +119,22 @@
 class AddCommunicationToCaseRequestRequestTypeDef(
     _RequiredAddCommunicationToCaseRequestRequestTypeDef,
     _OptionalAddCommunicationToCaseRequestRequestTypeDef,
 ):
     pass
 
 
+AddCommunicationToCaseResponseTypeDef = TypedDict(
+    "AddCommunicationToCaseResponseTypeDef",
+    {
+        "result": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttachmentDetailsTypeDef = TypedDict(
     "AttachmentDetailsTypeDef",
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
@@ -131,14 +145,32 @@
     {
         "code": str,
         "name": str,
     },
     total=False,
 )
 
+DateIntervalTypeDef = TypedDict(
+    "DateIntervalTypeDef",
+    {
+        "startDateTime": str,
+        "endDateTime": str,
+    },
+    total=False,
+)
+
+SupportedHourTypeDef = TypedDict(
+    "SupportedHourTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+    },
+    total=False,
+)
+
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "subject": str,
         "communicationBody": str,
     },
 )
@@ -159,27 +191,40 @@
 
 class CreateCaseRequestRequestTypeDef(
     _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
 
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAttachmentRequestRequestTypeDef = TypedDict(
     "DescribeAttachmentRequestRequestTypeDef",
     {
         "attachmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "caseIdList": Sequence[str],
+        "displayId": str,
+        "afterTime": str,
+        "beforeTime": str,
+        "includeResolvedCases": bool,
+        "language": str,
+        "includeCommunications": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeCasesRequestRequestTypeDef = TypedDict(
     "DescribeCasesRequestRequestTypeDef",
     {
@@ -192,14 +237,38 @@
         "maxResults": int,
         "language": str,
         "includeCommunications": bool,
     },
     total=False,
 )
 
+_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "caseId": str,
+    },
+)
+_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "beforeTime": str,
+        "afterTime": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
+    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeCommunicationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommunicationsRequestRequestTypeDef",
     {
         "caseId": str,
     },
 )
 _OptionalDescribeCommunicationsRequestRequestTypeDef = TypedDict(
@@ -217,14 +286,24 @@
 class DescribeCommunicationsRequestRequestTypeDef(
     _RequiredDescribeCommunicationsRequestRequestTypeDef,
     _OptionalDescribeCommunicationsRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeCreateCaseOptionsRequestRequestTypeDef = TypedDict(
+    "DescribeCreateCaseOptionsRequestRequestTypeDef",
+    {
+        "issueType": str,
+        "serviceCode": str,
+        "language": str,
+        "categoryCode": str,
+    },
+)
+
 DescribeServicesRequestRequestTypeDef = TypedDict(
     "DescribeServicesRequestRequestTypeDef",
     {
         "serviceCodeList": Sequence[str],
         "language": str,
     },
     total=False,
@@ -243,14 +322,33 @@
     {
         "code": str,
         "name": str,
     },
     total=False,
 )
 
+DescribeSupportedLanguagesRequestRequestTypeDef = TypedDict(
+    "DescribeSupportedLanguagesRequestRequestTypeDef",
+    {
+        "issueType": str,
+        "serviceCode": str,
+        "categoryCode": str,
+    },
+)
+
+SupportedLanguageTypeDef = TypedDict(
+    "SupportedLanguageTypeDef",
+    {
+        "code": str,
+        "language": str,
+        "display": str,
+    },
+    total=False,
+)
+
 DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     {
         "checkIds": Sequence[str],
     },
 )
 
@@ -306,14 +404,24 @@
         "name": str,
         "description": str,
         "category": str,
         "metadata": List[str],
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
 RefreshTrustedAdvisorCheckRequestRequestTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     {
         "checkId": str,
     },
 )
 
@@ -321,14 +429,34 @@
     "ResolveCaseRequestRequestTypeDef",
     {
         "caseId": str,
     },
     total=False,
 )
 
+ResolveCaseResponseTypeDef = TypedDict(
+    "ResolveCaseResponseTypeDef",
+    {
+        "initialCaseStatus": str,
+        "finalCaseStatus": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
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
 TrustedAdvisorCostOptimizingSummaryTypeDef = TypedDict(
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     {
         "estimatedMonthlySavings": float,
         "estimatedPercentMonthlySavings": float,
     },
 )
@@ -385,53 +513,19 @@
 class AddAttachmentsToSetRequestRequestTypeDef(
     _RequiredAddAttachmentsToSetRequestRequestTypeDef,
     _OptionalAddAttachmentsToSetRequestRequestTypeDef,
 ):
     pass
 
 
-AddAttachmentsToSetResponseTypeDef = TypedDict(
-    "AddAttachmentsToSetResponseTypeDef",
-    {
-        "attachmentSetId": str,
-        "expiryTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddCommunicationToCaseResponseTypeDef = TypedDict(
-    "AddCommunicationToCaseResponseTypeDef",
-    {
-        "result": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAttachmentResponseTypeDef = TypedDict(
     "DescribeAttachmentResponseTypeDef",
     {
         "attachment": AttachmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResolveCaseResponseTypeDef = TypedDict(
-    "ResolveCaseResponseTypeDef",
-    {
-        "initialCaseStatus": str,
-        "finalCaseStatus": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommunicationTypeDef = TypedDict(
     "CommunicationTypeDef",
     {
         "caseId": str,
@@ -449,82 +543,61 @@
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
     total=False,
 )
 
-DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+CommunicationTypeOptionsTypeDef = TypedDict(
+    "CommunicationTypeOptionsTypeDef",
     {
-        "caseIdList": Sequence[str],
-        "displayId": str,
-        "afterTime": str,
-        "beforeTime": str,
-        "includeResolvedCases": bool,
-        "language": str,
-        "includeCommunications": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "type": str,
+        "supportedHours": List[SupportedHourTypeDef],
+        "datesWithoutSupport": List[DateIntervalTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "caseId": str,
-    },
-)
-_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+DescribeSeverityLevelsResponseTypeDef = TypedDict(
+    "DescribeSeverityLevelsResponseTypeDef",
     {
-        "beforeTime": str,
-        "afterTime": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "severityLevels": List[SeverityLevelTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
-    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-):
-    pass
-
-
-DescribeSeverityLevelsResponseTypeDef = TypedDict(
-    "DescribeSeverityLevelsResponseTypeDef",
+DescribeSupportedLanguagesResponseTypeDef = TypedDict(
+    "DescribeSupportedLanguagesResponseTypeDef",
     {
-        "severityLevels": List[SeverityLevelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "supportedLanguages": List[SupportedLanguageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     {
         "statuses": List[TrustedAdvisorCheckRefreshStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RefreshTrustedAdvisorCheckResponseTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     {
         "status": TrustedAdvisorCheckRefreshStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrustedAdvisorChecksResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     {
         "checks": List[TrustedAdvisorCheckDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrustedAdvisorCategorySpecificSummaryTypeDef = TypedDict(
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     {
         "costOptimizing": TrustedAdvisorCostOptimizingSummaryTypeDef,
@@ -533,15 +606,15 @@
 )
 
 DescribeCommunicationsResponseTypeDef = TypedDict(
     "DescribeCommunicationsResponseTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": List[CommunicationTypeDef],
@@ -550,15 +623,24 @@
     total=False,
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeCreateCaseOptionsResponseTypeDef = TypedDict(
+    "DescribeCreateCaseOptionsResponseTypeDef",
+    {
+        "languageAvailability": str,
+        "communicationTypes": List[CommunicationTypeOptionsTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrustedAdvisorCheckResultTypeDef = TypedDict(
     "TrustedAdvisorCheckResultTypeDef",
     {
         "checkId": str,
@@ -614,27 +696,27 @@
     total=False,
 )
 
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrustedAdvisorCheckSummariesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     {
         "summaries": List[TrustedAdvisorCheckSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCasesResponseTypeDef = TypedDict(
     "DescribeCasesResponseTypeDef",
     {
         "cases": List[CaseDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support/type_defs.pyi` & `mypy-boto3-support-1.27.0/mypy_boto3_support/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,55 +19,63 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
+    "AddCommunicationToCaseResponseTypeDef",
     "AttachmentDetailsTypeDef",
     "CategoryTypeDef",
+    "DateIntervalTypeDef",
+    "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
+    "CreateCaseResponseTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCasesRequestRequestTypeDef",
+    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeCommunicationsRequestRequestTypeDef",
+    "DescribeCreateCaseOptionsRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "DescribeSeverityLevelsRequestRequestTypeDef",
     "SeverityLevelTypeDef",
+    "DescribeSupportedLanguagesRequestRequestTypeDef",
+    "SupportedLanguageTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     "TrustedAdvisorCheckRefreshStatusTypeDef",
     "DescribeTrustedAdvisorCheckResultRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef",
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
+    "PaginatorConfigTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
+    "ResolveCaseResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetRequestRequestTypeDef",
-    "AddAttachmentsToSetResponseTypeDef",
-    "AddCommunicationToCaseResponseTypeDef",
-    "CreateCaseResponseTypeDef",
     "DescribeAttachmentResponseTypeDef",
-    "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
     "ServiceTypeDef",
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
-    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    "CommunicationTypeOptionsTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
+    "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
     "DescribeServicesResponseTypeDef",
+    "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
@@ -77,22 +85,20 @@
     {
         "fileName": str,
         "data": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddAttachmentsToSetResponseTypeDef = TypedDict(
+    "AddAttachmentsToSetResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "attachmentSetId": str,
+        "expiryTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "_RequiredAddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
@@ -110,14 +116,22 @@
 
 class AddCommunicationToCaseRequestRequestTypeDef(
     _RequiredAddCommunicationToCaseRequestRequestTypeDef,
     _OptionalAddCommunicationToCaseRequestRequestTypeDef,
 ):
     pass
 
+AddCommunicationToCaseResponseTypeDef = TypedDict(
+    "AddCommunicationToCaseResponseTypeDef",
+    {
+        "result": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttachmentDetailsTypeDef = TypedDict(
     "AttachmentDetailsTypeDef",
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
@@ -128,14 +142,32 @@
     {
         "code": str,
         "name": str,
     },
     total=False,
 )
 
+DateIntervalTypeDef = TypedDict(
+    "DateIntervalTypeDef",
+    {
+        "startDateTime": str,
+        "endDateTime": str,
+    },
+    total=False,
+)
+
+SupportedHourTypeDef = TypedDict(
+    "SupportedHourTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+    },
+    total=False,
+)
+
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "subject": str,
         "communicationBody": str,
     },
 )
@@ -154,27 +186,40 @@
 )
 
 class CreateCaseRequestRequestTypeDef(
     _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAttachmentRequestRequestTypeDef = TypedDict(
     "DescribeAttachmentRequestRequestTypeDef",
     {
         "attachmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "caseIdList": Sequence[str],
+        "displayId": str,
+        "afterTime": str,
+        "beforeTime": str,
+        "includeResolvedCases": bool,
+        "language": str,
+        "includeCommunications": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeCasesRequestRequestTypeDef = TypedDict(
     "DescribeCasesRequestRequestTypeDef",
     {
@@ -187,14 +232,36 @@
         "maxResults": int,
         "language": str,
         "includeCommunications": bool,
     },
     total=False,
 )
 
+_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "caseId": str,
+    },
+)
+_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "beforeTime": str,
+        "afterTime": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
+    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeCommunicationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommunicationsRequestRequestTypeDef",
     {
         "caseId": str,
     },
 )
 _OptionalDescribeCommunicationsRequestRequestTypeDef = TypedDict(
@@ -210,14 +277,24 @@
 
 class DescribeCommunicationsRequestRequestTypeDef(
     _RequiredDescribeCommunicationsRequestRequestTypeDef,
     _OptionalDescribeCommunicationsRequestRequestTypeDef,
 ):
     pass
 
+DescribeCreateCaseOptionsRequestRequestTypeDef = TypedDict(
+    "DescribeCreateCaseOptionsRequestRequestTypeDef",
+    {
+        "issueType": str,
+        "serviceCode": str,
+        "language": str,
+        "categoryCode": str,
+    },
+)
+
 DescribeServicesRequestRequestTypeDef = TypedDict(
     "DescribeServicesRequestRequestTypeDef",
     {
         "serviceCodeList": Sequence[str],
         "language": str,
     },
     total=False,
@@ -236,14 +313,33 @@
     {
         "code": str,
         "name": str,
     },
     total=False,
 )
 
+DescribeSupportedLanguagesRequestRequestTypeDef = TypedDict(
+    "DescribeSupportedLanguagesRequestRequestTypeDef",
+    {
+        "issueType": str,
+        "serviceCode": str,
+        "categoryCode": str,
+    },
+)
+
+SupportedLanguageTypeDef = TypedDict(
+    "SupportedLanguageTypeDef",
+    {
+        "code": str,
+        "language": str,
+        "display": str,
+    },
+    total=False,
+)
+
 DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     {
         "checkIds": Sequence[str],
     },
 )
 
@@ -297,14 +393,24 @@
         "name": str,
         "description": str,
         "category": str,
         "metadata": List[str],
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
 RefreshTrustedAdvisorCheckRequestRequestTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     {
         "checkId": str,
     },
 )
 
@@ -312,14 +418,34 @@
     "ResolveCaseRequestRequestTypeDef",
     {
         "caseId": str,
     },
     total=False,
 )
 
+ResolveCaseResponseTypeDef = TypedDict(
+    "ResolveCaseResponseTypeDef",
+    {
+        "initialCaseStatus": str,
+        "finalCaseStatus": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
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
 TrustedAdvisorCostOptimizingSummaryTypeDef = TypedDict(
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     {
         "estimatedMonthlySavings": float,
         "estimatedPercentMonthlySavings": float,
     },
 )
@@ -372,53 +498,19 @@
 
 class AddAttachmentsToSetRequestRequestTypeDef(
     _RequiredAddAttachmentsToSetRequestRequestTypeDef,
     _OptionalAddAttachmentsToSetRequestRequestTypeDef,
 ):
     pass
 
-AddAttachmentsToSetResponseTypeDef = TypedDict(
-    "AddAttachmentsToSetResponseTypeDef",
-    {
-        "attachmentSetId": str,
-        "expiryTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddCommunicationToCaseResponseTypeDef = TypedDict(
-    "AddCommunicationToCaseResponseTypeDef",
-    {
-        "result": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAttachmentResponseTypeDef = TypedDict(
     "DescribeAttachmentResponseTypeDef",
     {
         "attachment": AttachmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResolveCaseResponseTypeDef = TypedDict(
-    "ResolveCaseResponseTypeDef",
-    {
-        "initialCaseStatus": str,
-        "finalCaseStatus": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommunicationTypeDef = TypedDict(
     "CommunicationTypeDef",
     {
         "caseId": str,
@@ -436,80 +528,61 @@
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
     total=False,
 )
 
-DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+CommunicationTypeOptionsTypeDef = TypedDict(
+    "CommunicationTypeOptionsTypeDef",
     {
-        "caseIdList": Sequence[str],
-        "displayId": str,
-        "afterTime": str,
-        "beforeTime": str,
-        "includeResolvedCases": bool,
-        "language": str,
-        "includeCommunications": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "type": str,
+        "supportedHours": List[SupportedHourTypeDef],
+        "datesWithoutSupport": List[DateIntervalTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "caseId": str,
-    },
-)
-_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+DescribeSeverityLevelsResponseTypeDef = TypedDict(
+    "DescribeSeverityLevelsResponseTypeDef",
     {
-        "beforeTime": str,
-        "afterTime": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "severityLevels": List[SeverityLevelTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
-    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-):
-    pass
-
-DescribeSeverityLevelsResponseTypeDef = TypedDict(
-    "DescribeSeverityLevelsResponseTypeDef",
+DescribeSupportedLanguagesResponseTypeDef = TypedDict(
+    "DescribeSupportedLanguagesResponseTypeDef",
     {
-        "severityLevels": List[SeverityLevelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "supportedLanguages": List[SupportedLanguageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     {
         "statuses": List[TrustedAdvisorCheckRefreshStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RefreshTrustedAdvisorCheckResponseTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     {
         "status": TrustedAdvisorCheckRefreshStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrustedAdvisorChecksResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     {
         "checks": List[TrustedAdvisorCheckDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrustedAdvisorCategorySpecificSummaryTypeDef = TypedDict(
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     {
         "costOptimizing": TrustedAdvisorCostOptimizingSummaryTypeDef,
@@ -518,15 +591,15 @@
 )
 
 DescribeCommunicationsResponseTypeDef = TypedDict(
     "DescribeCommunicationsResponseTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": List[CommunicationTypeDef],
@@ -535,15 +608,24 @@
     total=False,
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeCreateCaseOptionsResponseTypeDef = TypedDict(
+    "DescribeCreateCaseOptionsResponseTypeDef",
+    {
+        "languageAvailability": str,
+        "communicationTypes": List[CommunicationTypeOptionsTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrustedAdvisorCheckResultTypeDef = TypedDict(
     "TrustedAdvisorCheckResultTypeDef",
     {
         "checkId": str,
@@ -597,27 +679,27 @@
     total=False,
 )
 
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrustedAdvisorCheckSummariesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     {
         "summaries": List[TrustedAdvisorCheckSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCasesResponseTypeDef = TypedDict(
     "DescribeCasesResponseTypeDef",
     {
         "cases": List[CaseDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/PKG-INFO` & `mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.26.61
-Summary: Type annotations for boto3.Support 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Support 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,55 +322,63 @@
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
     AttachmentTypeDef,
-    ResponseMetadataTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
     CategoryTypeDef,
+    DateIntervalTypeDef,
+    SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
+    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCasesRequestRequestTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
+    DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
+    DescribeSupportedLanguagesRequestRequestTypeDef,
+    SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
+    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
+    ResolveCaseResponseTypeDef,
+    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
-    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
     ServiceTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    CommunicationTypeOptionsTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
+    DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
     RecentCaseCommunicationsTypeDef,
     DescribeServicesResponseTypeDef,
+    DescribeCreateCaseOptionsResponseTypeDef,
     TrustedAdvisorCheckResultTypeDef,
     TrustedAdvisorCheckSummaryTypeDef,
     CaseDetailsTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
@@ -383,42 +391,42 @@
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

### Comparing `mypy-boto3-support-1.26.61/mypy_boto3_support.egg-info/SOURCES.txt` & `mypy-boto3-support-1.27.0/mypy_boto3_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.26.61/setup.py` & `mypy-boto3-support-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-support.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-support",
-    version="1.26.61",
+    version="1.27.0",
     packages=["mypy_boto3_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Support 1.26.61 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Support 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/",
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


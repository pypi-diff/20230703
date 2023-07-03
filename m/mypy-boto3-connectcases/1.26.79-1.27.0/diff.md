# Comparing `tmp/mypy-boto3-connectcases-1.26.79.tar.gz` & `tmp/mypy-boto3-connectcases-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcases-1.27.0.tar", last modified: Mon Jul  3 19:50:36 2023, max compression
```

## Comparing `mypy-boto3-connectcases-1.26.79.tar` & `mypy-boto3-connectcases-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-02-24 21:22:07.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-02-24 21:22:07.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29408 2023-02-24 21:22:07.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.287066 mypy-boto3-connectcases-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-07-03 19:50:36.287066 mypy-boto3-connectcases-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.287066 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-03 19:35:06.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-03 19:35:06.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-07-03 19:35:06.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29458 2023-07-03 19:35:06.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.287066 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-07-03 19:50:36.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:36.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:36.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:36.000000 mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:36.287066 mypy-boto3-connectcases-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:35:05.000000 mypy-boto3-connectcases-1.27.0/setup.py
```

### Comparing `mypy-boto3-connectcases-1.26.79/LICENSE` & `mypy-boto3-connectcases-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-connectcases-1.26.79/PKG-INFO` & `mypy-boto3-connectcases-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.26.79
-Summary: Type annotations for boto3.ConnectCases 1.26.79 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectCases 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,63 +333,63 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
-    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     CaseSummaryTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
+    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
+    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
+    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    CreateDomainResponseTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
-    CreateTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDomainResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
@@ -437,42 +437,42 @@
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

### Comparing `mypy-boto3-connectcases-1.26.79/README.md` & `mypy-boto3-connectcases-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,63 +301,63 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
-    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     CaseSummaryTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
+    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
+    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
+    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    CreateDomainResponseTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
-    CreateTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDomainResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
@@ -405,42 +405,42 @@
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

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.py` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.pyi` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__main__.py` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.26.79\nVersion:         1.26.79\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.ConnectCases 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.79")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.py` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.pyi` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.py` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "RegionName",
 )
 
 
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
-FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text"]
+FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text", "Url"]
 OrderType = Literal["Asc", "Desc"]
 RelatedItemTypeType = Literal["Comment", "Contact"]
 SearchCasesPaginatorName = Literal["search_cases"]
 SearchRelatedItemsPaginatorName = Literal["search_related_items"]
 TemplateStatusType = Literal["Active", "Inactive"]
 ConnectCasesServiceName = Literal["connectcases"]
 ServiceName = Literal[
@@ -58,14 +58,15 @@
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
@@ -105,14 +106,15 @@
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
@@ -191,14 +193,15 @@
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
@@ -209,14 +212,15 @@
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
@@ -252,14 +256,15 @@
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
@@ -278,16 +283,19 @@
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
@@ -371,15 +379,17 @@
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

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.pyi` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "PaginatorName",
     "RegionName",
 )
 
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
-FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text"]
+FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text", "Url"]
 OrderType = Literal["Asc", "Desc"]
 RelatedItemTypeType = Literal["Comment", "Contact"]
 SearchCasesPaginatorName = Literal["search_cases"]
 SearchRelatedItemsPaginatorName = Literal["search_related_items"]
 TemplateStatusType = Literal["Active", "Inactive"]
 ConnectCasesServiceName = Literal["connectcases"]
 ServiceName = Literal[
@@ -56,14 +56,15 @@
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
@@ -103,14 +104,15 @@
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
@@ -189,14 +191,15 @@
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
@@ -207,14 +210,15 @@
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
@@ -250,14 +254,15 @@
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
@@ -276,16 +281,19 @@
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
@@ -369,15 +377,17 @@
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

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.py` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchcasespaginator)
         """
 
 
@@ -78,13 +78,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.pyi` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchcasespaginator)
         """
 
 class SearchRelatedItemsPaginator(Paginator):
@@ -74,13 +74,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.py` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,63 +34,63 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
     "CaseSummaryTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
+    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
+    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
+    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
-    "CreateCaseResponseTypeDef",
-    "CreateDomainResponseTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
-    "CreateTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDomainResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
@@ -177,25 +177,14 @@
 )
 
 
 class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
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
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -247,21 +236,40 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -277,14 +285,41 @@
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
 
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
+        "fieldId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
+    {
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -292,14 +327,23 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -308,14 +352,21 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
@@ -357,14 +408,27 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -490,14 +554,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -533,14 +605,25 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -623,98 +706,15 @@
 
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
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
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
     "BatchPutFieldOptionsRequestRequestTypeDef",
     {
         "domainId": str,
@@ -724,32 +724,32 @@
 )
 
 ListFieldOptionsResponseTypeDef = TypedDict(
     "ListFieldOptionsResponseTypeDef",
     {
         "nextToken": str,
         "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
         "comment": CommentContentTypeDef,
@@ -808,15 +808,15 @@
         "layoutConfiguration": LayoutConfigurationTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
@@ -843,15 +843,15 @@
 
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
@@ -871,15 +871,15 @@
 
 
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
@@ -888,24 +888,24 @@
 )
 
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -940,15 +940,15 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
@@ -1022,15 +1022,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1096,15 +1096,15 @@
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchCasesResponseItemTypeDef = TypedDict(
     "_RequiredSearchCasesResponseItemTypeDef",
     {
         "caseId": str,
@@ -1158,15 +1158,15 @@
 
 
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
@@ -1185,23 +1185,23 @@
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
         "eventBridge": EventBridgeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
@@ -1239,15 +1239,15 @@
     "GetLayoutResponseTypeDef",
     {
         "content": LayoutContentTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
```

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.pyi` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -33,63 +33,63 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
     "CaseSummaryTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
+    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
+    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
+    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
-    "CreateCaseResponseTypeDef",
-    "CreateDomainResponseTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
-    "CreateTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDomainResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
@@ -172,25 +172,14 @@
     },
     total=False,
 )
 
 class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
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
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -242,21 +231,40 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -270,14 +278,41 @@
 )
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
+        "fieldId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
+    {
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -285,14 +320,23 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -301,14 +345,21 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
@@ -350,14 +401,27 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -475,14 +539,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -516,14 +588,25 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -602,98 +685,15 @@
     pass
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
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
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
     "BatchPutFieldOptionsRequestRequestTypeDef",
     {
         "domainId": str,
@@ -703,32 +703,32 @@
 )
 
 ListFieldOptionsResponseTypeDef = TypedDict(
     "ListFieldOptionsResponseTypeDef",
     {
         "nextToken": str,
         "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
         "comment": CommentContentTypeDef,
@@ -785,15 +785,15 @@
         "layoutConfiguration": LayoutConfigurationTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
@@ -818,15 +818,15 @@
     pass
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
@@ -844,15 +844,15 @@
     pass
 
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
@@ -861,24 +861,24 @@
 )
 
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -911,15 +911,15 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
@@ -987,15 +987,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1057,15 +1057,15 @@
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchCasesResponseItemTypeDef = TypedDict(
     "_RequiredSearchCasesResponseItemTypeDef",
     {
         "caseId": str,
@@ -1115,15 +1115,15 @@
     pass
 
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
@@ -1142,23 +1142,23 @@
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
         "eventBridge": EventBridgeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
@@ -1196,15 +1196,15 @@
     "GetLayoutResponseTypeDef",
     {
         "content": LayoutContentTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
```

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.26.79
-Summary: Type annotations for boto3.ConnectCases 1.26.79 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectCases 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,63 +333,63 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
-    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     CaseSummaryTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
+    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
+    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
+    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    CreateDomainResponseTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
-    CreateTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDomainResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
@@ -437,42 +437,42 @@
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

### Comparing `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy-boto3-connectcases-1.27.0/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.79/setup.py` & `mypy-boto3-connectcases-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-connectcases.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.26.79",
+    version="1.27.0",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCases 1.26.79 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.ConnectCases 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/",
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


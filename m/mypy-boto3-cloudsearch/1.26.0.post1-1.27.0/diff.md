# Comparing `tmp/mypy-boto3-cloudsearch-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cloudsearch-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearch-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:12 2022, max compression
+gzip compressed data, was "mypy-boto3-cloudsearch-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-cloudsearch-1.26.0.post1.tar` & `mypy-boto3-cloudsearch-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:12.052840 mypy-boto3-cloudsearch-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15305 2022-11-01 21:43:12.052840 mypy-boto3-cloudsearch-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13848 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:12.044840 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18569 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    18537 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8702 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8700 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    25479 2022-11-01 21:31:36.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    25454 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:12.052840 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15305 2022-11-01 21:43:11.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-11-01 21:43:11.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:11.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:11.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:11.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-01 21:43:11.000000 mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:12.052840 mypy-boto3-cloudsearch-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-11-01 21:31:35.000000 mypy-boto3-cloudsearch-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.942952 mypy-boto3-cloudsearch-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-03 19:50:29.938953 mypy-boto3-cloudsearch-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.938953 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:57.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.938953 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-03 19:50:29.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 19:50:29.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:29.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:50:29.000000 mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.942952 mypy-boto3-cloudsearch-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:33:56.000000 mypy-boto3-cloudsearch-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/LICENSE` & `mypy-boto3-cloudsearch-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/PKG-INFO` & `mypy-boto3-cloudsearch-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearch
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CloudSearch 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudSearch 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
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
 
 <a id="mypy-boto3-cloudsearch"></a>
 
 # mypy-boto3-cloudsearch
 
 [![PyPI - mypy-boto3-cloudsearch](https://img.shields.io/pypi/v/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,15 +305,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BuildSuggestersResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
     DateArrayOptionsTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
@@ -330,30 +331,30 @@
     DocumentSuggesterOptionsTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
     DoubleArrayOptionsTypeDef,
     DoubleOptionsTypeDef,
     IndexDocumentsRequestRequestTypeDef,
+    IndexDocumentsResponseTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
+    ListDomainNamesResponseTypeDef,
+    ResponseMetadataTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
     AnalysisSchemeTypeDef,
-    BuildSuggestersResponseTypeDef,
-    IndexDocumentsResponseTypeDef,
-    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
     ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
     IndexFieldTypeDef,
@@ -398,42 +399,42 @@
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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/README.md` & `mypy-boto3-cloudsearch-1.27.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudsearch"></a>
 
 # mypy-boto3-cloudsearch
 
 [![PyPI - mypy-boto3-cloudsearch](https://img.shields.io/pypi/v/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,15 +273,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BuildSuggestersResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
     DateArrayOptionsTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
@@ -299,30 +299,30 @@
     DocumentSuggesterOptionsTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
     DoubleArrayOptionsTypeDef,
     DoubleOptionsTypeDef,
     IndexDocumentsRequestRequestTypeDef,
+    IndexDocumentsResponseTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
+    ListDomainNamesResponseTypeDef,
+    ResponseMetadataTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
     AnalysisSchemeTypeDef,
-    BuildSuggestersResponseTypeDef,
-    IndexDocumentsResponseTypeDef,
-    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
     ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
     IndexFieldTypeDef,
@@ -367,42 +367,42 @@
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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/__main__.py` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearch 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CloudSearch 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/client.py` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,25 +135,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#define_analysis_scheme)
         """
 
     def define_expression(
         self, *, DomainName: str, Expression: ExpressionTypeDef
     ) -> DefineExpressionResponseTypeDef:
         """
-        Configures an ` Expression` for the search domain.
+        Configures an `Expression` for the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.define_expression)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#define_expression)
         """
 
     def define_index_field(
         self, *, DomainName: str, IndexField: IndexFieldTypeDef
     ) -> DefineIndexFieldResponseTypeDef:
         """
-        Configures an ` IndexField` for the search domain.
+        Configures an `IndexField` for the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.define_index_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#define_index_field)
         """
 
     def define_suggester(
         self, *, DomainName: str, Suggester: SuggesterTypeDef
@@ -183,25 +183,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#delete_domain)
         """
 
     def delete_expression(
         self, *, DomainName: str, ExpressionName: str
     ) -> DeleteExpressionResponseTypeDef:
         """
-        Removes an ` Expression` from the search domain.
+        Removes an `Expression` from the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.delete_expression)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#delete_expression)
         """
 
     def delete_index_field(
         self, *, DomainName: str, IndexFieldName: str
     ) -> DeleteIndexFieldResponseTypeDef:
         """
-        Removes an ` IndexField` from the search domain.
+        Removes an `IndexField` from the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.delete_index_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#delete_index_field)
         """
 
     def delete_suggester(
         self, *, DomainName: str, SuggesterName: str
```

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/client.pyi` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -126,24 +126,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.define_analysis_scheme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#define_analysis_scheme)
         """
     def define_expression(
         self, *, DomainName: str, Expression: ExpressionTypeDef
     ) -> DefineExpressionResponseTypeDef:
         """
-        Configures an ` Expression` for the search domain.
+        Configures an `Expression` for the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.define_expression)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#define_expression)
         """
     def define_index_field(
         self, *, DomainName: str, IndexField: IndexFieldTypeDef
     ) -> DefineIndexFieldResponseTypeDef:
         """
-        Configures an ` IndexField` for the search domain.
+        Configures an `IndexField` for the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.define_index_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#define_index_field)
         """
     def define_suggester(
         self, *, DomainName: str, Suggester: SuggesterTypeDef
     ) -> DefineSuggesterResponseTypeDef:
@@ -169,24 +169,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#delete_domain)
         """
     def delete_expression(
         self, *, DomainName: str, ExpressionName: str
     ) -> DeleteExpressionResponseTypeDef:
         """
-        Removes an ` Expression` from the search domain.
+        Removes an `Expression` from the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.delete_expression)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#delete_expression)
         """
     def delete_index_field(
         self, *, DomainName: str, IndexFieldName: str
     ) -> DeleteIndexFieldResponseTypeDef:
         """
-        Removes an ` IndexField` from the search domain.
+        Removes an `IndexField` from the search domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client.delete_index_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/client/#delete_index_field)
         """
     def delete_suggester(
         self, *, DomainName: str, SuggesterName: str
     ) -> DeleteSuggesterResponseTypeDef:
```

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/literals.py` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,25 @@
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
@@ -145,30 +147,35 @@
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
@@ -194,14 +201,15 @@
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
@@ -246,51 +254,57 @@
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
@@ -303,14 +317,15 @@
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
@@ -322,28 +337,35 @@
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
@@ -352,14 +374,15 @@
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
@@ -370,55 +393,64 @@
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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/literals.pyi` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,25 @@
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
@@ -143,30 +145,35 @@
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
@@ -192,14 +199,15 @@
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
@@ -244,51 +252,57 @@
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
@@ -301,14 +315,15 @@
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
@@ -320,28 +335,35 @@
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
@@ -350,14 +372,15 @@
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
@@ -368,55 +391,64 @@
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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/type_defs.py` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "OptionStatusTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BuildSuggestersResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "DateArrayOptionsTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
@@ -57,30 +57,30 @@
     "DocumentSuggesterOptionsTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
     "DoubleArrayOptionsTypeDef",
     "DoubleOptionsTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
+    "IndexDocumentsResponseTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
+    "ListDomainNamesResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
     "AnalysisSchemeTypeDef",
-    "BuildSuggestersResponseTypeDef",
-    "IndexDocumentsResponseTypeDef",
-    "ListDomainNamesResponseTypeDef",
     "DefineExpressionRequestRequestTypeDef",
     "ExpressionStatusTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
     "IndexFieldTypeDef",
@@ -154,22 +154,19 @@
 BuildSuggestersRequestRequestTypeDef = TypedDict(
     "BuildSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BuildSuggestersResponseTypeDef = TypedDict(
+    "BuildSuggestersResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FieldNames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -496,14 +493,22 @@
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+IndexDocumentsResponseTypeDef = TypedDict(
+    "IndexDocumentsResponseTypeDef",
+    {
+        "FieldNames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -584,14 +589,33 @@
         "SortEnabled": bool,
         "HighlightEnabled": bool,
         "AnalysisScheme": str,
     },
     total=False,
 )
 
+ListDomainNamesResponseTypeDef = TypedDict(
+    "ListDomainNamesResponseTypeDef",
+    {
+        "DomainNames": Dict[str, str],
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
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -646,38 +670,14 @@
 )
 
 
 class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
 
-BuildSuggestersResponseTypeDef = TypedDict(
-    "BuildSuggestersResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IndexDocumentsResponseTypeDef = TypedDict(
-    "IndexDocumentsResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainNamesResponseTypeDef = TypedDict(
-    "ListDomainNamesResponseTypeDef",
-    {
-        "DomainNames": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
@@ -790,39 +790,39 @@
     },
 )
 
 DescribeServiceAccessPoliciesResponseTypeDef = TypedDict(
     "DescribeServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceAccessPoliciesResponseTypeDef = TypedDict(
     "UpdateServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAvailabilityOptionsResponseTypeDef = TypedDict(
     "DescribeAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAvailabilityOptionsResponseTypeDef = TypedDict(
     "UpdateAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
         "Options": AnalysisSchemeTypeDef,
@@ -838,31 +838,31 @@
     },
 )
 
 DefineExpressionResponseTypeDef = TypedDict(
     "DefineExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteExpressionResponseTypeDef = TypedDict(
     "DeleteExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExpressionsResponseTypeDef = TypedDict(
     "DescribeExpressionsResponseTypeDef",
     {
         "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -878,47 +878,47 @@
     },
 )
 
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainEndpointOptionsResponseTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineIndexFieldRequestRequestTypeDef = TypedDict(
     "DefineIndexFieldRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -934,90 +934,90 @@
     },
 )
 
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateScalingParametersResponseTypeDef = TypedDict(
     "UpdateScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineAnalysisSchemeResponseTypeDef = TypedDict(
     "DefineAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAnalysisSchemeResponseTypeDef = TypedDict(
     "DeleteAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAnalysisSchemesResponseTypeDef = TypedDict(
     "DescribeAnalysisSchemesResponseTypeDef",
     {
         "AnalysisSchemes": List[AnalysisSchemeStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineSuggesterResponseTypeDef = TypedDict(
     "DefineSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSuggesterResponseTypeDef = TypedDict(
     "DeleteSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSuggestersResponseTypeDef = TypedDict(
     "DescribeSuggestersResponseTypeDef",
     {
         "Suggesters": List[SuggesterStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineIndexFieldResponseTypeDef = TypedDict(
     "DefineIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteIndexFieldResponseTypeDef = TypedDict(
     "DeleteIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIndexFieldsResponseTypeDef = TypedDict(
     "DescribeIndexFieldsResponseTypeDef",
     {
         "IndexFields": List[IndexFieldStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch/type_defs.pyi` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "OptionStatusTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BuildSuggestersResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "DateArrayOptionsTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
@@ -56,30 +56,30 @@
     "DocumentSuggesterOptionsTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
     "DoubleArrayOptionsTypeDef",
     "DoubleOptionsTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
+    "IndexDocumentsResponseTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
+    "ListDomainNamesResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
     "AnalysisSchemeTypeDef",
-    "BuildSuggestersResponseTypeDef",
-    "IndexDocumentsResponseTypeDef",
-    "ListDomainNamesResponseTypeDef",
     "DefineExpressionRequestRequestTypeDef",
     "ExpressionStatusTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
     "IndexFieldTypeDef",
@@ -151,22 +151,19 @@
 BuildSuggestersRequestRequestTypeDef = TypedDict(
     "BuildSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BuildSuggestersResponseTypeDef = TypedDict(
+    "BuildSuggestersResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FieldNames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -477,14 +474,22 @@
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+IndexDocumentsResponseTypeDef = TypedDict(
+    "IndexDocumentsResponseTypeDef",
+    {
+        "FieldNames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -565,14 +570,33 @@
         "SortEnabled": bool,
         "HighlightEnabled": bool,
         "AnalysisScheme": str,
     },
     total=False,
 )
 
+ListDomainNamesResponseTypeDef = TypedDict(
+    "ListDomainNamesResponseTypeDef",
+    {
+        "DomainNames": Dict[str, str],
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
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -625,38 +649,14 @@
     },
     total=False,
 )
 
 class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
-BuildSuggestersResponseTypeDef = TypedDict(
-    "BuildSuggestersResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IndexDocumentsResponseTypeDef = TypedDict(
-    "IndexDocumentsResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainNamesResponseTypeDef = TypedDict(
-    "ListDomainNamesResponseTypeDef",
-    {
-        "DomainNames": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
@@ -765,39 +765,39 @@
     },
 )
 
 DescribeServiceAccessPoliciesResponseTypeDef = TypedDict(
     "DescribeServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceAccessPoliciesResponseTypeDef = TypedDict(
     "UpdateServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAvailabilityOptionsResponseTypeDef = TypedDict(
     "DescribeAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAvailabilityOptionsResponseTypeDef = TypedDict(
     "UpdateAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
         "Options": AnalysisSchemeTypeDef,
@@ -813,31 +813,31 @@
     },
 )
 
 DefineExpressionResponseTypeDef = TypedDict(
     "DefineExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteExpressionResponseTypeDef = TypedDict(
     "DeleteExpressionResponseTypeDef",
     {
         "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExpressionsResponseTypeDef = TypedDict(
     "DescribeExpressionsResponseTypeDef",
     {
         "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -853,47 +853,47 @@
     },
 )
 
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainEndpointOptionsResponseTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineIndexFieldRequestRequestTypeDef = TypedDict(
     "DefineIndexFieldRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -909,90 +909,90 @@
     },
 )
 
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateScalingParametersResponseTypeDef = TypedDict(
     "UpdateScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineAnalysisSchemeResponseTypeDef = TypedDict(
     "DefineAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAnalysisSchemeResponseTypeDef = TypedDict(
     "DeleteAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAnalysisSchemesResponseTypeDef = TypedDict(
     "DescribeAnalysisSchemesResponseTypeDef",
     {
         "AnalysisSchemes": List[AnalysisSchemeStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineSuggesterResponseTypeDef = TypedDict(
     "DefineSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSuggesterResponseTypeDef = TypedDict(
     "DeleteSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSuggestersResponseTypeDef = TypedDict(
     "DescribeSuggestersResponseTypeDef",
     {
         "Suggesters": List[SuggesterStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefineIndexFieldResponseTypeDef = TypedDict(
     "DefineIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteIndexFieldResponseTypeDef = TypedDict(
     "DeleteIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIndexFieldsResponseTypeDef = TypedDict(
     "DescribeIndexFieldsResponseTypeDef",
     {
         "IndexFields": List[IndexFieldStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/PKG-INFO` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearch
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CloudSearch 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudSearch 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
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
 
 <a id="mypy-boto3-cloudsearch"></a>
 
 # mypy-boto3-cloudsearch
 
 [![PyPI - mypy-boto3-cloudsearch](https://img.shields.io/pypi/v/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,15 +305,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BuildSuggestersResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
     DateArrayOptionsTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
@@ -330,30 +331,30 @@
     DocumentSuggesterOptionsTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
     DoubleArrayOptionsTypeDef,
     DoubleOptionsTypeDef,
     IndexDocumentsRequestRequestTypeDef,
+    IndexDocumentsResponseTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
+    ListDomainNamesResponseTypeDef,
+    ResponseMetadataTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
     AnalysisSchemeTypeDef,
-    BuildSuggestersResponseTypeDef,
-    IndexDocumentsResponseTypeDef,
-    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
     ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
     IndexFieldTypeDef,
@@ -398,42 +399,42 @@
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

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/mypy_boto3_cloudsearch.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearch-1.27.0/mypy_boto3_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.26.0.post1/setup.py` & `mypy-boto3-cloudsearch-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cloudsearch.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearch",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudSearch 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CloudSearch 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
     keywords="boto3 cloudsearch type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cloudsearch": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cloudsearch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/",
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


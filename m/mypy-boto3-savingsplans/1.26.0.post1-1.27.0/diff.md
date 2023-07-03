# Comparing `tmp/mypy-boto3-savingsplans-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-savingsplans-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-savingsplans-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:58 2022, max compression
+gzip compressed data, was "mypy-boto3-savingsplans-1.27.0.tar", last modified: Mon Jul  3 19:51:24 2023, max compression
```

## Comparing `mypy-boto3-savingsplans-1.26.0.post1.tar` & `mypy-boto3-savingsplans-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.148848 mypy-boto3-savingsplans-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13616 2022-11-01 21:43:58.148848 mypy-boto3-savingsplans-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12155 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.144848 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10159 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8679 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8677 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    11472 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11467 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.148848 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13616 2022-11-01 21:43:57.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-11-01 21:43:57.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:57.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:57.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:57.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:57.000000 mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:58.148848 mypy-boto3-savingsplans-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:40:56.000000 mypy-boto3-savingsplans-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.787951 mypy-boto3-savingsplans-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-07-03 19:51:24.787951 mypy-boto3-savingsplans-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.787951 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-03 19:47:29.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-03 19:47:29.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-03 19:47:29.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.787951 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-07-03 19:51:24.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:51:24.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:24.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:24.000000 mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:24.787951 mypy-boto3-savingsplans-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:47:28.000000 mypy-boto3-savingsplans-1.27.0/setup.py
```

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/LICENSE` & `mypy-boto3-savingsplans-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/PKG-INFO` & `mypy-boto3-savingsplans-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-savingsplans
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SavingsPlans 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SavingsPlans 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/
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
 
 <a id="mypy-boto3-savingsplans"></a>
 
 # mypy-boto3-savingsplans
 
 [![PyPI - mypy-boto3-savingsplans](https://img.shields.io/pypi/v/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-savingsplans?color=blue)](https://pypistats.org/packages/mypy-boto3-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SavingsPlans 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[boto3.SavingsPlans 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
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
 [mypy-boto3-savingsplans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,30 +309,30 @@
 
 `mypy_boto3_savingsplans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_savingsplans.type_defs import (
     CreateSavingsPlanRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSavingsPlanResponseTypeDef,
     DeleteQueuedSavingsPlanRequestRequestTypeDef,
     SavingsPlanRateFilterTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ParentSavingsPlanOfferingTypeDef,
+    ResponseMetadataTypeDef,
     SavingsPlanOfferingPropertyTypeDef,
     SavingsPlanOfferingRatePropertyTypeDef,
     SavingsPlanRatePropertyTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeSavingsPlanRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingsRequestRequestTypeDef,
     DescribeSavingsPlansRequestRequestTypeDef,
     DescribeSavingsPlansResponseTypeDef,
     SavingsPlanOfferingTypeDef,
     SavingsPlanOfferingRateTypeDef,
@@ -349,42 +350,42 @@
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

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/README.md` & `mypy-boto3-savingsplans-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-savingsplans"></a>
 
 # mypy-boto3-savingsplans
 
 [![PyPI - mypy-boto3-savingsplans](https://img.shields.io/pypi/v/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-savingsplans?color=blue)](https://pypistats.org/packages/mypy-boto3-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SavingsPlans 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[boto3.SavingsPlans 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
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
 [mypy-boto3-savingsplans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,30 +277,30 @@
 
 `mypy_boto3_savingsplans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_savingsplans.type_defs import (
     CreateSavingsPlanRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSavingsPlanResponseTypeDef,
     DeleteQueuedSavingsPlanRequestRequestTypeDef,
     SavingsPlanRateFilterTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ParentSavingsPlanOfferingTypeDef,
+    ResponseMetadataTypeDef,
     SavingsPlanOfferingPropertyTypeDef,
     SavingsPlanOfferingRatePropertyTypeDef,
     SavingsPlanRatePropertyTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeSavingsPlanRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingsRequestRequestTypeDef,
     DescribeSavingsPlansRequestRequestTypeDef,
     DescribeSavingsPlansResponseTypeDef,
     SavingsPlanOfferingTypeDef,
     SavingsPlanOfferingRateTypeDef,
@@ -318,42 +318,42 @@
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

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/client.py` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/client.pyi` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/literals.py` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,23 +91,25 @@
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
@@ -117,30 +119,35 @@
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
@@ -166,14 +173,15 @@
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
@@ -218,51 +226,57 @@
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
@@ -275,14 +289,15 @@
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
@@ -294,28 +309,35 @@
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
@@ -324,14 +346,15 @@
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
@@ -342,55 +365,64 @@
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

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/literals.pyi` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -89,23 +89,25 @@
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
@@ -115,30 +117,35 @@
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
@@ -164,14 +171,15 @@
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
@@ -216,51 +224,57 @@
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
@@ -273,14 +287,15 @@
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
@@ -292,28 +307,35 @@
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
@@ -322,14 +344,15 @@
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
@@ -340,55 +363,64 @@
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

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/type_defs.py` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,33 +32,32 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateSavingsPlanRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateSavingsPlanResponseTypeDef",
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     "SavingsPlanRateFilterTypeDef",
     "SavingsPlanOfferingRateFilterElementTypeDef",
     "SavingsPlanOfferingFilterElementTypeDef",
     "SavingsPlanFilterTypeDef",
     "SavingsPlanTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ParentSavingsPlanOfferingTypeDef",
+    "ResponseMetadataTypeDef",
     "SavingsPlanOfferingPropertyTypeDef",
     "SavingsPlanOfferingRatePropertyTypeDef",
     "SavingsPlanRatePropertyTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateSavingsPlanResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribeSavingsPlanRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingsRequestRequestTypeDef",
     "DescribeSavingsPlansRequestRequestTypeDef",
     "DescribeSavingsPlansResponseTypeDef",
     "SavingsPlanOfferingTypeDef",
     "SavingsPlanOfferingRateTypeDef",
@@ -82,29 +81,24 @@
         "purchaseTime": Union[datetime, str],
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSavingsPlanRequestRequestTypeDef(
     _RequiredCreateSavingsPlanRequestRequestTypeDef, _OptionalCreateSavingsPlanRequestRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSavingsPlanResponseTypeDef = TypedDict(
+    "CreateSavingsPlanResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "savingsPlanId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteQueuedSavingsPlanRequestRequestTypeDef = TypedDict(
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     {
         "savingsPlanId": str,
@@ -175,27 +169,46 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 ParentSavingsPlanOfferingTypeDef = TypedDict(
     "ParentSavingsPlanOfferingTypeDef",
     {
         "offeringId": str,
         "paymentOption": SavingsPlanPaymentOptionType,
         "planType": SavingsPlanTypeType,
         "durationSeconds": int,
         "currency": CurrencyCodeType,
         "planDescription": str,
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
 SavingsPlanOfferingPropertyTypeDef = TypedDict(
     "SavingsPlanOfferingPropertyTypeDef",
     {
         "name": SavingsPlanOfferingPropertyKeyType,
         "value": str,
     },
     total=False,
@@ -231,30 +244,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateSavingsPlanResponseTypeDef = TypedDict(
-    "CreateSavingsPlanResponseTypeDef",
-    {
-        "savingsPlanId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDescribeSavingsPlanRatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSavingsPlanRatesRequestRequestTypeDef",
     {
         "savingsPlanId": str,
     },
 )
 _OptionalDescribeSavingsPlanRatesRequestRequestTypeDef = TypedDict(
@@ -263,22 +260,20 @@
         "filters": Sequence[SavingsPlanRateFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeSavingsPlanRatesRequestRequestTypeDef(
     _RequiredDescribeSavingsPlanRatesRequestRequestTypeDef,
     _OptionalDescribeSavingsPlanRatesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeSavingsPlansOfferingRatesRequestRequestTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingRatesRequestRequestTypeDef",
     {
         "savingsPlanOfferingIds": Sequence[str],
         "savingsPlanPaymentOptions": Sequence[SavingsPlanPaymentOptionType],
         "savingsPlanTypes": Sequence[SavingsPlanTypeType],
         "products": Sequence[SavingsPlanProductTypeType],
@@ -326,15 +321,15 @@
 )
 
 DescribeSavingsPlansResponseTypeDef = TypedDict(
     "DescribeSavingsPlansResponseTypeDef",
     {
         "savingsPlans": List[SavingsPlanTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SavingsPlanOfferingTypeDef = TypedDict(
     "SavingsPlanOfferingTypeDef",
     {
         "offeringId": str,
@@ -383,29 +378,29 @@
 )
 
 DescribeSavingsPlansOfferingsResponseTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingsResponseTypeDef",
     {
         "searchResults": List[SavingsPlanOfferingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSavingsPlansOfferingRatesResponseTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingRatesResponseTypeDef",
     {
         "searchResults": List[SavingsPlanOfferingRateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSavingsPlanRatesResponseTypeDef = TypedDict(
     "DescribeSavingsPlanRatesResponseTypeDef",
     {
         "savingsPlanId": str,
         "searchResults": List[SavingsPlanRateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans/type_defs.pyi` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,32 +32,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateSavingsPlanRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateSavingsPlanResponseTypeDef",
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     "SavingsPlanRateFilterTypeDef",
     "SavingsPlanOfferingRateFilterElementTypeDef",
     "SavingsPlanOfferingFilterElementTypeDef",
     "SavingsPlanFilterTypeDef",
     "SavingsPlanTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ParentSavingsPlanOfferingTypeDef",
+    "ResponseMetadataTypeDef",
     "SavingsPlanOfferingPropertyTypeDef",
     "SavingsPlanOfferingRatePropertyTypeDef",
     "SavingsPlanRatePropertyTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateSavingsPlanResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribeSavingsPlanRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingRatesRequestRequestTypeDef",
     "DescribeSavingsPlansOfferingsRequestRequestTypeDef",
     "DescribeSavingsPlansRequestRequestTypeDef",
     "DescribeSavingsPlansResponseTypeDef",
     "SavingsPlanOfferingTypeDef",
     "SavingsPlanOfferingRateTypeDef",
@@ -81,27 +82,26 @@
         "purchaseTime": Union[datetime, str],
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSavingsPlanRequestRequestTypeDef(
     _RequiredCreateSavingsPlanRequestRequestTypeDef, _OptionalCreateSavingsPlanRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+CreateSavingsPlanResponseTypeDef = TypedDict(
+    "CreateSavingsPlanResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "savingsPlanId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteQueuedSavingsPlanRequestRequestTypeDef = TypedDict(
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     {
         "savingsPlanId": str,
@@ -172,27 +172,46 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 ParentSavingsPlanOfferingTypeDef = TypedDict(
     "ParentSavingsPlanOfferingTypeDef",
     {
         "offeringId": str,
         "paymentOption": SavingsPlanPaymentOptionType,
         "planType": SavingsPlanTypeType,
         "durationSeconds": int,
         "currency": CurrencyCodeType,
         "planDescription": str,
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
 SavingsPlanOfferingPropertyTypeDef = TypedDict(
     "SavingsPlanOfferingPropertyTypeDef",
     {
         "name": SavingsPlanOfferingPropertyKeyType,
         "value": str,
     },
     total=False,
@@ -228,30 +247,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateSavingsPlanResponseTypeDef = TypedDict(
-    "CreateSavingsPlanResponseTypeDef",
-    {
-        "savingsPlanId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDescribeSavingsPlanRatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSavingsPlanRatesRequestRequestTypeDef",
     {
         "savingsPlanId": str,
     },
 )
 _OptionalDescribeSavingsPlanRatesRequestRequestTypeDef = TypedDict(
@@ -260,20 +263,22 @@
         "filters": Sequence[SavingsPlanRateFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeSavingsPlanRatesRequestRequestTypeDef(
     _RequiredDescribeSavingsPlanRatesRequestRequestTypeDef,
     _OptionalDescribeSavingsPlanRatesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeSavingsPlansOfferingRatesRequestRequestTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingRatesRequestRequestTypeDef",
     {
         "savingsPlanOfferingIds": Sequence[str],
         "savingsPlanPaymentOptions": Sequence[SavingsPlanPaymentOptionType],
         "savingsPlanTypes": Sequence[SavingsPlanTypeType],
         "products": Sequence[SavingsPlanProductTypeType],
@@ -321,15 +326,15 @@
 )
 
 DescribeSavingsPlansResponseTypeDef = TypedDict(
     "DescribeSavingsPlansResponseTypeDef",
     {
         "savingsPlans": List[SavingsPlanTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SavingsPlanOfferingTypeDef = TypedDict(
     "SavingsPlanOfferingTypeDef",
     {
         "offeringId": str,
@@ -378,29 +383,29 @@
 )
 
 DescribeSavingsPlansOfferingsResponseTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingsResponseTypeDef",
     {
         "searchResults": List[SavingsPlanOfferingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSavingsPlansOfferingRatesResponseTypeDef = TypedDict(
     "DescribeSavingsPlansOfferingRatesResponseTypeDef",
     {
         "searchResults": List[SavingsPlanOfferingRateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSavingsPlanRatesResponseTypeDef = TypedDict(
     "DescribeSavingsPlanRatesResponseTypeDef",
     {
         "savingsPlanId": str,
         "searchResults": List[SavingsPlanRateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/PKG-INFO` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-savingsplans
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SavingsPlans 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SavingsPlans 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/
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
 
 <a id="mypy-boto3-savingsplans"></a>
 
 # mypy-boto3-savingsplans
 
 [![PyPI - mypy-boto3-savingsplans](https://img.shields.io/pypi/v/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-savingsplans.svg?color=blue)](https://pypi.org/project/mypy-boto3-savingsplans)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-savingsplans?color=blue)](https://pypistats.org/packages/mypy-boto3-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SavingsPlans 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[boto3.SavingsPlans 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
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
 [mypy-boto3-savingsplans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,30 +309,30 @@
 
 `mypy_boto3_savingsplans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_savingsplans.type_defs import (
     CreateSavingsPlanRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSavingsPlanResponseTypeDef,
     DeleteQueuedSavingsPlanRequestRequestTypeDef,
     SavingsPlanRateFilterTypeDef,
     SavingsPlanOfferingRateFilterElementTypeDef,
     SavingsPlanOfferingFilterElementTypeDef,
     SavingsPlanFilterTypeDef,
     SavingsPlanTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ParentSavingsPlanOfferingTypeDef,
+    ResponseMetadataTypeDef,
     SavingsPlanOfferingPropertyTypeDef,
     SavingsPlanOfferingRatePropertyTypeDef,
     SavingsPlanRatePropertyTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeSavingsPlanRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
     DescribeSavingsPlansOfferingsRequestRequestTypeDef,
     DescribeSavingsPlansRequestRequestTypeDef,
     DescribeSavingsPlansResponseTypeDef,
     SavingsPlanOfferingTypeDef,
     SavingsPlanOfferingRateTypeDef,
@@ -349,42 +350,42 @@
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

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/mypy_boto3_savingsplans.egg-info/SOURCES.txt` & `mypy-boto3-savingsplans-1.27.0/mypy_boto3_savingsplans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-savingsplans-1.26.0.post1/setup.py` & `mypy-boto3-savingsplans-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-savingsplans.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-savingsplans",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_savingsplans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SavingsPlans 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.SavingsPlans 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 savingsplans type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_savingsplans": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_savingsplans": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_savingsplans/",
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

